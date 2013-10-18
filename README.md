Mandatory Permissions   
   Add the INTERNET and ACCESS_NETWORK_STATE permissions to your AndroidManifest.xml file just before the closing </manifest> tag:   
   <uses-permission android:name="android.permission.INTERNET" />      
   <uses-permission android:name="android.permission.ACCESS_NETWORK_STATE" />
   
   Including AvazuTracking Libraries:   
   Just add the avazutracking-android-sdk.jar to the Libs folder in your project.
   Code Changes:   
   Invoke the method within the onCreate of your first activity.   
   ```java
   AvazuTracking.getInstance(Context context).reportAppDownloadGoal();   
   ```
   
   Required:Yes   
   Description:Context object   
   Example:AvazuTracking.getIntance(this).reportAppDownLoadGoal()
