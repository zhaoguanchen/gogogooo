# How to solve Leetcode with Golang?

 ## 1. Array

### create

```go
var array [4]int
```



### Iterate

### sort

Sort 2-D array. use `sort.Slice()`.

```go
package main

import (
	"fmt"
	"sort"
)

func main() {
	interval := [][]int{
		{2, 3},
		{2, 2},
		{3, 3},
		{1, 3},
		{5, 7},
		{2, 2},
		{4, 6},
	}
	sort.Slice(interval, func(i, j int) bool {
		if interval[i][0] == interval[j][0] {
			return interval[i][1] < interval[j][1]
		}
		return interval[i][0] < interval[j][0]
	})
	fmt.Println(interval)
}
```



## 2. Queue





 
