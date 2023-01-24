![GitHub](https://img.shields.io/github/license/rstolpe/ConvertSID?style=plastic)  
![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/rstolpe/ConvertSID?sort=semver&style=plastic)  ![Last release](https://img.shields.io/github/release-date/rstolpe/ConvertSID?style=plastic)
![GitHub last commit](https://img.shields.io/github/last-commit/rstolpe/ConvertSID?style=plastic)  
![PSGallery downloads](https://img.shields.io/powershellgallery/dt/ConvertSID?style=plastic)

# ConvertSID
This module will convert SID to plain text so you can read it.
I have added the result from PSScriptAnalyzer in [test folder](https://github.com/rstolpe/ConvertSID/tree/main/test)

# Links
* [My PowerShell Collection](https://github.com/rstolpe/PSCollection)
* [Webpage/Blog](https://www.stolpe.io)
* [Twitter](https://twitter.com/rstolpes)
* [LinkedIn](https://www.linkedin.com/in/rstolpe/)
* [PowerShell Gallery](https://www.powershellgallery.com/profiles/rstolpe)

# Help
Below I have specified things that I think will help people with this module.  
You can also see the API for each function in the [help folder](https://github.com/rstolpe/ConvertSID/tree/main/help)

## Install
Install for current user
```
Install-Module -Name ConvertSID -Scope CurrentUser -Force
```

Install for all users
```
Install-Module -Name ConvertSID -Scope AllUsers -Force
```

## Example
```
Convert-SID -SID "<SID>"
```
If this SID was for an Active Directory user this would return the domain\username of that user, example stolpe.io\rstolpe  
You can also add multiple SIDs at the same time just separate them with a comma, example ```Convert-SID -SID "<SID1>", "<SID2>"```
```
Convert-SID -SID "<SID>" -Trim
```
Sometimes you don't want the domain\ part in return then you can use -Trim switch and it will just return the name after the domain\, example rstolpe

