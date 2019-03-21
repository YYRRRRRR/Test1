# 主要思路 代码及截图

实验一

### 实验代码
改段代码验证了Activity的生命周期
MainActivity.java
```
package com.example.hp.test1;

import android.support.v7.app.AppCompatActivity;
import android.os.Bundle;
import android.util.Log;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Log.i("MainActivityLife","调用onCreate()");
    }
    @Override
    protected void onStart(){
        super.onStart();
        Log.i("MainActivityLife","调用onStart()");
    }
    @Override
    protected void onResume(){
        super.onResume();
        Log.i("MainActivityLife","调用onResume()");
    }
    @Override
    protected void onPause(){
        super.onPause();
        Log.i("MainActivityLife","调用onPause()");
    }
    @Override
    protected void onStop(){
        super.onStop();
        Log.i("MainActivityLife","调用onStop()");
    }

    protected void onDestory(){
        super.onDestroy();
        Log.i("MainActivityLife","调用onDestory()");
    }
    @Override
    protected void onRestart(){
        super.onRestart();
        Log.i("MainActivityLife","调用onRestart()");
    }
}

```
