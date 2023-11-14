# Ex.No: 2 To develop an application that uses GUI Components with Fonts and Colors. 
Note: Create button for colors and fonts while clicking color or font button should change 


## AIM:

To create an application that uses GUI Components with Fonts and Colors using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:
```
Step 1: Open Android Studio and then click on File -> New -> New project.
Step 2: Then type the Application name as HelloWorld and click Next.
Step 3: Then select the Minimum SDK as shown below and click Next.
Step 4: Then select the Empty Activity and click Next. Finally click Finish.
Step 5: Design layout in activity_main.xml
Step 6: Display message give in MainActivity file.
Step 7: Save and run the application.
```

## PROGRAM:
```
/*
Program to print the text “GUIcomponent”.
Developed by:dyaneshwaran
Registeration Number :212221040046
*/
```
## ACTIVITYMAIN.XML
```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"

    tools:context=".MainActivity">
    <TextView
        android:id="@+id/textView"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_margin="30dp"
        android:layout_marginTop="296dp"
        android:gravity="center"
        android:text="Hello World!"
        android:textSize="25sp"
        android:textStyle="bold"
        app:layout_constraintBottom_toTopOf="@+id/button1"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.266"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        tools:ignore="MissingConstraints" />
    <Button
        android:id="@+id/button1"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_margin="20dp"
        android:layout_marginBottom="48dp"
        android:gravity="center"
        android:text="Change font size"
        android:textSize="25sp"
        app:layout_constraintBottom_toTopOf="@+id/button2"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.25"
        app:layout_constraintStart_toStartOf="parent"
        tools:ignore="HardcodedText,MissingConstraints,VisualLintButtonSize" />
    <Button
        android:id="@+id/button2"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_margin="20dp"
        android:gravity="center"
        android:text="Change color"
        android:textSize="25sp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.4"
        app:layout_constraintStart_toStartOf="parent"
        tools:ignore="HardcodedText,MissingConstraints,VisualLintButtonSize" />
</androidx.constraintlayout.widget.ConstraintLayout>
```

## MAINACTIVITY.JAVA
```
package com.example.gui;

import android.annotation.SuppressLint;
import android.graphics.Color;
import android.os.Bundle;
import android.widget.Button;
import android.widget.TextView;

import androidx.appcompat.app.AppCompatActivity;
public class MainActivity extends AppCompatActivity {
    int ch=1;
    float font=30;
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        @SuppressLint({"MissingInflatedId", "LocalSuppress"}) final TextView t = findViewById(R.id.textView);
        @SuppressLint({"MissingInflatedId", "LocalSuppress"}) Button b1 = findViewById(R.id.button1);
        b1.setOnClickListener(v -> {
            t.setTextSize(font);
            font = font + 5;
            if (font == 50)
                font = 30;
        });
        @SuppressLint({"MissingInflatedId", "LocalSuppress"}) Button b2 = findViewById(R.id.button2);
        b2.setOnClickListener(v -> {
            switch (ch) {
                case 1:
                    t.setTextColor(Color.RED);
                    break;
                case 2:
                    t.setTextColor(Color.GREEN);
                    break;
                case 3:
                    t.setTextColor(Color.BLUE);
                    break;
                case 4:
                    t.setTextColor(Color.CYAN);
                    break;
                case 5:
                    t.setTextColor(Color.YELLOW);
                    break;
                case 6:
                    t.setTextColor(Color.MAGENTA);
                    break;
            }
            ch++;
            if (ch == 7)
                ch = 1;
        });
    }}
```
## OUTPUT

![image](https://github.com/suryacse05/Mobile-Application-Development/assets/114641798/2a04e597-cf3b-4743-9835-43ce42947983)
![image](https://github.com/suryacse05/Mobile-Application-Development/assets/114641798/c0ec438d-3d0c-4a2c-9049-a31d0b6fc991)
![image](https://github.com/suryacse05/Mobile-Application-Development/assets/114641798/c875d082-657b-4cd7-b4e0-cc000bab7384)





## RESULT
Thus a Simple Android Application that uses GUI Components with Fonts and Colors using Android Studio is developed and executed successfully.


