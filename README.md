# Ex.No:1  To create a HelloWorld Activity using all lifecycles methods to display messages.

## NAME : SHREYESHKAR SEKAR
## REGISTER NUMBER : 212224220099

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
Developed by: SHREYESHKAR SEKAR
Registeration Number : 212224220099
*/
```

MainActivity.java :
```
package com.example.lifecycleactivity;

import android.os.Bundle;
import android.widget.Toast;
import androidx.activity.EdgeToEdge;
import androidx.appcompat.app.AppCompatActivity;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        EdgeToEdge.enable(this);
        setContentView(R.layout.activity_main);

        Toast toast = Toast.makeText(
                getApplicationContext(),
                "onCreate Called",
                Toast.LENGTH_LONG
        );
        toast.show();
    }

    @Override
    protected void onStart() {
        super.onStart();

        Toast toast = Toast.makeText(
                getApplicationContext(),
                "onStart Called",
                Toast.LENGTH_LONG
        );
        toast.show();
    }

    @Override
    protected void onRestart() {
        super.onRestart();

        Toast toast = Toast.makeText(
                getApplicationContext(),
                "onRestart Called",
                Toast.LENGTH_LONG
        );
        toast.show();
    }

    @Override
    protected void onPause() {
        super.onPause();

        Toast toast = Toast.makeText(
                getApplicationContext(),
                "onPause Called",
                Toast.LENGTH_LONG
        );
        toast.show();
    }

    @Override
    protected void onResume() {
        super.onResume();

        Toast toast = Toast.makeText(
                getApplicationContext(),
                "onResume Called",
                Toast.LENGTH_LONG
        );
        toast.show();
    }

    @Override
    protected void onStop() {
        super.onStop();

        Toast toast = Toast.makeText(
                getApplicationContext(),
                "onStop Called",
                Toast.LENGTH_LONG
        );
        toast.show();
    }

    @Override
    protected void onDestroy() {
        super.onDestroy();

        Toast toast = Toast.makeText(
                getApplicationContext(),
                "onDestroy Called",
                Toast.LENGTH_LONG
        );
        toast.show();
    }
}

```
Activity_main.xml : 
```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:id="@+id/main"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <TextView
        android:id="@+id/textView"
        android:layout_width="113dp"
        android:layout_height="22dp"
        android:text="LifeCycle Activity"
        android:textColor="#C72929"
        android:textColorLink="#1E9BD5"
        app:layout_constraintBottom_toTopOf="@+id/textView3"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.512" />

    <TextView
        android:id="@+id/textView3"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Welcome to Anroid Studio"
        android:textColor="#ABA24D"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.497"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.669" />

</androidx.constraintlayout.widget.ConstraintLayout>



```

## OUTPUT

<img width="1600" height="999" alt="WhatsApp Image 2026-10-29 at 11 05 37 AM (2)" src="https://github.com/user-attachments/assets/b4fe9795-3b93-4312-ac32-455b0d6a0250" />

<img width="1600" height="999" alt="WhatsApp Image 2026-10-29 at 11 05 40 AM (1)" src="https://github.com/user-attachments/assets/b84bbdd4-7bb0-4156-8987-ea0f16843c99" />


## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
