# Question-1-to-10

Question-1
 Python Arithmetic Operators
As the name suggests, Arithmetic Operators are used in Arithmetic (Mathematics) operations.

Let’s assume following two variables:

x = 5
y = 2
Operator	Name & Meaning	Example & Result
+	Addition: Add two operands or unary plus	x + y = 7
–	Subtraction: Subtract right operand from the left	x – y = 3
*	Multiplication: Multiplies two operands	x * y = 10
/	Division: Divides left operand by the right one	x / y = 2.5
%	Modulus – Takes the remainder	x % y = 1
//	Floor division: Division that results into the whole number truncating digits after decimal point	x // y = 2
**	Exponent – left operand raised to the power of right	x**y (5^2) = 25 

                                    Python Relational Operator or Comparison Operator
Relational or Comparison Operators are used to compare the operands on the either side of them.
Operator	Meaning
>	Greater than: Eg. x > y will return true if x is greater than y
<	Less than: Eg. x < y will return true if x is less than y
==	Equal to: Eg. x == y will return true if x is equal to y
!=	Not equal to:eg x != y  will return true 
>=	Greater Than or Equal to: Eg. x >= y will return true if x is greater than or equal to y
<=	Less Than or Equal to: Eg. x <= y will return true if x is less than or equal to y
                                         examples 
x=4
y=6
x>y # check if x is greater than y
x<y # check if x is less than y
x==y # if x is equal to y
x != y # if x is not equal to y  
x >= y # if x is greater than or equal to y   
x <= #  if x is less than or equal to y

                                Python Logical Operators
There are three Python logical operators: and or and not.

Operator	Meaning
and	(x and y) will return true if x and y both are true
or	(x or y) will return true if either of x or y is true
not	(not x) will return true if x is false or will return false if x is true. not reverses or complements the operands
                                                           examples
x=1
y=2
x>2 and y>1 # to get true both condition must be true
x>2 or y>1 # to get true either of x or y must be true
not x<2 # x is less than 2 , which is true , but not will make it false .

                                             Python Assignment Operators
As simple as it sounds assignment operators are used for assigning values to variables.

Operator	Example 	         Meaning
=       	x = 1          	Assigns 1 to x
+=	      x += 1	          x = x + 1
-=	      x -= 1          	x = x – 1
/=	      x /= 1	          x = x / 1
%=	      x %= 1	          x = x % 1
*=      	x *= 1	          x = x * 1
**=	      x **= 1         	x= x ** 1
//=	x //= 1	x = x // 1
                                                        Python Bitwise Operators
Bitwise operators are used to compare (binary) numbers:

Operator	             Name	                            Description
& 	                   AND	                       Sets each bit to 1 if both bits are 1
|	                      OR                         Sets each bit to 1 if one of two bits is 1
 ^	                    XOR	                      Sets each bit to 1 if only one of two bits is 1
~ 	                    NOT	                     Inverts all the bits
<<	               Zero fill left shift	       Shift left by pushing zeros in from the right and let the leftmost bits fall off
>>	               Signed right shift	         Shift right by pushing copies of the leftmost bit in from the left, and let the rightmost bits fall off




Question-2

(a) print('1\n21\n321\n4321')
(b)print('1\n121\n12321\n1234321\n12321\n121\n1')
  # " \n ” indicates that the line ends here and the remaining characters would be displayed in a new line                           
                                or
 (b)n = int(input('Enter no of rows '))
for i in range(1, n+1):
    for j in range(1, n-i+1):
        print(end=' ')
    for j in range (1, i+ 1):
        print(j, end=' ')
    for j in range (i-1, 0, -1):
        print(j, end=' ')
    print()
for i in range (1,n):
    for j in range(1, i+1):
        print(end=' ')
    for j in range (1, n-i):
        print(j, end=' ')
    for j in range (n-i, 0, -1):
        print(j, end=' ')
    print()

Question-4

import math
def func():
    print('table of sin in the range of 0-10 with increament of 0.2')
    for x in range(0,10):
        print(math.sin(x))
        x=x+0.2
    print()
    print('table of cos')
   
    for x in range(0,10):
        print(math.cos(x))
        x=x+0.2
    print()
    print('table of tan')
    
    for x in range(0,10):
        print(math.tan(x))
        x=x+0.2
    print()
func()
 Question-5
 
 def main():
    year=int(input('\nenter year to check it is leap year or not'))
    if (year%4)==0:
       if (year%100)==0:
          if (year%400)==0:
           print('*\nIT IS A LEAP YEAR*')
          else:
              print('*\nIT IA NOT A LEAP YEAR*')
       else:
          print('*\nIT IS NOT LEAP YEAR*')
    else:
        print('*\nIT IS NOT A LEAP YEAR*')
if __name__=='__main__':
    main()
    
Question -6

def square():
    x = int(input("Enter a side of the building  : "))
    print("Area of building is  : ", x*x)
def rectangle():
    l = int(input("Enter Length of the buliding   : "))
    b = int(input("Enter Breadth of the building  : "))
    print("Area of the building is                :  ", l*b)
def circle():
    r = int(input("Enter the radius of building   : "))
    print("Area of the building is                : ",3.14*(r**2) )

print("what is the shape of bulding? ")
print("1) Square? ")
print("2) Rectangle? ")
print("3) Circle? ")

while True:
    choice = int(input("Enter your choice  : "))
    if choice == 1:
        square()
    elif choice == 2:
        rectangle()
    elif choice == 3:
        circle()
    else:
        print("Check the options again and retry : ")
        continue
        
 Question -7
 
while True:
    product = 1
    n = int(input("Enter the number of which u need factorial  : "))
    if n<0:
        print("please only enter a negative number -_- ")
    else:
        for i in range(1,n+1):
            product = product*i
        print(product)
        
 Question-8
 
 def main():
  n=int(input('enter no.:'))
  x=0
  y=1
  z=0
  while(z<=n):
    print(z)
    x=y
    y=z
    z=x+y
if __name__=='__main__':
    main()

Question-9

def reverse_n():
    n = int(input("Enter a number  : "))
    while (n>0):
        a = n % 10
        reverse = reverse * 10 + a
        n = n // 10
    print(reverse, "is the reverse of ",n)  
    
      
def sum_n():
    n = int(input("Enter a number  : "))
    sum =0
    while(n > 0):
        a = n % 10
        sum = sum + a
        n = n // 10

    print(sum, "is the sum of digits of ",n)

reverse_n()
sum_n()

Question-10

def computing_lcm():

   x = int(input("Enter a number       : "))
   y = int(input("Enter another number :"))
   if x > y:
       bigger = x
   else:
       bigger = y

   while(True):
       if((bigger % x == 0) and (bigger % y == 0)):
           lcm = bigger
           break
       bigger += 1

   return lcm

print("The L.C.M. is", computing_lcm())
