# DataStructures

1) Arrays
Memory representations
    Each box is 1Byte in memory int[] takes 4Byte to store one int value. 
    if int[] is having 5 values then int[5] needs 20 Bytes to store entire array.
      |..||||||||||||..|
      |--|-|-|-|-|-|-|-|-|-|-|-|--|
      
      ```
      int[2] = {5,6};{0000000000000101,0000000000000110}
      ```
      int value are first converted as binaries inorder to get stored in memory. Any info should be converted as binary to get stored in memmory.
      |..|||||||||..|
      |--|-|-|-|-|-|-|-|-|--|
      |--|0000|0000|0000|0101|0000|0000|0000|0110|--|
      |Ad|100|101|102|103|104|105|106|107|--|
      
      Totally 8 bytes to store int[2];
      
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
      
        |-|C1|c2|c3|
        |-|--|--|--|
        |R1|1|2|3|
        |R2|4|5|6|
        |R3|7|8|9|
        
    Memory Representation[single dimention since the memory is an tap which contain sequential bytes]:
    
    |..||||||||||||..|
    |--|-|-|-|-|-|-|-|-|-|-|-|--|
    |--|1|2|3|4|5|6|7|8|9|-|-|--|
    
         * Row major representation [default] int[] a[2][2] = { {a[0][0],a[0][1]},{a[1][0],a[1][1]}}; =>{1,2,3,4,5,6,7,8,9}=> {{1,2,3},{4,5,6},{7,8,9}};
         * Column major representation a[3][3] ={{1,4,7},{2,5,8},{3,6,9}};

2) Linked List
    * Sinle Linked List
    * Double Linked List
