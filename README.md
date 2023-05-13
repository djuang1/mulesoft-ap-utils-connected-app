# MuleSoft Anypoint Platform Utility

This is a python script that leverages the Anypoint Platform APIs to retrieve User, Runtime Manager, and API Manager data. *.csv files are created with the data from the platform. In order to use this script, you need to create a Connected App.

## Setup

### Get Connect App Client ID and Secret
1. Login to Anypoint Platform
2. Navigate Access Management
3. Click on Connected Apps
4. Click on *Create app* under the *Owned Apps* tab
5. Give the app a name
6. Under *Type*, click on App acts on its own behalf (client credentials)
7. Click on Add Scopes
8. Select the scopes you need and click on Next
9. Select the Business Groups you need and click on Next
10. Click Add Scopes
11. Click on Save
12. Click on Copy Id
13. Click on Copy Secret

### Get Organization ID
1. In Anypoint Platform, under *Access Management*, click on *Business Groups*
2. Click on the name of the parent Group
3. Copy down the *Business Group ID* 

## Usage

Replace the client_id, client_secret, and org_id with the values you collected during the setup.

```python PlatformUtilsConnectedApp.py --k <client_id> --s <client_secret> --o <org_id>```