---
applicable: SharePoint Online
external help file: PnP.PowerShell.dll-Help.xml
Module Name: PnP.PowerShell
online version: https://docs.microsoft.com/powershell/module/sharepoint-pnp/add-pnptenantsequencesubsite
schema: 2.0.0
title: Add-PnPTenantSequenceSubSite
---

# Add-PnPTenantSequenceSubSite

## SYNOPSIS
Adds a tenant sequence sub site object to a tenant sequence site object

## SYNTAX

```
Add-PnPTenantSequenceSubSite -SubSite <TeamNoGroupSubSite> -Site <SiteCollection> [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

## DESCRIPTION

## EXAMPLES

### EXAMPLE 1
```powershell
Add-PnPTenantSequenceSubSite -Site $mysite -SubSite $mysubsite
```

Adds an existing subsite object to an existing sequence site object

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

### -Site
The site to add the subsite to

```yaml
Type: SiteCollection
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -SubSite
The subsite to add

```yaml
Type: TeamNoGroupSubSite
Parameter Sets: (All)
Aliases:

Required: True
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