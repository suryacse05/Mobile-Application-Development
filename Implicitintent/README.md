# Ex.No:3 Develop program to create a text field and a button “Navigate”. When you enter “www.google.com” and press navigate button it should open google page using Implicit Intents.


## AIM:

To create a navigate button using Implicit Intent to display the google page using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:
Step 1: Open Android Stdio and then click on File -> New -> New project.
Step 2: Then type the Application name as HelloWorld and click Next.
Step 3: Then select the Minimum SDK as shown below and click Next.
Step 4: Then select the Empty Activity and click Next. Finally click Finish.
Step 5: Design layout in activity_main.xml.
Step 6: Display message give in MainActivity file.
Step 7: Save and run the application.
## PROGRAM:
```
/*
Program to print the text “Implicitintent”.
Developed by:AGALYA.J
Registeration Number :212221040007
*/
```
## MAINACTIVITY.JAVA
```
package com.example.intent_implementation;
import androidx.appcompat.app.AppCompatActivity;
import android.content.Intent;
import android.net.Uri;
import android.os.Bundle;
import android.view.View;
import android.widget.Button;
import android.widget.EditText;
public class MainActivity extends AppCompatActivity {
Button button;
EditText e1;
@Override
protected void onCreate(Bundle savedInstanceState) {
super.onCreate(savedInstanceState);
setContentView(R.layout.activity_main);
button = findViewById(R.id.button);
e1 = findViewById(R.id.E1);
button.setOnClickListener(view -> {
String url = e1.getText().toString();
Intent i1 = new Intent(Intent.ACTION_VIEW, Uri.parse(url));
startActivity(i1);
});
}
}
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
android:layout_width="wrap_content"
android:layout_height="wrap_content"
android:layout_marginStart="4dp"
android:layout_marginTop="52dp"
android:text="@string/enter_an_url"
android:textSize="26sp"
app:layout_constraintStart_toStartOf="parent"
app:layout_constraintTop_toTopOf="parent"
tools:ignore="ExtraText" />
<EditText
android:id="@+id/E1"
android:layout_width="wrap_content"
android:layout_height="wrap_content"
android:layout_marginTop="120dp"
android:ems="10"
android:inputType="textPersonName"
android:text=""
android:textColor="#2196F3"
app:layout_constraintEnd_toEndOf="parent"
app:layout_constraintHorizontal_bias="0.791"
app:layout_constraintStart_toStartOf="parent"
app:layout_constraintTop_toTopOf="parent" />
<Button
android:id="@+id/button"
android:layout_width="wrap_content"
android:layout_height="wrap_content"
android:layout_marginBottom="484dp"
android:text="Jump Into"
app:backgroundTint="#4CAF50"
app:layout_constraintBottom_toBottomOf="parent"
app:layout_constraintEnd_toEndOf="parent"
app:layout_constraintHorizontal_bias="0.462"
app:layout_constraintStart_toStartOf="parent" />
</androidx.constraintlayout.widget.ConstraintLayout>
```
## OUTPUT
![image](https://github.com/suryacse05/Mobile-Application-Development/assets/117981388/f6668c42-af55-4b1e-bb09-9d06bee97ce0)
![image](https://github.com/suryacse05/Mobile-Application-Development/assets/117981388/aaeef486-4d22-4647-8dc9-730fc1082e17)
## RESULT
Thus a Simple Android Application create a navigate button using Implicit Intent to display the google page using Android Studio is developed and executed successfully.


