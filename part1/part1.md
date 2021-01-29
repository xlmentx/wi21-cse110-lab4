VARIABLES & SCOPING  
1. What will happen at line 11 and why?   
  var doesn't have scope, so whetever happened to it last remains stored.
  Therefore, the value of prices.length-1 will be printed.  
2. What will happen at line 12 and why?  
  var doesn't have scope, so whetever happened to it last remains stored.
  Therefore, the value of prices[prices.length-1]*(1-discount) will be printed.  
3. What will happen at line 13 and why?  
  var doesn't have scope, so whetever happened to it last remains stored.
  Therefore, the value of the last discountedPrice rounded to two decimal places will be printed.  
4. What will the function return if we call discountPrices([100, 200, 300], .5) ?  
  The function will take the prices and multiply them by 1-discount, then round to two decimal places, 
  and finaly push the results onto dicounted to be returned   
  [100*(1-0.5),200*(1-0.5),300*(1-0.5)]->[50,100,150]->return[50,100,150]  
5. What will happen at line 11 and why?  
  Let is block scoped and i is outside of this line 11's scope. 
  A no such variable Error will occur.  
6. What will happen at line 12 and why?  
  let is also block scoped and discountedPrice does not exist here. 
  A no such variable Error will occur.  
7. What will happen at line 13 and why?  
  let is within scope, so whetever happened to it last remains stored.
  Therefore, the value of the last discountedPrice rounded to two decimal places will be printed.  
8. What will the function return if we call discountPrices([100, 200, 300], .5) ?  
  The function will take the prices and multiply them by 1-discount, then round to two decimal places, 
  and finaly push the results onto dicounted to be returned  
  [100*(1-0.5),200*(1-0.5),300*(1-0.5)] -> [50,100,150] -> return[50,100,150]  
9. What will happen at line 11 and why?  
  Let is block scoped, i is outside of this line 11's scope. 
  A no such variable Error will occur.  
10. What will happen at line 12 and why?  
  const is also block scoped, discountedPrice does not exist here. 
  A no such variable Error will occur.  
11. What will happen at line 13 and why?  
  finalPrice is constant and can not be reassigned like line 7 is trying to do. 
  So assuming the program gets to line 13, 0 would be printed out.  
12. What will the function return for discountPrices([100, 200, 300], .5)?  
  Since finalPrice is a constant set to 0, dicounted.push() will always push 0.
  Since dicounted is constant you can't change it, but you can add to it. 
  Therefore, line 8 will always push 0's and final discount will be [0,0,0].  

DATA TYPES
1. Accessing the value of the name property in the student object  
  student.name  
2. Accessing the value of the Grad Year property in the student object  
  student['Grad Year']  
3. Calling the function for the greeting property in the student object  
  student.greeting()  
4. Accessing the name property of the object in the Favorite Teacher property in student  
  student['Favorite Teacher'].name  
5. Access the first index in the array of the courseLoad property of the student object  
  student.courseLoad[0]  

BASIC OPERATORS & TYPE CONVERSION  

Arithmetic  
  1. [‘3’+2=32]: because the first element is a char, it assumes you want to concatenate the second.  
  2. [‘3’-2=1]: because the second element is subtracted, it assumes both are numbers.  
  3. [3+null=3]: because the first element is a number, it assumes both are numbers.  
  4. [‘3’+null=3null]: because the first element is a char, it assumes you want to concatenate the second.  
  5. [true+3=4]: because the second element is not a boolean, it assumes the first isn't either.  
  6. [false+null=0]: because the second element is not a boolean, it assumes the first isn't either.  
  7. [“3”+undefined=3undefined]: because the first element is a string, it assumes you want to concatenate the second.  
  8. [“3”-undefined=NaN]: because the second element is subtracted, it assumes both are numbers.  
  
Comparison  
  1. [‘2’>1=true]: because the first char is greater than the char of the second.  
  2. [‘2’<‘12’=false]: because the first char is greater than the first char of the second.  
  3. [2==‘2’=true]: because the the first is a number, it assumes the second is also a number.  
  4. [2===‘2’=false]: because both elements are of different type.  
  5. [true==2=false]: because the second element is a number, it assumes true is 1.  
  6. [true===Boolean(2)=true]: because both are of the same type and Boolean(x) returns true for x>0.  

Explain the difference between to == and === operators.  
    == compares equivalance with auto type matching.  
    === compares both type match and value equivalence  

CONDITIONALS
  1. Explain what gets printed and why.  
  2==true is false, so "Hello!" wont be printed.  
  2 is true, so "How are you?" wont be printed.  
  Since 2 was true and "Goodbye" is part of the same ladder, "Goodbye" wont be printed.
  
