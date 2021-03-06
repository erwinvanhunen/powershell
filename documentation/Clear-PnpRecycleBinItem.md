---
applicable: SharePoint Online
external help file: PnP.PowerShell.dll-Help.xml
Module Name: PnP.PowerShell
online version: https://docs.microsoft.com/powershell/module/sharepoint-pnp/clear-pnprecyclebinitem
schema: 2.0.0
title: Clear-PnPRecycleBinItem
---

# Clear-PnPRecycleBinItem

## SYNOPSIS
Permanently deletes all or a specific recycle bin item

## SYNTAX

### All (Default)
```
Clear-PnPRecycleBinItem [-All] [-SecondStageOnly] [-Force] [-RowLimit <Int32>] [-Connection <PnPConnection>]
 [<CommonParameters>]
```

### Identity
```
Clear-PnPRecycleBinItem -Identity <RecycleBinItemPipeBind> [-Force] [-Connection <PnPConnection>]
 [<CommonParameters>]
```

## DESCRIPTION

## EXAMPLES

### EXAMPLE 1
```powershell
Get-PnPRecycleBinItem | ? FileLeafName -like "*.docx" | Clear-PnpRecycleBinItem
```

Permanently deletes all the items in the first and second stage recycle bins of which the file names have the .docx extension

### EXAMPLE 2
```powershell
Clear-PnpRecycleBinItem -Identity 72e4d749-d750-4989-b727-523d6726e442
```

Permanently deletes the recycle bin item with Id 72e4d749-d750-4989-b727-523d6726e442 from the recycle bin

### EXAMPLE 3
```powershell
Clear-PnpRecycleBinItem -Identity $item -Force
```

Permanently deletes the recycle bin item stored under variable $item from the recycle bin without asking for confirmation from the end user first

### EXAMPLE 4
```powershell
Clear-PnPRecycleBinItem -All -RowLimit 10000
```

Permanently deletes up to 10,000 items in the recycle bin

## PARAMETERS

### -All
Clears all items

```yaml
Type: SwitchParameter
Parameter Sets: All
Aliases:

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

### -Force
If provided, no confirmation will be asked to restore the recycle bin item

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

### -Identity
Id of the recycle bin item or the recycle bin item itself to permanently delete

```yaml
Type: RecycleBinItemPipeBind
Parameter Sets: Identity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -RowLimit
Limits deletion to specified number of items

Only applicable to: SharePoint Online, SharePoint Server 2019, SharePoint Server 2016

```yaml
Type: Int32
Parameter Sets: All
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SecondStageOnly
If provided, only all the items in the second stage recycle bin will be cleared

Only applicable to: SharePoint Online

```yaml
Type: SwitchParameter
Parameter Sets: All
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## RELATED LINKS

[SharePoint Developer Patterns and Practices](https://aka.ms/sppnp)