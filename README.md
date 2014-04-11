####Mandatory Permissions 

######Add the INTERNET and ACCESS_NETWORK_STATE permissions to your AndroidManifest.xml file just before the closing </manifest> tag:   

   ```xml
   <uses-permission android:name="android.permission.INTERNET" />      
   <uses-permission android:name="android.permission.ACCESS_NETWORK_STATE" />
   ```
    
######Including AvazuTracking Libraries:   
- Just add the avazutracking-android-sdk.jar to the Libs folder in your project.  
![pic](http://d.pcs.baidu.com/thumbnail/2360ff40f5e7c32e19b27ef8599193c4?fid=2050215414-250528-3840253792&time=1397203685&sign=FDTAER-DCb740ccc5511e5e8fedcff06b081203-BA74MkWE3F88thNBYF%2F9HIoO5iM%3D&rt=sh&expires=8h&r=777836295&sharesign=unknown&size=c710_u500&quality=100)
   
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

