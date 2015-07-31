# mahonia
Automatically exported from code.google.com/p/mahonia

code.google.com上的一个备份。

使用方法：
~~~ go
  # git clone git clone https://github.com/doumadou/mahonia.git /usr/lib/golang/src/code.google.com/p/mahonia
~~~

转码例子：
~~~ go
  package main

  import (
	  "fmt"
	  "code.google.com/p/mahonia"
  )

  func main() {
  	s := "<span class=\"red\">3.1\u6298/</span>\u5706\u9886\u957f\u88d9\u5047\u4e24\u4ef6\u8d34\u5e03\u77ed\u8896\u8fde\u8863\u88d9\uff082\u8272\u9009\uff09"

  	enc := mahonia.NewDecoder("utf8")
    fmt.Println(enc.ConvertString(s))
  }
~~~
