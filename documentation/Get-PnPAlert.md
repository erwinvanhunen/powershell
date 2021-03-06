---
applicable: SharePoint Online
external help file: PnP.PowerShell.dll-Help.xml
Module Name: PnP.PowerShell
online version: https://docs.microsoft.com/powershell/module/sharepoint-pnp/get-pnpalert
schema: 2.0.0
title: Get-PnPAlert
---

# Get-PnPAlert

## SYNOPSIS
Returns registered alerts for a user.

## SYNTAX

```
Get-PnPAlert [[-List] <ListPipeBind>] [-User <UserPipeBind>] [-Title <String>] [-Web <WebPipeBind>]
 [-Connection <PnPConnection>] [<CommonParameters>]
```

## DESCRIPTION

## EXAMPLES

### EXAMPLE 1
```powershell
Get-PnPAlert
```

Returns all registered alerts for the current user

### EXAMPLE 2
```powershell
Get-PnPAlert -List "Demo List"
```

Returns all alerts registered on the given list for the current user.

### EXAMPLE 3
```powershell
Get-PnPAlert -List "Demo List" -User "i:0#.f|membership|Alice@contoso.onmicrosoft.com"
```

Returns all alerts registered on the given list for the specified user.

### EXAMPLE 4
```powershell
Get-PnPAlert -Title "Demo Alert"
```

Returns all alerts with the given title for the current user. Title comparison is case sensitive.

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

### -List
The ID, Title or Url of the list.

Only applicable to: SharePoint Online, SharePoint Server 2019

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

### -Title
Retrieve alerts with this title. Title comparison is case sensitive.

Only applicable to: SharePoint Online, SharePoint Server 2019

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

### -User
User to retrieve the alerts for (User ID, login name or actual User object). Skip this parameter to retrieve the alerts for the current user. Note: Only site owners can retrieve alerts for other users.

Only applicable to: SharePoint Online, SharePoint Server 2019

```yaml
Type: UserPipeBind
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

Only applicable to: SharePoint Online, SharePoint Server 2019

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