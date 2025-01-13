---
external help file: C64OSTool.dll-Help.xml
Module Name: C64OSUtil
online version:
schema: 2.0.0
---

# Expand-C64CarFile

## SYNOPSIS
Expands a general car file

## SYNTAX

```
Expand-C64CarFile -Car <C64Car> [-Path] <String> [-FilenameConvention <filenameConvntion>] [<CommonParameters>]
```

## DESCRIPTION
Expands a general car file

## EXAMPLES

### Example 1
```powershell
PS C:\> {{ Add example code here }}
```

{{ Add example description here }}

## PARAMETERS

### -Car
The inputz oobject

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
Thepath to werite to.
Works best when pointing to an empty directory.

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

### -FilenameConvention
The Filename COnvention to use.
Cfg.
Expand-C64OSInstaller.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### C64OSTool.C64Car
## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS
