---
applicable: SharePoint Online
external help file: PnP.PowerShell.dll-Help.xml
Module Name: PnP.PowerShell
online version: https://docs.microsoft.com/powershell/module/sharepoint-pnp/get-pnpteamsapp
schema: 2.0.0
title: Get-PnPTeamsApp
---

# Get-PnPTeamsApp

## SYNOPSIS

**Required Permissions**

  * Microsoft Graph API : One of AppCatalog.Read.All, Directory.ReadWrite.All

Gets one Microsoft Teams App or a list of all apps.

## SYNTAX

```
Get-PnPTeamsApp [-Identity <TeamsAppPipeBind>] [-ByPassPermissionCheck] [<CommonParameters>]
```

## DESCRIPTION

## EXAMPLES

### EXAMPLE 1
```powershell
Get-PnPTeamsApp
```

Retrieves all the Microsoft Teams Apps

### EXAMPLE 2
```powershell
Get-PnPTeamsApp -Identity a54224d7-608b-4839-bf74-1b68148e65d4
```

Retrieves a specific Microsoft Teams App

### EXAMPLE 3
```powershell
Get-PnPTeamsApp -Identity "MyTeamsApp"
```

Retrieves a specific Microsoft Teams App

## PARAMETERS

### -ByPassPermissionCheck
Allows the check for required permissions in the access token to be bypassed when set to $true

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Identity
Specify the name, id or external id of the app.

```yaml
Type: TeamsAppPipeBind
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