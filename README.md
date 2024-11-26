##实验一 数据类型、运算符与表达式
##一、实验目的
1、了解算法的概念、特性、算法在程序设计中的地位。
2、熟悉算法的表示方法。
3、掌握用流程图表示一个算法。
4、能独立设计一个问题的算法,并根据该算法编出问题的程序。
5、掌握C语言数据类型，熟悉如何定义一个整型、字符型和实型变量，以及对它们赋值的方法，了解以上类型数据输出时所用的格式转换符。
6、学会使用C的有关算术运算符，以及包含这些运算符的表达式，特别是自加、自减运算符的使用。
7、进一步熟悉C程序的编辑、编译、连接和运行的过程。
##二、实验准备
1、复习算法的概念和特性。
2、复习算法的几种表示方式。3、复习C语言的数据类型。
4、复习各种运算符和表达式。
##三、实验内容
1、运行程序并回答问题:
#include<stdio.h> 
int main()
{
	printf("%c", '/007');
	return 0;
}
问题:如果执行printf("%c＂,'0x7')会得到什么结果?为什么?
![004552afbbab2d7ebf435eb44f089fa7](https://github.com/user-attachments/assets/f7e33620-df65-49a9-a0f2-591271c4935b)
7，因为x是十六进制，7比16小所以不进位
#include<stdio.h> 
void main()
{
	char c1, c2;
	c1 = getchar();
	c2 = getchar();
	putchar(c1);
	putchar(c2);
	return 0;
}
问题：把c1，c2定义成整型变量是否可以？为什么？采用同样的输入值观察结果。
可以 char:![F1K$21572IACX21X4BFKEL](https://github.com/user-attachments/assets/eb90d975-2b26-4b0a-bef8-3a607c58005b)
int:![L{T2WXWN0{LPK{)D{D1XT66](https://github.com/user-attachments/assets/b32edc6c-5582-45f3-824e-c9670615b795)
2、输人程序并运行:
#include<stdio.h>
void main()
{
   char c1, c2;
   c1 = 97; c2 = 98;
   printf("%c %c\n", c1, c2);
   return 0;
}
在此基础上:
·加printf("%d,%d",c1,c2)；运行。![f7b64f14f790225c6679aadd9aedccbb](https://github.com/user-attachments/assets/ff96740c-3591-4e19-9696-413431a6b6e3)
·将第二行改为:int c1,c2；运行。![be02fd7cfa451af945ef126ddac35580](https://github.com/user-attachments/assets/f77ca395-7319-400b-a297-e05b8c78be72)
·将第三行改为:c1=300;c2=400;运行。![6317ecbd2ea7b8fba4075029710bc4e3](https://github.com/user-attachments/assets/acfbb93c-938b-4a0e-b651-f492627ba593)
#include<stdio.h>
void main()
{
	int c1, c2;
	c1 = 300; c2 = 400;
	printf("%c %c\n", c1, c2);
	printf("%d,%d", c1, c2);
	return 0;
}
3、输入程序并运行：
#include<stdio .h>
void main()
｛
char c1='a',c2='b',c3='c',c4='\101' ,c5='\116';
printf("a%cb%c\tc%c\tabc\n" ,c1,c2,c3);     
printf("\t\b%c%c",c4,c5);
return 0;
｝
![f5d5577562084e336a7e85452d79d9ad](https://github.com/user-attachments/assets/cc19dd0d-5402-4a26-a51a-4b5b82bad2bc)
