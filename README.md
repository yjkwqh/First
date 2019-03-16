@[TOC](First Test)

# 第一个实验
## 实验要求
验证Activity的生命周期

## 核心代码
···
public class First_Activity extends AppCompatActivity {

    public static final String TAG="MainActivity";
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        Log.d(TAG,"OnCreat");
        setContentView(R.layout.first_layout);
    }

    @Override
    protected void onStart() {
        super.onStart();
        Log.d(TAG,"OnStart");
    }

    @Override
    protected void onPostResume() {
        super.onPostResume();
        Log.d(TAG,"OnResume");
    }

    @Override
    protected void onPause() {
        super.onPause();
        Log.d(TAG,"OnPause");
    }

    @Override
    protected void onStop() {
        super.onStop();
        Log.d(TAG,"OnStop");
    }

    @Override
    protected void onRestart() {
        super.onRestart();
        Log.d(TAG,"OnRestart");
    }

    @Override
    protected void onDestroy() {
        super.onDestroy();
        Log.d(TAG,"OnDestroy");
    }
}
···
## 运行截图
1.进入软件![在这里插入图片描述](https://img-blog.csdnimg.cn/20190316213135859.png)
2.home键退出![在这里插入图片描述](https://img-blog.csdnimg.cn/20190316213719164.png)
3.再次进入软件![在这里插入图片描述](https://img-blog.csdnimg.cn/20190316213753581.png)
4.关闭软件![在这里插入图片描述](https://img-blog.csdnimg.cn/20190316213818325.png)
