# C-language
学习C语言中敲的一些代码
#include<stdio.h>
#include<stdlib.h>
#include<string.h>
#include<windows.h>

int main()
{
    char arr1[]="hello world";
    char arr2[]="###########";

    int left = 0;
    int right = strlen(arr1)-1;//计算长度strlen-#include<string.h>

    while(left <= right)
    {
        arr2[left] = arr1[left];
        arr2[right] = arr1[right];//根据输出效果来看，主要输出语句为arr2，所以将arr1的值全部赋予arr2
        printf("%s\n",arr2);
        Sleep(1000);//休息一秒——Sleep(毫秒)-#include<windows.h>
        system("cls");//执行系统命令的一个函数-cls-清空屏幕-#inlcude<stdlib.h>
        left++;
        right--;
    }
    printf("%s\n",arr1);
    system("pause");
    return 0;
}
