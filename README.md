# FirstStepsRSK
## Node configuration

After downloading the RSK node and opening it on IntelliJ, add debug configuration like:

![alt text](screenshots/debug_config.png)

Add rsk.log file from project directory in order to see full log:

![alt text](screenshots/add_logs.png)

In case node is not logging, it is probable you have to update the Graddle runner preferences. It is needed to uncheck option 'Delegate IDE build/run actions to Gradle' and select 'Platform Test Runner' on combobox:

![alt text](screenshots/runner_config.png)

