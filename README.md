# Scripts4Admins
Scripts are designed to be used in companies where their primary IDM is Google Workspace.
Created by Josh Lee

## Prerequisites
- GAM (Google Apps Manager)
- WinSCP

### Create Script
This script was origionally designed to pull a CSV from Clever and create new student accounts based on if accounts are already in Google or not. Script to pull information from Clever can be changed around with any FTP server. Just change the header information, grade matching to department to change what OU the user will get their account created in.

#### Setup
- Change FTP credentials and path
- Change CSV processing information
- Change GAM script data
- Change created domain for logging
- Enable script execution:
  ```
  Set-ExecutionPolicy RemoteSigned
  ```

### Suspend Script
This script was origionally designed to pull a CSV from Clever and suspend old student accounts based on if accounts are active in the SIS sheet or not. Script to pull information from Clever and can be changed around with any FTP server. Just change the header information, grade matching to department to change what OU the user will get their account created in.

#### Setup
- Change FTP credentials and path
- Change CSV processing information
- Change GAM script data
- Change created domain for logging