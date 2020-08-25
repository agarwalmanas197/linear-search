# linear-search
Linear Search

Problem: Given an array arr[] of n elements, write a function to search a given element x in arr[].

Examples :

Input : arr[] = {10, 20, 80, 30, 60, 50, 
                     110, 100, 130, 170}
          x = 110;
Output : 6
Element x is present at index 6

Input : arr[] = {10, 20, 80, 30, 60, 50, 
                     110, 100, 130, 170}
           x = 175;
Output : -1
Element x is not present in arr[].

A simple approach is to do linear search, i.e

Start from the leftmost element of arr[] and one by one compare x with each element of arr[]
If x matches with an element, return the index.
If x doesn’t match with any of elements, return -1.

// Java code for linearly searching x in arr[]. 
// If x   is present then return its location, otherwise  
// return -1  

  

class GFG  
{  

public static int search(int arr[], int x) 
{ 

    int n = arr.length; 

    for(int i = 0; i < n; i++) 

    { 

        if(arr[i] == x) 

            return i; 

    } 

    return -1; 
} 

  

public static void main(String args[]) 
{ 

    int arr[] = { 2, 3, 4, 10, 40 };  

    int x = 10; 

      

    int result = search(arr, x); 

    if(result == -1) 

        System.out.print("Element is not present in array"); 

    else

        System.out.print("Element is present at index " + result); 
} 
} 
Output:
Element is present at index 3
The time complexity of above algorithm is O(n).

Linear search is rarely used practically because other search algorithms such as the binary search algorithm and hash tables allow significantly faster searching comparison to Linear search.
