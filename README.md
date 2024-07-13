
# Fuzzy Logic Implementation for Restaurant Tipping System
This repository contains Python code that implements a fuzzy logic system using scikit-fuzzy to estimate the appropriate tip percentage based on three input variables: food quality, service quality, and ambiance.
## Dependencies
Make sure you have scikit-fuzzy installed:## Usage
1. Clone the repository:
   
 2. Run the fuzzy logic simulation:
Open the Python script restaurant_tipping_fuzzy.ipynb and execute it. Ensure you have Python and the necessary libraries installed.

## Input Variables:
- Food Quality: Ranges from 0 to 10, defining the quality of the food.
- Service Quality: Ranges from 0 to 10, indicating the quality of service provided.
- Ambiance: Ranges from 0 to 10, representing the quality of the restaurant's atmosphere.

## Output:
- Tip Percentage: Ranges from 0 to 30, indicating the recommended tip percentage based on the fuzzy logic rules.

## System Overview
The system uses triangular membership functions for both input and output variables. It defines 12 rules to determine the appropriate tip based on different combinations of food quality, service quality, and ambiance.

## Example Usage
```python
tipping.input['food_quality'] = 9
tipping.input['service_quality'] = 9
tipping.input['ambiance'] = 9
tipping.compute()
print(f"Recommended tip percentage: {tipping.output['tip']:.2f}%")
```
## Visualization
The system includes a visualization of the output variable (tip percentage) which can be displayed using:
```python
tip.view(sim=tipping)
```

