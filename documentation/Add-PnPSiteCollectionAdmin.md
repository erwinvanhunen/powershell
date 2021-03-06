---
applicable: SharePoint Online
external help file: PnP.PowerShell.dll-Help.xml
Module Name: PnP.PowerShell
online version: https://docs.microsoft.com/powershell/module/sharepoint-pnp/add-pnpsitecollectionadmin
schema: 2.0.0
title: Add-PnPSiteCollectionAdmin
---

# Add-PnPSiteCollectionAdmin

## SYNOPSIS
Adds one or more users as site collection administrators to the site collection in the current context

## SYNTAX

```
Add-PnPSiteCollectionAdmin
 -Owners <System.Collections.Generic.List`1[PnP.PowerShell.Commands.Base.PipeBinds.UserPipeBind]>
 [-Connection <PnPConnection>] [<CommonParameters>]
```

## DESCRIPTION
This command allows adding one to many users as site collection administrators to the site collection in the current context. It does not replace or remove existing site collection administrators.

## EXAMPLES

### EXAMPLE 1
```powershell
Add-PnPSiteCollectionAdmin -Owners "user@contoso.onmicrosoft.com"
```

This will add user@contoso.onmicrosoft.com as an additional site collection owner to the site collection in the current context

### EXAMPLE 2
```powershell
Add-PnPSiteCollectionAdmin -Owners @("user1@contoso.onmicrosoft.com", "user2@contoso.onmicrosoft.com")
```

This will add user1@contoso.onmicrosoft.com and user2@contoso.onmicrosoft.com as additional site collection owners to the site collection in the current context

### EXAMPLE 3
```powershell
Get-PnPUser | ? Title -Like "*Doe" | Add-PnPSiteCollectionAdmin
```

This will add all users with their title ending with "Doe" as additional site collection owners to the site collection in the current context

## PARAMETERS

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

### -Owners
Specifies owner(s) to add as site collection administrators. They will be added as additional site collection administrators to the site in the current context. Existing administrators will stay. Can be both users and groups.

```yaml
Type: System.Collections.Generic.List`1[PnP.PowerShell.Commands.Base.PipeBinds.UserPipeBind]
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

## RELATED LINKS

[SharePoint Developer Patterns and Practices](https://aka.ms/sppnp)