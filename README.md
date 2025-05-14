# EX-16-LEFT-SHIFT-OPERATION
Name: Somesh Sanjay V

Register Number: 24002358
## AIM
To write a C Program to perform the basic left shift operation for 44 integer number with 3 shifts.

## ALGORITHM
1.	Start the program.
2.	Assign values of a and b as 44 and 3.
3.	Use left shift operator (<<) and shift the value of a three times.
4.	Display the result.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>

int main() { int num = 44; int shifts = 3;

int result = num << shifts;

printf("Number before left shift: %d\n", num);
printf("Number after left shift by %d positions: %d\n", shifts, result);

return 0;
}
```
## OUTPUT


![WhatsApp Image 2025-05-14 at 09 13 42_b94107c9](https://github.com/user-attachments/assets/1fd9e7b5-8c20-4d67-818f-71e94bb17d00)







## RESULT
Thus the program to perform the basic left shift operation for 44 integer number with 3 shifts has been executed successfully.




 
 


# EX-17-TWO-NUMBERS-ARE-EQUAL-OR-NOT


## AIM

Write a C Program to check whether the two numbers are equal or not using simple if statement.

## ALGORITHM

1.	Start the program.
2.	Read two numbers.
3.	If first number is equal to second number, display both are equal.
4.	Otherwise display both are not equal.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>

int main() { int num1, num2;

printf("Enter the first number: ");
scanf("%d", &num1);

printf("Enter the second number: ");
scanf("%d", &num2);

if (num1 == num2)
{
    printf("The numbers are equal.\n");
}
else
{
    printf("The numbers are not equal.\n");
}

return 0;
}
```

## OUTPUT
 ![WhatsApp Image 2025-05-14 at 09 13 42_06895f59](https://github.com/user-attachments/assets/6b4f305d-541f-4ba9-984c-67f20df6634b)

## RESULT

Thus the program to check whether the two numbers are equal or not using simple if statement has been executed successfully
 
 


# EX-18-STRING-LOWERCASE-CONVERSION
## AIM
Write a C Program to convert the given string into lowercase.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using tolower( ) function convert the given string into its lowercase.
4.	Display the result.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h> #include <ctype.h>

int main() { char str[100];

printf("Enter a string: ");
fgets(str, sizeof(str), stdin); 

for (int i = 0; str[i] != '\0'; i++)
{
    str[i] = tolower(str[i]); 
}

printf("Lowercase string: %s\n", str);

return 0;
}
```

## OUTPUT


![WhatsApp Image 2025-05-14 at 09 13 42_ba241cc3](https://github.com/user-attachments/assets/db042d20-ddf7-4663-8bed-529bf0c9737b)


## RESULT
Thus the program to convert the given string into lowercase has been executed successfully
 
 


# EX-19-COUNT-OF-WORDS-IN-A-STRING
## AIM
Write a C Program to count the total number of words in a given string using do While loop.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using for loop, inspect the string character by character.
4.	Whenever a space is encountered increment count by 1.
5.	Display the result.
6.	Stop the program.

## PROGRAM
```
#include <stdio.h> #include <ctype.h>

int main() { char str[100]; int wordCount = 0, i = 0; int inWord = 0; printf("Enter a string: "); fgets(str, sizeof(str), stdin); do { if (isspace(str[i])) {

        inWord = 0;
    } 
    else if (!isspace(str[i]) && inWord == 0)
    {
       
        wordCount++;
        inWord = 1; 
    }
    i++;
}
while (str[i] != '\0'); 
printf("Total number of words: %d\n", wordCount);

return 0;
}


```
## OUTPUT


![WhatsApp Image 2025-05-14 at 09 13 43_a177a4c1](https://github.com/user-attachments/assets/b0678f7a-b482-48f5-a16d-de13ec464d37)



## RESULT
Thus the program to count the total number of words in a given string using do While loop has been executed successfully
 
 


# EX  -20 -COMPARING TWO STRINGS
## AIM
write a Program to compare two strings without using strcmp().
## ALGORITHM
Step 1: Start the program.
Step 2: Declare two character arrays c1 and c2 of size 100 to store the strings. Also, declare an integer variable
             flag and initialize it to 0, and i for indexing.      
Step 3: Read the first string c1 using scanf("%[^\n]", c1); — this reads input until a newline is encountered 
            (i.e., can include spaces).
Step 4: Read the second string c2 using scanf("%s", c2); — this reads input until a space or newline (i.e., no 
            spaces in the second string).
Step 5: Start comparing characters of both strings from index i = 0.
Step 6: Repeat the following while neither c1[i] nor c2[i] is '\0' (i.e., end of string):
•	If c1[i] is not equal to c2[i], set flag = 1.
•	Increment i by 1.
Step 7: After the loop, check the value of flag:
•	If flag == 0, print "strings are same".
•	Otherwise, print "strings are not same".
Step 8: End the program.

## PROGRAM
```
#include <stdio.h>

int main() { char str1[100], str2[100]; int i = 0, result = 0;

printf("Enter the first string: ");
fgets(str1, sizeof(str1), stdin);

printf("Enter the second string: ");
fgets(str2, sizeof(str2), stdin);

while (str1[i] != '\0' && str2[i] != '\0')
{
    if (str1[i] != str2[i])
    {
        result = 1;
        break;
    }
    i++;
}

if (str1[i] != str2[i])
{
    result = 1; 
}

if (result == 0)
{
    printf("The strings are equal.\n");
} 
else
{
    printf("The strings are not equal.\n");
}

return 0;
}
```

## OUTPUT
![WhatsApp Image 2025-05-14 at 09 13 43_1ec7befe](https://github.com/user-attachments/assets/4d35bc3c-b5e7-4ac2-8bbb-6575ea2a6ffb)

 

## RESULT
Thus the C Program to compare two strings without using strcmp() has been executed successfully.

