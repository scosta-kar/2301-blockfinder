# 2301-blockfinder

Suppose we are looking for an appartment. we are interested in moving to a block that minimizes the distance traveled to a list of utilities we are interested in.


The blocks are represented by a list of adjacent blocks:

```
[
    {
        "school": true,
        "library": false,
        "pharmacy": false
    },
    {
        "school": false,
        "library": false,
        "pharmacy": false
    },
    {
        "school": false,
        "library": true,
        "pharmacy": false
    },
    {
        "school": false,
        "library": false,
        "pharmacy": false
    },
    {
        "school": false,
        "library": false,
        "pharmacy": true
    },
    {
        "school": false,
        "library": false,
        "pharmacy": false
    },
]
```

For each block, you can walk up or down the list to find the utility. The number of blocks you walk represent the distance.

The sencond parameter is a list of utilities we are interested in:
```
["school", "library", "pharmacy"]
```

We are looking to find the block that minimizes the maximum distance traveled to get to any of the utilities.

Assumptions:
- Every block has a property corresponding to each of the utilities we are interested in.