package com.example.android.practiceset2;



import android.app.Activity;
import android.os.Bundle;
import android.view.View;
import android.widget.TextView;

/**

 This app displays an order form to order coffee.
 */
public class MainActivity extends Activity {

   String text="Ritik";
   String mobileno="Call " + 123;

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);


    int day1=15;
    int day2=22;
    int day3=18;

       display(day1+day2+(day3/3));

    }
    
        public void display(int i){
        TextView t=(TextView) findViewById(R.id.display_text_view);
        t.setText(""+i);

    }
