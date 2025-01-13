---
external help file: C64OSTool.dll-Help.xml
Module Name: C64OSUtil
online version:
schema: 2.0.0
---

# Export-C64OSCarfile

## SYNOPSIS
Exports an object of Type C64OSCar to a restore.car file

## SYNTAX

```
Export-C64OSCarfile -C64OS <C64OSCar> [-Path] <String> [<CommonParameters>]
```

## DESCRIPTION
Exports an object of Type C64OSCarto a restore.car file.

## EXAMPLES

### Update restore.car and write result as car file to a file.
```
C:\PS> get-C64OSRestore restore.car | Merge-C64OSUpdate .\updates\1.01.update.car, .\updates\1.02.update.car, .\updates\1.03.update.car | Export-C64OSCarfile -Path .\restore-1.03.car
```

## PARAMETERS

### -C64OS
Rhe Object to export

```yaml
Type: C64OSCar
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Path
The file to write to

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### C64OSTool.C64OSCar
## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS
