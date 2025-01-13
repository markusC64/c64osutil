---
external help file: C64OSTool.dll-Help.xml
Module Name: C64OSUtil
online version:
schema: 2.0.0
---

# Get-C64CarArchive

## SYNOPSIS
Reads a general CAR archive into an object

## SYNTAX

### FromFile
```
Get-C64CarArchive [-Path] <String> [<CommonParameters>]
```

### FromC64OS
```
Get-C64CarArchive -C64OS <C64OSCar> [<CommonParameters>]
```

## DESCRIPTION
Reads a general CAR archive into an object

## EXAMPLES

### Read a car file
```powershell
PS C:\> Get-C64CarArchive backdrops1.car
```

On Mac or Linux, use '/' instead of '\' in paths.

## PARAMETERS

### -Path
the file to read from

```yaml
Type: String
Parameter Sets: FromFile
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -C64OS
In order to convert an C64 OS restore.car object (a special car file) use this parameter

```yaml
Type: C64OSCar
Parameter Sets: FromC64OS
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### C64OSTool.C64OSCar
## OUTPUTS

### C64OSTool.C64Car
## NOTES

## RELATED LINKS
