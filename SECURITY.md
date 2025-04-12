Sensitive security issues can be reported to security@grapheneos.org. Please
use the regular issue tracker if the issue does not need to be kept private.
```
type: crash
osVersion: google/sargo/sargo:12/SP2A.220505.008/2023020600:user/release-keys
package: com.google.android.gms:244034029
process: com.google.android.gms.ui
processUptime: 1347703 ms
GmsCompatConfig version: 156

java.lang.RuntimeException: An error occurred while executing doInBackground()
	at gxd.done(:com.google.android.gms@244034029@24.40.34 (190400-682300402):34)
	at java.util.concurrent.FutureTask.finishCompletion(FutureTask.java:383)
	at java.util.concurrent.FutureTask.setException(FutureTask.java:252)
	at java.util.concurrent.FutureTask.run(FutureTask.java:271)
	at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1167)
	at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:641)
	at java.lang.Thread.run(Thread.java:920)
Caused by: java.lang.SecurityException: You need MANAGE_USERS permission to: Cannot get seed account information
	at android.os.Parcel.createExceptionOrNull(Parcel.java:2436)
	at android.os.Parcel.createException(Parcel.java:2420)
	at android.os.Parcel.readException(Parcel.java:2396)
	at android.os.Parcel.readException(Parcel.java:2338)
	at android.os.IUserManager$Stub$Proxy.getSeedAccountOptions(IUserManager.java:3033)
	at android.os.UserManager.getSeedAccountOptions(UserManager.java:3292)
	at abdh.b(:com.google.android.gms@244034029@24.40.34 (190400-682300402):16)
	at abcj.loadInBackground(:com.google.android.gms@244034029@24.40.34 (190400-682300402):3)
	at gww.onLoadInBackground(:com.google.android.gms@244034029@24.40.34 (190400-682300402):1)
	at gwv.a(:com.google.android.gms@244034029@24.40.34 (190400-682300402):3)
	at gxc.call(:com.google.android.gms@244034029@24.40.34 (190400-682300402):16)
	at java.util.concurrent.FutureTask.run(FutureTask.java:266)
	... 3 more

```
