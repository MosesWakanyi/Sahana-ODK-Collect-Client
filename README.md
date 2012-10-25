Sahana-ODK-Collect-Client
=========================

Sahana specific version of ODK collect client


Files modified :

1. InstanceUploaderActivity.java
	Method name -  protected void onCreate(Bundle savedInstanceState) { ... }
	Code added - 
	 mInstanceUploaderTask.setLogon(getSettingsFromPreferences().getString(PreferencesActivity.KEY_USERNAME, ""));
         mInstanceUploaderTask.setPassword(getSettingsFromPreferences().getString(PreferencesActivity.KEY_PASSWORD, ""));

2. InstanceUploaderTask.java

	Method name -  protected HashMap<String, String> doInBackground(Long... values) { ... }
	Code added - 
	
	Please refer here - http://pastebin.ubuntu.com/1303842/

Other basic changes from the link - http://code.google.com/r/jaxtrx-edenodkcollect/source/detail?r=0e210c972d00b28b03b6e681bfa74fa97a9d57bf
ServerPreferences.java is refactored to PreferencesActivity.java



