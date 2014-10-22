# Java Tools

## javap 方法签名
F:\Cocos2dSpace\cocos2dx\08_CrossCpp\proj.android>javap -classpath bin/classes -s org.cocos2dx.cpp.Tools
Compiled from "Tools.java"
public class org.cocos2dx.cpp.Tools {
  static {};
    descriptor: ()V

  public org.cocos2dx.cpp.Tools();
    descriptor: ()V

  public static void init(android.content.Context);
    descriptor: (Landroid/content/Context;)V

  public static void showToast(java.lang.String);
    descriptor: (Ljava/lang/String;)V
}


## javah 头文件生成
F:\Cocos2dSpace\cocos2dx\08_CrossCpp\proj.android\src>javah org.cocos2dx.cpp.Tools

About Me
==
a student in ysu