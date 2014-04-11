####Mandatory Permissions 

######Add the INTERNET and ACCESS_NETWORK_STATE permissions to your AndroidManifest.xml file just before the closing </manifest> tag:   

   ```xml
   <uses-permission android:name="android.permission.INTERNET" />      
   <uses-permission android:name="android.permission.ACCESS_NETWORK_STATE" />
   ```
    
######Including AvazuTracking Libraries:   
- Just add the avazutracking-android-sdk.jar to the Libs folder in your project.  
![pic](http://pan.baidu.com/s/1dDf5hJF)
   
######Code Changes:  
- Invoke the method within the onCreate of your first activity.

   ```java
   AvazuTracking.getInstance(Context context).reportAppDownloadGoal("id");   
   ```

<table cellspacing="0">
 <tr>
   <th>Parameter</th>
   <th>Required</th>
   <th>Description</th>
   <th>Example</th>
 </tr>
 <tr>
   <td><code>Context context</code></td>
   <td>Yes</td>
   <td><code>Context object</code></td>
   <td><code>AvazuTracking.getIntance(this);</code></td>
 </tr>
 <tr>
   <td><code>String uniqid</code></td>
   <td>Yes</td>
   <td><code>Custom ID</code></td>
   <td><code>AvazuTracking.getIntance(this).reportAppDownLoadGoal("id");</code></td>
 </tr>
</table>  

