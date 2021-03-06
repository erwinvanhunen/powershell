---
applicable: SharePoint Online
external help file: PnP.PowerShell.dll-Help.xml
Module Name: PnP.PowerShell
online version: https://docs.microsoft.com/powershell/module/sharepoint-pnp/clear-pnptenantrecyclebinitem
schema: 2.0.0
title: Clear-PnPTenantRecycleBinItem
---

# Clear-PnPTenantRecycleBinItem

## SYNOPSIS

**Required Permissions**

* SharePoint: Access to the SharePoint Tenant Administration site

Permanently deletes a site collection from the tenant scoped recycle bin

## SYNTAX

```
Clear-PnPTenantRecycleBinItem -Url <String> [-Wait] [-Force] [-Connection <PnPConnection>] [<CommonParameters>]
```

## DESCRIPTION
The Clear-PnPTenantRecycleBinItem cmdlet allows a site collection that has been deleted and still exists in the tenant recycle bin to be permanently deleted from the recycle bin as well.

## EXAMPLES

### EXAMPLE 1
```powershell
Clear-PnPTenantRecycleBinItem -Url https://tenant.sharepoint.com/sites/contoso
```

This will permanently delete site collection with the url 'https://tenant.sharepoint.com/sites/contoso' from the tenant recycle bin

### EXAMPLE 2
```powershell
Clear-PnPTenantRecycleBinItem -Url https://tenant.sharepoint.com/sites/contoso -Wait
```

This will permanently delete site collection with the url 'https://tenant.sharepoint.com/sites/contoso' from the tenant recycle bin and will wait with executing further PowerShell commands until the operation has completed

## PARAMETERS

### -Connection
Optional connection to be used by the cmdlet. Retrieve the value for this parameter by either specifying -ReturnConnection on Connect-PnPOnline or by executing Get-PnPConnection.

Only applicable to: SharePoint Online

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

### -Force
If provided, no confirmation will be asked to permanently delete the site collection from the tenant recycle bin

Only applicable to: SharePoint Online

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

### -Url
Url of the site collection to permanently delete from the tenant recycle bin

Only applicable to: SharePoint Online

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

### -Wait
If provided, the PowerShell execution will halt until the operation has completed

Only applicable to: SharePoint Online

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

## RELATED LINKS

[SharePoint Developer Patterns and Practices](https://aka.ms/sppnp)