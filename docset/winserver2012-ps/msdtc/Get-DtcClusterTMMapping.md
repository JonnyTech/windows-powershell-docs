---
external help file: MsDTC_Cmdlets.xml
online version: 
schema: 2.0.0
ms.assetid: A0E89672-2370-41BC-9142-3657C4792194
---

# Get-DtcClusterTMMapping

## SYNOPSIS
Gets cluster DTC Mapping data.

## SYNTAX

```
Get-DtcClusterTMMapping [-CimSession <CimSession[]>] [-Name <String>] [-ThrottleLimit <Int32>]
```

## DESCRIPTION
The **Get-DtcClusterTMMapping** cmdlet gets cluster Distributed Transaction Coordinator (DTC) Mapping data.
If you do not specify the **Name** parameter, the cmdlet gets all cluster Transaction Manager (TM) mapping data.
This cmdlet is supported on clustered computers only.

## EXAMPLES

### Example 1: Get cluster mapping
```
PS C:\>Get-DtcClusterTMMapping -Name "TestMapping"
```

This example get the cluster DTC TM mapping for the **MappingName** TestMapping.

## PARAMETERS

### -CimSession
Runs the cmdlet in a remote session or on a remote computer.
Enter a computer name or a session object, such as the output of a New-CimSessionhttp://go.microsoft.com/fwlink/p/?LinkId=227967 or Get-CimSessionhttp://go.microsoft.com/fwlink/p/?LinkId=227966 cmdlet.
The default is the current session on the local computer.

```yaml
Type: CimSession[]
Parameter Sets: (All)
Aliases: Session

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
Specifies the **MappingName**.
If you do not specify this parameter, the cmdlet gets all TM mappings.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue, ByPropertyName)
Accept wildcard characters: False
```

### -ThrottleLimit
Specifies the maximum number of concurrent operations that can be established to run the cmdlet.
If this parameter is omitted or a value of `0` is entered, then Windows PowerShell® calculates an optimum throttle limit for the cmdlet based on the number of CIM cmdlets that are running on the computer.
The throttle limit applies only to the current cmdlet, not to the session or to the computer.

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

## INPUTS

## OUTPUTS

### DtcClusterTMMapping
This cmdlet returns a **DtcClusterTMMapping** object that contains the specified **MappingName** value.
If you do not specify a **MappingName**, this cmdlet gets all mappings.

## NOTES

## RELATED LINKS

[Add-DtcClusterTMMapping](./Add-DtcClusterTMMapping.md)

[Remove-DtcClusterTMMapping](./Remove-DtcClusterTMMapping.md)

[Set-DtcClusterTMMapping](./Set-DtcClusterTMMapping.md)
