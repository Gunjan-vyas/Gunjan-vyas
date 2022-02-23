#include<iostream>
#include <stdio.h>      /* printf, scanf, puts, NULL */
#include <stdlib.h>     /* srand, rand */
#include <time.h>       /* time */
#include<algorithm>
using namespace std;
bool isNotrepeating (int s[],int n){
	for(int i=0;i<n;i++){
		for(int j=i+1;j<n;j++)
		{
			if(s[i]==s[j])
			return false;
		}
	}
	return true;
}
int main(){
    
  srand (time(NULL));
    int NumToPredict = rand() % 8999+1000;  // give random number range 
    int s[4];
    do{
	for(int i=0;i<4;i++){
        s[i]=NumToPredict%10;
        NumToPredict=NumToPredict/10;
    }
}while(!isNotrepeating(s,4));
    // for(int i=0;i<4;i++){
    //    cout<<s[i]<<endl;
    // }
    //taking input
      int b[4];
      int n=100;
    do{
    int a;
    cin>>a;
    for(int i=3;i>=0;i--){
        b[i]=a%10;
        a=a/10;
    }
    int count=0;
    for(int i=0;i<4;i++){
        if(b[i]==s[i]){
            count++;
        }
    }
    int sizeb=sizeof(b)/sizeof(b[0]);
    //cout<<" size of b" <<sizeb<<endl;

    if(b[0]==0 && b[1]==0 &&b[2]==0&&b[3]==0){
    cout<<" the number was "<<s[0]<<s[1]<<s[2]<<s[3]<<endl;
	return 0;	
	}
    else if(!isNotrepeating(b,4) || sizeb<3){
    	cout<<" you have given repeating digit or not given 4 digit number "<<endl;
    	continue;
	}
    if(count==4){
        cout<<" ooowho you got it right !!"<<endl;
        break;
        return 0;
    } 
    // BULL Calculation - if match the index 
    int countBull=0;
    for(int i=0;i<4;i++){
        if(b[i]==s[i]){
            countBull++;
        }
    }
    int countC=0;
    for(int i=0;i<4;i++){
        for(int j=0;j<4;j++){
            if(s[i]==b[j] && i!=j){
                countC++;
            }
        }
    }
   // int countcow= countC-countBull;
    cout<<" for given number "<<countC<<" cow "<<" and "<<countBull<<" bull "<<endl;
    n--;
    }while(n>0);
    return 0;
}