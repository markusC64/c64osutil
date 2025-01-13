---
external help file: C64OSTool.dll-Help.xml
Module Name: C64OSUtil
online version:
schema: 2.0.0
---

# New-C64CarArchiveDate

## SYNOPSIS
Creates an object representing the creation date of a car file

## SYNTAX

### value
```
New-C64CarArchiveDate -Year <Byte> -Month <Byte> -Day <Byte> -Hour <Byte> -Minute <Byte> [<CommonParameters>]
```

### now
```
New-C64CarArchiveDate [-Now] [<CommonParameters>]
```

## DESCRIPTION
Creates an object representing the creation date of a car file

See New-C64CarArchive for an example.

## EXAMPLES

### Example 1
```powershell
PS C:\> {{ Add example code here }}
```

{{ Add example description here }}

## PARAMETERS

### -Year
The actual year minus 1900

```yaml
Type: Byte
Parameter Sets: value
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Month
The actual month

```yaml
Type: Byte
Parameter Sets: value
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Day
The actual day

```yaml
Type: Byte
Parameter Sets: value
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Hour
The actual Hour

```yaml
Type: Byte
Parameter Sets: value
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Minute
The actual Minute

```yaml
Type: Byte
Parameter Sets: value
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Now
Create an object using the current timestamp

```yaml
Type: SwitchParameter
Parameter Sets: now
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None
## OUTPUTS

### CommodoreDisk.Archive.car.carDateTime
## NOTES

## RELATED LINKS
