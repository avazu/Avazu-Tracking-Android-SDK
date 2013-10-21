####Mandatory Permissions 

######Add the INTERNET and ACCESS_NETWORK_STATE permissions to your AndroidManifest.xml file just before the closing </manifest> tag:   

   ```xml
   <uses-permission android:name="android.permission.INTERNET" />      
   <uses-permission android:name="android.permission.ACCESS_NETWORK_STATE" />
   ```
    
######Including AvazuTracking Libraries:   
- Just add the avazutracking-android-sdk.jar to the Libs folder in your project.
   
   
######Code Changes:  
- Invoke the method within the onCreate of your first activity.

   ```java
   AvazuTracking.getInstance(Context context).reportAppDownloadGoal();   
   ```
   
<table>
<tr>
<th>Parameter</th>
<th>Required</th>
<th>Description</th>
<th>Example</th>
</tr>
<tr>
<td>Context context</td>
<td>Yes</td>
<td>Context object</td>
<td>AvazuTracking.getIntance(this).reportAppDownLoadGoal()</td>
</tr>
</table>
