# Challenge 1

## * Part I Automate the calculations

* There are 5 loans in this list
* The total of the loans in this list is 2750
* The average loan amount of the loans in this list is 550.0

## * Part II Analyze loan data

* The future value on the loan is 1000
* The remaining months on the loan is 9
* The fair value of the loan is  861.77
* The loan is worth at least the cost to buy it.

## * Part III Perform financial calculations


### Main Calculator Used
```
def calculate_present_value (future_value, remaining_months, annual_discount_rate):
    present_value = round(future_value / (1 + annual_discount_rate/12) ** remaining_months, 2)
    return present_value 

```
* The present value of the loan is: 820.08

## * Part IV Conditionally filter lists of loans

This is the list of inexpensive loans: 
[{'loan_price': 500, 'remaining_months': 13, 'repayment_interval': 'bullet', 'future_value': 1000}, {'loan_price': 200, 'remaining_months': 16, 'repayment_interval': 'bullet', 'future_value': 1000}]