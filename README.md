# POWERTAC-PROJECT
#java11
How to set-up PowerTAC environment ... (For Ubuntu, but should be the same procedure for other OS too)

Step 1: Install jdk-11.0.* and set-up the PATH 
Step 2: Install maven (sudo apt-get install maven)
Step 3: git clone and compile PowerTAC server-distribution 
Step 4: Compile the broker and test run 
    • To compile: mvn compile
    • To run: mvn exec:exec

Download boot files from https://powertac.org/log_archive/PowerTAC_2021_finals.html.

## github

### POWER TECH
https://github.com/powertac

### sever diistribution
https://github.com/powertac/server-distribution


## TO RUN SERVER	
mvn -Pcli -Dexec.args="--sim --boot-data finals_2021_1.xml --weather-data boot-log/finals_2021_1.state --brokers ZI"

## To run BROKER
mvn compile
mvn exec:exec
