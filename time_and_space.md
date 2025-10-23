# Time and Space Complexity

- This helps us compare two algorithms
- Resource Consumption
    - Time = How much computational time does the algo take
    - Space = How much memory comsumption does the algo take.

Generally there is a positive linear relationship between time and space, so if a algo takes more time then generally it would take up more space and vice versa.

## Costs

Basic Operations | Costs |
-----------------|-------|
a+b | 1|
a-b | 1|
a>0 | 1|
if..| 1|

Example 
The following function would take 3n+1 as the cost

```python
def fun(n,x):
    counter = n # ---------------- free
    amount = 0  # ---------------- free
    while counter > 0: # --------- n
        amount = amount + x # ---- n
        counter = counter - 1 # -- n
    #----------------------------- 1 for loop exit
    return amount
# Total cost n+n+n+1 = 3n+1
```

## Comparing Paramaters

### Perormance Analysis - Comparing two implementations
- In which language is it implemented
- Processor used, etc.....

### Input Size
- We can consdier the input size, but there would be follwoing issues
    - Some inputs will be better suited to one and not the other
- Consdier the follwing example for insertion sort
    - Best Case = Already sorted array in ascending order
    - Average Case = Average taken from sorting a large number of arrays
    - Worst Case = Array sorted in descending order
