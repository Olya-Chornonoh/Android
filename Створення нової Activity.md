Для створення нової [[Activity]] необхідно:
1. ***Створити макетний файл*** (каталог */src/main/res/layout*), де задати інтерфейс майбутньої Activity.
   ```xml
   <?xml version="1.0" encoding="utf-8"?>  
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"  
    xmlns:app="http://schemas.android.com/apk/res-auto"  
    xmlns:tools="http://schemas.android.com/tools"  
    android:layout_width="match_parent"  
    android:layout_height="match_parent"  
    tools:context=".MainActivity4">  
  
</androidx.constraintlayout.widget.ConstraintLayout>
```
2. Створити клас [[Activity]].
   ```java
   public class MainActivity4 extends AppCompatActivity {  
  
    @Override  
    protected void onCreate(Bundle savedInstanceState) {  
        super.onCreate(savedInstanceState);  
        setContentView(R.layout.activity_main4);  
    }  
}
```
В класі [[Activity]] необхідно як мінімум перевизначити метод життєвого циклу **onCreate**, де потрібно вказати макетний файл, з яким зв'язується [[Activity]], за допомогою методу **setContentView(R.layout.activity_main4);**
3. Додати опис Activity в файл **[[Android Manifest]]**:
   ```xml
   <activity  
    android:name=".MainActivity4"  
    android:exported="false" />
```

**Замість цих трьох пунктів можна створити [[Activity]] через AndriodStudio. Тоді ці всі пункти виповнить IDE***.
![[Pasted image 20221016223519.png]]
