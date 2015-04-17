####Mandatory Permissions 

######Add the INTERNET and ACCESS_NETWORK_STATE permissions to your AndroidManifest.xml file just before the closing </manifest> tag:   

   ```xml
   <uses-permission android:name="android.permission.INTERNET" />      
   <uses-permission android:name="android.permission.ACCESS_NETWORK_STATE" />
   ```
    
######Including AvazuTracking Libraries:   
- Just add the Avazu-Tracking-Android-SDK.jar to the Libs folder in your project.  
   
######Code Changes:  
- Invoke the method within the onCreate of your first activity.

   ```java
   AvazuTracking.getInstance(Context context).reportAppDownloadGoal("uniqid",sales,"eventname","eventvalue");   
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
   <td><code>String uniqid</code>,<code>int sales</code>,<code>String eventname</code>,<code>String eventvalue</code></td>
   <td>Yes</td>
   <td><code>Custom ID</code>,<code>Number of the Sales</code>,<code>String eventName</code>,<code>String eventValue</code></td>
   <td><code>AvazuTracking.getIntance(this).reportAppDownLoadGoal("uniqid",sales,"eventname","eventvalue");</code></td>
 </tr>
</table>  

