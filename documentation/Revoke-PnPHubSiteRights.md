---
applicable: SharePoint Online
external help file: PnP.PowerShell.dll-Help.xml
Module Name: PnP.PowerShell
online version: https://docs.microsoft.com/powershell/module/sharepoint-pnp/revoke-pnphubsiterights
schema: 2.0.0
title: Revoke-PnPHubSiteRights
---

# Revoke-PnPHubSiteRights

## SYNOPSIS

**Required Permissions**

* SharePoint: Access to the SharePoint Tenant Administration site

Revoke permissions to the permissions already in place to associate sites to Hub Sites for one or more specific users

## SYNTAX

```
Revoke-PnPHubSiteRights [-Identity] <HubSitePipeBind> -Principals <String[]> [-Connection <PnPConnection>]
 [<CommonParameters>]
```

## DESCRIPTION

## EXAMPLES

### EXAMPLE 1
```powershell
Revoke-PnPHubSiteRights -Identity https://contoso.sharepoint.com/sites/hubsite -Principals "myuser@mydomain.com","myotheruser@mydomain.com"
```

This example shows how to revoke the rights of myuser and myotheruser to associate their sites with the provided Hub Site

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

### -Identity
{{ Fill Identity Description }}

```yaml
Type: HubSitePipeBind
Parameter Sets: (All)
Aliases: HubSite

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Principals
{{ Fill Principals Description }}

```yaml
Type: String[]
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## RELATED LINKS

[SharePoint Developer Patterns and Practices](https://aka.ms/sppnp)