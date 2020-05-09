# note7-setDialogTheme
将Activity的主题样式设置为对话框的样式
## 在项目的styles.xml文件中自定义样式：  
```java
<style name="TitleMenuRightDialogStyle" parent="android:Theme.Dialog" >
    <item name="android:windowAnimationStyle">@style/AnimTop2</item>
    <item name="android:windowFrame">@null</item><!--边框-->
    <item name="android:windowIsFloating">true</item><!--是否浮现在activity之上-->
    <item name="android:windowIsTranslucent">true</item><!--半透明-->
    <item name="android:windowNoTitle">true</item><!--无标题--> 
    <item name="android:windowBackground">@android:color/transparent</item><!--背景透明-->
    <item name="android:backgroundDimEnabled">false</item><!--模糊-->        
</style>
```  
## 在相应的activity中应用该them  
```java
<activity android:name=".TestActivity" 
          android:theme="@style/TitleMenuRightDialogStyle">
</activity>  
```
