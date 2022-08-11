---
layout: default
title: String Split At New Line
parent: String
grand_parent: Actions
---
# String Split At New Line
Splits a string into two at the specified offset. When the offset is given is negative, the location is counted from the end of the string.

New line에 split이 되어 Array의 element들이 만들어 집니다.
보내 주신 예시를 보면 string에 abc abc abc를 넣으셨는데, new line이 사라집니다. 
File등에서 읽어 온 data에 바로 적용해야 합니다.



## Properties
```yaml
String: Location of the string to work on
parts: Number parts to split the string (0 is infinity)
trim: 
```

## Output
```yaml
Output-location: Location to store the output data
```

### Example
Input string 

```
abc
abc
abc
```

parts `2`

will output  `["abc", "abc abc"]`


## Sample Configuration
Click to [learn how to paste configuration](https://docs.apiautoflow.com/docs/tutorials/course-1-basics/lesson-6-reusable-custom-actions/#cut-and-paste-configuration) into your solution.


```yaml
{
  "$action": "organization/group",
  "do": [
    {
      "$action": "organization/group",
      "do": [
        {
          "$action": "string/unescape",
          "output-location": {
            "__$afref__": "data",
            "path": [
              "newline"
            ]
          },
          "string": "\\n"
        },
        {
          "$action": "string/join",
          "array": [
            "abc",
            "abc",
            "abc"
          ],
          "output-location": {
            "__$afref__": "data",
            "path": [
              "text"
            ]
          },
          "separator": {
            "__$afref__": "data",
            "path": [
              "newline"
            ]
          }
        }
      ],
      "name": "Sample String with New Line"
    },
    {
      "$action": "string/split-at-newline",
      "output-location": {
        "__$afref__": "data",
        "path": [
          "out"
        ]
      },
      "parts": 2,
      "string": {
        "__$afref__": "data",
        "path": [
          "text"
        ]
      },
      "trim": false
    }
  ],
  "name": "Sample: Split At New Line"
}
```