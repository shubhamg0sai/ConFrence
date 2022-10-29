# ConFrence
A video call confrence application bye using jitsi

Use pre-build SDK artifacts/binaries
In your project, add the Maven repository https://github.com/jitsi/jitsi-maven-repository/raw/master/releases and the dependency org.jitsi.react:jitsi-meet-sdk into your build.gradle files.

The repository typically goes into the build.gradle file in the root of your project:

build.gradle
'''
* allprojects {
*    repositories {
*        maven {
*            url "https://github.com/jitsi/jitsi-maven-repository/raw/master/releases"
*        }
*        google()
*        mavenCentral()
*        maven { url 'https://www.jitpack.io' }
*    }
*}
'''

Dependency definitions belong in the individual module build.gradle files:
'''
dependencies {
    // (other dependencies)
    implementation ('org.jitsi.react:jitsi-meet-sdk:+') { transitive = true }
}
'''

