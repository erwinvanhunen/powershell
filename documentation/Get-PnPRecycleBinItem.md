---
applicable: SharePoint Online
external help file: PnP.PowerShell.dll-Help.xml
Module Name: PnP.PowerShell
online version: https://docs.microsoft.com/powershell/module/sharepoint-pnp/get-pnprecyclebinitem
schema: 2.0.0
title: Get-PnPRecycleBinItem
---

# Get-PnPRecycleBinItem

## SYNOPSIS
Returns the items in the recycle bin from the context

## SYNTAX

### All (Default)
```
Get-PnPRecycleBinItem [-RowLimit <Int32>] [-Connection <PnPConnection>] [-Includes <String[]>]
 [<CommonParameters>]
```

### Identity
```
Get-PnPRecycleBinItem [-Identity <Guid>] [-Connection <PnPConnection>] [-Includes <String[]>]
 [<CommonParameters>]
```

### FirstStage
```
Get-PnPRecycleBinItem [-FirstStage] [-RowLimit <Int32>] [-Connection <PnPConnection>] [-Includes <String[]>]
 [<CommonParameters>]
```

### SecondStage
```
Get-PnPRecycleBinItem [-SecondStage] [-RowLimit <Int32>] [-Connection <PnPConnection>] [-Includes <String[]>]
 [<CommonParameters>]
```

## DESCRIPTION

## EXAMPLES

### EXAMPLE 1
```powershell
Get-PnPRecycleBinItem
```

Returns all items in both the first and the second stage recycle bins in the current site collection

### EXAMPLE 2
```powershell
Get-PnPRecycleBinItem -Identity f3ef6195-9400-4121-9d1c-c997fb5b86c2
```

Returns all a specific recycle bin item by id

### EXAMPLE 3
```powershell
Get-PnPRecycleBinItem -FirstStage
```

Returns all items in only the first stage recycle bin in the current site collection

### EXAMPLE 4
```powershell
Get-PnPRecycleBinItem -SecondStage
```

Returns all items in only the second stage recycle bin in the current site collection

### EXAMPLE 5
```powershell
Get-PnPRecycleBinItem -RowLimit 10000
```

Returns items in recycle bin limited by number of results

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

### -FirstStage
Return all items in the first stage recycle bin

```yaml
Type: SwitchParameter
Parameter Sets: FirstStage
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Identity
Returns a recycle bin item with a specific identity

```yaml
Type: Guid
Parameter Sets: Identity
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RowLimit
Limits return results to specified amount

Only applicable to: SharePoint Online, SharePoint Server 2019, SharePoint Server 2016

```yaml
Type: Int32
Parameter Sets: All, FirstStage, SecondStage
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SecondStage
Return all items in the second stage recycle bin

```yaml
Type: SwitchParameter
Parameter Sets: SecondStage
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## RELATED LINKS

[SharePoint Developer Patterns and Practices](https://aka.ms/sppnp)