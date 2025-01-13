---
external help file: C64OSTool.dll-Help.xml
Module Name: C64OSUtil
online version:
schema: 2.0.0
---

# Export-C64Carfile

## SYNOPSIS
Write a general car file object to a CAR file.

## SYNTAX

```
Export-C64Carfile -Car <C64Car> [-Path] <String> [<CommonParameters>]
```

## DESCRIPTION
Write a general car file object to a CAR file.

## EXAMPLES

### Example 1
```powershell
PS C:\> Get-C64CarArchive backdrops1.car | Export-C64Carfile -Path d:\foo.car
```

On Mac or Linux, use '/' instead of '\' in paths.

## PARAMETERS

### -Car
The input object

```yaml
Type: C64Car
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

### C64OSTool.C64Car
## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS
