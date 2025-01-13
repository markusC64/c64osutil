---
external help file: C64OSTool.dll-Help.xml
Module Name: C64OSUtil
online version:
schema: 2.0.0
---

# New-C64CarArchive

## SYNOPSIS
Creates a new general car object

## SYNTAX

```
New-C64CarArchive -CarType <carType> -Version <Byte> -Date <carDateTime> -NotesASCII <String>
 [<CommonParameters>]
```

## DESCRIPTION
Creates a new general car object

## EXAMPLES

### Create a new car file
```
$car =  New-C64CarArchive -CarType install -Version 2 `
   -Date (New-C64CarArchiveDate -Year 123 -Month 6 -Day 4 -Hour 8 -Minute 0) `
   -NotesASCII "PWSH only: Upd C64OS 1.0->1.0P"
Update-C64CarArchive -Car $car -Path / -Directory  -FileType ([byte][char]'D') -FilenameASCII "d 1.0P <- 1.0"
Update-C64CarArchive -Car $car -Path "/services/File Manager/init.o"  -File -FileType ([byte][char]'P') -FileContent (Get-Content -Raw -AsByteStream 1.0p\init.o.PRG )
Update-C64CarArchive -Car $car -Path "/utilities/Installer"  -File -FileType ([byte][char]'P') -FileContent (Get-Content -Raw -AsByteStream 1.0p\Installer.PRG )
Update-C64CarArchive -Car $car -Path "/settings/version.t"  -File -FileType ([byte][char]'S') -FileContent (Get-Content -Raw -AsByteStream 1.0p\version.t.SEQ )
Export-C64Carfile -Car $car -Path 1.0p.update.car
```

On Mac or Linux, use '/' instead of '\' in paths.

## PARAMETERS

### -CarType
@{Text=}

```yaml
Type: carType
Parameter Sets: (All)
Aliases:
Accepted values: general, restore, install

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Version
@{Text=}

```yaml
Type: Byte
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Date
@{Text=}

```yaml
Type: carDateTime
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NotesASCII
@{Text=}

```yaml
Type: String
Parameter Sets: (All)
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

### C64OSTool.C64Car
## NOTES

## RELATED LINKS
