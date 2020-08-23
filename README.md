# MyProject-app-build.gradle
repositories {
    mavenCentral()
}
dependencies {
    //Otras dependencias
    implementation 'com.tappx.sdk.android:tappx-sdk:3.+'
    implementation 'com.google.android.gms:play-services-base:12.0.0'
    implementation 'com.google.android.gms:play-services-ads:12.0.0'
    'com.android.application'

android {
    compileSdkVersion 25
    buildToolsVersion "25.0.2"
    defaultConfig {
        applicationId "com.tappx.samples"
        minSdkVersion 16
        targetSdkVersion 23
        versionCode 512
        versionName "5.12"
    }
    buildTypes {
        release {
            minifyEnabled false
            proguardFiles getDefaultProguardFile('proguard-android.txt'), 'proguard-rules.pro'
        }
    }
}
repositories {
    mavenCentral()
}

dependencies {
    implementation fileTree(dir: 'libs', include: ['*.jar'])
    implementation 'com.tappx.sdk.android:tappx-sdk:3.+'
    implementation 'com.google.android.gms:play-services-base:12.0.0'
    implementation 'com.google.android.gms:play-services-ads:12.0.0'
}
