class student:
    name = None
    age = None

    def __init__(self, name, age):  #构造方法
        self.name = name
        self.age = age

    def __str__(self):  #str魔术方法
        return f'该student类对象，name = {self.name}， age = {self.age}'

    def __lt__(self, other):  #it魔术方法， 用于比较， 只能用小于 大于
        return self.age < other.age

    def __le__(self, other):  #le魔术方法， 用于比较， 只能用小于等于 大于等于
        return self.age <= other.age

    def __eq__(self, other):  #eq魔术方法， 用于判断， ==
        return self.age == other.age

    def say_hello(self, a, b):  #成员函数里面必须要带self

        print(self.name, a, b)  #调用成员变量时要用self.
"""
stu_1 = student()  #创建对象

stu_1.name = 'xiaoming'
stu_1.age = 19

a = 0
b = 0
stu_1.say_hello(a, b)
"""
a=0
b=0

stu_2 = student('xiaohong', 19)  #利用构造方法
stu_2.say_hello(a, b)
print()

stu_3 = student('xiaogang', 17)  #利用str魔术方法
print(stu_3)
print()

stu_4 = student('xiaoli', 18)  #利用lt魔术方法
print(stu_4 < stu_3)
print(stu_4 > stu_3)
print()

stu_5 = student('xiaoya', 20)  #利用le魔术方法
print(stu_5 <= stu_3)
print(stu_5 >= stu_3)
print()

stu_6 = student('xiaoxing', 21)
print(stu_6 == stu_3)
