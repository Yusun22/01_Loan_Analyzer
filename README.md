# Challenge 1
Background: I work for a lending startup engaged in microcredit loans. The company needs help valuing these loans. In this Challenge, I will automate a process that does just that.

## * Part I Automate the calculations
In this part of the Challenge, the goal is to use loops and variables to automate the calculations for the loan portfolio summaries. Below is a summary of the loan portfolio using the len and sum functions. 

* There are 5 loans in this list
* The total of the loans in this list is $2,750.00
* The average loan amount of the loans in this list is $550.00

## * Part II Analyze loan data
In this part of the Challenge, the goal is to use more detailed data for one of these loans to calculate present value (i.e., fair price), of what this loan would be worth.

The monthly version of the present value formula was used where the discount rate was set to 20%:

Present Value = Future Value / (1+ Annual_Discount_Rate/12)**Months

* The future value on the loan is $1000.00
* The remaining months on the loan is 9
* The fair value of the loan is  $861.77
* The loan is worth at least the cost to buy it.

## * Part III Perform financial calculations
The goal of this section is to create a financial function to calculate new loans for the company. 

### Main Calculator Used
```
def calculate_present_value (future_value, remaining_months, annual_discount_rate):
    present_value = round(future_value / (1 + annual_discount_rate/12) ** remaining_months, 2)
    return present_value 

```
* The present value of the loan is: $820.08

## * Part IV Conditionally filter lists of loans
The goal here is to loop through a series of loans that the company is considering and filter them to find the inexpensive ones, which is defined as loan price less than or equal to $500. 

This is the list of inexpensive loans: 
[{'loan_price': 500, 'remaining_months': 13, 'repayment_interval': 'bullet', 'future_value': 1000}, 
{'loan_price': 200, 'remaining_months': 16, 'repayment_interval': 'bullet', 'future_value': 1000}]
