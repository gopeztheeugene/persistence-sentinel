# persistence-sentinel-check
Runs a series of kql queries to inspect persistence on compromised host/s by using the Az cmdlets. Allows an option to enter known compromised user/s and will then query devices the user/s logged into(depends on entered date).

***Kql queries the following:
a. Scheduled task creations and updates from defender's telemetry and collected security events.
b. Run and RunOnce Registry Keys
c. WinLogon Registry Key
d. Service installation (will include Service registry ImagePath modifications soon).
e. File creations in startup folder
f. Modifications to File Association (https://attack.mitre.org/techniques/T1546/001/)
g. Wmi subscriptions
h. Group Manipulation
i. User Manipulation
