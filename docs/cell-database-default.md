`NETWORK_TYPE;MCC;MNC;LAC;CID;PSC;CHANNEL;LATITUDE;LONGITUDE;ACCURACY;DESCRIPTION`

| Parameter | Type | Description | Import |
| --- | --- | --- | --- |
| NETWORK_TYPE | String | `C` (CDMA), `G` (GSM), `W` (WCDMA), `T` (TDSCDMA), `L` (LTE), `N` (5G NR) | Mandatory for CDMA |
| MCC | String | 3 digits | Mandatory |
| MNC | String | 2 or 3 digits | Mandatory |
| LAC | Int | NID (CDMA), LAC (GSM, WCDMA, TDSCDMA), TAC (LTE, 5G NR) | Mandatory |
| CID | Long | BID (CDMA), CID (GSM, WCDMA, TDSCDMA), CI (LTE), NCI (5G NR) | Mandatory |
| PSC | Int | SID (CDMA), BSIC (GSM), PSC (WCDMA), CPID (TDSCDMA), PCI (LTE, 5G NR) | Mandatory for CDMA |
| CHANNEL | Int | ARFCN (GSM, 5G NR), UARFCN (WCDMA, TDSCDMA), EARFCN (LTE) ||
| LATITUDE | Double | `[-90;90]`, `.` as separator ||
| LONGITUDE | Double | `[-180;180]`, `.` as separator ||
| ACCURACY | Int | in meters ||
| DESCRIPTION | String | text ||

GSM:<br>
MCC = 262, MNC = 02, LAC = 510, CID = 9571, LATITUDE = -90.0, LONGITUDE = 180.0, ACCURACY = 100, DESCRIPTION = info<br>
`G;262;02;510;9571;;;-90.0;180.0;100;info`

LTE:<br>
MCC = 230, MNC = 01, LAC = 16464, CI = 1144587 (eNodeB = 4471, sector = 11), PCI = 49, EARFCN = 3025, LATITUDE = -90.0, LONGITUDE = 180.0, ACCURACY = 100, DESCRIPTION = info<br>
`L;230;01;16464;1144587;49;3025;-90.0;180.0;100;info`