package com.example.activity;

import android.os.Bundle;
import android.util.Log;
import androidx.appcompat.app.AppCompatActivity;
import android.view.View;
import android.widget.Toast;

public class MainActivity extends AppCompatActivity {
    String tag= "DialogFragmentExample";

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
    }

    public void showMessage(String message){
        Toast.makeText(getBaseContext(), message, Toast.LENGTH_SHORT).show();
    }

    public void doSelectedItem(int which, boolean isChecked){
        showMessage(AlertDialogFragment.items[which] + (isChecked ? "Seleccionado" : "No seleccionado"));
    }
    public void actionClick(String action){
        showMessage(action + " pushado");
        Log.d(tag, "El usuario seleciono" + action);
    }
    public void onClick(View v){
        AlertDialogFragment dialogFragment = AlertDialogFragment.newInstance("Estas seguro que quieres hacer esto?");
        dialogFragment.show(getSupportFragmentManager(), "dialog");
    }


}
