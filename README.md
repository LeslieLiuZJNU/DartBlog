# DartBlog
Blog for learning Dart language.
Focus on the difference to Java.


## 格式化输出
```
print("$name有$num元钱。");
```


## 基本类型
```
Var a;
```


## 类型的判断
```
if(a is int)
```


## 类型的转换
```
int.parse(String)
double.parse(String)

int num=0;
num.toString();

try{//空字符串转换为0
  String a="";
  b=double.parse(a);
  print(b);
}catch(error){
  print(0);
}
```


## 集合类型（List、Set、Map）
```
//List
string = list.join(', ')  //list转换为字符串，以“, ”隔开。
list = string.toList(', ')  //string转换为list，识别“, ”作为分隔符。
list.fillRange(begin,end,Object); //把 [begin,end) 下标的成员改成Object。


//Map
var person1 = { //第一种定义方法
  "name":"A",
  "age":"20"
}
var person2 = new Map();  //第二种定义方法
person2["name"] = "B";
person2.add("age":20);
person2.remove("age");

person1.keys.toList(); //所有关键字转换成List
person1.values.toList();  //所有值转换成List

//集合遍历forEach
list.forEach(
(value){
  print(value);
}
);
```



## 赋值运算符
```
b??=5;  //非空则赋值
```

