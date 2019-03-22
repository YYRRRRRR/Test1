## 实验一

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
### 实验截图
#### Helloword截图
(https://img-blog.csdnimg.cn/20190319235917995.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQwOTQ2MDUz,size_16,color_FFFFFF,t_70)
#### 生命周期测试截图
(https://img-blog.csdnimg.cn/20190319113055747.png)
