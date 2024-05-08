# Ex.No:3 Develop program to create a text field and a button “Navigate”. When you enter “www.geeksforgeeks.org” and press navigate button it should open google page using Implicit Intents.

## AIM:

To create a navigate button using Implicit Intent to display the gmail page using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:
Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as ImplicitIntent and click Next.

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Display message give in MainActivity file.

Step 7: Save and run the application.



## PROGRAM:
/*
Program to print the text “Implicitintent”.
Developed by: GANESH S
Registeration Number :21222040042
*/
## ACTIVITY_MAIN.XML
```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <TextView
        android:id="@+id/textView2"
        android:layout_width="233dp"
        android:layout_height="61dp"
        android:layout_marginTop="36dp"
        android:text="IMPLICITY INTENT"
        android:textSize="24sp"
        app:layout_constraintBottom_toTopOf="@+id/editTextText"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.0" />

    <EditText
        android:id="@+id/editTextText"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginBottom="124dp"
        android:ems="10"
        android:inputType="text"
        android:text=""
        app:layout_constraintBottom_toTopOf="@+id/button"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.497"
        app:layout_constraintStart_toStartOf="parent" />

    <Button
        android:id="@+id/button"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginBottom="316dp"
        android:text="Click Here"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent" />
</androidx.constraintlayout.widget.ConstraintLayout>
```
## MAINACTIVITY.JAVA
```
package com.example.implicityintent;

import androidx.appcompat.app.AppCompatActivity;

import android.content.Intent;
import android.net.Uri;
import android.os.Bundle;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Intent intent=new Intent(Intent.ACTION_VIEW);
        intent.setData(Uri.parse("http://www.geeksforgeeks.org/"));
        startActivity(intent);
    }

}
```

## OUTPUT
![MAD 03 2](https://github.com/ganeshshanmugavel27/ImplicitIntent-MAD/assets/122046208/55c36047-ed36-4016-b7e0-bb384962cf5d)
![MAD 03 1](https://github.com/ganeshshanmugavel27/ImplicitIntent-MAD/assets/122046208/893594b7-40d4-4a13-96a2-226236872923)
![MAD EX 03 3](https://github.com/ganeshshanmugavel27/ImplicitIntent-MAD/assets/122046208/97da20ac-5209-42d0-b84c-ea8cd6ddf2d7)





## RESULT
Thus a Simple Android Application create a navigate button using Implicit Intent to display the gmail page using Android Studio is developed and executed successfully.


