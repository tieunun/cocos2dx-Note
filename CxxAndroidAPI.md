###C++调用AndroidAPI
JniMethodInfo methodInfo;
//包名，方法名，类型
JniHelper::getStaticMethodInfo(methodInfo,"org/cocos2dx/cpp/Tools","showToast","(Ljava/lang/String;)V");
//jClazzID,jMethodID,值
JniHelper::getEnv()->CallStaticVoidMethod(methodInfo.classID,methodInfo.methodID,JniHelper::getEnv()->NewStringUTF("Hello Java Test"));