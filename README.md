#include <stdio.h>
int main()
{
    int decimalnum, remainder, quotient;
    int octalNumber[100], i = 1, j;
     scanf("%d", &decimalnum);
    quotient = decimalnum;
    while (quotient != 0)
      {
          octalNumber[i++] = quotient % 8;
          quotient = quotient / 8;
      }
   for (j = i - 1; j > 0; j--)
        printf("%d", octalNumber[j]);
  return 0;

}
