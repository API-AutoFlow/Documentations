---
layout: default
title: Internal Actions
nav_order: 5
has_children: true
permalink: /docs/internal-actions
---
# Commonly used actions

## Array
[Count](https://docs.apiautoflow.com/docs/internal-actions/array/count/):  Counts the number of elements in the list.

[Insert-At](https://docs.apiautoflow.com/docs/internal-actions/array/insert-at/):  Inserts the element in a given position. Commonly used with Iteration/for-each to extract data from a list of objects

[Sort](https://docs.apiautoflow.com/docs/internal-actions/array/sort/): Used to sort array elements in ascending order

[Unique](https://docs.apiautoflow.com/docs/internal-actions/array/unique/): Used to remove duplicate elements from the list

## Conditional
[IF](https://docs.apiautoflow.com/docs/internal-actions/conditional/if/): If condition is used in many logic scenarios from processing simple tasks, to automating complex workflows.

## Config
[Start-Timer](https://docs.apiautoflow.com/docs/internal-actions/config-autoflow/timer-start/):  Used to start the timer based on a condition.

[Stop-Timer](https://docs.apiautoflow.com/docs/internal-actions/config-autoflow/timer-stop/):  Used to stop the timer based on a condition. Commonly used to start or stop the time after the flow or iteration is complete.

## Data
[Expression](https://docs.apiautoflow.com/docs/internal-actions/data/expression/): Used to apply code script (Elixir) for functions not supported with the built-in actions.

[Log](https://docs.apiautoflow.com/docs/internal-actions/data/log/): Used to debug the solution.

[Set](https://docs.apiautoflow.com/docs/internal-actions/data/set/): Used to apply data.

[Get-Variable](https://docs.apiautoflow.com/docs/internal-actions/data/get-variable/): Used often to get value from the Environment variable.

## DateTime
[Now](https://docs.apiautoflow.com/docs/internal-actions/date-time/now/): Used to get the current time

[Current-Unix-Time](https://docs.apiautoflow.com/docs/internal-actions/date-time/current-unix-time/): Used to get current unix-time for easier time calculations

## Flow
[Flow](https://docs.apiautoflow.com/docs/internal-actions/flow/call/): Used to group chain of actions into a reusable function

## Integer
[To-String](https://docs.apiautoflow.com/docs/internal-actions/integer/to-string/): Used to convert a number into a string

## Iteration
[Filter](https://docs.apiautoflow.com/docs/internal-actions/iteration/filter/): Lightest on compute. Commonly used to filter out elements from a large list of data.

[For-Each](https://docs.apiautoflow.com/docs/internal-actions/iteration/foreach/): Used when extracting out certain values from the data. Does not change the original data.

[MAP](https://docs.apiautoflow.com/docs/internal-actions/iteration/map/): Used to change the original data. Does not extract a certain value from the data

## JSON
[Decode](https://docs.apiautoflow.com/docs/internal-actions/json/decode/): Commonly used when working with HTTP Request body.  Data in the request body is normally a JSON string hence needs to be decoded into an object.

## Organization
[Group](https://docs.apiautoflow.com/docs/internal-actions/organization/group/):  Commonly used to organize and group the actions. It is also convenient when moving a group of actions between flows.

## String
[Base-64-Encode](https://docs.apiautoflow.com/docs/internal-actions/string/base64-encode/): Commonly used to encode ID and Password.

[Base-64-URL-Encode](https://docs.apiautoflow.com/docs/internal-actions/string/base64-url-encode/): Commonly used to convert a string into a URL.

[Character-Decode](https://docs.apiautoflow.com/docs/internal-actions/string/character-decode/): Commonly used when working with foreign characters.

[Join](https://docs.apiautoflow.com/docs/internal-actions/string/join/):  URL, query, system command, etc in most cases is a combination of value from many sources.  String/join is used to concatenate those values into a single string.

[Replace](https://docs.apiautoflow.com/docs/internal-actions/string/replace/): Commonly used for working with a timestamp. E.g. changing YYYY/MM/DD to YYYY-MM-DD by replacing / with - .

[Slice](https://docs.apiautoflow.com/docs/internal-actions/string/slice/): Commonly used when retrieving just the year (YYYY) from YYYYMMDD. Slice at position 4.

[Split-At](https://docs.apiautoflow.com/docs/internal-actions/string/split-at/): Commonly used when splitting YYYYMMDD to make YYYY and MMDD from. Split at position 4.

[Split-With](https://docs.apiautoflow.com/docs/internal-actions/string/split-with/):  Commonly used when splitting YYYY/MM/DD to make YYYY, MM, and DD. Split with character /.

[To-Integer](https://docs.apiautoflow.com/docs/internal-actions/string/to-integer/): Commonly used to convert string to an integer.


{: .fs-6 .fw-300 }
