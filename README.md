# CloudBeds Integrator
A public repo for cloudbeds-integrator tools to assist customer success

## Integrator Helper App

This app provides some tools to help perform ad-hoc maintenance on the CloudBeds integrator.  It is not a part of the CloudBeds integrator app itself because it includes tools to assist in resolving rare edge cases.

### Download Link

* [Windows (x64)](https://github.com/shannahcloudbeds/cb-pna-tools-releases/releases/download/master/Cb.Pna.Tools.Installer-win-x64-%40master_25JD.zip)

### Installation Instructions

1. [Download](https://github.com/shannahcloudbeds/cb-pna-tools-releases/releases/download/master/Cb.Pna.Tools.Installer-win-x64-%40master_25JD.zip) the installer.
2. Extract the installer zip file, and run it.
3. Click "Run Anyway"
4. In the install wizard, select "Add to Start Menu", and click "Install".  Then "Proceed".
5. When it asks if you want to open the app now, select "No".


### Fixing Liquibase Lock Issue

This helper app can be used to resolve the issue with `liquibase.exception.LockException: Could not acquire change log lock.`

**How to fix**

1. Stop the CloudBeds Integrator.  (I.e. open the CloudBeds Integrator app and toggle the "Running" switch to off.
2. Right-click on "Cb Pna Tools master" in the start menu, and select "More" > "Run as administrator"
3. Press "Upgrade Database"
4. If it was successful, it should say "Query executed successfully.  Rows affected 1"
5. Close the "Cb Pna Tools master" app.
6. Start the CloudBeds Integrator app again.
