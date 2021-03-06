---
applicable: SharePoint Online
external help file: PnP.PowerShell.dll-Help.xml
Module Name: PnP.PowerShell
online version: https://docs.microsoft.com/powershell/module/sharepoint-pnp/get-pnpjavascriptlink
schema: 2.0.0
title: Get-PnPJavaScriptLink
---

# Get-PnPJavaScriptLink

## SYNOPSIS
Returns all or a specific custom action(s) with location type ScriptLink

## SYNTAX

```
Get-PnPJavaScriptLink [[-Name] <String>] [-Scope <CustomActionScope>] [-ThrowExceptionIfJavaScriptLinkNotFound]
 [-Web <WebPipeBind>] [-Connection <PnPConnection>] [<CommonParameters>]
```

## DESCRIPTION

## EXAMPLES

### EXAMPLE 1
```powershell
Get-PnPJavaScriptLink
```

Returns all web scoped JavaScript links

### EXAMPLE 2
```powershell
Get-PnPJavaScriptLink -Scope All
```

Returns all web and site scoped JavaScript links

### EXAMPLE 3
```powershell
Get-PnPJavaScriptLink -Scope Web
```

Returns all Web scoped JavaScript links

### EXAMPLE 4
```powershell
Get-PnPJavaScriptLink -Scope Site
```

Returns all Site scoped JavaScript links

### EXAMPLE 5
```powershell
Get-PnPJavaScriptLink -Name Test
```

Returns the web scoped JavaScript link named Test

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

### -Name
Name of the Javascript link. Omit this parameter to retrieve all script links

```yaml
Type: String
Parameter Sets: (All)
Aliases: Key

Required: False
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Scope
Scope of the action, either Web, Site or All to return both, defaults to Web

```yaml
Type: CustomActionScope
Parameter Sets: (All)
Aliases:
Accepted values: Web, Site, All

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ThrowExceptionIfJavaScriptLinkNotFound
Switch parameter if an exception should be thrown if the requested JavaScriptLink does not exist (true) or if omitted, nothing will be returned in case the JavaScriptLink does not exist

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

## RELATED LINKS

[SharePoint Developer Patterns and Practices](https://aka.ms/sppnp)