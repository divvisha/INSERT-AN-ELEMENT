# EXPERIMENT-7 JAVA PROGRAM TO INSERT AN ELEMENT IN AN ARRAY.

## AIM:
   To write a Java program to insert an element in an Array.

## ALGORITHM:
   1. Open Intelli J application or any other code editor.

   2. Create an array with a name of your choice.

   3. Using Scanner, Input a number or a element from the user.

   4. Using for loop insert the input element at the end of the array.

   5. Display the append array in the terminal.

## PROGRAM:

import java.util.Scanner;<br>
public class Main<br>
{<br>
    public static void main(String[] args)<br>
    {<br>
        int n, pos, x;<br>
        Scanner s = new Scanner(System.in);<br>
        System.out.print("Enter no. of elements you want in array:");<br>
        n = s.nextInt();<br>
        int a[] = new int[n+1];<br>
        System.out.println("Enter all the elements:");<br>
        for(int i = 0; i < n; i++)<br>
        {<br>
            a[i] = s.nextInt();<br>
        }<br>
        System.out.print("Enter the position where you want to insert element:");<br>
        pos = s.nextInt();<br>
        System.out.print("Enter the element you want to insert:");<br>
        x = s.nextInt();<br>
        for(int i = (n-1); i >= (pos-1); i--)<br>
        {<br>
            a[i+1] = a[i];<br>
        }<br>
        a[pos-1] = x;<br>
        System.out.print("After inserting:");<br>
        for(int i = 0; i < n; i++)<br>
        {<br>
            System.out.print(a[i]+",");<br>
        }<br>
        System.out.print(a[n]);<br>
    }<br>
}

## OUTPUT:
<img width="364" alt="java ex7 op" src="https://github.com/divvisha/INSERT-AN-ELEMENT/assets/127508123/d1f8feb3-616d-4806-ae55-6e745b5b217c">

## RESULT:
Thus the program to insert an element in an array has been created and executed successfully. 
