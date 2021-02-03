##python 语法

[__name__]()
[with]()
[none]()

#### __name__ :
1.python是解释性语言，当python执行到当前文件时，当前文件的__name__ 为main。
````
test.py
import hello
// hello
print(hello.__name__) 
// __main__
print(__name__)
//python test.py ,此时会执行这个，执行main（）方法，从而有一个函数入口
if(__name__ == "__main__")
    main()

````

#### with
1. with 类似于上下文管理工具：
````
// with 新建了一个心类，当with语句执行完之后会自动释放这个类
with newClass():
    test()

````

#### none 
1. none 给我的理解是not type，因为python赋值是才确定类型