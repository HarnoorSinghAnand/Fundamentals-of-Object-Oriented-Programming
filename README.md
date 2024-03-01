# Fundamentals-of-Object-Oriented-Programming
1.	In the field of programming, Iteration Statements are helpful when we need a specific task in repetition. They’re essential as they reduce hours of work to seconds. An iteration is a sequence of instructions that is continually repeated until a certain condition is reached. As per given statement you need to implement the task using iterations. 
A number is said to be valid if it is divisible by 8. Develop a logic that allows the user to keep entering numbers as long as the input is valid and also displays a count of the valid numbers. 
Sample Input and Output:
Enter the number
8
Enter the number
16
Enter the number
96
Enter the number
6
Total 3 numbers are valid numbers. 

#include <iostream>

using namespace std;

int main() {
    int valid_count = 0;
    int number;
    char choice;

    do {
        cout << "Enter the number: ";
        cin >> number;

        if (number % 8 == 0) {
            valid_count++;
        } else {
            cout << "Invalid number. Please enter a number divisible by 8." << endl;
        }

        cout << "Do you want to enter another number? (yes/no): ";
        cin >> choice;
    } while (choice == 'y' || choice == 'Y');

    cout << "Total " << valid_count << " numbers are valid numbers." << endl;

    return 0;
}
In this program, a do-while loop is used to repeatedly ask the user for input until they decide to stop. Inside the loop, the user is prompted to enter a number. If the number is divisible by 8, the valid_count variable is incremented. If not, an error message is displayed. After each iteration, the user is asked if they want to enter another number. The loop continues as long as the user inputs 'y' or 'Y'. Finally, the program prints the total count of valid numbers entered by the user.





