# R-Language
Decision

1. if Statement
The if statement executes a block of code if the condition evaluates to TRUE.
Syntax:
if (condition) {
  # Code to execute if condition is TRUE
}
Example:
x <- 10
if (x > 5) {
  print("x is greater than 5")
}
Output:
[1] "x is greater than 5"
________________________________________
2. if...else Statement
The if...else statement provides an alternative block of code to execute when the condition is FALSE.
Syntax:
if (condition) {
  # Code to execute if condition is TRUE
} else {
  # Code to execute if condition is FALSE
}
Example:
x <- 3
if (x > 5) {
  print("x is greater than 5")
} else {
  print("x is less than or equal to 5")
}
Output:
[1] "x is less than or equal to 5"
________________________________________
3. if...else if...else Statement
This allows you to test multiple conditions in sequence.
Syntax:
if (condition1) {
  # Code if condition1 is TRUE
} else if (condition2) {
  # Code if condition2 is TRUE
} else {
  # Code if none of the conditions are TRUE
}
Example:
x <- 15
if (x < 5) {
  print("x is less than 5")
} else if (x >= 5 & x <= 10) {
  print("x is between 5 and 10")
} else {
  print("x is greater than 10")
}
Output:
[1] "x is greater than 10"
________________________________________
4. switch Statement
The switch statement selects one of many possible blocks of code to execute based on the value of an expression.
Syntax:
switch(expression, 
       case1 = value1,
       case2 = value2,
       ...
       default)
Example:
day <- 3
result <- switch(day,
                 "Monday",
                 "Tuesday",
                 "Wednesday",
                 "Thursday",
                 "Friday",
                 "Saturday",
                 "Sunday")
print(result)
Output:
[1] "Wednesday"
============================================

a<-as.numeric(readline(prompt = "enter a number"))

b<-as.numeric(readline(prompt = "enter a number"))


c<-readline(prompt = "enter the operation sum,sub,mul,div")

result<-switch(c,
               "sum"=a+b,
               "sub"=a-b,
               "mul"=a*b,
               "div"=a/b)
result
________________________________________
5. Vectorized Decision Making with ifelse
The ifelse function is a vectorized way to apply conditions to vectors.
Syntax:
ifelse(test, yes, no)
Example:
x <- c(1, 2, 3, 4, 5)
result <- ifelse(x %% 2 == 0, "Even", "Odd")
print(result)
Output:
[1] "Odd"  "Even" "Odd"  "Even" "Odd"
________________________________________
