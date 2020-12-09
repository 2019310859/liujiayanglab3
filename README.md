# liujiayanglab3
实验三

# 实验目的
1.掌握Java中抽象类和抽象方法的定义。
2.掌握Java中接口的定义，熟练掌握接口的定义形式以及接口的实现方法。 
3.了解异常的使用方法，并在程序中根据输入情况做异常处理。

# 实验内容
某学校为了给学生提供勤工俭学机会，也减轻授课教师的部分压力，准许博士研究生参与课程的助教工作。此时，该博士研究生有双重身份：学生和助教教师。
1.设计两个管理接口：学生管理接口和教师管理接口。学生接口必须包括缴纳学费、查学费的方法；教师接口包括发放薪水和查询薪水的方法。
2.设计博士研究生类，实现上述的两个接口，该博士研究生应具有姓名、性别、年龄、每学期学费、每月薪水等属性。（其他属性及方法，可自行发挥）
3.编写测试类，并实例化至少两名博士研究生，统计他们的年收入和学费。根据两者之差，算出每名博士研究生的年应纳税金额（国家最新工资纳税标准，请自行检索）。

# 实验要求
1.在博士研究生类中实现各个接口定义的抽象方法; 
2.对年学费和年收入进行统计，用收入减去学费，求得纳税额；
3.国家最新纳税标准（系数），属于某一时期的特定固定值，与实例化对象没有关系，考虑如何用static final修饰定义。
4.实例化研究生类时，可采用运行时通过main方法的参数args一次性赋值，也可采用Scanner类实现运行时交互式输入。
5.根据输入情况，要在程序中做异常处理。

# 实验过程
1·设计接口Student和Teacher，其中Student接口包括setPay()方法和getPay()方法以及常量pay，Teacher接口包括setSalaly()和getSalaly()方法以及常量salaly。
2·定义一个博士类Doctor，实现Student接口和Teacher接口，编写主程序中需要调用的程序。
3.主程序中通过键盘输入，获取研究生编号，调取研究生信息，并输出各类数据。
4.计算月收入和学费，算出应纳税金额。

# 实验结果
请输入你的编号：
12
请输入正确编号！

请输入你的编号：
1
编号：1  姓名: 张三  性别: 男  年龄: 23
待缴学费：0.0
应缴学费：1500.0
待领工资：10000.0
应领工资：20000.0
应交税：446.25元

# 实验感想
本次实验学会了Java中抽象类和抽象方法的使用，了解了如何定义抽象。同时学会了接口的使用，接口中的常量及程序可以被直接调用。主程序中尝试使用if作为异常处理，如果编号存在则程序正常运行，若编号错误或不是数字，则给出提示“请输入正确编号！”同时返回程序第一步，再次获取研究生编号。借此机会了解了国家税率计算方法，完成了计算方法的实现。
