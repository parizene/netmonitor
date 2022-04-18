## Clf v2.0

`{CID}{LAC}{MCC}{MNC}<TAB>{DESCRIPTION}`

| Parameter | Description |
| --- | --- |
| CID | 4 digits (hex) |
| LAC | 4 digits (hex) |
| MCC | 3 digits |
| MNC | 2 or 3 digits |
| DESCRIPTION | text, 100 characters |

MCC = 262, MNC = 02, LAC = 510 (0x01FE), CID = 9571 (0x2563), DESCRIPTION = info<br>
`256301FE26202<TAB>info`

## Clf v2.1

`{CID}{LAC}{MCC}{MNC}<TAB>{DESCRIPTION}`

| Parameter | Description |
| --- | --- |
| CID | 5 digits |
| LAC | 5 digits |
| MCC | 3 digits |
| MNC | 2 or 3 digits |
| DESCRIPTION | text, 100 characters |

MCC = 262, MNC = 02, LAC = 510, CID = 9571, DESCRIPTION = info<br>
`095710051026202<TAB>info`

## Clf v3.0 (hex)

`MCCMNC;CID;LAC;RNC;POS-LAT;POS-LON;POS-RAT;DESCRIPTION;RFU`

| Parameter | Description |
| --- | --- |
| MCC | 3 digits |
| MNC | 2 or 3 digits |
| CID | 4 digits (hex, `0x` prefix) |
| LAC | 4 digits (hex, `0x` prefix) |
| RNC | 4 digits (hex, `0x` prefix), used only for WCDMA |
| POS-LAT | latitude `[-90;90]`, `.` as separator |
| POS-LON | longitude `[-180;180]`, `.` as separator |
| POS-RAT | always `-1` |
| DESCRIPTION | text |
| RFU | always `0` |

MCC = 262, MNC = 02, LAC = 510, CID = 9571, LATITUDE = -90.0, LONGITUDE = 180.0, DESCRIPTION = info<br>
`26202;0x2563;0x01FE;0x0000;-90.0;180.0;-1;info;0`

## Clf v3.0 (dec)

`MCCMNC;CID;LAC;RNC;POS-LAT;POS-LON;POS-RAT;DESCRIPTION;RFU`

| Parameter | Description |
| --- | --- |
| MCC | 3 digits |
| MNC | 2 or 3 digits |
| CID | 5 digits |
| LAC | 5 digits |
| RNC | 5 digits, used only for WCDMA |
| POS-LAT | latitude `[-90;90]`, `.` as separator |
| POS-LON | longitude `[-180;180]`, `.` as separator |
| POS-RAT | always `-1` |
| DESCRIPTION | text |
| RFU | always `0` |

MCC = 262, MNC = 02, LAC = 510, CID = 9571, LATITUDE = -90.0, LONGITUDE = 180.0, DESCRIPTION = info<br>
`26202;09571;00510;00000;-90.0;180.0;-1;info;0`
