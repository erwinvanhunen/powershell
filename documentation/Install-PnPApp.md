---
applicable: SharePoint Online
external help file: PnP.PowerShell.dll-Help.xml
Module Name: PnP.PowerShell
online version: https://docs.microsoft.com/powershell/module/sharepoint-pnp/install-pnpapp
schema: 2.0.0
title: Install-PnPApp
---

# Install-PnPApp

## SYNOPSIS
Installs an available app from the app catalog

## SYNTAX

```
Install-PnPApp [-Identity] <AppMetadataPipeBind> [-Scope <AppCatalogScope>] [-Wait]
 [-Connection <PnPConnection>] [<CommonParameters>]
```

## DESCRIPTION

## EXAMPLES

### EXAMPLE 1
```powershell
Install-PnPApp -Identity 99a00f6e-fb81-4dc7-8eac-e09c6f9132fe
```

This will install an app that is available in the tenant scoped app catalog, specified by the id, to the current site.

### EXAMPLE 2
```powershell
Install-PnPApp -Identity 99a00f6e-fb81-4dc7-8eac-e09c6f9132fe -Scope Site
```

This will install an app that is available in the site collection scoped app catalog, specified by the id, to the current site.

### EXAMPLE 3
```powershell
Get-PnPApp -Identity 99a00f6e-fb81-4dc7-8eac-e09c6f9132fe | Install-PnPApp
```

This will install the given app from the tenant scoped app catalog into the site.

### EXAMPLE 4
```powershell
Get-PnPApp -Identity 99a00f6e-fb81-4dc7-8eac-e09c6f9132fe -Scope Site | Install-PnPApp
```

This will install the given app from the site collection scoped app catalog into the site.

## PARAMETERS

### -Connection
Optional connection to be used by the cmdlet. Retrieve the value for this parameter by either specifying -ReturnConnection on Connect-PnPOnline or by executing Get-PnPConnection.

Only applicable to: SharePoint Online, SharePoint Server 2019

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
Specifies the Id or an actual app metadata instance

Only applicable to: SharePoint Online, SharePoint Server 2019

```yaml
Type: AppMetadataPipeBind
Parameter Sets: (All)
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Scope
Defines which app catalog to use. Defaults to Tenant

Only applicable to: SharePoint Online, SharePoint Server 2019

```yaml
Type: AppCatalogScope
Parameter Sets: (All)
Aliases:
Accepted values: Tenant, Site

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Wait
If specified the execution will pause until the app has been installed in the site.

Only applicable to: SharePoint Online, SharePoint Server 2019

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