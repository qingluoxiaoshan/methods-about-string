# 字符串相关的操作：

```
var str="12abg"
```

## 	1.字符串的长度


	
	console.log(str.length);===4

## 	2.字符串相对应的索引值

```
	console.log(str[1]);====2
```

## 	3.将字符串的字母全部转换为大写

​	

```
console.log(str.toUpperCase());===转换为大写
```

## 	4.concat拼接字符串

```
console.log(str.concat("你是我的","哈哈哈"))====12abg你是我的哈哈哈
```

## 	5.slice(start: int, end: int)截取字符串，返回的是一个新的字符串

```
console.log(str.slice(3,7)) ====bg  （开始位置，结束位置）不包括结束的位置，若只有一个字符串则返回的是起始位置到结束位置，若传的是负数，则是字符串的长度加负数

	console.log(str.slice(-3,-2))====a
```

## 	6.substring(start: int, end: int)跟slice差不多

​		当第一个参数比第二个参数小的时候，与slice是一样的， 当第一个参数比第二个参数大的时候，第一个参数表示结束位置，第二个表示开始的位置
​		如果是负数则表示，则把赋值转换为0

```
	console.log(str.substring(-2,2))
```

## 	7.split(separator: string, limit: int) 以什么分割，返回的是数组

​		第一个参数是分割的字符串，第二个参数是返回数组的个数
​		若只有一个参数，则返回的是整个数组
 			

```
var str = "12,23,58,ab"

		console.log(str.split(",", 3)) ===["12","23","58"]

		console.log(str.split(","))======["12","23","58","ab"]
```

##  	8.charAt()  里面参数是索引，根据索引位置查找对应的字符串



		var str = "agfadfgdgh";	
		console.log(str.charAt(4)); ====d

