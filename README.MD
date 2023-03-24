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
Add path in your pubspec.yaml to connect dna_flutterplugin with your flutter project,
as shown below.
<br/>
<img src="https://raw.githubusercontent.com/maedilaziman/dev-flutter-android-dnasdk/master/Screenshots/IMG_03.png" width="300" />
<br/>
Select info.plist and add App Transport Security Settings until Privacy - Location When In Use Usage Description as shown below.
<br/>
<img src="https://raw.githubusercontent.com/maedilaziman/dev-ios-sigmonsdk/master/Screenshots/IMG_03.png" width="300" />
<br/>
You have successfully add SigmonSDK.framework to your project
<h2>How To Use</h2>
<br/>
Open your UIViewController class, then import SigmonSDK, in that class please implement protocol SMSDKMainSpeedTestComm and SMSDKMainSpeedTestSetCredentialComm as shown below.
<br/>
<img src="https://raw.githubusercontent.com/maedilaziman/dev-ios-sigmonsdk/master/Screenshots/IMG_04.png" width="300" />
This set credential key is mandatory, you can't fill empty credential key
<pre>
    <code>
	func setCredentialKey() -> String {
    	    return credentialKey
	}
   </code>
</pre>
Before you can test speed, SDK will return info whether set credential key was successful or not, 
if successful then the value of data.success = true,  
and if not then the value of data.success = false, and data.error will provide information 
about the error description
<pre>
    <code>
	func onCompleteSetCredentialKey(data: CredentialKeyData) {
    	    print("SDKTest_set_credential: \(data.success) ; Error: \(data.error)")
	}
   </code>
</pre>
<br/>
Declare SMSDKMainSpeedTestUI and SMSDKMainSpeedTestMainUI classes as shown below.
<br/>
<img src="https://raw.githubusercontent.com/maedilaziman/dev-ios-sigmonsdk/master/Screenshots/IMG_05.png" width="300" />
<br/>
Initialize SMSDKMainSpeedTestUI and SMSDKMainSpeedTestMainUI classes as shown below.
<br/>
<img src="https://raw.githubusercontent.com/maedilaziman/dev-ios-sigmonsdk/master/Screenshots/IMG_06.png" width="300" />
<br/>
After you have initialize SMSDKMainSpeedTestUI and SMSDKMainSpeedTestMainUI classes, you can add startSpeedTest() action in your event. Like the image below.
(startSpeedTest() method will return an empty string if there is no error message.)
<br/>
<img src="https://raw.githubusercontent.com/maedilaziman/dev-ios-sigmonsdk/master/Screenshots/IMG_07.png" width="300" />
<br/>
<b>Note:</b> before you access startSpeedTest() action, you must initialize SMSDKMainSpeedTestUI and SMSDKMainSpeedTestMainUI classes
<br/>