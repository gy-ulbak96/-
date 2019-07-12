# 01. 기본 알고리즘

------

### 연습문제 

[Q1]

```} 
int max4(int a, int b, int c, int d){
int max = a;
if (b > max) max = b;
if (c > max) max = c;
if (d > max) max = d;
return max;
}
```

[Q2]

```
int min3(int a, int b, int c){
int min = a;
if (b < min) min = b;
if (c < min) min = c;
return min;
}
```

[Q3]

```
int min4(int a, int b, int c, int d){
int min = a;
if (b < min) min = b;
if (c < min) min = c;
if (d < min) min = d;
return min;
}
```

[Q4]

```
#include <stdio.h>

int median(int a, int b, int c){
if (a >= b)
	if (b > c)
		return b;
	else if (a <= c)
		return a;
	else
		return c;
else if (a < c)
	return c
else if (b < c)
	return b;
else
	return a;
		
}

int main(void)
{
int a, b, c;

printf("세 정수의 중앙 값을 구하자");
printf("median(%d,%d,%d) = %d\n",1,2,3,median(1,2,3));
... #이런 식으로 13개 해당하는 것 작성
return 0;
}
```

[Q5]

if ((b >= a && c <= a) || (b <= a && c >= a) 설명

여기서 (b >= a 및 b <= a)의 판단을 거꾸로 뒤집은 판단이 다음 else 이후에 else if ((a > b && c < b) || (a < b && c > b)라는 식으로 이어집니다.  

첫 번째 if가 성립하지 않는 경우 두 번째 if에서도 같은 판단을 하므로 이 알고리즘은 효율적이지는 않습니다.
