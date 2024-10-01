# Experiment-16
Aim : To study and implement Exceptional Handling in C++.
# Exceptional Handling 
Exception handling in C++ is a mechanism to handle runtime errors or unexpected situations that occur during the execution of a program. These errors can disrupt the normal flow of the program, and exception handling allows the programmer to gracefully handle them without crashing the program.

Key Concepts:
Exception: An exception is an event that occurs during the execution of a program that disrupts its normal flow. Common examples include divide-by-zero errors, invalid array index access, or invalid input.

Throwing an Exception: When an error occurs, an exception is "thrown" using the throw keyword. This transfers control to an appropriate exception handler.

Catching an Exception: The thrown exception is caught using the catch keyword, which is part of a try-catch block. The exception handler catches the exception and defines what should be done to resolve or handle the error.

Try Block: Code that might throw an exception is placed inside a try block. If an exception is thrown, control passes to the catch block.

# CODE :
Experiment 16 (a)
```
// Exceptional Handling 
// Name --> Aditya Agarwal
// PRN --> 23070123162

# include <iostream>
using namespace std;

int main(){
    float n1,n2,ans;
    cout << "Enter the value of numbers 1 & 2 : ";
    cin >> n1 >> n2;
    try{
        if(n2==0){
            throw n2;
        }
        else{
            ans = n1/n2;
            cout << "Answer = " << ans << endl;
        }
    }
    catch(float num){
        cout << "ERROR : Division by " << num << endl;
    }
}
```
OUTPUT :
![image](https://github.com/user-attachments/assets/9da485b1-c786-45c4-911f-8613ce8adb73)

Experiment 16 (b):
```
// Exceptional Handling 

# include <iostream>
using namespace std;

int main(){
    int age;
    cout << "Enter age : ";
    cin >> age;
    try{
        if(age<18){
            throw age;
        }
        else{
            cout << "Age : " << age << endl << "APPROVED" << endl;
        }
    }

    catch(int a ){
        cout << "ERROR: Underage ! ("<< age <<")" << endl;
    }
}
```
OUTPUT :
![image](https://github.com/user-attachments/assets/82a549b4-4a7f-44ac-80d5-626d3003d930)

CONCLUSION :
We have learned and implemented Exceptional Handling in C++ programming .

