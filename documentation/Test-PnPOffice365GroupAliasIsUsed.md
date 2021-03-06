---
applicable: SharePoint Online
external help file: PnP.PowerShell.dll-Help.xml
Module Name: PnP.PowerShell
online version: https://docs.microsoft.com/powershell/module/sharepoint-pnp/test-pnpoffice365groupaliasisused
schema: 2.0.0
title: Test-PnPOffice365GroupAliasIsUsed
---

# Test-PnPOffice365GroupAliasIsUsed

## SYNOPSIS
Tests if a given alias is already used used

## SYNTAX

```
Test-PnPOffice365GroupAliasIsUsed -Alias <String> [-Connection <PnPConnection>] [<CommonParameters>]
```

## DESCRIPTION
This command allows you to test if a provided alias is used or free, helps decide if it can be used as part of connecting an Office 365 Unified group to an existing classic site collection.

## EXAMPLES

### EXAMPLE 1
```powershell
Test-PnPOffice365GroupAliasIsUsed -Alias "MyGroup"
```

This will test if the alias MyGroup is already used

## PARAMETERS

### -Alias
Specifies the alias of the group. Cannot contain spaces.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Connection
Optional connection to be used by the cmdlet. Retrieve the value for this parameter by either specifying -ReturnConnection on Connect-PnPOnline or by executing Get-PnPConnection.

```yaml
Type: PnPConnection
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## RELATED LINKS

[SharePoint Developer Patterns and Practices](https://aka.ms/sppnp)