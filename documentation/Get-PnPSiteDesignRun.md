---
applicable: SharePoint Online
external help file: PnP.PowerShell.dll-Help.xml
Module Name: PnP.PowerShell
online version: https://docs.microsoft.com/powershell/module/sharepoint-pnp/get-pnpsitedesignrun
schema: 2.0.0
title: Get-PnPSiteDesignRun
---

# Get-PnPSiteDesignRun

## SYNOPSIS
Retrieves a list of site designs applied to a specified site collection. If the WebUrl parameter is not specified we show the list of designs applied to the current site. The returned output includes the ID of the scheduled job, the web and site IDs, and the site design ID, version, and title.

## SYNTAX

```
Get-PnPSiteDesignRun [-SiteDesignId <Guid>] [-WebUrl <String>] [-Web <WebPipeBind>]
 [-Connection <PnPConnection>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION

## EXAMPLES

### EXAMPLE 1
```powershell
Get-PnPSiteDesignRun
```

This example returns a list of the site designs applied to the current site. Providing a specific site design ID will return the details for just that applied site design.

### EXAMPLE 2
```powershell
Get-PnPSiteDesignRun -WebUrl https://mytenant.sharepoint.com/sites/project
```

This example returns a list of the site designs applied to the specified site. Providing a specific site design ID will return the details for just that applied site design.

## PARAMETERS

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
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

### -SiteDesignId
The ID of the site design to apply.

```yaml
Type: Guid
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Web
This parameter allows you to optionally apply the cmdlet action to a subweb within the current web. In most situations this parameter is not required and you can connect to the subweb using Connect-PnPOnline instead. Specify the GUID, server relative url (i.e. /sites/team1) or web instance of the web to apply the command to. Omit this parameter to use the current web.

```yaml
Type: WebPipeBind
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WebUrl
The URL of the site collection where the site design will be applied. If not specified the design will be applied to the site you connected to with Connect-PnPOnline.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs. The cmdlet is not run.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## RELATED LINKS

[SharePoint Developer Patterns and Practices](https://aka.ms/sppnp)