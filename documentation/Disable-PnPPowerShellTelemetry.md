---
applicable: SharePoint Online
external help file: PnP.PowerShell.dll-Help.xml
Module Name: PnP.PowerShell
online version: https://docs.microsoft.com/powershell/module/sharepoint-pnp/disable-pnppowershelltelemetry
schema: 2.0.0
title: Disable-PnPPowerShellTelemetry
---

# Disable-PnPPowerShellTelemetry

## SYNOPSIS
Disables PnP PowerShell telemetry tracking

## SYNTAX

```
Disable-PnPPowerShellTelemetry [-Force] [<CommonParameters>]
```

## DESCRIPTION
Disables PnP PowerShell telemetry tracking

## EXAMPLES

### EXAMPLE 1
```powershell
Disable-PnPPowerShellTelemetry
```

Will prompt you to confirm to disable telemetry tracking.

### EXAMPLE 2
```powershell
Disable-PnPPowerShellTelemetry -Force
```

Will disable telemetry tracking without prompting.

## PARAMETERS

### -Force
Specifying the Force parameter will skip the confirmation question.

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