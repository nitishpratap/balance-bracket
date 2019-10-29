#include<stdio.h>
#include<string.h>
#include<stdlib.h>
int top =-1;
char stack[50];

void push(char n)
{
    if(top==50)
        printf("Overflow\n");
    else
    {
        top++;
        stack[top]=n;
    }
}
void pop()
{
    char item;



    item=stack[top];
    top--;
    if(top==-1)
        printf("Correct\n");

}
int main()
{
    char arr[50];
    printf("Enter  the string\n");
    gets(arr);
    for(int i=1;i<=strlen(arr);i++)
    {
        if(arr[i]=='(')
            push('(');
        else if(arr[i]==')')
            pop();


}
if(top>=0)
     {
         printf("Incorrect\n");}
}
