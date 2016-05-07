# Prefs
[![](https://jitpack.io/v/GrenderG/Prefs.svg)](https://jitpack.io/#GrenderG/Prefs)

Simple Android SharedPreferences wrapper.

Repository
--

Add this in your root `build.gradle` file (**not** your module `build.gradle` file):

```gradle
allprojects {
	repositories {
		...
		maven { url "https://jitpack.io" }
	}
}
```

Dependency
--

Add this to your module's `build.gradle` file (make sure the version matches the JitPack badge above):

```gradle
dependencies {
	...
	compile 'com.github.GrenderG:Prefs:1.1'
}
```

Usage
--

``` java
  Prefs.with(yourContext).readInt(YOUR_KEY_VALUE);
  Prefs.with(yourContext).readInt(YOUR_KEY_VALUE, defaultValue);
  
  Prefs.with(yourContext).writeInt(YOUR_KEY_VALUE, valueToStore);
```
