`MCC;MNC;LAC;CID;LATITUDE;LONGITUDE;DESCRIPTION;ACCURACY`

| Parameter | Description |
| --- | --- |
| MCC | 3 digits |
| MNC | 2 or 3 digits (GSM, WCDMA, LTE, 5G), 5 digits SID (CDMA) |
| LAC | LAC (GSM, WCDMA), TAC (LTE, 5G), NID (CDMA) |
| CID | CID (GSM, WCDMA), CI (LTE, eNodeB+sector), NCI (5G), BID (CDMA) |
| LATITUDE | `[-90;90]`, `.` as separator |
| LONGITUDE | `[-180;180]`, `.` as separator |
| ACCURACY | in meters, `-1` if location is exact, `0` if unknown |
| DESCRIPTION | text |

GSM:<br>
MCC = 262, MNC = 02, LAC = 510, CID = 9571, LATITUDE = -90.0, LONGITUDE = 180.0, ACCURACY = 100, DESCRIPTION = info<br>
`262;02;510;9571;-90.0;180.0;info;100`

LTE:<br>
MCC = 230, MNC = 01, LAC = 16464, CI = 1144587 (eNodeB = 4471, sector = 11), LATITUDE = -90.0, LONGITUDE = 180.0, ACCURACY = 100, DESCRIPTION = info<br>
`230;01;16464;1144587;-90.0;180.0;info;100`