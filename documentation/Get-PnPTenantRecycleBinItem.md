---
applicable: SharePoint Online
external help file: PnP.PowerShell.dll-Help.xml
Module Name: PnP.PowerShell
online version: https://docs.microsoft.com/powershell/module/sharepoint-pnp/get-pnptenantrecyclebinitem
schema: 2.0.0
title: Get-PnPTenantRecycleBinItem
---

# Get-PnPTenantRecycleBinItem

## SYNOPSIS

**Required Permissions**

* SharePoint: Access to the SharePoint Tenant Administration site

Returns all modern and classic site collections in the tenant scoped recycle bin

## SYNTAX

```
Get-PnPTenantRecycleBinItem [-Connection <PnPConnection>] [<CommonParameters>]
```

## DESCRIPTION
This command will return all the items in the tenant recycle bin for the Office 365 tenant you are connected to. Be sure to connect to the SharePoint Online Admin endpoint (https://yourtenantname-admin.sharepoint.com) in order for this command to work.

## EXAMPLES

### EXAMPLE 1
```powershell
Get-PnPTenantRecycleBinItem
```

Returns all modern and classic site collections in the tenant scoped recycle bin

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

## RELATED LINKS

[SharePoint Developer Patterns and Practices](https://aka.ms/sppnp)