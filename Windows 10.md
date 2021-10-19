# Administrative Tools
## Local Security Policy
### Account Policies
#### Passwords
- Password history : 10
- Maximum Password age - 90 users, 30 admins
- Minimum password age - 10-30 days
- Mimimum password length - 10 characters
- Complexity requirements - Enable
- Reversible encryption - Disable
#### Account Lockout Policies
- Account lockout duration - 30 min
- account lockout threshold - 3-10 invalid login attempts
- Reset account lockout counter after - 30 min
### Advanced Audit Policy  Configurations
#### System Audit Policies...
##### Account Logon
- Audit Credential Validation - Enable
# Windows Defender
- turn everything on
# Windows firewall
- check what's on
# Windows update
- enable
# Users
- `mmc`
- File -> Add/Remove Snap-in...
	- Local Users and Groups
		- Add >
		- OK
- Disable Guest
- Check Admin group
- Passwords
- Delete unauthorized accounts
- Add required accounts
# Local Security Policy
## Advanced Audit Policy Configuration
### System Audit Policies
- Audit Credential Validation - Success
## Local Policies
### Security Options
- Interactive Logon: Don't displayl... - 
	- Configure 
		- Enabled
# Turn Windows features on or off
- Simple TCPIP services - uncheck
# Group policy
## Computer Configuration
### Administrative Templates
#### Windows Componenets
##### Remote Desktop Session host
###### Connections
- Allow user to connect remotely - disable
# Prohibited files
`Get-ChildItem -Path C:\xx\x -Recurse -File -Name | sort length –Descending`
# Required Software
From ReadMe - check software version
	That's usually where updates are located
# Unauthorized software
`add or remove programs`
uninstall anything not approved
