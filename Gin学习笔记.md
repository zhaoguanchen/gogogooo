# Go学习笔记

入门Web框架：Gin



## 1. 简介

  

## 2. 环境与配置

### 2.1 安装Gin

```go
go get -u -v github.com/gin-gonic/gin
```

## 3. 如何使用

#### 1. 第一个程序

```go
package main

import (
	"github.com/gin-gonic/gin"
)

func main() {
	r := gin.Default()
	r.GET("/ping", func(c *gin.Context) {
		c.JSON(200, gin.H{
			"message": "pong",
		})
	})
	err := r.Run()
	if err != nil {
		return
	} // listen and serve on 0.0.0.0:8080
}

```



 
