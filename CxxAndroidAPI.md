###C++调用AndroidAPI
1.//Jni方法信息
JniMethodInfo methodInfo;
2.//包名，方法名，类型
JniHelper::getStaticMethodInfo(methodInfo,"org/cocos2dx/cpp/Tools","showToast","(Ljava/lang/String;)V");
3.//jClazzID,jMethodID,值
JniHelper::getEnv()->CallStaticVoidMethod(methodInfo.classID,methodInfo.methodID,JniHelper::getEnv()->NewStringUTF("Hello Java Test"));