//C program for implementation of Buvvle sort
#include <stdio.h>

void
swap (int *xp, int *yp)
{
  int temp = *xp;
  *xp = *yp;
  *yp = temp;
}


void
bubbleSort (int arr[], int n)
{
  int i, j;
  for (i = 0; i < n - 1; i++)
    {
      printf (" Outer loop step %d ", i);
      printArray (arr, n);
      //Last i elements already in place
      for (j = 0; j < n - i - 1; j++)
	{
	  printf (" Inner loop step %d before decision  ", i);
	  printArray (arr, n);
	  if (arr[j] > arr[j + 1])
	    {
	      swap (&arr[j], &arr[j + 1]);
	    }
	  printf (" Inner loop step %d  after decision", i);
	  printArray (arr, n);
	}
      printf
	("==============================================================\n");
    }
}

/*Funcition to print an array */
void
printArray (int arr[], int size)
{
  int i;
  for (i = 0; i < size; i++)
    printf ("%d ", arr[i]);
  printf ("\n");
}

//Driver program to test aboce functions

int
main ()
{
  int arr[] = { 64, 34, 25, 12, 22, 11, 90 };
  int n = sizeof (arr) / sizeof (arr[0]);
  printf ("Nonsorted array: \n");
  printArray (arr, n);

  bubbleSort (arr, n);

  printf ("Sorted array: \n");
  printArray (arr, n);
  return 0;
}
