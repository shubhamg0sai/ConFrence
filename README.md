# ConFrence
A video call confrence application bye using jitsi

# Use pre-build SDK artifacts/binaries
In your project, add the Maven repository https://github.com/jitsi/jitsi-maven-repository/raw/master/releases and the dependency org.jitsi.react:jitsi-meet-sdk into your build.gradle files.

The repository typically goes into the build.gradle file in the root of your project:

build.gradle
```
allprojects {
    repositories {
        maven {
            url "https://github.com/jitsi/jitsi-maven-repository/raw/master/releases"
        }
        google()
        mavenCentral()
        maven { url 'https://www.jitpack.io' }
    }
}
```





# Using the API
Jitsi Meet SDK is an Android library which embodies the whole Jitsi Meet experience and makes it reusable by third-party apps.

First, add Java 1.8 compatibility support to your project by adding the following lines into your build.gradle file:
build.gradle

```
compileoptions {
    sourcecompatibility javaversion.version_1_8
    targetcompatibility javaversion.version_1_8
}
```




