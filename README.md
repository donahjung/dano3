#include <stdio.h>

int intpower(int m, int n);
int intlnput(void);

int main(void)
{
 int a, b;
 printf("두개의 정수 입력: ");

 a = intlnput();
 b = intlnput();
 
 printf("결과값 = %d", intpower(a, b));

 getchar(); getchar();
 return 0;
}

int intpower(int m, int n)
{
 int z = 1, i = 1;
 for (i = 1; i <= n; i++)
  z *= m;
 return z;
}

int intlnput(void)
{
 int x;
 scanf_s("%d", &x);
 return x;
} 
