---
applicable: SharePoint Online
external help file: PnP.PowerShell.dll-Help.xml
Module Name: PnP.PowerShell
online version: https://docs.microsoft.com/powershell/module/sharepoint-pnp/disconnect-pnponline
schema: 2.0.0
title: Disconnect-PnPOnline
---

# Disconnect-PnPOnline

## SYNOPSIS
Disconnects the context

## SYNTAX

```
Disconnect-PnPOnline [-Connection <PnPConnection>] [<CommonParameters>]
```

## DESCRIPTION
Disconnects the current context and requires you to build up a new connection in order to use the Cmdlets again. Using Connect-PnPOnline to connect to a different site has the same effect.

## EXAMPLES

### EXAMPLE 1
```powershell
Disconnect-PnPOnline
```

This will clear out all active tokens

## PARAMETERS

### -Connection
Connection to be used by cmdlet

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