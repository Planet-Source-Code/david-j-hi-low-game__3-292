<div align="center">

## Hi\-Low Game


</div>

### Description

A simple guess the number game.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[David J](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/david-j.md)
**Level**          |Beginner
**User Rating**    |4.0 (16 globes from 4 users)
**Compatibility**  |C, C\+\+ \(general\)
**Category**       |[Games](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/games__3-13.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/david-j-hi-low-game__3-292/archive/master.zip)





### Source Code

```
// Hi-Low Program	David Javaheri	2-8-99
#include <stdlib.h>
#include <iostream.h>
#include <time.h>
main()
{
int	num, guess;
srand( (unsigned) time(NULL) ); //Seeds rand()
num=(rand()%100)+1;
cout<<"Guess a number between 1 and 100"<<endl;
cin>>guess;
while(guess!=num)
{
	if(guess<num)
	{
		cout<<"Too Low. Try Again"<<endl;
		cin>>guess;
	}
	if(guess>num)
	{
		cout<<"Too High. Try Again"<<endl;
		cin>>guess;
	}
}
if(guess==num)
{
	cout<<"You Are Correct"<<endl;
}
return 0;
}
```

