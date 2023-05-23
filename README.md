- 👋 Hi, I’m @Settibathulasuryakumari
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
Settibathulasuryakumari/Settibathulasuryakumari is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
#include<stdio.h>
int fact(int);
int main(){
    int i,r,sum=0,n,num,f;
    printf("enter a number:");
    scanf("%d",&n);
    num=n;
    while(n!=0){
        r=n%10;
        f=fact(r);
        sum=sum+f;
        n=n/10;
    }
    if(num==sum){
    printf("%d is a strong number",num);
    }
    else{
        printf("%d is a weak number",num);
    }
    return 0;
}
int fact(int x){
    int k;
    if(x==0||x==1){
        return 1;
    }
    else
    k=x*fact(x-1);
    return k;
}
