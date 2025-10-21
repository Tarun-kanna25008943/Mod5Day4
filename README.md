# EX-04 Program to Count Alphabets, Digits, and Special Characters in a String

## AIM:
To write a C program that counts and displays the total number of alphabets, digits, and special characters present in a given string.

## ALGORITHM:

1. Start
2. Read a string ch.
3. Initialize alpha = 0, digit = 0, splch = 0.
4. For each character in the string:
    * If it’s an alphabet → alpha++
    * Else if it’s a digit → digit++
    * Else → splch++
5. Print the values of alpha, digit, and splch.
6. Stop

## PROGRAM:
```
#include <stdio.h>
#include <string.h>
#include <ctype.h>

int main()
{
    char ch[100];
    scanf("%[^\n]%*c",ch);
    int len = strlen(ch);
    int alpha = 0,digit = 0,splch = 0;
    for(int i = 0; i < len; i++)
    {
        if(isalpha(ch[i]))
        {
            alpha++;
        }
        else if(isdigit(ch[i]))
        {
            digit++;
        }
        else
        {
            splch++;
        }
    }
    printf("Number of Alphabets in the string is : %d\n",alpha);
    printf("Number of Digits in the string is : %d\n",digit);
    printf("Number of Special characters in the string is : %d",splch);
}
```

## OUTPUT:
<img width="674" height="168" alt="image" src="https://github.com/user-attachments/assets/97ae6e33-58a1-4b29-b45e-5adb132d2710" />

## RESULT:
The program successfully counts and displays the total number of alphabets, digits, and special characters in a given string.
