<div align="center">

## Binary to decmal<br/>by jheikage

</div>

### Description

Convert Binary to decimal, simple algo. Good for beginners!

### Source Code

#include <iostream>
#include <math.h>
using namespace std;
void main(){
	int val,i,j,x;
	char p[100];
	cout<<"Enter binary:";cin>>p;
	val=0;
	x=2;
	j=0;
	for(i = char_traits<char>::length(p)-1;i > -1;i--){
		x =pow(2,j);
		switch(p[i]){
		case '0':
			x = 0;
			break;
		case '1':
			x = x;
			break;
		default:
			goto out;
			break;
		}
		val += x;
		j++;
	}
	cout<<val<<endln;
out:
	return;
}

