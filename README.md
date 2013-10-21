####Mandatory Permissions 

######Add the INTERNET and ACCESS_NETWORK_STATE permissions to your AndroidManifest.xml file just before the closing </manifest> tag:   

   ```xml
   <uses-permission android:name="android.permission.INTERNET" />      
   <uses-permission android:name="android.permission.ACCESS_NETWORK_STATE" />
   ```
    
######Including AvazuTracking Libraries:   
- Just add the avazutracking-android-sdk.jar to the Libs folder in your project.  
![pic](http://d.pcs.baidu.com/thumbnail/1d745fbbea1e31a887c09a42e5e03346?fid=2050215414-250528-3206699477&time=1382332983&sign=FDTAR-DCb740ccc5511e5e8fedcff06b081203-3gQcBHnw1mz512yKOwFR5eTq97c%3D&rt=sh&expires=8h&r=234169259&size=c710_u500&quality=100)
   
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
<td>AvazuTracking.getIntance(this);</td>
</tr>
<tr>
<td>String uniqid</td>
<td>Yes</td>
<td>Custom ID</td>
<td>AvazuTracking.getIntance(this).reportAppDownLoadGoal("id");</td>
</tr>
</table>

