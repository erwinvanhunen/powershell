---
applicable: SharePoint Online
external help file: PnP.PowerShell.dll-Help.xml
Module Name: PnP.PowerShell
online version: https://docs.microsoft.com/powershell/module/sharepoint-pnp/set-pnplistinformationrightsmanagement
schema: 2.0.0
title: Set-PnPListInformationRightsManagement
---

# Set-PnPListInformationRightsManagement

## SYNOPSIS
Get the site closure status of the site which has a site policy applied

## SYNTAX

```
Set-PnPListInformationRightsManagement -List <ListPipeBind> [-Enable <Boolean>] [-EnableExpiration <Boolean>]
 [-EnableRejection <Boolean>] [-AllowPrint <Boolean>] [-AllowScript <Boolean>] [-AllowWriteCopy <Boolean>]
 [-DisableDocumentBrowserView <Boolean>] [-DocumentAccessExpireDays <Int32>]
 [-DocumentLibraryProtectionExpireDate <DateTime>] [-EnableDocumentAccessExpire <Boolean>]
 [-EnableDocumentBrowserPublishingView <Boolean>] [-EnableGroupProtection <Boolean>]
 [-EnableLicenseCacheExpire <Boolean>] [-LicenseCacheExpireDays <Int32>] [-GroupName <String>]
 [-PolicyDescription <String>] [-PolicyTitle <String>] [-TemplateId <String>] [-Web <WebPipeBind>]
 [-Connection <PnPConnection>] [<CommonParameters>]
```

## DESCRIPTION

## EXAMPLES

### EXAMPLE 1
```powershell
Set-PnPListInformationRightsManagement -List "Documents" -Enabled $true
```

Enables Information Rights Management (IRM) on the list.

## PARAMETERS

### -AllowPrint
Sets a value indicating whether the viewer can print the downloaded document.

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AllowScript
Sets a value indicating whether the viewer can run a script on the downloaded document.

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AllowWriteCopy
Sets a value indicating whether the viewer can write on a copy of the downloaded document.

```yaml
Type: Boolean
Parameter Sets: (All)
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

### -DisableDocumentBrowserView
Sets a value indicating whether to block Office Web Application Companion applications (WACs) from showing this document.

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DocumentAccessExpireDays
Sets the number of days after which the downloaded document will expire.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DocumentLibraryProtectionExpireDate
Sets the date after which the Information Rights Management (IRM) protection of this document library will stop.

```yaml
Type: DateTime
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Enable
Specifies whether Information Rights Management (IRM) is enabled for the list.

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EnableDocumentAccessExpire
Sets a value indicating whether the downloaded document will expire.

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EnableDocumentBrowserPublishingView
Sets a value indicating whether to enable Office Web Application Companion applications (WACs) to publishing view.

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EnableExpiration
Specifies whether Information Rights Management (IRM) expiration is enabled for the list.

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EnableGroupProtection
Sets a value indicating whether the permission of the downloaded document is applicable to a group.

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EnableLicenseCacheExpire
Sets whether a user must verify their credentials after some interval.

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EnableRejection
Specifies whether Information Rights Management (IRM) rejection is enabled for the list.

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -GroupName
Sets the group name (email address) that the permission is also applicable to.

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

### -LicenseCacheExpireDays
Sets the number of days that the application that opens the document caches the IRM license. When these elapse, the application will connect to the IRM server to validate the license.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -List
The list to set Information Rights Management (IRM) settings for.

```yaml
Type: ListPipeBind
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PolicyDescription
Sets the permission policy description.

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

### -PolicyTitle
Sets the permission policy title.

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

### -TemplateId

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