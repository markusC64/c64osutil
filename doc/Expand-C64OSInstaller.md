---
external help file: C64OSTool.dll-Help.xml
Module Name: C64OSUtil
online version:
schema: 2.0.0
---

# Expand-C64OSInstaller

## SYNOPSIS
Create an installer from a restore.car object and optionally installs C64 OS

## SYNTAX

```
Expand-C64OSInstaller -C64OS <C64OSCar> [-Path] <String> [-ExtensionInRoot <Boolean>]
 [-FilenameConvention <filenameConvntion>] [-Install <Boolean>] [-SkipRestoreCar <Boolean>]
 [<CommonParameters>]
```

## DESCRIPTION
Create an installer from a restore.car object and optionally installs C64 OS

## EXAMPLES

### Typical workflow
```
C:\PS> get-C64OSRestore restore.car | Merge-C64OSUpdate .\updates\1.01.update.car, .\updates\1.02.update.car, .\updates\1.03.update.car | Expand-C64OSInstaller d:\ -Install $true
```

On Mac or Linux, use '/' instead of '\' in paths.

## PARAMETERS

### -C64OS
The restore.car object to use

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
The path where to save the output.
Must be an empty directory.

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

### -ExtensionInRoot
Enable or disable extensions in root, that is ".prg", ".seq".

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

### -FilenameConvention
Choose a filename convention:
Raw             - '.prg' and '.seq" files, sd2iec compatible
Ultimate64    -  prg' and '.seq" files, ultimate 64 compatible
x00               - (default) creates x00 files

```yaml
Type: filenameConvntion
Parameter Sets: (All)
Aliases:
Accepted values: ultimate64, raw, x00

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Install
Enables installation of C64 OS that is extracting the "OS" directory

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

### -SkipRestoreCar
Disables creating of restore.car

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### C64OSTool.C64OSCar
## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS
