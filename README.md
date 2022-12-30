# no-misleading-json-path
A small function that imitate json path
# Usage
## Example 1
```
{
        "person": [
            {
                "name": "homie",
                "address": "46 dict"
            },
            {
                "name": "bro",
                "address": "64 tcid"
            }
        ]
    }
```
- json path
```
person.[1].name
```
- Result
```
"bro"
```
## Example 2
```
[
    [
        {"name":"a"},
        {"name":"b"}
    ],
    [
        {"name":"b"},
        {"name":"a"}
    ],
    [
        {"name":"c"},
        {"name":"c"}
    ]
]
```
- json path
```
[*].[*].name
```
- Result
```
[
    ["a","b"],
    ["b","a"],
    ["c","c"]
]
```