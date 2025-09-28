# persistence-sentinel
Runs a series of kql queries using the Az cmdlets to inspect persistence on compromised host/s. Allows an option to enter known compromised user/s and will then query devices the user/s logged into(depending on entered date).


Kql queries the following persistence mechanisms:<br />
>Scheduled task creations and updates<br />
>Run and RunOnce Registry Keys<br />
>WinLogon Registry Key<br />
>Service installation (will include Service registry ImagePath modifications soon)<br />
>File creations in startup folder<br />
>Modifications to File Association (https://attack.mitre.org/techniques/T1546/001/)<br />
>Wmi Subscriptions<br />
>Group Manipulation<br />
>User Manipulation<br />
