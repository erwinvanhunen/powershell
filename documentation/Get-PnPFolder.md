---
applicable: SharePoint Online
external help file: PnP.PowerShell.dll-Help.xml
Module Name: PnP.PowerShell
online version: https://docs.microsoft.com/powershell/module/sharepoint-pnp/get-pnpfolder
schema: 2.0.0
title: Get-PnPFolder
---

# Get-PnPFolder

## SYNOPSIS
Return a folder object

## SYNTAX

### Folder By Url
```
Get-PnPFolder [-Url] <String> [-Web <WebPipeBind>] [-Connection <PnPConnection>] [-Includes <String[]>]
 [<CommonParameters>]
```

### Folders In List
```
Get-PnPFolder [-List] <ListPipeBind> [-Web <WebPipeBind>] [-Connection <PnPConnection>] [-Includes <String[]>]
 [<CommonParameters>]
```

## DESCRIPTION
Retrieves a folder if it exists or all folders inside a provided list or library. Use Resolve-PnPFolder to create the folder if it does not exist.

## EXAMPLES

### EXAMPLE 1
```powershell
Get-PnPFolder -Url "Shared Documents"
```

Returns the folder called 'Shared Documents' which is located in the root of the current web

### EXAMPLE 2
```powershell
Get-PnPFolder -Url "/sites/demo/Shared Documents"
```

Returns the folder called 'Shared Documents' which is located in the root of the current web

### EXAMPLE 3
```powershell
Get-PnPFolder -List "Shared Documents"
```

Returns the folder(s) residing inside a folder called 'Shared Documents'

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

### -List
Name, ID or instance of a list or document library to retrieve the folders residing in it for.

```yaml
Type: ListPipeBind
Parameter Sets: Folders In List
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Url
Site or server relative URL of the folder to retrieve. In the case of a server relative url, make sure that the url starts with the managed path as the current web.

```yaml
Type: String
Parameter Sets: Folder By Url
Aliases: RelativeUrl

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Web
The web to apply the command to. Omit this parameter to use the current web.

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

## RELATED LINKS

[SharePoint Developer Patterns and Practices](https://aka.ms/sppnp)[Resolve-PnPFolder](https://github.com/MicrosoftDocs/office-docs-powershell/blob/master/sharepoint/sharepoint-ps/sharepoint-pnp/Resolve-PnPFolder.md)