# Monte Carlo Sales Forecast

Mini project (No. 59) for BBA (AI), Symbiosis Artificial Intelligence Institute.

A Python program that simulates thousands of possible monthly sales outcomes to estimate expected revenue and the risk of missing a target.

## Features
- Simulates 10,000 months (adjustable) using random units sold and random price
- Calculates mean, median and standard deviation (risk)
- Finds worst case (5th percentile) and best case (95th percentile)
- Shows the chance of reaching your revenue target
- Text histogram of outcomes
- Input validation, with defaults for every field
- Two versions: command line and a tkinter GUI

## Concepts Used
- `random` module (`random.gauss`)
- `statistics` module (`mean`, `median`, `stdev`)
- Functions, loops and list comprehensions
- `tkinter` (GUI version)

## How It Works
1. Enter expected units, units uncertainty, average price, price uncertainty, target and number of simulations.
2. Each simulation picks random units and a random price. Revenue = units x price.
3. The program repeats this thousands of times and summarises the results.

## Files
| File | Description |
|------|-------------|
| `monte_carlo_sales_forecast.py` | Command-line version |
| `monte_carlo_gui.py` | tkinter GUI version |

## Run
```bash
python monte_carlo_sales_forecast.py
python monte_carlo_gui.py
```
No extra libraries needed.

## Sample Output
```
Expected revenue (mean) : Rs. 99,671
Risk (std deviation)    : Rs. 17,586
Worst case (5th pct)    : Rs. 71,727
Best case (95th pct)    : Rs. 129,468
Chance of hitting Rs. 100,000 : 47.6%
```

## Author
Priyanshu, BBA (AI), SAII Pune
