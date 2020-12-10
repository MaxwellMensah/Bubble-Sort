# Bubble-Sort

Bubble Sort is a simple algorithm which is used to sort a given set of n elements provided in form of an array with n number of elements. Bubble Sort compares all the element one by one and sort them based on their values.

If the given array has to be sorted in ascending order, then bubble sort will start by comparing the first element of the array with the second element, if the first element is greater than the second element, it will swap both the elements, and then move on to compare the second and the third element, and so on.

If we have total n elements, then we need to repeat this process for n-1 times.

## Implementing Bubble Sort Algorithm
Following are the steps involved in bubble sort(for sorting a given array in ascending order):

1. Starting with the first element(index = 0), compare the current element with the next element of the array.
2. If the current element is greater than the next element of the array, swap them.
3. If the current element is less than the next element, move to the next element. Repeat Step 1.


# Code for Bubble Sort

#include<stdio.h> <br/>

int main(){                                                       <br/>

   int count, temp, i, j, number[30];                              <br/>

   printf("How many numbers are u going to enter?: ");                <br/>
   scanf("%d",&count);                                                <br/>

   printf("Enter %d numbers: ",count);                               <br/><br/>

   for(i=0;i<count;i++)                              <br/>
   scanf("%d",&number[i]);                                             <br/>

   /* This is the main logic of bubble sort algorithm 
    */                                                            <br/>
    
   for&nbsp;(i=count-2;i>=0;i--){               <br/>                         
      for(j=0;j<=i;j++){<br/>
        if(number[j]>number[j+1]){<br/>
           temp=number[j];<br/>
           number[j]=number[j+1];<br/>
           number[j+1]=temp;<br/>
        }<br/>
      }<br/>
   }<br/>
<br/>
   printf("Sorted elements: ");                    <br/>
   for(i=0;i<count;i++)                    <br/>
      printf(" %d",number[i]);                    <br/><br/>

   return 0;                             <br/>
}
