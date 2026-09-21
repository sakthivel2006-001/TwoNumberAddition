


Two Number Addition Android App
AIM
To develop an Android application using Android Studio that accepts two numbers from the user and displays their sum in a result text box.

DESCRIPTION
This application takes two numerical values as input. When the user clicks the ADD button, the application calculates the sum and displays the result.

TECHNOLOGY USED
Android Studio

Java

XML

AndroidX AppCompat

PROGRAM
The main Java logic is implemented in MainActivity.java.

addButton.setOnClickListener(v -> {
    String first = number1.getText().toString();
    String second = number2.getText().toString();

    if (first.isEmpty() || second.isEmpty()) {
        Toast.makeText(this, "Please enter both numbers",
                Toast.LENGTH_SHORT).show();
        return;
    }

    double sum = Double.parseDouble(first)
            + Double.parseDouble(second);

    result.setText(String.valueOf(sum));
});
OUTPUT
Test Case
First Number: 25

Second Number: 35

Summation Result: 60

The application successfully adds the two numbers and displays the result.

STUDENT DETAILS
Name: SAKTHIVEL S

Register Number: 212223220090

NOTE
The image included in this repository is an expected output/reference image. For final academic submission, replace it with a screenshot taken from the application actually running in Android Studio/emulator.
