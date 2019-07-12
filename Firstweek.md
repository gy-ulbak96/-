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
	return c;
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

숫자가 3개 일 때는 다음과 같은 작성 방법과 실습 1C-1의 복잡도가 비슷하나 숫자가 5개, 7개로 늘어났을 때 다음과 같은 작성 방법을 따른다면 and와 or을 이용하여 따지기 복잡해진다.
