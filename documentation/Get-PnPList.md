---
applicable: SharePoint Online
external help file: PnP.PowerShell.dll-Help.xml
Module Name: PnP.PowerShell
online version: https://docs.microsoft.com/powershell/module/sharepoint-pnp/get-pnplist
schema: 2.0.0
title: Get-PnPList
---

# Get-PnPList

## SYNOPSIS
Returns lists from SharePoint

## SYNTAX

```
Get-PnPList [[-Identity] <ListPipeBind>] [-ThrowExceptionIfListNotFound] [-Web <WebPipeBind>]
 [-Connection <PnPConnection>] [-Includes <String[]>] [<CommonParameters>]
```

## DESCRIPTION

## EXAMPLES

### EXAMPLE 1
```powershell
Get-PnPList
```

Returns all lists in the current web

### EXAMPLE 2
```powershell
Get-PnPList -Identity 99a00f6e-fb81-4dc7-8eac-e09c6f9132fe
```

Returns a list with the given id

### EXAMPLE 3
```powershell
Get-PnPList -Identity Lists/Announcements
```

Returns a list with the given url

### EXAMPLE 4
```powershell
Get-PnPList | Where-Object {$_.RootFolder.ServerRelativeUrl -like "/lists/*"}
```

This examples shows how to do wildcard searches on the list URL. It returns all lists whose URL starts with "/lists/" This could also be used to search for strings inside of the URL.

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
The ID, name or Url (Lists/MyList) of the list

```yaml
Type: ListPipeBind
Parameter Sets: (All)
Aliases:

Required: False
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ThrowExceptionIfListNotFound
Switch parameter if an exception should be thrown if the requested list does not exist (true) or if omitted, nothing will be returned in case the list does not exist

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

[SharePoint Developer Patterns and Practices](https://aka.ms/sppnp)