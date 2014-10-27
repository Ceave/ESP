
#include <stdio.h>

//Initialisierung
int matrklNr = 1014203;
int count=2;
int backCount=2;

//Execute
main()
{
  while(count<=9)
  {
    if (matrklNr >= 0)
    {
      printf("%9d * %d \n", matrklNr, count);
      matrklNr*=count; 
    } 
    else 
    {
      printf("An overflow has occurred!");
      return(0);
    }
    count++;
  }
  
  while(backCount <= 9)
  {
    printf("%9d / %d \n", matrklNr, backCount);
    matrklNr/=backCount;
    backCount++;
  }
  printf("%9d \n", matrklNr);
  return 0;
}
