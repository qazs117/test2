# test2
1. 1)c언어의 특징
제어구조와 제어문을 가지고 있으며 포인터 사용이 가능하다. 사용자 중심의 고급언어이면서 하드웨어를 직접 제어할 수 있는 저급언어이다.
2)c언어의 장점
이식성이 뛰어나다, 다양성을가진다, 유연성이 좋다, 혼합성을 가진다

2. c언어의 활용
1) 게임프로그래밍
2) 운영체제 및 필수 시스템 개발
3) 모바일

3. #incude<stdio.h>
int main(){
float a=5.2, b=3.5, c;
c= a+b;
printf("%f\n",c);
}

4. #incude<stdio.h>
int main(){
float a=, b=, c;
scanf("%f%f",&a,&b);
c= a+b;
printf("%f\n",c);
}

5.#include<stdio.h> float add(float a, float b){ return(a+b); }
int main(){ float a=5.5, b=8.4;  printf("%f\n", add(a,b)); }

6.#include<stdio.h> #include<stdlib.h> int add(int a, int b) { return a + b; } int main() { int a, b; FILE* fp = fopen("my.txt", "r"); if (fp == NULL) { puts("File not found!!"); exit(0); } fscanf(fp, "%d%d", &a, &b); fclose(fp); printf("%d\n", add(a, b)); }

7.#include<stdio.h>

 int main() {
int i;
const char* c[3] = { "Banana", "Orange", "Kiwi" };
for(i=0;i<3;i++)
printf("%s\n", c[i]);}

8.#include<stdio.h> #include<stdlib.h> int main(int n, char* v[]) { int a, b, c; if (n < 4){ printf("매개변수가 모자라요.\n"); exit(0); } a = atoi(v[1]); b = atoi(v[3]); switch (v[2][0]) { case '*': c = a * b; break; default: break; } printf("%d\n", c); }

9.#include<stdio.h>

struct User {

	
char n[80];
	
int age;

char t[80];

};

void main() {

struct User we[2] = {

{"sdds",18 , "qazs@naver.com"},{"stfe",17 ,"sdwse@naver.com"}
};

printf("%s\t%d\t%s\n", we[0].n, we[0].age, we[0].t);
	printf("%s\t%d\t%s\n", we[1].n, we[1].age, we[1].t);

}

10.#include<stdio.h>

struct User {
	
char n[80];
	
int age;

char t[80];
};

void pr(struct User* we) {

printf("%s %d %s\n", we->n, we->age, we->t);

we++;

printf("%s %d %s\n", we->n, we->age, we->t);

}

int main() {

struct User we[2] = { {"jcshim", 19, "wlsd@naver.com"},{ "jbshim", 20, "sdds@naver.com" } };

pr(we);

}
