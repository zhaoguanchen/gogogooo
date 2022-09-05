# Go学习笔记

这是一篇go语言学习笔记，记录基础语法。



## 1. 简介

### 1.1 发展历史

Go 语言起源 2007 年，并于 2009 年正式对外发布。

时间轴：

- 2007 年 9 月 21 日：雏形设计
- 2009 年 11 月 10日：首次公开发布
- 2010 年 1 月 8 日：当选 2009 年年度语言
- 2010 年 5 月：谷歌投入使用
- 2011 年 5 月 5 日：Google App Engine 支持 Go 语言



### 1.2 优势特点

- 简化问题，易于学习
- 内存管理，简洁语法，易于使用
- 快速编译，高效开发
- 高效执行
- 并发支持，轻松驾驭
- 静态类型
- 标准类库，规范统一
- 易于部署
- 文档全面
- 免费开源

### 1.3 适用领域

Go 语言被设计成一门应用于搭载 Web 服务器，存储集群或类似用途的巨型中央服务器的系统编程语言。对于高性能分布式系统领域而言，Go 语言无疑比大多数其它语言有着更高的开发效率。

值得注意的是，因为垃圾回收和自动内存分配的原因，Go 语言不适合用来开发对实时性要求很高的软件。



## 2. 环境与配置

### 2.1 Mac环境下安装

- Go的安装

官网下载安装包，根据指示点击傻瓜式安装。

默认安装目录为：`/usr/local/go`

### 2.2 IDE

直接推荐Jetbrains全家桶：[Goland](https://www.jetbrains.com/go/download/#section=mac)

此外，其他轻量文本编辑器也可，如 Sublime Text。

## 3. 语法规则

### 3.0 基础语法

#### 1. 第一个程序

```go
package main

import "fmt"

func main() {
	fmt.Println("Hello World!")
}
```

- package main：声明了 main.go 所在的包，Go 语言中使用包来组织代码。一般一个文件夹即一个包，包内可以暴露类型或方法供其他包使用。（与java一样）
- import “fmt”：fmt 是 Go 语言的一个标准库/包，用来处理标准输入输出。（fmt包非常常见）
- func main：main 函数是整个程序的入口，main 函数所在的包名也必须为 `main`。(与java main方法类似)
- fmt.Println(“Hello World!”)：调用 fmt 包的 Println 方法，打印出 “Hello World!”



如何运行？

1. 在文件所在目录下，执行：

```go
go run main.go
```

2. 使用IDE的情况下，点击`Run`。



#### 2. 命名，关键字

##### 文件

Go 的源文件以 `.go` 为后缀名存储在计算机中，这些文件名均由小写字母组成，如 `scanner.go` 。如果文件名由多个部分组成，则使用下划线 `_` 对它们进行分隔，如 `scanner_test.go` 。文件名不包含空格或其他特殊字符。

有效的标识符必须以字母（可以使用任何 UTF-8 编码的字符或 `_`）开头，然后紧跟着 0 个或多个字符或 Unicode 数字，如：X56、group1、_x23、i、өԑ12。

##### 关键字

| break    | default     | func   | interface | select |
| -------- | ----------- | ------ | --------- | ------ |
| case     | defer       | go     | map       | struct |
| chan     | else        | goto   | package   | switch |
| const    | fallthrough | if     | range     | type   |
| continue | for         | import | return    | var    |







### 3.1 数据类型





### 3.2 流程控制语句





### 3.3 函数





### 3.4 结构体、方法和接口



