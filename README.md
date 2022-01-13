# Module 8 Lab Guide (part 2)
## Getting Started
[Lab Introduction Video](https://youtu.be/4qre8IRmaUw)

## Lab Activity 2 - Dynamic Die
### Problem Description
In this activity, you will using the Die class and the DieButton class that we developed in the deeper look videos. This is an example of code reuse which is core principle of Object Oriented Programming. For this activity you will create a class named DynamicDie that will enable the end-user to customize both the skin and the number of sides of a single DieButton. Three custom die face image sets (skins) have been provided for up to 20 sides on a single die. They are called Triangle, Diamond and Honeycomb and you can find them in the A1-DynamicDie folder.

<img src="images/Lab08-DynamicDie.png" alt="Dynamic Die Screenshot">

### Requirements
The screenshot above shows a sample GUI for this activity.  You may use the same layout or design your own.  Either way, your GUI must contain the following components

+ **DieButton:** You must include a single die button that roles when clicked.  When the program begins, the DieButton should have 6 sides and use the Triangle skin.
+ **JButton:** You must include a JButton that will role the die when clicked.
+ **JButton:** You must include a JButton that will reconfigure the exiting DieButton by first removing it from the parent panel, creating a new DieButton object with the specified number of sides and skin, then adding it back to the parent panel.  This button will also need to *revalidate* and *repaint* the parent panel to ensure the updated DieButton is displayed properly.
+ **JComboBox:** You must include a JComboBox that will allow the user to chose one of the three available skins from a dropdown list.
+ **JTextField:** You must include a JTextField to allow the user to type in the number of sides they want for their die.  Valid values are in the range of 2 through 20.  See the error handling section below for how to address unexpected values.
+ **JLabel:** You must include a JLabel that contains the text "Style" and position it near the JComboBox.
+ **JLabel:** You must include a JLabel that contains the text "Sides" and position it near the JTextField.

### Error Handling
When the reconfigure JButton is pressed, it will read the current values from the JTextField and the JComboBox.  If the user specified a non-integer value for the number of sides, you should catch the NumberFormatException and display a JOptionPane with the message "Please enter an integer value!".  If the user specified an integer value outside of the valid range [2 - 20], display a JOptionPane with the message "Please enter values in the range of 2 - 20 inclusive!".

### Implementation Guide
1. Expand the folder named A1-DynamicDie and create a new file named DynamicDie.java
2. Copy Die.java and DieButton.java from the [Mod08 Code Examples](https://github.com/lhindman/cs121-mod08-examples.git) into the A1-DynamicDie folder.
3. Design a program to satisfy the requirement in the Problem Description and enter the program code in DynamicDie.java
4. Test the program and pay particular attention to boundary/edge cases and invalid input.
5. Commit the changes to your local repository with a message stating that Activity 1 is completed.
6. Push the changes from your local repository to the github classroom repository.

## Coding Journal (Optional)
Keep a journal of your activities as you work on this lab. Many of the best engineers that I have worked with professionally have kept some sort of engineering journal. I personally packed notebooks around with me for nearly 8 years before I began keeping my notes electronically.   

Your journal can track ideas, bugs, cool links, code snippets, shell commands, rants, or simply a reflection on what worked well or not-so-well with this lab activity. I will not be grading the content of your journal, but I will expect at least two timestamped journal entries of at least a 75 to 150 words each added to the provided Journal.md file.  The purpose of this component is to help develop the habit of taking notes and creating documentation while you code. The more detail you provide the better as that will help you if you ever need to refer back to this project in the future.

## Markdown Resources
Markdown is a notation that is used to format text documents.  It is widely used in Software Development shops around the world, which is why we're asking you to use it in your lab documentation.  

Github provides a guide for getting started:  [Mastering Markdown](https://guides.github.com/features/mastering-markdown/)
