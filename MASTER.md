#include<stdio.h>
#include<math.h>
#include<conio.h>
int a,b,n; float ans=0.0;
void sum(void); //prototype declaration
void difference(void);
void multiplication(void);
void division(void);
void log_func(void);
void sine(void);
void cosine(void);
void tangent(void);
void power(void);

void sum()
{
    printf("Enter the first number:");
    scanf("%d",&a);
    printf("Enter the second number:");
    scanf("%d",&b);
    ans=a+b;
    printf("The sum is: %f",ans);
    getche();
    printf("\n");
    main();
}
void difference()
{
    printf("Enter the first number:");
    scanf("%d",&a);
    printf("Enter the second number:");
    scanf("%d",&b);
    ans=a-b;
    printf("The difference is: %f",ans);
    getche();
    printf("\n");
    main();
}
void multiplication()
{
    printf("Enter the first number:");
    scanf("%d",&a);
    printf("Enter the second number:");
    scanf("%d",&b);
    ans=a*b;
    printf("The product is: %f",ans);
    getche();
    printf("\n");
    main();
}
void division()
{
    printf("Enter the first number:");
    scanf("%d",&a);
    printf("Enter the second number:");
    scanf("%d",&b);
    ans=a/b;
    printf("The quotient is: %f",ans);
    getche();
    printf("\n");
    main();
}
void log_func()
{
    printf("Enter the number:");
    scanf("%d",&n);
    ans=log10(n);
    printf("The log value of the entered number is: %f",ans);
    getche();
    printf("\n");
    main();
}
void sine()
{
    printf("Enter the number:");
    scanf("%d",&n);
    ans=sin(n);
    printf("The sine value of the entered number is: %f",ans);
    getche();
    printf("\n");
    main();
}
void cosine()
{
    printf("Enter the number:");
    scanf("%d",&n);
    ans=cos(n);
    printf("The cosine value of the entered number is: %f",ans);
    getche();
    printf("\n");
    main();
}
void tangent()
{
    printf("Enter the number:");
    scanf("%d",&n);
    ans=tan(n);
    printf("The tan value of the entered number is: %f",ans);
    getche();
    printf("\n");
    main();
}

void power()
{
    int power;
    printf("Enter the number:");
    scanf("%d",&n);
    printf("Enter the power value:");
    scanf("%d",&power);
    ans=pow(n,power);
    printf("The answer is: %f",ans);
    getche();
    printf("\n");
    main();
}

int main()
{
    int op;
    printf("1.Sum \n");
    printf("2.Difference \n");
    printf("3.Multiplication \n");
    printf("4.Division \n");
    printf("5.Log \n");
    printf("6.Sine \n");
    printf("7.Cosine \n");
    printf("8.Tangent \n");
    printf("9.Power \n");
    printf("10.Exit \n");
    printf("Enter your option:");
    scanf("%d",&op);
    if(op==1)
        sum();
    else if(op==2)
        difference();
    else if(op==3)
        multiplication();
    else if(op==4)
        division();
    else if(op==5)
        log_func();
    else if(op==6)
        sine();
    else if(op==7)
        cosine();
    else if(op==8)
        tangent();
    else if(op==9)
        power();
    else if(op==10)
            exit(1);
    else
        printf("Invalid option!");
}
