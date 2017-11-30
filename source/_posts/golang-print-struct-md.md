---
title: golang print struct
date: 2017-11-30 17:24:25
tags: [golang,struct]
categories: golang
---
## golang 如何打印出结构体struct的全部信息？
在程序调试中，经常用到fmt.Println(a)或者fmt.Printf("%v",a)。
```
package main
import "fmt"

type Eg struct {
   name string
   age  int  
}

func main() {
     a: = Eg{"tom",21}
     fmt.Println(a)
     fmt.Printf("%v",a)
     fmt.Printf("%+v",a)
}
```
此例输出：
```
{tom 21}
{tom 21}{name:tom age:21}
```

