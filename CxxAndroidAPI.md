###C++����AndroidAPI
JniMethodInfo methodInfo;
//������������������
JniHelper::getStaticMethodInfo(methodInfo,"org/cocos2dx/cpp/Tools","showToast","(Ljava/lang/String;)V");
//jClazzID,jMethodID,ֵ
JniHelper::getEnv()->CallStaticVoidMethod(methodInfo.classID,methodInfo.methodID,JniHelper::getEnv()->NewStringUTF("Hello Java Test"));