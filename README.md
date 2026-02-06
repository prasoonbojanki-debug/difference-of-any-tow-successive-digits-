# difference-of-any-tow-successive-digits-
#include<stdio.h>
int main(){
	int x,y,n,count=0,k=1,difference=0,c=0;
	printf("enter the no:");
	scanf("%d",&x);
	printf("enter the digit:");
	scanf("%d",&n);
	y=x;
	while(y!=0){
		y=y/10;
		count =count+1;
	}
	for(int i=1;i<=count;i++){
		int a=x%10;
		int b=k*a;
		if(i==n){
			difference=b-difference;
		}
		if(i==(n+1)){
			difference=b-difference;
		}
		k=k*10;
		x=x/10;
	}
	printf("%d",difference);
	return 0;
}

