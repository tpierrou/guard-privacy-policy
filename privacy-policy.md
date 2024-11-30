## Guard: Privacy Policy

### Data collected by the app

I hereby state, to the best of my knowledge and belief, that all data collected and shared by the app is stated in this privacy policy. 
Guard is not collecting any personally identifiable information (PII). Any data used by Guard is for the purpose of providing core app functionality. By using the Service, You agree to the collection and use of information in accordance with this Privacy Policy. 
All data is stored locally in your device only, and can be simply erased by clearing the app's data or uninstalling it. No analytics software is present in the app. Data is communicated in an encrypted state to API endpoints provided by [NVD](https://nvd.nist.gov/developers), [MalwareBazaar](https://bazaar.abuse.ch/api/) and [URLhaus](https://urlhaus.abuse.ch/api/) for security checks, but is not stored there.

Data stored locally on your device, for the purpose of providing core app functionality, are:

- Names of apps downloaded from untrusted sources.
- Hashes of files deemed as malware.
- Names of software deemed as vulnerable.

Data in encrypted transit is:

- CPE:s consisting of non-system app package information when looking for matches in the [NVD](https://nvd.nist.gov/developers)
- Files deemed suspicious are transferred in hashed format when looking for matches in [MalwareBazaar](https://bazaar.abuse.ch/)
- Links provided by the user when looking for matches in [URLhaus](https://urlhaus.abuse.ch/)

### Explanation of permissions requested in the app

<br/>

| Permission | Why it is required |
| :---: | --- |
| `android.permission.WAKE_LOCK` | Required to start the threat scan in the background. Automatically granted by the system; cannot be revoked by user. |
 `android.permission.POST_NOTIFICATIONS` | Required by the app to post notifications. Has to be granted by the user manually; can be revoked by the system or the user at any time. Notifies the user when a threat scan is finished. |
 `android.permission.INTERNET` | Required for communicating with external API:s when threat scanning. |
 `android.permission.MANAGE_EXTERNAL_STORAGE, android.permission.WRITE_EXTERNAL_STORAGE, android.permission.READ_EXTERNAL_STORAGE` | Required for malware scanning. `MANAGE_EXTERNAL_STORAGE` is for API level 33 and above, `WRITE_EXTERNAL_STORAGE` and `READ_EXTERNAL_STORAGE` for Api level 32 and below. |
 `android.permission.QUERY_ALL_PACKAGES` | Required by the app to get all non system apps to search for known vulnerabilities in them. |
 `android.permission.ACCESS_COARSE_LOCATION, android.permission.ACCESS_FINE_LOCATION` | Required by the app to search for nearby Wi-Fi devices, because of usage of WifiManager.getScanResults() | 
 `"android.permission.ACCESS_NETWORK_STATE"` | Required by the app to determine if the device is connected to Wi-Fi. By default, the threat scan is only running when the app is connected to an unmetered Wi-Fi. |
  `"android.permission.ACCESS_WIFI_STATE"` | Required by the app to get security information about the current Wi-Fi connection. |
 
