# persistence-sentinel-check
Runs a series of kql queries to inspect persistence on compromised host/s by using the Az cmdlets. Allows an option to enter known compromised user/s and will then query devices the user/s logged into(depends on entered date).
<br />
***Kql queries the following persistence mechanisms:<br />
a. Scheduled task creations and updates from defender's telemetry and collected security events<br />
b. Run and RunOnce Registry Keys<br />
c. WinLogon Registry Key<br />
d. Service installation (will include Service registry ImagePath modifications soon)<br />
e. File creations in startup folder<br />
f. Modifications to File Association (https://attack.mitre.org/techniques/T1546/001/)<br />
g. Wmi subscriptions<br />
h. Group Manipulation<br />
i. User Manipulation<br />
