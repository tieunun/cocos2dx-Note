##C++����AndroidAPI
####1.//Jni������Ϣ
JniMethodInfo methodInfo;
####2.//������������������
JniHelper::getStaticMethodInfo(methodInfo,"org/cocos2dx/cpp/Tools","showToast","(Ljava/lang/String;)V");
####3.//jClazzID,jMethodID,ֵ
JniHelper::getEnv()->CallStaticVoidMethod(methodInfo.classID,methodInfo.methodID,JniHelper::getEnv()->NewStringUTF("Hello Java Test"));