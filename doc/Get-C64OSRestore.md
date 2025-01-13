---
external help file: C64OSTool.dll-Help.xml
Module Name: C64OSUtil
online version:
schema: 2.0.0
---

# Get-C64OSRestore

## SYNOPSIS
Reads the file "restore.car" from a C64 OS installation into memory

## SYNTAX

### FromFile
```
Get-C64OSRestore [-Path] <String> [<CommonParameters>]
```

### FromCAR
```
Get-C64OSRestore -Car <C64Car> [<CommonParameters>]
```

## DESCRIPTION
This cmdlet raeds the file "restore.car" from a C64 OS installation into memory.
Source can be a file or an object.

## EXAMPLES

### Read restore.car
```
C:\PS> Get-C64OSRestore .\restore.car
```

On Mac or Linux, use '/' instead of '\' in paths.

### Read restore.car and assign to a variable
```
C:\PS> G$c64os = Get-C64OSRestore .\restore.car
```

On Mac or Linux, use '/' instead of '\' in paths.

## PARAMETERS

### -Path
In order to read the restore.car from a file, use this parammeter with the actual path.

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

### -Car
In order to read the restore.car from an object of type C64Car, use this parameter.

```yaml
Type: C64Car
Parameter Sets: FromCAR
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

### C64OSTool.C64OSCar
This object type represents a 'restore.car' as part of C64 OS.

## NOTES

## RELATED LINKS
