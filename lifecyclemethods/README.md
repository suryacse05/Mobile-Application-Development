# Ex.No:1 To create a HelloWorld Activity using all lifecycles methods to display messages.


## AIM:

To create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio.

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
Program to print the text “Hello World”.
Developed by:NIRANJANA DEVI S
Registeration Number : 212221220036
*/
```

## Activity_main.xml:

<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android" xmlns:app="http://schemas.android.com/apk/res-auto" xmlns:tools="http://schemas.android.com/tools" android:layout_width="match_parent" android:layout_height="match_parent" tools:context=".MainActivity">

~~~
<TextView
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:textSize="40dp"
    android:text="Hello World!"
    app:layout_constraintBottom_toBottomOf="parent"
    app:layout_constraintEnd_toEndOf="parent"
    app:layout_constraintStart_toStartOf="parent"
    app:layout_constraintTop_toTopOf="parent" />
~~~
</androidx.constraintlayout.widget.ConstraintLayout>

## MainActivity.java:

package com.example.myapplication;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle; import android.widget.Toast;

public class MainActivity extends AppCompatActivity {

@Override
protected void onCreate(Bundle savedInstanceState) {
    super.onCreate(savedInstanceState);
    setContentView(R.layout.activity_main);
    Toast toast = Toast.makeText(getApplicationContext(), "onCreate Called", Toast.LENGTH_LONG);
    toast.show();
}
protected void onStart() {
    super.onStart();
    Toast toast = Toast.makeText(getApplicationContext(), "onStart Called", Toast.LENGTH_LONG);
    toast.show();
}
@Override
protected void onRestart() {
    super.onRestart();
    Toast toast = Toast.makeText(getApplicationContext(), "onRestart Called", Toast.LENGTH_LONG);
    toast.show();
}
protected void onPause() {
    super.onPause();
    Toast toast = Toast.makeText(getApplicationContext(), "onPause Called", Toast.LENGTH_LONG);
    toast.show();
}
protected void onResume() {
    super.onResume();
    Toast toast = Toast.makeText(getApplicationContext(), "onResume Called", Toast.LENGTH_LONG);
    toast.show();
}
protected void onStop() {
    super.onStop();
    Toast toast = Toast.makeText(getApplicationContext(), "onStop Called", Toast.LENGTH_LONG);
    toast.show();
}
protected void onDestroy() {
    super.onDestroy();
    Toast toast = Toast.makeText(getApplicationContext(), "onDestroy Called", Toast.LENGTH_LONG);
    toast.show();
}
}

## OUTPUT

![image](https://github.com/suryacse05/Mobile-Application-Development/assets/141748873/19c0e4a3-a6ae-40aa-aac6-eab5334e2f28)

![image](https://github.com/suryacse05/Mobile-Application-Development/assets/141748873/813e965a-5b31-4688-b596-635efc9e1665)

![image](https://github.com/suryacse05/Mobile-Application-Development/assets/141748873/03130827-7b91-4c3f-9944-e154e270eccb)

![image](https://github.com/suryacse05/Mobile-Application-Development/assets/141748873/eee95dd7-bbda-43c2-a2ea-e4577dbaf367)

![image](https://github.com/suryacse05/Mobile-Application-Development/assets/141748873/3dbc53d7-b123-4fe2-91c5-aa3116d1ffbd)

![image](https://github.com/suryacse05/Mobile-Application-Development/assets/141748873/286e4cc4-f87f-4c4c-9fe6-f8be47c67303)

![image](https://github.com/suryacse05/Mobile-Application-Development/assets/141748873/60158562-29bb-47c6-b3df-573363ef8489)

![image](https://github.com/suryacse05/Mobile-Application-Development/assets/141748873/9d44693b-a220-4d87-b3de-e899f7ff0e20)

![image](https://github.com/suryacse05/Mobile-Application-Development/assets/141748873/1058718d-7e62-4c06-b0d6-9880166a056c)

![image](https://github.com/suryacse05/Mobile-Application-Development/assets/141748873/0bc22ce3-3320-46bd-ab5b-2a4c9f7b5559)

![image](https://github.com/suryacse05/Mobile-Application-Development/assets/141748873/ab1659a1-32f5-4b1d-944e-e767693d6e0c)

![image](https://github.com/suryacse05/Mobile-Application-Development/assets/141748873/5a68a47c-e367-46f3-b12b-d3c17e05fbf2)

![image](https://github.com/suryacse05/Mobile-Application-Development/assets/141748873/f21f5d20-add8-4aec-badf-37391f322ca6)

![image](https://github.com/suryacse05/Mobile-Application-Development/assets/141748873/d12fee05-b656-4221-9b3f-2650a1395e31)

![image](https://github.com/suryacse05/Mobile-Application-Development/assets/141748873/4b77f154-d484-47e1-9c98-ba72d01f7b30)

![image](https://github.com/suryacse05/Mobile-Application-Development/assets/141748873/651328f4-3f38-49a7-b98b-f6d8d889805d)



## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
