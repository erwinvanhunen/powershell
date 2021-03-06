---
applicable: SharePoint Online
external help file: PnP.PowerShell.dll-Help.xml
Module Name: PnP.PowerShell
online version: https://docs.microsoft.com/powershell/module/sharepoint-pnp/get-pnptenanttemplate
schema: 2.0.0
title: Get-PnPTenantTemplate
---

# Get-PnPTenantTemplate

## SYNOPSIS

**Required Permissions**

* SharePoint: Access to the SharePoint Tenant Administration site

Generates a provisioning tenant template from a site. If the site is a hubsite any connected site will be included.

## SYNTAX

### Extract a template to a file
```
Get-PnPTenantTemplate [-SiteUrl <String>] [-Out] <String> [-Force]
 [-Configuration <ExtractConfigurationPipeBind>] [-Connection <PnPConnection>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### Extract a template as an object
```
Get-PnPTenantTemplate [-SiteUrl <String>] [-AsInstance] [-Configuration <ExtractConfigurationPipeBind>]
 [-Connection <PnPConnection>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION

## EXAMPLES

### EXAMPLE 1
```powershell
Get-PnPTenantTemplate -Out tenanttemplate.xml
```

Extracts a tenant template

## PARAMETERS

### -AsInstance
Returns the template as an in-memory object, which is an instance of the ProvisioningHierarchy type of the PnP Core Component. It cannot be used together with the -Out parameter.

Only applicable to: SharePoint Online

```yaml
Type: SwitchParameter
Parameter Sets: Extract a template as an object
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Configuration
Specify a JSON configuration file to configure the extraction progress.

Only applicable to: SharePoint Online

```yaml
Type: ExtractConfigurationPipeBind
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

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
Overwrites the output file if it exists.

Only applicable to: SharePoint Online

```yaml
Type: SwitchParameter
Parameter Sets: Extract a template to a file
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Out
Filename to write to, optionally including full path

Only applicable to: SharePoint Online

```yaml
Type: String
Parameter Sets: Extract a template to a file
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SiteUrl

Only applicable to: SharePoint Online

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