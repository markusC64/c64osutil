---
external help file: C64OSTool.dll-Help.xml
Module Name: C64OSUtil
online version:
schema: 2.0.0
---

# Merge-C64OSUpdate

## SYNOPSIS
Merge C64 OS Updates into restore.car

## SYNTAX

### FromCar
```
Merge-C64OSUpdate -C64OS <C64OSCar> [-Car] <C64Car[]> [-Force] [<CommonParameters>]
```

### FromFile
```
Merge-C64OSUpdate -C64OS <C64OSCar> [-Path] <String[]> [-Force] [<CommonParameters>]
```

## DESCRIPTION
This Cmdlet merges C64 OS updates into an object representing C64 OS restore.car.
It heurestically checks if the update can be applied.
If that check fails, you can try to apply the update with the parameter '-force'

## EXAMPLES

### Merge Updates
```
C:\PS> get-C64OSRestore restore.car | Merge-C64OSUpdate .\updates\1.01.update.car, .\updates\1.02.update.car, .\updates\1.03.update.car
```

On Mac or Linux, use '/' instead of '\' in paths.

## PARAMETERS

### -C64OS
The object containg restore.car to patch

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

### -Car
The patch to be applied as an object

```yaml
Type: C64Car[]
Parameter Sets: FromCar
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Force
Skip heuristic for checking if update can be applied

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

### -Path
The patch to be applied as a file resp.
files.

```yaml
Type: String[]
Parameter Sets: FromFile
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
An object representing restre.car of C64 OS

## OUTPUTS

### C64OSTool.C64OSCar
An object representing restre.car of C64 OS

## NOTES

## RELATED LINKS
