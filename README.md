# vs2013-20201-19
learn
#define _CRT_SECURE_NO_WARNINGS 1
#include<stdio.h>
#include<string.h>
#include<windows.h>
int main()
{
	int i = 0;
	char password[20] = { 0 };
	for (i = 0; i < 3; i++)
	{
		printf("请输入密码:>");
		scanf("%s", password);
		if (strcmp(password, "123456") == 0)//==不能用来比较两个字符串是否相等，应该使用一个库函数-strcmp
		{
			printf("登陆成功\n");
			break;
		}
		else
		{
			printf("密码错误\n");
		}
	}
	if (i == 3)
		printf("三次密码均错误，退出程序\n");
	return 0;
}
//int age = 20;
//if (age < 18)
//printf("未成年\n");

/*int age = 10;
if (age < 18)
printf("未成年\n");
else if (age >= 18 && age < 28)
printf("青年\n");
else if (age >= 28 && age < 50)
printf("壮年\n");
else if (age >= 50 && age < 90)
printf("老年\n");
else
printf("老不死\n");*/

//int a = 0;
//int b = 2;
//if (a == 1)
//if (b == 2)
//printf("hehe\n");
//else
//printf("haha\n");

/*int a = 0;
int b = 2;
if (a == 1)
if (b == 2)
printf("hehe\n");
else
printf("haha\n");*/

//int a = 0;
//int b = 2;
//if (a == 1)
//{
//	if (b == 2)
//		printf("hehe\n");
//	else
//		printf("haha\n");
//}

//int num = 4;
//if (num = 5)//=赋值==判断相等
//{
//	printf("hehe\n");
//}

//int num = 4;
//if (5 == num)
//{
//	printf("hehe\n");
//}

//int i = 1;
//while (i <= 100)
//{
//	if (i % 2 == 1)
//		printf("%d", i);
//	i++;
//}

//int day = 0;
//scanf("%d", &day);
//switch (day)
//{
//case1:
//	printf("星期1\n");
//	break;
//case2:
//	printf("星期2\n");
//	break;
//case3:
//	printf("星期3\n");
//	break;
//case4:
//	printf("星期4\n");
//	break;
//case5:
//	printf("星期5\n");
//	break;
//case6:
//	printf("星期6\n");
//	break;
//case7:
//	printf("星期7\n");
//	break;
//}

//int day = 0;
//scanf("%d", &day);
//switch (day)
//{
//case 1:
//case 2:
//case 3:
//case 4:
//case 5:
//	printf("工作日\n");
//	break;
//case 6:
//case 7:
//	printf("休息日\n");
//	break;
//default:
//	printf("输入错误\n");
//
//}

//int i = 1;
//while (i <= 10)
//{
//	printf("%d", i);
//	i++;
//}

//int i = 1;
//while (i <= 10)
//{
//	if (5 == i)
//		continue;
//	printf("%d\n", i);
//	i++;
//}

//int i = 1;
//while (i <= 10)
//{
//	if (5 == i)
//		break;
//	printf("%d\n", i);
//	i++;
//}

//int ch = 0;
//while ((ch = getchar()) != EOF)
//putchar(ch);

//int ch = getchar();
//putchar(ch);
//printf("%c\n", ch);

//int ch = 0;
////ctrl+z
////EOF-end of file->-1 文件结束标志
//while ((ch = getchar()) != EOF)
//{
//	putchar(ch);
//}

//int ret = 0;
//int ch = 0;
//char password[20] = { 0 };
//printf("请输入密码:>");
//scanf("%s", password);//输入密码，并存放在password数据中
//while ((ch = getchar()) != '\n')
//{
//	;
//}
//printf("请确认(Y/N):>");
//ret = getchar();//Y/N
//if (ret == 'Y')
//{
//	printf("确认成功\n");
//}
//else
//{
//	printf("放弃确认\n");
//}

//int ch = 0;
//while ((ch = getchar()) != EOF)
//{
//	if (ch<'0' || ch>'9')
//		continue;
//	putchar(ch);
//}

//int i = 0;//初始化
//while (i < 10)//判断
//{
//	//…
//	i++;//调整
//}

////实际的问题：使用for循环在屏幕上打印1~10的数字
//	int i = 0;
//	for (i = 1; i <= 10; i++)
//	{
//		printf("%d\n", i);
//	}

//int i = 0;
//for(i = 1; i <= 10;i++)
//{
//	if (i == 5)
//		break;
//	printf("%d", i);
//}

//int arr[10] = { 1, 2, 3, 4, 5, 6, 7, 8, 9, 10 };
//int i = 0;
////10次循环
////10次打印
////10个元素
//for (i = 0; i < 10; i++)
//{
//	printf("%d", arr[i]);
//}

//int i = 0;
////前闭后开的写法
//for (i = 0; i < 10;i++)
//{ }
////两边都是闭区间
//for (i = 0; i <= 9;i++)
//{ }

////变种1
//for (;;)
//{
//	printf("hehe\n");
//}
////变种2
//int x, y;
//for (x = 0, y = 0; x < 2 && y < 5; ++x, y++)
//{
//	printf("hehe\n");
//}

//int i = 0;
//int k = 0;
//for (i = 0, k = 0; k = 0; i++, k++)//k=0不是判断语句
//k++;

//int i = 1;
//do
//{
//	printf("%d", i);
//	i++;
//} 
//while (i <= 10);

//int i = 1;
//do
//{
//	if (i == 5)
//		break;
//	printf("%d", i);
//	i++;
//} 
//while (i <= 10);

//int i = 1;
//do
//{
//	if (i == 5)
//		continue;
//	printf("%d", i);
//	i++;
//} 
//while (i <= 10);

//int i = 0;
//int n = 0;
//int ret = 1;
//scanf("%d", &n);
//for (i = 1; i <= n; i++)
//{
//	ret = ret*i;
//}
//printf("ret=%d\n", ret);

//int i = 1;
//int n = 1;
//int ret = 1;
//scanf("%d",&n);
//while (i <= n)
//{
//	ret = ret*i;
//	i++;
//}
//printf("ret=%d\n", ret);

//int i = 0;
//int n = 0;
//int ret = 1;
//int sum = 0;
//for (n = 1; n <= 3; n++)
//{
//	ret = 1;
//	for (i = 1; i <= n; i++)
//	{
//		ret = ret*i;
//	}
//	susum + ret;
//}

//int i = 1;
//int n = 1;
//int ret = 1;
//int sum = 0;
//while (n <= 10)
//{
//	while (i <= n)
//	{
//		ret = ret*i;
//		i++;
//	}
//	sum = sum + ret;
//	n++;
//}
//printf("sum=%d\n", sum);

//int arr[] = { 1, 2, 3, 4, 5, 6, 7, 8, 9, 10 };
//int k = 7;
//int sz = sizeof(arr) / sizeof(arr[0]);//计算元素个数
//int left = 0;//左下标
//int right = sz - 1;//右下标
//while (left < right)
//{
//	int mid = (left + right) / 2;
//	if (arr[mid] > k)
//	{
//		right = mid - 1;
//	}
//	else if (arr[mid] < k)
//	{
//		left = mid + 1;
//	}
//	else
//	{
//		printf("找到了，下标是：%d\n", mid);
//		break;
//	}
//}
//if (left > right)
//{
//	printf("找不到\n");
//}

////welcome to bit!!!!!!
////####################
////w##################!
////……
////char arr[] = "abc";
////[a b c \0]
////0 1 2 3
////4 - 2
//char arr1[] = "welcome t bit!!!!!!";
//char arr2[] = "###################";
//int left = 0;
////int right=sizeof(arr1/sizeof(arr[0]-2;//err
//int right = strlen(arr) - 1;
//while (left <= right)
//{
//	arr2[left] = arr1[left];
//	arr2[right] = arr1[right];
//	printf("%s\n", arr2);
//	//休息一秒
//	Sleep(1000);
//	//执行系统命令的一个函数-cls-清空屏幕
//	system("cls");
//	left++;
//	right--;
//}
