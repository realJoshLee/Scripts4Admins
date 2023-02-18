# Scripts4Admins
Scripts are designed to be used in companies where their primary IDM is Google Workspace. Scripts and dashboard are free to be edited and customized to your personal or business needs to help make everyones lives easier. No matter if this information is edited or not, there is no warranty or support.
Everything is databaseless so there is no need for a SQL database to house information. All information is cross referenced directly from Google to the CSV that will be pulled from your SIS/HR dept. If there is a user/employee in the SIS/HR CSV that is not in Google, then an account will be created. Same goes for suspending old users, if there is a user/employee that is not in the SIS/HR CSV but still active in the set OU in Google then their account will be suspended and moved.
Created by Josh Lee

## Prerequisites
- GAM (Google Apps Manager)
- WinSCP
- Enable script execution on device that will run all of these scripts:
  ```
  Set-ExecutionPolicy RemoteSigned
  ```

## Pre-Setup
These scripts are suggested to be ran directly on the machine that GAM is installed on. Download all of these files and make sure that you have the GAM portion in all of the scripts pointing to the location of gam.exe on your machine and then set the location of where the output for all of the script logs will be for the dashboard (if you decide to use the dashboard). From there, follow the individual setup instructions for each script and then setup scheduling in task scheduler on Windows.

### Create Script
This script was origionally designed to pull a CSV from Clever and create new student accounts based on if accounts are already in Google or not. Script to pull information from Clever can be changed around with any FTP server. Just change the header information, grade matching to department to change what OU the user will get their account created in.

#### Setup
- Change FTP credentials and path
- Change CSV processing information
- Change GAM script data
- Change created domain for logging

### Suspend Script
This script was origionally designed to pull a CSV from Clever and suspend old student accounts based on if accounts are active in the SIS sheet or not. Script to pull information from Clever and can be changed around with any FTP server. Just change the header information, grade matching to department to change what OU the user will get their account created in.

#### Setup
- Change FTP credentials and path
- Change CSV processing information
- Change GAM script data
- Change created domain for logging