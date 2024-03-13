# [JSL02] Submission: Debug the DOM

You will: 
1. Use the Starter Code Repo, 
2. Code your solution,
3. Commit changes to your repo
3. Submit GitHub Repo Link to LMS [JSL02] Submission Project Tab

# Debugging Duplicate Goals

**Debugging Brief:**
In the current code, users can add the same fitness goal multiple times, leading to duplicate entries in the goal list. To enhance the user experience and prevent duplicates, you need to implement a check to ensure that the same goal cannot be added more than once. If a duplicate goal is detected, it should NOT be added to the list.

![alt text](JSL02_Solution.png)

**Issue:** Users can add duplicate fitness goals.
**Debugging Task:** Prevent users from adding the same goal more than once.

- The goal is to prevent users from adding duplicate fitness goals to the list.
- You need to check if the goal being added already exists in the list before appending it.
- Display an alert to inform the user if they are trying to add a duplicate goal.
- Focus on the code structure within the function and how to handle duplicates.

**Explanation:**
1. We first retrieve all the existing goals in the `goalList` using `querySelectorAll`.
2. Then, we iterate through each existing goal and compare its text content with the new goal input.
3. If a duplicate is found, we display an alert message and exit the function using `return` to prevent the duplicate goal from being added.
4. If no duplicate is found, we proceed to create and add the new goal as before.

Check out the practice challenges on Scrimba here: https://scrimba.com/playlist/pwVxGLDUW
 Fitness Tracker App




Welcome to the Fitness Tracker App! This app helps you keep track of your workouts, fitness goals, and water intake.


## Features

- **Welcome Message:** Displays a welcome message with today's date.
- **Workout Tracker:** Allows you to input and display your workout routine.
- **Goal Tracker:** Helps you set fitness goals and prevents duplicate goals from being added.
- **Water Intake Tracker:** Tracks your daily water intake.
- **Progress Charts:** Provides updated workout and calorie intake progress.
- **Theme Toggle:** Lets you switch between light and dark themes.
- **Meal Plan Submission:** Allows you to submit your meal plan.

## Usage

1. **Workout Tracker**: Enter your workout routine in the input field and click "Submit".
2. **Goal Tracker**: Set your fitness goals in the input field and click "Submit".
3. **Water Intake Tracker**: Click the "Increase" or "Decrease" buttons to update your water intake.
4. **Theme Toggle**: Click the "Theme Toggle" button to switch between light and dark themes.
5. **Meal Plan Submission**: Fill out the meal plan form and click "Submit".


The code also includes comments with hints for preventing duplicate goals from being submitted and mentions the need to debug to address this issue