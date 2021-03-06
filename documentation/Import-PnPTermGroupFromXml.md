---
applicable: SharePoint Online
external help file: PnP.PowerShell.dll-Help.xml
Module Name: PnP.PowerShell
online version: https://docs.microsoft.com/powershell/module/sharepoint-pnp/import-pnptermgroupfromxml
schema: 2.0.0
title: Import-PnPTermGroupFromXml
---

# Import-PnPTermGroupFromXml

## SYNOPSIS
Imports a taxonomy TermGroup from either the input or from an XML file.

## SYNTAX

### XML
```
Import-PnPTermGroupFromXml [[-Xml] <String>] [-Connection <PnPConnection>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

### File
```
Import-PnPTermGroupFromXml [-Path <String>] [-Connection <PnPConnection>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

## DESCRIPTION

## EXAMPLES

### EXAMPLE 1
```powershell
Import-PnPTermGroupFromXml -Xml $xml
```

Imports the XML based termgroup information located in the $xml variable

### EXAMPLE 2
```powershell
Import-PnPTermGroupFromXml -Path input.xml
```

Imports the XML file specified by the path.

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

### -Path
The XML File to import the data from

```yaml
Type: String
Parameter Sets: File
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

### -Xml
The XML to process

```yaml
Type: String
Parameter Sets: XML
Aliases:

Required: False
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

## RELATED LINKS

[SharePoint Developer Patterns and Practices](https://aka.ms/sppnp)