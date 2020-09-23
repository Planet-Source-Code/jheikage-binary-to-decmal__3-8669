<div align="center">

## Binary to decmal


</div>

### Description

Convert Binary to decimal, simple algo. Good for beginners!
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[jheikage](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/jheikage.md)
**Level**          |Beginner
**User Rating**    |4.0 (16 globes from 4 users)
**Compatibility**  |C, C\+\+ \(general\), Microsoft Visual C\+\+
**Category**       |[Coding Standards](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/coding-standards__3-32.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/jheikage-binary-to-decmal__3-8669/archive/master.zip)





### Source Code

```
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
```

