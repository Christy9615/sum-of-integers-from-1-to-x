# sum-of-integers-from-1-to-x
Lab Practice 10/11/2016

#include <iostream>

using namespace std;

int main() 
{
    // Declare x, sum, n are integer
    int x, sum, n;
    
    // Prompt for a positive value for x
    cout << "please enter a positive integer of x"<< endl;
    cin >> x;
    
    while(x<0)
    {
        // if x is less than 0, output error message and ask user to enter
        // another positive integer for x and store in x 
        cout <<"Error Message, please enter a positive integer"<< endl;
        cin >> x;
    }
    
    // Assign 0 to sum and 1 to n
    sum=0;
    n=1;
    
    // while loop to sum all integers from 1 to x, the variable n is our loop 
    // counter that will increment by 1 each time through the loop until n>x
    while(n<=x)
    {
        // sum is assigned to sum + n
        sum+=n;
        // increment n by 1
        n+=1;
        // if problem requires count down, we have to have control variable
        // be increment or decrement, so there are true false judgment for while
    }
    
    // Output the sum from 1 to x, which is the variable store in sum
    cout << "sum of all integers from 1 to " << x << " is " << sum << endl;

    return 0;
}

