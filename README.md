# some-code
some code in c




#include<stdio.h>
int aseries(int);
int bseries(int);
int cseries(int);
int dseries(int);
main()
{
    int n;
    printf("enter the no of terms");
    scanf("%d",&n);
    printf("the series is");
    if(n>0)
    {
        aseries(n);
        bseries(n);
        cseries(n);
        dseries(n);
    }
    else
        printf("invalid no of terms");
}
int aseries(int a)
{
    printf("\n");
    int t1=2,t2=10,t3,i;
    if(a==1)
        printf("%d",t1);
    else if(a>=2)
    {
        printf("%d %d",t1,t2);
        for(i=3; i<=a; i++)
        {
            t3=t2+t2-t1+6;
            printf(" %d",t3);
            t1=t2;
            t2=t3;
        }
    }
}
int bseries(int b)
{
    printf("\n");
    int t1=2,t2=6,t3,i;
    if(b==1)
        printf("%d",t1);
    else if(b>=2)
    {
        printf("%d %d",t1,t2);
        for(i=3; i<=b; i++)
        {
            t3=t2+t2-t1+2;
            printf(" %d",t3);
            t1=t2;
            t2=t3;
        }
    }
}
int cseries(int c)
{
    printf("\n");
    int t1=1,t2=3,t3,i;
    if(c==1)
        printf("%d",t1);
    else if(c>=2)
    {
        printf("%d %d",t1,t2);
        for(i=3; i<=c; i++)
        {

            t3=t2+t2-t1+1;
            printf(" %d",t3);
            t1=t2;
            t2=t3;
        }
    }
}
int dseries(int d)
{
    printf("\n");
    int i;
    for(i=1; i<=d; i++)
        if(i%2==0)
            printf(" %d",i*i);
        else
            printf(" %d",i*i*i);
}
