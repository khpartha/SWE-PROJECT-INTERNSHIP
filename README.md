# AI-Driven PET Production Forecaster and Calculator

Welcome to the AI-Driven PET Production Forecaster and Calculator repository! This project aims to help manufacturers in the plastic industry optimize their plastic (PET) usage and predict future production demands. By leveraging Machine Learning (ML) for forecasting and a PET consumption calculator, users can estimate monthly production requirements, the total PET needed (in grams), and the associated cost (based on a per-gram rate).

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [Usage](#usage)
- [Workflow Description](#workflow-description)
- [Future Enhancements](#future-enhancements)
- [Contributing](#contributing)
 

## Overview

In the plastic manufacturing industry, it’s crucial to accurately forecast production volumes to minimize costs and ensure a steady supply of raw materials. This repository showcases:-
- A Machine Learning model (Linear Regression or Neural Network) to predict monthly production numbers based on historical data.
- A PET Calculator that computes how many grams of PET are required for a single product (e.g., a plastic cup), given its dimensions and thickness.
- A Cost Estimator that multiplies the predicted production requirement by the PET needed per product and a user-defined cost per gram.
The result is a holistic solution to forecast production demand and calculate material requirements in a single step.

## Features

- **User Input:** Dynamically accepts the cup's diameter and height.
- **Accurate Calculations:** Estimates the volume of the cup's walls, bottom, and handle.
- **Material Estimation:** Converts the calculated volume to weight (grams) using the density of PET.
- **Extensible Code:** Clean and well-documented code that can be easily modified or extended.


- **Production Forecasting**
Uses historical data (months and production volumes) to train a model for predicting future production demand.
Demonstrates both scikit-learn (Linear Regression) and TensorFlow (Neural Network) approaches.

- **PET Usage Calculation**
Translates product dimensions (outer radius, inner radius, height, and optional handle dimensions) into an estimated PET weight in grams.
Allows customization of thickness, density, and shape (via geometry formulas).

- **Cost Estimation**
Allows users to set a cost per gram (e.g., 20 rupees/gram).
Quickly derives total monthly cost based on forecasted production.

- **Easy Integration**
Written in Python, a widely used language for AI, data science, and scripting.
Flexible structure that can be adapted to real-world or synthetic data.

- **Visualization**

Generates plots using Matplotlib to visualize both historical production data and model predictions

## Installation

 **Clone the repository:**

   ```bash
   git clone https://github.com/khpartha/PETcal.git
 
``` 
## Usage
Run the Python script from the command line:

 ```bash
  python pet_cup_calculator.py
```

You will be prompted to enter the cup's diameter and height (both in inches). The program will then output the estimated amount of PET required in grams.

**Example Interaction**
 ```python
Enter the diameter of the cup (in inches): 6
Enter the height of the cup (in inches): 6
The estimated amount of PET required: 72 grams
```
## How It Works
- **1. User Input:** The script prompts the user for the cup's diameter and height. 
- **2. User Input:** The cup is modeled as a hollow cylinder for the body.
   
- **3. Weight Estimation:** The total volume is calculated and then converted to weight using the density of PET (approx. 0.050 lb/in³).
Finally, the weight is converted from pounds to grams.
  
The clear modular structure of the code allows for easy maintenance and future expansion of features.

## Contact 
For any questions, suggestions, or contributions, please feel free to contact me at 4khundrakpampartha@gmail.com.




