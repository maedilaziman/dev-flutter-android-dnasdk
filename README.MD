# About
Flutter Android DNA SDK Development
<h2>Requirements</h2>
<ul>
<li>Android Studio Dolphin 2021.3.1 Patch 1</li>
<li>Java 8</li>
<li>Flutter 3.3.8</li>
</ul>
<h2>Minimum Android SDK Version</h2>
<ul>
<li>Minimum SDK Version: 24</li>
</ul>
<br/>
<h2>How To Install</h2>
<br/>
After downloading dna_flutterplugin, please add dna_flutterplugin to your computer document, usually in windows is in C document.
<br/>
<br/>
Add path in your pubspec.yaml to connect dna_flutterplugin with your flutter project,
as shown below.
<br/>
<img src="https://raw.githubusercontent.com/maedilaziman/dev-flutter-android-dnasdk/master/Screenshots/IMG_03.png" width="400" />
<br/>
Add all dependencies library in app build.gradle as shown below.
<br/>
<img src="https://raw.githubusercontent.com/maedilaziman/dev-flutter-android-dnasdk/master/Screenshots/IMG_01.png" width="400" />
<br/>
Below is all dependencies library:
<pre>
    <code>
	// Multidex
    implementation 'com.android.support:multidex:1.0.3'

    // google support library ---------------------------------------------------------------------
    implementation 'androidx.appcompat:appcompat:1.1.0'
    implementation 'com.google.android.material:material:1.1.0'
    implementation 'androidx.cardview:cardview:1.0.0'
    implementation 'androidx.recyclerview:recyclerview:1.1.0'
    implementation 'androidx.legacy:legacy-support-v13:1.0.0'
    implementation 'androidx.constraintlayout:constraintlayout:1.1.3'
    implementation 'androidx.vectordrawable:vectordrawable:1.1.0'

    implementation platform('com.google.firebase:firebase-bom:26.0.0')
    implementation 'com.google.firebase:firebase-messaging:20.2.4'
    implementation 'com.google.firebase:firebase-analytics:17.5.0'
    implementation 'com.google.firebase:firebase-crashlytics:17.2.1'
    implementation 'com.google.firebase:firebase-crashlytics-ndk:17.2.2'

    // google maps library ------------------------------------------------------------------------
    implementation 'com.google.android.gms:play-services-maps:17.0.0'
    implementation('com.google.android.libraries.places:places:1.0.0') {
        exclude module: 'glide'
    }


    // third party dependencies -------------------------------------------------------------------
    implementation 'com.balysv:material-ripple:1.0.2'                  // ripple effect
    implementation 'com.github.bumptech.glide:glide:3.7.0'             // image loader
    implementation 'com.mikhaellopez:circularimageview:4.3.1'          // circle image view
    implementation 'com.github.pchmn:MaterialChipsInput:1.0.5'         // material chip
    implementation 'com.hootsuite.android:nachos:1.1.1'                // material chips
    implementation 'com.google.android:flexbox:0.3.2'                  // google flexible box
    implementation 'com.squareup.retrofit2:retrofit:2.9.0'             // API library
    implementation 'com.squareup.retrofit2:converter-gson:2.9.0'       // API library
    implementation   'io.jsonwebtoken:jjwt:0.7.0'                        // JWT library

    // v3d ----------------------------------------------------------------------------------------
    implementation(group: 'com.v3d.android', name: 'eqcore', version: '9.7.1.11')
    implementation "com.j256.ormlite:ormlite-core:5.0"
    implementation "net.zetetic:android-database-sqlcipher:3.5.9"
    implementation "io.github.rburgst:okhttp-digest:2.7"
    implementation "com.vividsolutions:jts:1.13"
    implementation "com.getkeepsafe.relinker:relinker:1.2.2"
    implementation "com.v3d.android:ticket:9.7.1.0"
    implementation "com.v3d.android:radio:9.7.1.0"
    implementation "com.v3d.android:location:9.7.1.0"
    implementation "com.v3d.android:core:9.7.1.0"
    implementation "com.v3d.android:logger:9.7.1.0"
    implementation "com.v3d.library.protobuf:library-model:5.0.1.1"
    implementation "com.v3d.android:gateway:9.7.1.0"
    implementation "com.v3d.library:eps:17.0.0.4"
    implementation "com.v3d.library:ormlite-android-cipher:5.0.5"
    implementation "com.v3d.library:youtube-android-player-api:1.2.2"
    implementation "com.v3d.library:mail:1.4"
    implementation "com.v3d.library:activation:1.0"
    implementation "com.v3d.library:lz4:1.4"
    implementation "com.v3d.library:v3dacra:4.9.1.12"
    implementation "com.v3d.library.protobuf:ticket:0.1.6"
    implementation "com.v3d.library:abstractgls:1.0.4"
    implementation "com.v3d.library:eqlogger:1.0.2"
    implementation "org.jetbrains.kotlin:kotlin-stdlib-jdk8:1.4.10"
    implementation "org.jetbrains.kotlin:kotlin-stdlib-jdk7:1.5.31"
    implementation "org.jetbrains.kotlinx:kotlinx-coroutines-android:1.3.0"
    implementation "org.jetbrains.kotlinx:kotlinx-coroutines-core:1.3.0"
    implementation "org.jetbrains.kotlin:kotlin-stdlib:1.5.31"
    implementation "org.jetbrains:annotations:13.0"
    implementation "org.jetbrains.kotlin:kotlin-stdlib-common:1.5.31"
    implementation "com.squareup.wire:wire-runtime:3.4.0"
    implementation "com.squareup.okhttp3:logging-interceptor:4.2.2"
    implementation "com.squareup.okhttp3:okhttp:4.8.1"
    implementation "com.squareup.okio:okio:2.8.0"
    implementation "com.google.android.gms:play-services-location:17.0.0"
    implementation "com.google.android.gms:play-services-base:17.0.0"
    implementation "com.google.android.gms:play-services-places-placereport:17.0.0"
    implementation "com.google.android.gms:play-services-tasks:17.0.0"
    implementation "com.google.android.gms:play-services-basement:17.0.0"
    implementation "com.google.code.gson:gson:2.8.5"
    implementation 'com.google.protobuf:protobuf-javalite:3.14.0'

    implementation 'fr.bmartel:jspeedtest:1.32.1'

    implementation 'com.google.guava:listenablefuture:9999.0-empty-to-avoid-conflict-with-guava'
   </code>
</pre>
<br/>
Add dependencies in project build.gradle as shown below.
<br/>
<img src="https://raw.githubusercontent.com/maedilaziman/dev-flutter-android-dnasdk/master/Screenshots/IMG_02.png" width="400" />
<br/>
Add tool replace in AndroidManifest as shown below.
<br/>
<img src="https://raw.githubusercontent.com/maedilaziman/dev-flutter-android-dnasdk/master/Screenshots/IMG_02.png" width="400" />
<br/>
You have successfully add DNA Flutter Plugin to your project
<h2>How To Use</h2>
<br/>
Before you call network test, you need login first,
first you need call flutter_android_initAuth for authentication
<pre>
    <code>
	Future<void> refresh_onCompleteInitAuth() async {
    	  await DnaSdkFlutterPlugin.flutter_android_initAuth ?? 'null_init_auth';
    	  if (!mounted) return;
  	}
   </code>
</pre>
After authentication success, you can call flutter_android_setUserData to login with phone number
<pre>
    <code>
	Future<String> get flutter_setPhoneNumber async {
    		final String phone = await _channel.invokeMethod('flutter_android_setUserData',<String, dynamic>{
      		   'phoneNumber': this.phoneNumber,
    		});
    		return phone;
  	}
   </code>
</pre>
<br/>
After success login, you can call other function to test the network, below is function to test the network
<pre>
    <code>
	refresh_onCompleteGetTimeFinishDownload();
	refresh_onCompleteGetTimeFinishUpload();
	refresh_onCompleteGetLatestNetworkTestResult();
   </code>
</pre>
For more details, you can see an example of calling all functions in the example flutter_test_call_dnasdk.
<br/>