---
external help file: C64OSTool.dll-Help.xml
Module Name: C64OSUtil
online version:
schema: 2.0.0
---

# Enable-IECDevice

## SYNOPSIS
Enables the IEC device for the ultimate 64 resp.
1541 ultimate.
Warning: This feature needs a suitable firmware on that device and is just for developers.

## SYNTAX

```
Enable-IECDevice -C64OS <C64OSCar> [<CommonParameters>]
```

## DESCRIPTION
Enables the IEC device for the ultimate 64 resp.
1541 ultimate.
Warning: This feature needs a suitable firmware on that device and is just for developers.

## EXAMPLES

### Example 1
```powershell
PS C:\> get-C64OSRestore restore.car | Enable-IECDevice
```

Warning: This feature needs a suitable firmware on that device and is just for developers.

## PARAMETERS

### -C64OS
@{Text=}

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### C64OSTool.C64OSCar
## OUTPUTS

### System.Object
## NOTES

## RELATED LINKS
