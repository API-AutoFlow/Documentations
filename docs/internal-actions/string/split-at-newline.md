---
layout: default
title: Split At New Line
parent: String
grand_parent: Internal Actions
---
# String Split At New Line
Splits a string at the **new line** into set number of **parts**. 

Note: Pasting text directly into the property __string__ removes the "new line".  To test the action, use the sample configuration below or [read the text directly from the file](https://docs.apiautoflow.com/docs/internal-actions/file/read).


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
Click to [learn how to paste configuration](https://docs.apiautoflow.com/docs/tutorial-video/course-basics/lesson-organization/#3-paste-configuration) into your solution.


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