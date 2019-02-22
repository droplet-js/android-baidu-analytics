# android-baidu-analytics

[![Build Status](https://cloud.drone.io/api/badges/v7lin/android-baidu-analytics/status.svg)](https://cloud.drone.io/v7lin/android-baidu-analytics)
[ ![Download](https://api.bintray.com/packages/v7lin/maven/baidu-analytics-android/images/download.svg) ](https://bintray.com/v7lin/maven/baidu-analytics-android/_latestVersion)

### snapshot

````
ext {
    latestVersion = '1.0.0-SNAPSHOT'
}

allprojects {
    repositories {
        ...
        maven {
            url 'https://oss.jfrog.org/artifactory/oss-snapshot-local'
        }
        ...
    }
}
````

### release

````
ext {
    latestVersion = '1.0.0'
}

allprojects {
    repositories {
        ...
        jcenter()
        ...
    }
}
````

### usage

android
````
...
android {
    ...
    defaultConfig{
        ...
        manifestPlaceholders = [TENCENT_APP_ID: "${appId}"]
        ...
    }
    ...
}
...
dependencies {
    ...
    implementation "io.github.v7lin:baidu-analytics-android:${latestVersion}"
    ...
}
...
````
