# SDP - a scalable size unit
An android lib that provides a new size unit - sdp (scalable dp). This size unit scales with the screen size. It can help Android developers with supporting multiple screens.

for text views please refer to [ssp](https://github.com/comando95/android-sdp) which is based on the sp size unit for texts. 

# Attention
Use it carefully! for example, in most cases you still need to design a different layout for tablets.


# Getting Started

To add sdp to your project (Using Android Studio and Gradle): 

  add implementation 'com.comando95.android-sdp:android-sdp:1.0.0' to your build.gradle dependencies block.
  
  for example:
  
  ```
  repositories {
    maven { url  = uri("https://jitpack.io") } or maven { url 'https://jitpack.io' }
  }
  dependencies {
    implementation 'com.github.comando95:android-sdp:1.0.0'
  }
  ```
See the [sdp_example.xml](https://github.com/comando95/android-sdp/blob/master/android-sdp/src/main/res/layout/sdp_example.xml) to see how to use to the sdp size unit.

For easy mapping of designs to sdp units, one can create designs with 300 pixels screen width - in this case each pixel in the design corresponds to 1 sdp.

# Note
The sdp size unit calculation includes some approximation due to some performance and usability constraints.
