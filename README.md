# BUV Best Daily Calorie Calculator
# Overview 
The Daily Calorie Calculator is A Python-based application designed to estimate a user's daily calorie requirements.
# Feature 
- Calculates Basal Metabolic Rate (BMR)
- Estimates Total Daily Energy Expenditure (TDEE)
- Provides calorie recommendations based on personal goals
- Supports 5 different activity levels
- Supports weight loss, weight gain, and maintenance goals
- Validates user input
- Handles invalid numerical input
- Requests users to re-enter invalid information
# How to Run
1. Download or clone the project files.
2. Open the Python source code in your preferred Python development environment.
3. Run the program.
4. Enter the required personal information such as age, weight(kg), and height(cm).
```python
age = int(input("Enter your age (13-120): "))
weight = float(input("Enter your weight (kg): "))
height = float(input("Enter your height (cm, 50-249): "))
```
5. Select your activity level.
```python
while not flag2:
    print("Activity Level: 1-Sedentary, 2-Light, 3-Moderate, 4-Active, 5-Very Active")
    activity_level = input("Choose (1-5): ")
    if activity_level == "1":
        tracker = activity(1.2)
        flag2 = True
    elif activity_level == "2":
        tracker = activity(1.375)
        flag2 = True
    elif activity_level == "3":
        tracker = activity(1.55)
        flag2 = True
    elif activity_level == "4":
        activity(1.725)
        flag2 = True
    elif activity_level == "5":
        activity(1.9)
        flag2 = True
    else:
        print("Invalid input, Try again")
```
6. select your personal goal.
```python
while not flag3:
    print("Goal: 1-Lose Weight, 2-Gain Weight, 3-Maintain Weight")
    goal = input("Choose (1-3): ")
    if goal == "1":
        daily_calories = tracker - 500
        flag3 = True
    elif goal == "2":
        daily_calories = tracker + 500
        flag3 = True
    elif goal == "3":
        daily_calories = tracker
        flag3 = True
    else:
        print("Invalid input, Try again")
```
7. View your calculated results.
```python
print(f"Your BMR: {bmr:.0f} kcal")
print(f"Your TDEE (maintenance calories): {tracker:.0f} kcal")
print(f"Recommended daily calorie intake: {daily_calories:.0f} kcal")
```
# How It Works

The program follows these main steps:

User Input
    ↓
Input Validation
    ↓
Calculate BMR
    ↓
Select Activity Level
    ↓
Calculate TDEE
    ↓
Select Personal Goal
    ↓
Calculate Recommended Calories
    ↓
Display Results
# Output

After processing the user's information, the program displays:

Your BMR: XXXX kcal
Your TDEE (maintenance calories): XXXX kcal
Recommended daily calorie intake: XXXX kcal
# DEMO

Enter your age (13-120): 17
Enter your weight (kg): 70
Enter your height (cm, 50-251): 175
Gender (male/female)male
Activity Level: 1-Sedentary, 2-Light, 3-Moderate, 4-Active, 5-Very Active
Choose (1-5): 1
2056.5
Goal: 1-Lose Weight, 2-Gain Weight, 3-Maintain Weight
Choose (1-3): 2
Your BMR: 1714 kcal
Your TDEE (maintenance calories): 2056 kcal
Recommended daily calorie intake: 2556 kcal


** Process exited - Return Code: 0 **

