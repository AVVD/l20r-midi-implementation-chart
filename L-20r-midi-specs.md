L-20 MIDI implementation table
===
## MIDI CC
*Work In Progress*
Dec|Hex|Channel|Name|TX|RX|Comment
---|---|---|---|---|---|---
4  |0x04|0, 2|USB 1-2, USB3-4|00,01|01|00 = Input, 01 = Usb
8  |0x08|1-16|REC/PLAY|00,01,02|01|00 = Disabled, 01 = Play, 02 = Rec
9  |0x09|1, 3|-|-|-|*17\_18, 19\_20*
10 |0x0A|1-16|PHASE|00,01|01|00 = Normal, 01 = Inverted
11 |0x0B|1, 3|-|-|-|*17\_18, 19\_20*
12 |0x0C|1-16|PAN|00-64|00-64|32 = Center
13 |0x0D|1, 3|-|-|-|*17\_18, 19\_20*
14 |0x0E|1-16|EQ ON/OFF|00,01|01|00 = On, 01 = Off
15 |0x0F|1, 3|-|-|-|*17\_18, 19\_20*
20 |0x14|1-16|EQ HIGH|00-3C|00-3C|1E = 0
21 |0x15|1, 3|-|-|-|*17\_18, 19\_20*
24 |0x18|1-16|EQ MID FREQ|00-60|00-60|30 = 0
25 |0x19|1, 3|-|-|-|*17\_18, 19\_20*
26 |0x1A|1-16|EQ MID|00-3C|00-3C|1E = 0
27 |0x1B|1, 3|-|-|-|*17\_18, 19\_20*
44 |0x2C|1-16|EQ LOW|00-3C|00-3C|1E = 0
45 |0x2D|1, 3|-|-|-|*17\_18, 19\_20*
46 |0x2E|1-16|EQ LOCUT|00-38|00-38|00 = 0
47 |0x2F|1, 3|-|-|-|*17\_18, 19\_20*
48 |0x30|1-16|MUTE|00,01|01|00 = Off, 01 = On
49 |0x31|1, 3|-|-|-|*17\_18, 19\_20*
50 |0x32|1-16|SOLO|00,01|01|00 = Off, 01 = On
51 |0x33|1, 3|-|-|-|*17\_18, 19\_20*
52 |0x34|1-16|SEND FX1|00-78|00-78|00 = 0
53 |0x35|1, 3|-|-|-|*17\_18, 19\_20*
54 |0x36|1-16|SEND FX2|00-78|00-78||
55 |0x37|1, 3|-|-|-|*17\_18, 19\_20*
60 |0x3C|1-16|FADER MIX MASTER|00-78|00-78|64 = 0dB
61 |0x3D|1, 3|-|-|-|*17\_18, 19\_20*
62 |0x3E|1-16|FADER MIX A|00-78|00-78
63 |0x3F|1, 3|-|-|-|*17\_18, 19\_20*
64 |0x40|1-16|FADER MIX B|00-78|00-78|
65 |0x41|1, 3|-|-|-|*17\_18, 19\_20*
66 |0x42|1-16|FADER MIX C|00-78|00-78|
67 |0x43|1, 3|-|-|-|*17\_18, 19\_20*
68 |0x44|1-16|FADER MIX D|00-78|00-78|
69 |0x45|1, 3|-|-|-|*17\_18, 19\_20*
70 |0x46|1-16|FADER MIX E|00-78|00-78|
71 |0x47|1, 3|-|-|-|*17\_18, 19\_20*
72 |0x48|1-16|FADER MIX F|00-78|00-78|
73 |0x3E|1, 3|-|-|-|*17\_18, 19\_20*
78 |0x4E|1|EFX1 Type|00-09|00-09|
-|-|2|EFX2 Type|00-09|00-09|
-|-|5|EFX1 Tone MSB|00-64|00-64
-|-|6|EFX1 Tone LSB|00-64|00-64
-|-|7|EFX2 Tone MSB|00-??|00-??
-|-|8|EFX2 Tone LSB|00-??|00-??
-|-|13|EFX1 Decay MSB|00-??|00-??
-|-|14|EFX1 Decay LSB|00-??|00-??
-|-|15|EFX2 Decay MSB|00-??|00-??
-|-|16|EFX2 Decay LSB|00-??|00-??
80|0x50|?|
-|-|5|FX1 MUTE|0,1|1|0 = Off, 1 = On
-|-|6|FX2 MUTE|0,1|1|0 = Off, 1 = On
-|-|9|FX1 SOLO|0,1|1|0 = Off, 1 = On
-|-|10|FX2 SOLO|0,1|1|0 = Off, 1 = On
-|-|c+1|FX1 FADER|00-78|00-78|64 = 0dB
-|-|d+1|FX2 FADER|00-78|00-78|64 = 0dB
83|0x53|1-6|VOLUME MONITOR A-F|00-78|00-78|64 = 0dB
84|0x54|9|Master selection button|1,2|1|1 = Play, 2 = Rec
-|-|10|MASTER MUTE|0,1|1|0 = Off, 1 = On
-|-|11|MASTER FADER|00-78|00-78|64 = 0dB
85|0x55|1|GLOBAL EQ 25Hz|00-60|00-60|
-|-|2|GLOBAL EQ 40Hz|00-60|00-60|
-|-|3|GLOBAL EQ 63Hz|00-60|00-60|
-|-|4|GLOBAL EQ 100Hz|00-60|00-60|
-|-|5|GLOBAL EQ 160Hz|00-60|00-60|
-|-|6|GLOBAL EQ 250Hz|00-60|00-60|
-|-|7|GLOBAL EQ 400Hz|00-60|00-60|
-|-|8|GLOBAL EQ 630Hz|00-60|00-60|
-|-|9|GLOBAL EQ 1kHz|00-60|00-60|
-|-|10|GLOBAL EQ 1.6kHz|00-60|00-60|
-|-|11|GLOBAL EQ 2.5kHz|00-60|00-60|
-|-|12|GLOBAL EQ 4kHz|00-60|00-60|
-|-|13|GLOBAL EQ 6.3kHz|00-60|00-60|
-|-|14|GLOBAL EQ 10kHz|00-60|00-60|
-|-|15|GLOBAL EQ 16kHz|00-60|00-60|
-|-|16|GLOBAL EQ ON/OFF|0,1|1|0 = Off, 1 = On
86|0x56|9|Scene on/off|0,1|1|0 = Off, 1 = On
87|0x57|6|Fader Mode M-F|0-6|0-6| Select Mix for VU Meter
-|-|9|LED PLAY PAUSE|?|x|
-|-|10|REC|?|?|
-|-|11|PLAY PAUSE|?|?|
-|-|12|STOP|?|?|
-|-|13|REWIND|?|?|
-|-|14|FAST FORWARD|?|?|
-|-|15|OVERDUB|?|?|
88|0x59|1|Marker|0-??|x|
-|-|5|Song HH..|0-99|x| HHhh:mm:ss
-|-|6|Sont ..hh|0-99|x|
-|-|7|Song mm|0-59|x|
-|-|8|Song ss|0-59|x|
-|-|9|Current HH..|0-99|x| HHhh:mm:ss
-|-|10|Current ..hh|0-99|x|
-|-|11|Current mm|0-59|x|
-|-|12|Current ss|0-59|x|

## SysEx
*Work In Progress*
### SysEx message
TX \/ RX|Start|Manufacturer ID|Device ID|Command|Data|End|Comment
---|---|---|---|---|---|---|---
-|F0|52 00 00|31|xx|xx..xx|F7|Generic
-|-|*Zoom*|*L20r*|-|-|-|
RX|F0|7E 00 06|01|-|-|F7|Universal MIDI Ident
TX|F0|7E 00 06|02|52|72 00 03 00 31 2E 31 33|F7|UMI Reply
-|-|-|-|*Zoom*|72 00 03 00 *L20r* 2E *1.13*|-|

*Work In Progress*
### Command
TX \/ RX|Command|Data|Name|Comment
---|---|---|---|---
RX|2B|-|Ask Channel Names
TX|2A|05 00 00 ...|Channel Names
RX|07|-|Ask Scene names
TX|06|00-02 ...|Scene names
RX|50|-|Start Monitoring Volumes
RX|51|-|Stop Monitor Volumes

### Data
Offset|Name|Values|Size|Type
---|---|---|---|---
0|Change Name|02|1
1|Tranche|01-12|1
2|ASCII Chars|XX XX XX XX XX XX XX XX|8|

Offset|Name|Values|Size|Type
---|---|---|---|---
0|Change Color|03|1
1|Tranche|01-12|1
2|Color|00-07|1

Offset|Name|Values|Size|Type
---|---|---|---|---
0|VU meters|04|1
1|Chan M-F|00-06|1
2|Meter values PRE|00-15|20
22|Meter values POST|00-15|20
42|Meter values MASTER| 00-15 |2

