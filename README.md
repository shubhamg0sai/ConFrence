# ConFrence
A video call confrence application bye using jitsi

Use pre-build SDK artifacts/binaries
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

Dependency definitions belong in the individual module build.gradle files:
```
dependencies {
    // (other dependencies)
    implementation ('org.jitsi.react:jitsi-meet-sdk:+') { transitive = true }
}
```


Jitsi Meet Handbook
Developer GuideMobileAndroid SDK
On this page
Android SDK
The Jitsi Meet Android SDK provides the same user experience as the Jitsi Meet app, in a customizable way which you can embed in your apps.

INFO
Android 6.0 (API level 23) or higher is required.

Sample applications using the SDK
If you want to see how easy integrating the Jitsi Meet SDK into a native application is, take a look at the sample applications repository.

Build your own, or use a pre-build SDK artifacts/binaries
Jitsi conveniently provides a pre-build SDK artifacts/binaries in its Maven repository. When you do not require any modification to the SDK itself or any of its dependencies, it's suggested to use the pre-build SDK. This avoids the complexity of building and installing your own SDK artifacts/binaries.

Use pre-build SDK artifacts/binaries
In your project, add the Maven repository https://github.com/jitsi/jitsi-maven-repository/raw/master/releases and the dependency org.jitsi.react:jitsi-meet-sdk into your build.gradle files.

The repository typically goes into the build.gradle file in the root of your project:

build.gradle
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


Dependency definitions belong in the individual module build.gradle files:

dependencies {
    // (other dependencies)
    implementation ('org.jitsi.react:jitsi-meet-sdk:+') { transitive = true }
}


#Using the API
Jitsi Meet SDK is an Android library which embodies the whole Jitsi Meet experience and makes it reusable by third-party apps.

First, add Java 1.8 compatibility support to your project by adding the following lines into your build.gradle file:
```
compileOptions {
    sourceCompatibility JavaVersion.VERSION_1_8
    targetCompatibility JavaVersion.VERSION_1_8
}
```


