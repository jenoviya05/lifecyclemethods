# Ex.No:2 To create a HelloWorld Activity using all lifecycles methods to display messages.


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
Program to print the text “Hello World”.
Developed by: JENOVIYA D
Registeration Number : 212225040151
```

## MAINACTIVITY.JAVA

~~~

package com.example.test;

import android.os.Bundle;
import android.widget.Toast;

import androidx.activity.EdgeToEdge;
import androidx.appcompat.app.AppCompatActivity;
import androidx.core.graphics.Insets;
import androidx.core.view.ViewCompat;
import androidx.core.view.WindowInsetsCompat;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast t = Toast.makeText(getApplicationContext(),"onCreate Called", Toast.LENGTH_LONG);
        t.show();

    }
    protected void onStart(){
        super.onStart();
        Toast t = Toast.makeText(getApplicationContext(),"onStart Called", Toast.LENGTH_LONG);
        t.show();
    }
    protected void onRestart(){
        super.onRestart();
        Toast t = Toast.makeText(getApplicationContext(), "onRestart Called", Toast.LENGTH_LONG);
        t.show();
    }
    protected void onPause(){
        super.onPause();
        Toast t = Toast.makeText(getApplicationContext(), "onPause Called", Toast.LENGTH_LONG);
        t.show();
    }
    protected void onResume(){
        super.onResume();
        Toast t = Toast.makeText(getApplicationContext(), "onResume Called", Toast.LENGTH_LONG);
        t.show();
    }
    protected void onStop(){
        super.onStop();
        Toast t = Toast.makeText(getApplicationContext(), "onStop Called", Toast.LENGTH_LONG);
        t.show();
    }
    protected void onDestroy(){
        super.onDestroy();
        Toast t = Toast.makeText(getApplicationContext(), "onDestroy Called", Toast.LENGTH_LONG);
        t.show();
    }


}

~~~

## ACTIVITY_MAIN.XML

~~~

<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:id="@+id/main"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <TextView
        android:id="@+id/textView2"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="WelcometoAndroidStudio"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />
</androidx.constraintlayout.widget.ConstraintLayout>

~~~


## OUTPUT
## onCreate()
<img width="1917" height="1078" alt="Screenshot 2026-10-26 222619" src="https://github.com/user-attachments/assets/2a811455-4e6c-4e81-9114-8ee059f36e3d" />

## onPause()
<img width="1917" height="1078" alt="Screenshot 2026-10-26 222636" src="https://github.com/user-attachments/assets/97a37137-7818-4931-8898-fca00dd29f5a" />

## onStart()
<img width="1917" height="1078" alt="Screenshot 2026-10-26 225957" src="https://github.com/user-attachments/assets/724b0672-6aa5-4d1f-94ae-7779bf860624" />

## onResume()
<img width="1917" height="1078" alt="Screenshot 2026-10-26 230024" src="https://github.com/user-attachments/assets/a40bb48d-fdbc-48aa-9d25-c4c35872a09c" />

## onRestart()
<img width="1917" height="1078" alt="Screenshot 2026-10-26 230213" src="https://github.com/user-attachments/assets/dc6e7e9b-640f-46d4-83dd-86535018b8ec" />

## activity_main.xml
<img width="1917" height="1078" alt="Screenshot 2026-10-26 230247" src="https://github.com/user-attachments/assets/91581e0c-865f-4e10-868a-8a67d006304a" />




## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
