# Scripts4Admins
Scripts are designed to be used in companies where their primary IDM is Google Workspace. Scripts and dashboard are free to be edited and customized to your personal or business needs to help make everyones lives easier. No matter if this information is edited or not, there is no warranty or support.
Created by Josh Lee

## Prerequisites
- GAM (Google Apps Manager)
- WinSCP
- Enable script execution on device that will run all of these scripts:
  ```
  Set-ExecutionPolicy RemoteSigned
  ```

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