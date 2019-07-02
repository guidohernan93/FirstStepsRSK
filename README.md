# FirstStepsRSK
## Node debugger configuration

After downloading the RSK node and opening it on IntelliJ, add debug configuration like:

![alt text](screenshots/debug_config.png)

Add rsk.log file from project directory in order to see full log:

![alt text](screenshots/add_logs.png)

In case node is not logging, it is probable you have to update the Graddle runner preferences. It is needed to uncheck option 'Delegate IDE build/run actions to Gradle' and select 'Platform Test Runner' on combobox:

![alt text](screenshots/runner_config.png)

## How to build jar file

In order to build a jar from any version, once you have the latest version of the tag you want you have to run this command from terminal:

``` ./gradlew build -x test ``` 

##### jar file is created on path /rskj/rskj-core/build/libs

(-x test parameter is added to exclude tests, so that building process is faster. You can leave it to run tests)


## Run Dockerized tests

After getting Docker, a good example to check test flow can be found here:

[wasabi-opcode tests](https://github.com/rsksmart/dockerized-network/tree/wasabi-opcodes/wasabi-opcodes)
