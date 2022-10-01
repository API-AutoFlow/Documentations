---
layout: default
title: Sort
parent: Array
grand_parent: Internal Actions
---
# Array Sort
Path is an array of keys. So, if you have a complex array with hierarchy of keys, you can give it a path so that it is ordered by the specific key value within the array of objects.

## Properties
```yaml
Array: Location of the list to sort
Path: Path is an array of keys
Order: Ascending or Descending
Value Type: Assign the correct data type to assess
```

## Output
```yaml
Output-location: Location to store the output data
```


### Example

Let's say you have an `array`

```yaml
[
  {
    "a": {
      "key1": 5,
      "key2": "first"
    }
  },
  {
    "a": {
      "key1": 2,
      "key2": "second"
    }
  },
  {
    "a": {
      "key1": 3,
      "key2": "third"
    }
  }
]
```

with `Path`

```yaml
[
  "a",
  "key1"
]
```

`order` **ascending** and `value-type` **integer**


#### Output

Result in “out” is 

```yaml
[
  {
    "a": {
      "key1": 2,
      "key2": "second"
    }
  },
  {
    "a": {
      "key1": 3,
      "key2": "third"
    }
  },
  {
    "a": {
      "key1": 5,
      "key2": "first"
    }
  }
]
```


## Sample Configuration
Click to [learn how to paste configuration](https://docs.apiautoflow.com/docs/tutorial-video/course-basics/lesson-organization/#3-paste-configuration) into your solution.


```yaml
{
  "$action": "array/sort-by-path",
  "array": [
    {
      "a": {
        "key1": 5,
        "key2": "first"
      }
    },
    {
      "a": {
        "key1": 2,
        "key2": "second"
      }
    },
    {
      "a": {
        "key1": 3,
        "key2": "third"
      }
    }
  ],
  "order": "ascending",
  "output-location": {
    "__$afref__": "data",
    "path": [
      "out"
    ]
  },
  "path": [
    "a",
    "key1"
  ],
  "value-type": "integer"
}
```


