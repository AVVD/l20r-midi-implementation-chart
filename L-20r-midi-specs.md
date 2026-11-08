L-20 MIDI implementation table
===
WIP

## MIDI CC
||Dec|Hex|Channel|Value|Name|Comment|
|-|-|-|-|-|-|-|
|To-validate|1|0x01|\*|x|COMP|?|
|To-validate|3|0x03|\*|x|USB1-2, USB3-4|?|
||4|0x04|\*|0,2|USB1-2, USB3-4|?|
|To-validate|8|0x08|\*|x|Channel selection buttons|?|
|To-validate|-|-|-|-|02 REC
|To-validate|-|-|-|-|01 PLAY
|To-validate|-|-|-|-|00 Disabled
||8|0x08|\*|x|REC/PLAY||
||9|0x09|1,3|x|REC/PLAY 17\_18,19\_20||
||10|0x0A|\*|x|PHASE
||-|-|-|-|01 Inverted
||-|-|-|-|00 Normal
||12|0x0C|\*|00-??|PAN
||12|0x0C|\*|00-??|PAN
||14|0x0E|\*|01|EQ ON/OFF
||14|0x0E|\*|01|EQ ON/OFF
||20|0x14|\*|00-??|EQ HIGH
||20|0x14|\*|00-??|EQ HIGH
||24|0x18|\*|00-??|EQ MID FREQ
||24|0x18|\*|00-??|EQ MID FREQ
||26|0x1A|\*|00-??|EQ MID
||26|0x1A|\*|00-??|EQ MID
||44|0x2C|\*|00-??|EQ LOW
||44|0x2C|\*|00-??|EQ LOW
||46|0x2E|\*|00-??|EQ LOCUT
||46|0x2E|\*|00-??|EQ LOCUT
||48|0x30|\*|x|MUTE
||-|-|-|-|01 muted
||-|-|-|-|00 unmuted
||49|0x31|1,3|x|MUTE
||50|0x32|\*|x|SOLO
||-|-|-|-|01 soloed
||-|-|-|-|00 unsolo
||51|0x33|1,3|x|SOLO
||52|0x34|\*|00-78|SEND FX1
||53|0x35|1,3|00-78|SEND FX1
||54|0x36|\*|00-78|SEND FX2|
||55|0x37|1,3|00-78|SEND FX2|
||60|0x3C|\*|00-78|FADER M
||-|-|-|52|0
||61|0x3D|1,3|00-78|FADER M 17\_18,19\_20
||62|0x3E|\*|00-78|FADER A
||64|0x40|\*|00-78|FADER B
||66|0x42|\*|00-78|FADER C
||68|0x44|\*|00-78|FADER D
||70|0x46|\*|00-78|FADER E
||72|0x48|\*|00-78|FADER F
||78|0x4E|1|00-09|EFX1 Type
||-|-|2|00-09|EFX2 Type
||-|-|5|00-64|EFX1 Tone MSB
||-|-|6|00-64|EFX1 Tone LSB
||-|-|7|00-??|EFX2 Tone MSB
||-|-|8|00-??|EFX2 Tone LSB
||-|-|13|00-??|EFX1 Decay MSB
||-|-|14|00-??|EFX1 Decay LSB
||-|-|15|00-??|EFX2 Decay MSB
||-|-|16|00-??|EFX2 Decay LSB
||80|0x50|?|
||-|-|5|-|FX1 MUTE
||-|-|9|-|FX1 SOLO
||-|-|c+1|-|FX1 FADER
||-|-|6|-|FX2 MUTE
||-|-|10|-|FX2 SOLO
||-|-|d+1|-|FX2 FADER
|To-validate|81|0x51|?|
|To-validate|82|0x52|?|
||83|0x53|1-6|00-78|VOLUME MONITOR A-F
||84|0x54|8|x|SOLO CLEAR|?
||-|-|-|-|03 cleared|?
||-|-|9|x|Master selection button
||-|-|-|-|02 REC
||-|-|-|-|01 PLAY|?
||-|-|-|-|00 Disabled|?
||-|-|10|x|MASTER MUTE
||-|-|-|-|01
||-|-|-|-|00
||-|-|11|00-78|MASTER FADER|-|-|
||85|0x55|1|00-60|GLOBAL EQ 25Hz
||-|-|2|00-60|GLOBAL EQ 40Hz
||-|-|3|00-60|GLOBAL EQ 63Hz
||-|-|4|00-60|GLOBAL EQ 100Hz
||-|-|5|00-60|GLOBAL EQ 160Hz
||-|-|6|00-60|GLOBAL EQ 250Hz
||-|-|7|00-60|GLOBAL EQ 400Hz
||-|-|8|00-60|GLOBAL EQ 630Hz
||-|-|9|00-60|GLOBAL EQ 1kHz
||-|-|10|00-60|GLOBAL EQ 1.6kHz
||-|-|11|00-60|GLOBAL EQ 2.5kHz
||-|-|12|00-60|GLOBAL EQ 4kHz
||-|-|13|00-60|GLOBAL EQ 6.3kHz
||-|-|14|00-60|GLOBAL EQ 10kHz
||-|-|15|00-60|GLOBAL EQ 16kHz
||-|-|16|01|GLOBAL EQ ON/OFF
|To-validate|86|0x56|\*|SCENE[...]|?|
||86|0x56|9|00-01|Scene on/off
|To-validate|87|0x57|\*|SCENE[...]|?|
||87|0x57|6|00-06|Fader Mode M-F
||-|-|9||LED PLAY PAUSE
||-|-|10|x|REC
||-|-|-|-|...
||-|-|11|x|PLAY PAUSE
||-|-|-|-|03
||-|-|12|x|STOP
||-|-|-|-|03
||-|-|13|x|REWIND
||-|-|-|-|03
||-|-|14|x|FAST FORWARD
||-|-|-|-|03
||-|-|15|x|OVERDUB
||-|-|-|-|03
||-|-|16|??-??|???
||88|0x59|\*|-|TIME|
||-|-|1|00-??|Marker
||-|-|5|00-99|Song hh..
||-|-|6|00-99|Sont ..hh
||-|-|7|00-59|Song mm
||-|-|8|00-59|Song ss
||-|-|9|00-99|Cur hh..
||-|-|10|00-99|Cur ..hh
||-|-|11|00-59|Cur mm
||-|-|12|00-59|Cur ss

## SysEx
WIP
||SysEx|M.ID Zoom|L-20r|Command|Data|End|Comment|
|-|-----|---------|-----|-------|----|---|-------|
||F0|52 00 00|31|XX|...|F7|Generic|
||F0|7E 00 06|01|||F7|Universal MIDI Ident ;To|
||F0|7E 00 06|02|52|72 00 03 00 31 2E 31 33|F7|52:Zoom 0x312E3133:1.13 ;From|
||F0|52 00 00|2B|XX||F7|Ask Channel Names ;To|
||F0|52 00 00|2A|08|05 00 00 ...|F7|Channel Names ;From|
||F0|52 00 00|07|00-02|...|F7|Ask Scene names ;To|
||F0|52 00 00|06|00-02|...|F7|Scene names ;From|
||F0|52 00 00|50|||F7|Monitor Volumes|
||F0|52 00 00|51|||F7|Stop Monitor Volumes|

WIP
||Command|Name|Comment|||
|-|-------|----|-------|-|-|
||02|Change Name
||-|01-12|Tranche
||-|-|09 00|?
||-|-|-|XX XX XX XX XX XX XX XX|ASCII Chars
||03|Change Color
||-|01-12|Tranche
||-|-|00-07|Color
||04|VU meters
||-|00-06|Chan Select M-F
||-|-|00..00| Meter values PRE
||-|-|00..00| Meter values POST
||-|-|00 00| Meter values MASTER

