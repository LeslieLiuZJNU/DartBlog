# DartBlog
Dart学习笔记，注重于该语言比较独特的地方。

## 格式化输出

$+变量名
```
print("$name有$num元钱。");
```

## 变量类型

自适应类型
```
Var a;
```

类型的判断
```
if(a is int)
```

类型的转换
数字与字符串的转换
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

## 运算符

非空则赋值
```
b??=5;
```

## 集合的操作（List、Set、Map）

list转换为字符串，以“, ”隔开。
```
string = list.join(', ')
```

string转换为list，识别“, ”作为分隔符。
```
list = string.toList(', ')
```



List批量赋值成员，[begin, end)。
```
list.fillRange(begin,end,Object);
```

Map（映射）两种定义方式。
```
var person1 = { //第一种定义方法
  "name":"A",
  "age":"20"
}

var person2 = new Map();  //第二种定义方法
person2["name"] = "B";
person2.add("age":20);
person2.remove("age");
```

Map转换为List。
```
person1.keys.toList(); //所有关键字转换成List
person1.values.toList();  //所有值转换成List
```

遍历集合 forEach方法

forEach()方法内，是一个匿名方法，这个匿名方法传入了value作为参数。
```
list.forEach(
(value){
  print(value);
}
);
```

遍历集合 map方法

map()方法内，是一个匿名方法，这个匿名方法传入了value作为参数，并将返回值一系列值打包成Map。
```
```

遍历集合 where方法
```
```

遍历集合 any方法
```
```

遍历集合 every方法
```
```
