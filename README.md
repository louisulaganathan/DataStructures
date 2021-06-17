# DataStructures

1) Arrays
    * 1-D
        * Sorted Array.   Insert an element in middle needs RIGHT shift all other elements. Deletion of an element also needs LEFT shift. Time Complexity @(n-p)
        ```INSERT
        for(i=a.length; i>= pos ; i--) 
        {
          a[i] = a[i-1]
        }
        a[pos-1] = num;
        size++
        
        ```
        * UnSorted Array.  No need of shifting. Swap the position value to the last and insert. Time Complexity @(1). Deletion needs replace last value to position
        ```
        a[a.length] = a[pos-1]; 
        a[pos-1] = num;
        ```
    * 2-D

2) Linked List
    * Sinle Linked List
    * Double Linked List
