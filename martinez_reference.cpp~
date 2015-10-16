// Name: Mario Martinez
// Date: 10/15/15
// Description: Implemented and tested functions using asserts.


#include <iostream>
#include <cassert>
#include <cstdlib>
#include <cmath>

using namespace std;

// **********************************************************
void sort(int& numA, int& numB, int& numC);
// Summary: Sorts three numbers in increasing order.
// Precondition: Three int values are passed by reference. The values
// are then put in order from smallest to largest.
// Postcondition: The values in each variable are changed to match the order, smallest to largest.
//
// ********************************************************
void numDigits(int  valA, int& n);
// Summary: Determins how many digits are in an integer.
// Precondition: Two parameters are passed into the function.
// One of the those values is a pass by reference.
// Postcondition: The one of those parameters is the assign the number of digits in the integer.
//
// ********************************************************
void computeSphere(double& a, double& v, double r);
// Summary: Calculates the area and volume of a sphere.
// Precondition: The function takes in three parameters.
// Two of the parameters is a pass by reference.
// Postcondition: Computes the area and volume of a sphere and assigns them to the values that were passed by reference.
//
// ********************************************************
void swap(int& A, int& B);
// Summary: It swap the place of two integers.
// Precondition: The function receive two parameters that are passed
// by reference.
// Postcondition: Computes the area and volume of a sphere and assigns them to the values that were passed by reference.
//

int main()
{
    const double E = 0.001;
    int numA = 5;
    int numB = 1;
    int numC = 100;
    int n = 0;
    double a = 0, v = 0, r = 5.0, r1 = 4.2;
    int a1, b1;
    int A = 1;
    int B = 3;
    
    //Test case for sort
    sort(numA, numB, numC);
    assert(numA == 1 );
    assert(numB == 5);
    assert(numC == 100);
    
    //Test case for numDigits
    numDigits(numC, n);
    assert(n == 3);
    numDigits(numA, n);
    assert(n == 1);
    
    //Test case for computeSphere
    computeSphere(a, v, r);
    assert(fabs(a - 523.583) < E);
    assert(fabs(v - 314.15) <  E);
    computeSphere(a, v, r1);
    assert(fabs(a - 310.329) < E);
    assert(fabs(v - 221.664) < E);
    
    //Test case for swap
    swap(A, B);
    assert(A == 3 && B == 1);
    A = 5, B = 19;
    swap(A, B);
    assert(A == 19 && B == 5);
    
    return 0;
}

void sort(int& numA, int& numB, int& numC)
{
    assert(numA >= 0 && numA <= 100);
    int temp;
    
    if(numA > numB)
    {
        temp = numB;
        numB = numA;
        numA = temp;
    }
    
    if(numA > numC)
    {
        temp = numC;
        numC = numA;
        numA = temp;
    }
    
    if(numB > numC)
    {
        temp = numB;
        numB = numC;
        numC = temp;
    }
    return;
}

void numDigits(int  valA, int& n)
{
    assert(valA >= -10000 && valA <= 10000);
    
    if (valA < 0)
    {
        valA = valA * -1;
    }
    
    if(valA < 10)
    {
        n = 1;
    }
    
    else if(valA < 100)
    {
        n = 2;
    }
    
    else if(valA < 1000)
    {
        n = 3;
    }
    else if(valA < 10000)
    {
        n = 4;
    }
    
    else
    {
        n = 5;
    }

}

void computeSphere(double& a, double& v, double r)
{
    assert(r >= 0 && r <= 10000);
    const double PI = 3.1415;
    a = (4.0/3.0) * PI * r * r * r;
    v = 4* PI * r * r;
}

void swap(int& A, int& B)
{
    assert(A >= 0 && B >= 0);
    int temp = A;
    A = B;
    B = temp;
}
