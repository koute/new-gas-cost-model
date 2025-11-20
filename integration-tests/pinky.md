Gas simulation at offset 0 with total cost of 26:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r9 = u8 [r7 + 0xb]
    D=========================eER  jump 24 if r9 == 0
```

Gas simulation at offset 6 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeE---------------------------------------R............  r9 = r8 >> 0x3
    DeE---------------------------------------R............  r10 = 0x17290
    .DeE--------------------------------------R............  r9 = r9 + r10
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeE-------------R............  r9 = u8 [r9 + 0]
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0xc] = a2
    .DeeE-------------------------------------------------R  fallthrough
```

Gas simulation at offset 24 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r9 = i16 [r7 + 0x6]
    DeE---------------------------------------R.............  r8 = r8 & 0x7
    DeE---------------------------------------R.............  r10 = 0x1
    .DeE--------------------------------------R.............  r8 = r8 << 0x8
    .D========================eE--------------R.............  r9 = r9 & 0xfffffffffffff8ff
    .D=========================eE-------------R.............  r8 = r8 | r9
    ..D=========================eE------------R.............  r9 = r8 + r10
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------R.............  u8 [r7 + 0x2] = a3
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u16 [r7 + 0x6] = r8
    ...D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r7 + 0x8] = r9
    ...DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  u8 [r7 + 22] = 0
    ...DeeeeeeeeeeeeeeeeeeeeeeE----------------------------R  jump [r0 + 0]
```

Gas simulation at offset 61 with total cost of 26:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r8 = u8 [r7 + 0xe]
    D=========================eER  jump 85 if r8 == 0
```

Gas simulation at offset 67 with total cost of 50:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........  r8 = u8 [r7 + 0x12]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........  r9 = u8 [r7 + 0x14]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........  u8 [r7 + 14] = 0
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x13] = a2
    .D========================eE------------------------R  jump 100 if r8 == 0
```

Gas simulation at offset 83 with total cost of 22:

```
    DeeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 85 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r8 = u8 [r7 + 0x13]
    D=========================eE--------------R  jump 116 if r8 == 0
```

Gas simulation at offset 92 with total cost of 26:

```
    DeER.........................  r8 = r8 + 0xffffffffffffffff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x13] = a1
    DeeeeeeeeeeeeeeeeeeeeeeE----R  jump [r0 + 0]
```

Gas simulation at offset 100 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r8 = u8 [r7 + 0xd]
    D=========================eE--------------R  jump 83 if r8 == 0
```

Gas simulation at offset 107 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r9 = u8 [r7 + 0x15]
    D=========================eE--------------R  jump 136 if r9 != 0
```

Gas simulation at offset 114 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 83
```

Gas simulation at offset 116 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r8 = u8 [r7 + 0xd]
    D=========================eE--------------R  jump 83 if r8 == 0
```

Gas simulation at offset 123 with total cost of 50:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........  r8 = u8 [r7 + 0x14]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........  r9 = u8 [r7 + 0x15]
    D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x13] = a1
    .D========================eE------------------------R  jump 83 if r9 == 0
```

Gas simulation at offset 136 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r8 = u16 [r7 + 0x6]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r10 = u8 [r7 + 0xf]
    DeE---------------------------------------R  r9 = r9 & 0xf
    .D========================eE--------------R  r9 = r8 >> r9
    .D========================eE--------------R  jump 170 if r10 == 0
```

Gas simulation at offset 152 with total cost of 45:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.....  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.....  r10 = u8 [r7 + 0x10]
    D=========================eeeeeeeeeeeeeeeeeeeeER  jump 181 if r10 == 0
```

Gas simulation at offset 159 with total cost of 21:

```
    DeER....................  r9 = r8 - r9
    DeER....................  r10 = 0x8
    D=eeeeeeeeeeeeeeeeeeeeER  jump 193 if r8 >=u r10
```

Gas simulation at offset 168 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 83
```

Gas simulation at offset 170 with total cost of 21:

```
    DeER....................  r9 = r9 + r8
    DeER....................  r10 = 0x8
    D=eeeeeeeeeeeeeeeeeeeeER  jump 193 if r8 >=u r10
```

Gas simulation at offset 179 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 83
```

Gas simulation at offset 181 with total cost of 21:

```
    DeER....................  r9 = r9 ^ 0xffffffffffffffff
    D=eER...................  r9 = r9 + r8
    DeE-R...................  r10 = 0x8
    D=eeeeeeeeeeeeeeeeeeeeER  jump 83 if r8 <u r10
```

Gas simulation at offset 193 with total cost of 21:

```
    DeER....................  r8 = zext16 r9
    DeER....................  r10 = 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeER  jump 83 if r10 <u r8
```

Gas simulation at offset 202 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r7 + 0x6] = r9
    DeeeeeeeeeeeeeeeeeeeeeeE---R  jump [r0 + 0]
```

Gas simulation at offset 207 with total cost of 26:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r9 = u8 [r7 + 0x8]
    D=========================eER  jump 231 if r9 == 0
```

Gas simulation at offset 213 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeE---------------------------------------R............  r9 = r8 >> 0x3
    DeE---------------------------------------R............  r10 = 0x17290
    .DeE--------------------------------------R............  r9 = r9 + r10
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeE-------------R............  r9 = u8 [r9 + 0]
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x9] = a2
    .DeeE-------------------------------------------------R  fallthrough
```

Gas simulation at offset 231 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r9 = i16 [r7 + 0]
    DeE---------------------------------------R.............  r8 = r8 & 0x7
    DeE---------------------------------------R.............  r10 = 0x1
    .DeE--------------------------------------R.............  r8 = r8 << 0x8
    .D========================eE--------------R.............  r9 = r9 & 0xfffffffffffff8ff
    .D=========================eE-------------R.............  r8 = r8 | r9
    ..D=========================eE------------R.............  r9 = r8 + r10
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u16 [r7 + 0] = r8
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r7 + 0x2] = r9
    ...DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  u8 [r7 + 0xa] = a3
    ...DeeeeeeeeeeeeeeeeeeeeeeE----------------------------R  jump [r0 + 0]
```

Gas simulation at offset 263 with total cost of 54:

```
    DeER.....................................................  r2 = 0
    DeER.....................................................  r7 = r7 + 0x7ff
    DeER.....................................................  r9 = r8 & 0x1
    .DeER....................................................  r11 = r8 >> 0x1
    .DeER....................................................  r10 = r8 >> 0x2
    ..DeER...................................................  r12 = r8 >> 0x3
    ..DeER...................................................  r8 = r8 << 0x3b
    ..DeER...................................................  r11 = r11 & 0x1
    ...DeER..................................................  r10 = r10 & 0x1
    ...DeER..................................................  r12 = r12 & 0x1
    ...DeER..................................................  r8 = r8 >> 0x3f
    ...DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u8 [r7 + 0xc] = a2
    ....DeeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u8 [r7 + 0x24] = a4
    ....DeeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u8 [r7 + 0x3e] = a5
    ....DeeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u8 [r7 + 0x79] = a3
    ....D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u8 [r7 + 0x8b] = a1
    .....D========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 143] = 0
    .....D========================eE------------------------R  jump 355 if r8 == 0
```

Gas simulation at offset 319 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r8 = u16 [r7 + 0x85]
    D=========================eE--------------R  jump 341 if r8 == 0
```

Gas simulation at offset 327 with total cost of 20:

```
    DeeeeeeeeeeeeeeeeeeeeER  jump 362 if r9 == 0
```

Gas simulation at offset 330 with total cost of 20:

```
    DeeeeeeeeeeeeeeeeeeeeER  jump 368 if r11 == 0
```

Gas simulation at offset 333 with total cost of 20:

```
    DeeeeeeeeeeeeeeeeeeeeER  jump 374 if r10 == 0
```

Gas simulation at offset 336 with total cost of 20:

```
    DeeeeeeeeeeeeeeeeeeeeER  jump 380 if r12 == 0
```

Gas simulation at offset 339 with total cost of 22:

```
    DeeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 341 with total cost of 50:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........  r8 = i16 [r7 + 0x81]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........  r2 = u16 [r7 + 0x83]
    D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r7 + 0x87] = r8
    .DeeE-----------------------------------------------R  fallthrough
```

Gas simulation at offset 355 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r7 + 0x85] = r2
    DeeeeeeeeeeeeeeeeeeeeE-----R  jump 330 if r9 != 0
```

Gas simulation at offset 362 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 13] = 0
    DeeeeeeeeeeeeeeeeeeeeE-----R  jump 333 if r11 != 0
```

Gas simulation at offset 368 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 37] = 0
    DeeeeeeeeeeeeeeeeeeeeE-----R  jump 336 if r10 != 0
```

Gas simulation at offset 374 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 122] = 0
    DeeeeeeeeeeeeeeeeeeeeE-----R  jump 339 if r12 != 0
```

Gas simulation at offset 380 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 63] = 0
    DeeeeeeeeeeeeeeeeeeeeeeE---R  jump [r0 + 0]
```

Gas simulation at offset 385 with total cost of 52:

```
    DeER...................................................  r1 = r1 + 0xffffffffffffffe8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u64 [r1 + 0x10] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u64 [r1 + 0x8] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u64 [r1 + 0] = r6
    .DeE------------------------R..........................  r9 = r8 >> 0xd
    .D=eE-----------------------R..........................  r9 = r9 << 0x2
    .DeE------------------------R..........................  r10 = 0x10000
    ..D=eE----------------------R..........................  r9 = r9 + r10
    ..D==eeeeeeeeeeeeeeeeeeeeeeeeeER.......................  r9 = i32 [r9 + 0]
    ..D===========================eER......................  r9 = r9 + r10
    ...D=======================eE---R......................  r6 = r7 + 0x7ff
    ...D===========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r9 + 0]
```

Gas simulation at offset 421 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................  r9 = u64 [r6 + 0x241]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................  r7 = u64 [r6 + 0x249]
    DeE------------------------R...........................  r10 = 0x17c80
    .D========================eeER.........................  r10 = r7 if r9 != 0
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  r12 = u64 [r10 + 0x18]
    .DeeE-------------------------------------------------R  fallthrough
```

Gas simulation at offset 441 with total cost of 26:

```
    DeER.........................  r7 = r6 + 0x27f
    DeeER........................  r7 = r9 if r9 != 0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER  r0 = u64 [r1 + 0x10]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER  r5 = u64 [r1 + 0x8]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0]
    .D=eE-----------------------R  r1 = r1 + 0x18
    ..DeeeeeeeeeeeeeeeeeeeeeeE--R  jump [r12 + 0]
```

Gas simulation at offset 461 with total cost of 2:

```
    DeER.  r9 = r8 >> 0x5
    DeER.  r10 = 0x201
    D=eER  jump 638 if r9 >=u r10
```

Gas simulation at offset 472 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeE---------------------------------------R...........  r8 = r8 & 0x1f
    D=eE--------------------------------------R...........  r8 = r8 << 0x2
    DeE---------------------------------------R...........  r9 = 0x10020
    .D=eE-------------------------------------R...........  r8 = r8 + r9
    .D==eeeeeeeeeeeeeeeeeeeeeeeeeE------------R...........  r8 = i32 [r8 + 0]
    .D===========================eE-----------R...........  r9 = r9 + r8
    .DeE--------------------------------------R...........  r8 = 0
    ..D===========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r9 + 0]
```

Gas simulation at offset 496 with total cost of 47:

```
    D.................................................  r7 = r8
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r0 = u64 [r1 + 0x10]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r5 = u64 [r1 + 0x8]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r6 = u64 [r1 + 0]
    .DeE-----------------------R......................  r1 = r1 + 0x18
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 511 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................  r9 = u64 [r6 + 0x241]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................  r7 = u64 [r6 + 0x249]
    DeE------------------------R...........................  r10 = 0x17c80
    .D========================eeER.........................  r10 = r7 if r9 != 0
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  r12 = u64 [r10 + 0x28]
    .DeeeeeeeeeeeeeeeE------------------------------------R  jump 441
```

Gas simulation at offset 532 with total cost of 47:

```
    DeER..............................................  r8 = r8 & 0x7ff
    D=eER.............................................  r7 = r7 + r8
    D==eeeeeeeeeeeeeeeeeeeeeeeeeER....................  r7 = u8 [r7 + 0]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE--R....................  r0 = u64 [r1 + 0x10]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-R....................  r5 = u64 [r1 + 0x8]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-R....................  r6 = u64 [r1 + 0]
    .D========================eE-R....................  r1 = r1 + 0x18
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 554 with total cost of 2:

```
    DeER.  r8 = r8 & 0x7
    D=eER  jump 690 if r8 == 2
```

Gas simulation at offset 562 with total cost of 2:

```
    DeER.  r9 = 0x4
    D=eER  jump 661 if r8 == r9
```

Gas simulation at offset 568 with total cost of 2:

```
    DeER.  r9 = 0x7
    D=eER  jump 742 if r8 != r9
```

Gas simulation at offset 575 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r8 = u16 [r6 + 0x209]
    D=========================eE--------------R  r5 = r8 << 0x32
    .D=========================eE-------------R  r9 = r5 >> 0x3a
    .DeE--------------------------------------R  r10 = 0x3f
    .D=========================eE-------------R  r5 = r5 >> 0x32
    ..D=========================eE------------R  jump 758 if r9 >=u r10
```

Gas simulation at offset 596 with total cost of 74:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r8 = u64 [r6 + 0x241]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r7 = u64 [r6 + 0x249]
    DeE---------------------------------------R..................................  r9 = 0x17c80
    .D========================eeE-------------R..................................  r9 = r7 if r8 != 0
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r9 = u64 [r9 + 0x48]
    ..DeE-------------------------------------------------R......................  r7 = r6 + 0x27f
    ..D=======================eeE-------------------------R......................  r7 = r8 if r8 != 0
    ...D.........................................................................  r8 = r5
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 14, jump [r9 + 0]
```

Gas simulation at offset 629 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = u16 [r6 + 0x209]
    D...........................  r12 = r7
    DeeeeeeeeeeeeeeeE----------R  jump 773
```

Gas simulation at offset 638 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  r9 = u64 [r6 + 0x241]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  r7 = u64 [r6 + 0x249]
    DeE---------------------------------------R............  r10 = 0x17c80
    .D========================eeE-------------R............  r10 = r7 if r9 != 0
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  r12 = u64 [r10 + 0x38]
    .DeeeeeeeeeeeeeeeE------------------------------------R  jump 441
```

Gas simulation at offset 661 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  r8 = u8 [r6 + 0x224]
    D=========================eE--------------R............  r7 = r7 + r8
    D==========================eE-------------R............  r7 = r7 + 0x7ff
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u8 [r7 + 0xa1]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R  r0 = u64 [r1 + 0x10]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R  r5 = u64 [r1 + 0x8]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R  r6 = u64 [r1 + 0]
    ..D========================eE-------------------------R  r1 = r1 + 0x18
    ..D========================eeeeeeeeeeeeeeeeeeeeeeE----R  jump [r0 + 0]
```

Gas simulation at offset 690 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r7 = u8 [r6 + 0x228]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r8 = u8 [r6 + 0x229]
    .D========================eE--------------R.............  r9 = r7 & 0xe0
    .D========================eE--------------R.............  r8 = r8 & 0x1f
    .D=========================eE-------------R.............  r8 = r8 | r9
    ..DeE-------------------------------------R.............  r9 = 0x1
    ..D========================eE-------------R.............  r7 = r7 & 0x7f
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u8 [r6 + 0x228] = a0
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u8 [r6 + 0x229] = a1
    ...DeeeeeeeeeeeeeeeeeeeeeeeeeE------------------------R.  u16 [r6 + 0x239] = r9
    ...D....................................................  r7 = r8
    ...DeeeeeeeeeeeeeeeeeeeeeeeeeE------------------------R.  r0 = u64 [r1 + 0x10]
    ...D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  r5 = u64 [r1 + 0x8]
    ....D========================eeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0]
    ....D================================================eER  r1 = r1 + 0x18
    ....D========================eeeeeeeeeeeeeeeeeeeeeeE---R  jump [r0 + 0]
```

Gas simulation at offset 742 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.......  unlikely
    DeE---------------------------------------R.......  r7 = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r0 = u64 [r1 + 0x10]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r5 = u64 [r1 + 0x8]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......  r6 = u64 [r1 + 0]
    .DeE--------------------------------------R.......  r1 = r1 + 0x18
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 758 with total cost of 28:

```
    DeER...........................  r9 = r8 & 0x1f
    D=eER..........................  r7 = r7 + r9
    D==eER.........................  r7 = r7 + 0x7ff
    .D==eeeeeeeeeeeeeeeeeeeeeeeeeER  r12 = u8 [r7 + 0x1a1]
    .DeeE-------------------------R  fallthrough
```

Gas simulation at offset 773 with total cost of 56:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...............................  r7 = u8 [r6 + 0x226]
    DeE------------------------R...............................  r9 = r5 >> 0x8
    DeE------------------------R...............................  r10 = 0x20
    .DeE-----------------------R...............................  r11 = 0x1
    .D========================eER..............................  r7 = r7 & 0x4
    .D=========================eeER............................  r11 = r10 if r7 != 0
    ..D==========================eER...........................  r8 = r8 + r11
    ..D===========================eER..........................  r8 = r8 << 0x31
    ..D============================eER.........................  r8 = r8 >> 0x31
    ..D=============================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r6 + 0x209] = r8
    ...DeE----------------------------------------------------R  jump 835 if r9 >=u 63
```

Gas simulation at offset 809 with total cost of 50:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........  r7 = u8 [r6 + 0x225]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........  u8 [r6 + 0x225] = a5
    D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x229] = a0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE------------------------R  r0 = u64 [r1 + 0x10]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE------------------------R  r5 = u64 [r1 + 0x8]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0]
    .D=========================eE-----------------------R  r1 = r1 + 0x18
    ..D========================eeeeeeeeeeeeeeeeeeeeeeE--R  jump [r0 + 0]
```

Gas simulation at offset 835 with total cost of 74:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r8 = u64 [r6 + 0x241]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r7 = u64 [r6 + 0x249]
    DeE---------------------------------------R..................................  r9 = 0x17c80
    .D========================eeE-------------R..................................  r9 = r7 if r8 != 0
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r9 = u64 [r9 + 0x48]
    ..DeE-------------------------------------------------R......................  r7 = r6 + 0x27f
    ..D=======================eeE-------------------------R......................  r7 = r8 if r8 != 0
    ...D.........................................................................  r8 = r5
    ...D.........................................................................  r5 = r12
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 16, jump [r9 + 0]
```

Gas simulation at offset 870 with total cost of 54:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.............................  r9 = u8 [r6 + 0x227]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.............................  r10 = u8 [r6 + 0x229]
    DeE------------------------R.............................  r8 = r5 & 0x30
    .D========================eER............................  r9 = r9 & 0x1
    .D=========================eeER..........................  r8 = r5 if r9 == 0
    ..D=======================eE--R..........................  r9 = r10 & 0xc0
    ..D==========================eER.........................  r9 = r9 | r8
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE--R.........................  u8 [r6 + 0x225] = a0
    ...D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x229] = a2
    ...D.....................................................  r7 = r8
    ...DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R  r0 = u64 [r1 + 0x10]
    ...D=======================eeeeeeeeeeeeeeeeeeeeeeeeeE---R  r5 = u64 [r1 + 0x8]
    ....D=======================eeeeeeeeeeeeeeeeeeeeeeeeeE--R  r6 = u64 [r1 + 0]
    ....D========================eE-------------------------R  r1 = r1 + 0x18
    ....D========================eeeeeeeeeeeeeeeeeeeeeeE----R  jump [r0 + 0]
```

Gas simulation at offset 917 with total cost of 25:

```
    DeER........................  r8 = 0x1
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r0 = u64 [r1 + 0x10]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r5 = u64 [r1 + 0x8]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0]
    .DeE-----------------------R  r1 = r1 + 0x18
    .DeeeeeeeeeeeeeeeE---------R  jump 5420
```

Gas simulation at offset 934 with total cost of 25:

```
    DeER........................  r8 = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r0 = u64 [r1 + 0x10]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r5 = u64 [r1 + 0x8]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0]
    .DeE-----------------------R  r1 = r1 + 0x18
    .DeeeeeeeeeeeeeeeE---------R  jump 5420
```

Gas simulation at offset 950 with total cost of 100:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r0 = u64 [r1 + 0x10]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r5 = u64 [r1 + 0x8]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r6 = u64 [r1 + 0]
    DeE------------------------R...........................................................................  r1 = r1 + 0x18
    .DeE-----------------------R...........................................................................  r8 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER.........................................................................  r7 = u8 [r8 + 0xd]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  r9 = u8 [r8 + 0x25]
    ..D=======================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  r10 = u8 [r8 + 0x3f]
    ..D=======================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  r11 = u8 [r8 + 0x7a]
    ...D========================eeeE--------------------R..................................................  r7 = r7 >u 0
    ....D==============================================eeeER...............................................  r9 = r9 >u 0
    ....D=================================================eER..............................................  r9 = r9 << 0x1
    .....D=================================================eER.............................................  r2 = r9 | r7
    .....D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER.............................................  r9 = u16 [r8 + 0x85]
    .....D=============================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r12 = u8 [r8 + 0x8f]
    ......D============================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r7 = u8 [r8 + 0x99]
    ......D=================================================eeeE-----------------R.........................  r11 = r11 >u 0
    .......D================================================eeeE-----------------R.........................  r10 = r10 >u 0
    .......D===================================================eE----------------R.........................  r11 = r11 << 0x2
    ........D==================================================eE----------------R.........................  r10 = r10 << 0x3
    ........D===================================================eE---------------R.........................  r10 = r10 | r11
    .........D==================================================eeeE-------------R.........................  r9 = r9 >u 0
    .........D==================================================================eER........................  r7 = r7 << 0x6
    ..........D====================================================eE-------------R........................  r9 = r9 << 0x4
    ..........D==================================================================eER.......................  r7 = r7 | r9
    ..........D==================================================eE----------------R.......................  r9 = r2 | r10
    ...........D================================================================eE-R.......................  r10 = r12 << 0x7
    ...........D==================================================================eER......................  r7 = r7 | r10
    ...........D===================================================================eER.....................  r7 = r7 | r9
    ............D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER..............  u8 [r8 + 153] = 0
    ............D===============================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r8 + 0x270] = a5
    ............D=============eeeeeeeeeeeeeeeeeeeeeeE-----------------------------------------------------R  jump [r0 + 0]
```

Gas simulation at offset 1045 with total cost of 78:

```
    DeER.............................................................................  r1 = r1 + 0xffffffffffffff88
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER....................................................  u64 [r1 + 0x70] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER....................................................  u64 [r1 + 0x68] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER....................................................  u64 [r1 + 0x60] = r6
    .D...............................................................................  r6 = r7
    .DeE------------------------R....................................................  r5 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER...................................................  u64 [r1 + 0x48] = r5
    ..D========================eER...................................................  r5 = r5 + 0x1
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r7 = i32 [r5 + 0x250]
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r8 = u16 [r5 + 0x72]
    ...D=================================================eER.........................  r9 = r7 + 0x1
    ...D==================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r5 + 0x250] = r9
    ...D=================================================eE-------------------------R  jump 1101 if r8 == 0
```

Gas simulation at offset 1086 with total cost of 26:

```
    DeER.........................  r8 = r8 + 0xffffffffffffffff
    DeER.........................  r7 = r7 & 0x1
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x72] = r8
    D=eE------------------------R  jump 1152 if r7 == 0
```

Gas simulation at offset 1098 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 1402
```

Gas simulation at offset 1101 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r8 = u8 [r5 + 0x74]
    D=========================eE--------------R  jump 1135 if r8 == 0
```

Gas simulation at offset 1108 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r8 = u8 [r5 + 0x79]
    D=========================eE--------------R  jump 1135 if r8 == 0
```

Gas simulation at offset 1115 with total cost of 57:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.................  r8 = u8 [r5 + 0x76]
    D=========================eE--------------R.................  r8 = r8 + 0x1
    .D=========================eE-------------R.................  r9 = r8 & 0xff
    ..D=========================eeeE----------R.................  r9 = r9 <u 0x20
    ...D===========================eeE--------R.................  r8 = 0 if r9 == 0
    ...D=============================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x76] = a1
    ....DeeE---------------------------------------------------R  fallthrough
```

Gas simulation at offset 1135 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r8 = i16 [r5 + 0x70]
    D=========================eE--------------R...........  r8 = r8 + 0x1
    DeE---------------------------------------R...........  r7 = r7 & 0x1
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x72] = r8
    .DeE-------------------------------------------------R  jump 1402 if r7 != 0
```

Gas simulation at offset 1152 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u16 [r5 + 0x8]
    D=========================eE--------------R  jump 1221 if r7 == 0
```

Gas simulation at offset 1159 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeE---------------------------------------R  r7 = r7 + 0xffffffffffffffff
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r8 = u16 [r5 + 0x20]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeE--------------R  u16 [r5 + 0x8] = r7
    .D========================eE--------------R  jump 1252 if r8 == 0
```

Gas simulation at offset 1172 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeE---------------------------------------R  r7 = r8 + 0xffffffffffffffff
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r8 = u16 [r5 + 0x38]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R  u16 [r5 + 0x20] = r7
    .D========================eE--------------R  jump 1283 if r8 == 0
```

Gas simulation at offset 1185 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeE---------------------------------------R  r7 = r8 + 0xffffffffffffffff
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r8 = u16 [r5 + 0x88]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R  u16 [r5 + 0x38] = r7
    .D========================eE--------------R  jump 1334 if r8 == 0
```

Gas simulation at offset 1200 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u8 [r5 + 0x7c]
    DeE---------------------------------------R  r8 = r8 + 0xffffffffffffffff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeE--------------R  u16 [r5 + 0x88] = r8
    .D========================eE--------------R  r7 = r7 & 0x1
    .D=========================eE-------------R  jump 1379 if r7 == 0
```

Gas simulation at offset 1218 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 1402
```

Gas simulation at offset 1221 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r7 = u8 [r5 + 0x16]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r8 = i16 [r5 + 0x6]
    DeE---------------------------------------R.............  r9 = 0x7
    .D========================eE--------------R.............  r10 = r7 + 0xffffffffffffffff
    .D=========================eeE------------R.............  r9 = r10 if r7 != 0
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x16] = a2
    ..D=======================eE---------------------------R  r7 = r8 + 0x1
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R  r8 = u16 [r5 + 0x20]
    ...D=======================eeeeeeeeeeeeeeeeeeeeeeeeeE--R  u16 [r5 + 0x8] = r7
    ...D========================eE-------------------------R  jump 1172 if r8 != 0
```

Gas simulation at offset 1252 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r7 = u8 [r5 + 0x2e]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r8 = i16 [r5 + 0x1e]
    DeE---------------------------------------R.............  r9 = 0x7
    .D========================eE--------------R.............  r10 = r7 + 0xffffffffffffffff
    .D=========================eeE------------R.............  r9 = r10 if r7 != 0
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x2e] = a2
    ..D=======================eE---------------------------R  r7 = r8 + 0x1
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R  r8 = u16 [r5 + 0x38]
    ...D=======================eeeeeeeeeeeeeeeeeeeeeeeeeE--R  u16 [r5 + 0x20] = r7
    ...D========================eE-------------------------R  jump 1185 if r8 != 0
```

Gas simulation at offset 1283 with total cost of 57:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.................  r7 = u16 [r5 + 0x3a]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.................  r8 = u8 [r5 + 0x3f]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.................  r9 = i16 [r5 + 0x36]
    .DeE--------------------------------------R.................  r11 = 0x6
    .D========================eeE-------------R.................  r11 = 0x1 if r8 == 0
    ..D=======================eE--------------R.................  r8 = r7 >> 0x1
    ...D========================eE------------R.................  r10 = r7 >> r11
    ...D=========================eE-----------R.................  r7 = r7 ^ r10
    ....D=========================eE----------R.................  r7 = r7 << 0x3f
    ....D==========================eE---------R.................  r7 = r7 >> 0x31
    ....D===========================eE--------R.................  r7 = r7 | r8
    ....D============================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x3a] = r7
    .....D====================eE-------------------------------R  r7 = r9 + 0x1
    .....DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------------------R  r8 = u16 [r5 + 0x88]
    .....D=====================eeeeeeeeeeeeeeeeeeeeeeeeeE------R  u16 [r5 + 0x38] = r7
    ......D========================eE--------------------------R  jump 1200 if r8 != 0
```

Gas simulation at offset 1334 with total cost of 50:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........  r7 = i16 [r5 + 0x7e]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........  r8 = u8 [r5 + 0x8d]
    D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x88] = r7
    .D========================eE------------------------R  jump 1550 if r8 == 0
```

Gas simulation at offset 1350 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r8 = u8 [r5 + 0x90]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r7 = u8 [r5 + 0x7c]
    D=========================eE--------------R...........  r8 = r8 + 0xffffffffffffffff
    .D=========================eE-------------R...........  r9 = r8 & 0xff
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x90] = a1
    .D==========================eeeeeeeeeeeeeeeeeeeeE----R  jump 1621 if r9 == 0
```

Gas simulation at offset 1373 with total cost of 2:

```
    DeER.  r7 = r7 & 0x1
    D=eER  jump 1402 if r7 != 0
```

Gas simulation at offset 1379 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u16 [r5 + 0x84]
    D=========================eE--------------R  jump 1402 if r7 == 0
```

Gas simulation at offset 1387 with total cost of 50:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........  r7 = i16 [r5 + 0x86]
    D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x272] = r7
    DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  u8 [r5 + 630] = 0x1
    .DeeE-----------------------------------------------R  fallthrough
```

Gas simulation at offset 1402 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u64 [r5 + 0x68]
    DeE------------------------R  r8 = 0x3ff0000000000000
    DeeeeeeeeeeeeeeeE----------R  r0 = 24, jump 33311
```

Gas simulation at offset 1420 with total cost of 26:

```
    DeER.........................  r8 = r7 << 0x1
    D=eER........................  r8 = r8 >> 0x1
    .DeER........................  r9 = 0x7ff0000000000000
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r5 + 0x68] = r7
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x40] = r6
    ..DeeeeeeeeeeeeeeeeeeeeE----R  jump 1459 if r9 <u r8
```

Gas simulation at offset 1445 with total cost of 2:

```
    DeER.  r8 = 0x40144ace15b7e8e7
    D=eER  jump 3028 if r7 <s r8
```

Gas simulation at offset 1459 with total cost of 15:

```
    DeER..............  r8 = 0xc0144ace15b7e8e7
    DeeeeeeeeeeeeeeeER  r0 = 26, jump 33311
```

Gas simulation at offset 1474 with total cost of 26:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r8 = u8 [r5 + 0xb]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  u64 [r5 + 0x68] = r7
    D=========================eER  jump 1674 if r8 == 0
```

Gas simulation at offset 1484 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r8 = u16 [r5 + 0x6]
    DeE---------------------------------------R  r7 = 0
    D=========================eE--------------R  jump 1677 if r8 <u 8
```

Gas simulation at offset 1495 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r9 = u8 [r5 + 0xc]
    D=========================eE--------------R  jump 1677 if r9 == 0
```

Gas simulation at offset 1503 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u8 [r5 + 0xd]
    D=========================eE--------------R  jump 1777 if r7 == 0
```

Gas simulation at offset 1511 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u8 [r5 + 0x15]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r9 = u8 [r5 + 0xf]
    D=========================eE--------------R  r7 = r7 & 0xf
    .D=========================eE-------------R  r7 = r8 >> r7
    .D========================eE--------------R  jump 1664 if r9 == 0
```

Gas simulation at offset 1528 with total cost of 45:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.....  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.....  r9 = u8 [r5 + 0x10]
    D=========================eeeeeeeeeeeeeeeeeeeeER  jump 1764 if r9 == 0
```

Gas simulation at offset 1536 with total cost of 22:

```
    DeER.....................  r7 = r8 - r7
    D=eER....................  r7 = zext16 r7
    D==eeeeeeeeeeeeeeeeeeeeER  jump 1674 if r7 >u 2046
```

Gas simulation at offset 1547 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 1777
```

Gas simulation at offset 1550 with total cost of 46:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER......  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R......  r7 = u8 [r5 + 0x8f]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R......  r8 = u8 [r5 + 0x91]
    .D========================eE--------------R......  r9 = r7 & 0x1
    .D=========================eeeeeeeeeeeeeeeeeeeeER  jump 1579 if r9 != 0
```

Gas simulation at offset 1565 with total cost of 1:

```
    DeER  jump 1591 if r8 <u 2
```

Gas simulation at offset 1569 with total cost of 26:

```
    DeER.........................  r8 = r8 + 0xfe
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x91] = a1
    DeeeeeeeeeeeeeeeE-----------R  jump 1591
```

Gas simulation at offset 1579 with total cost of 1:

```
    DeER  jump 1591 if r8 >=u 126
```

Gas simulation at offset 1583 with total cost of 26:

```
    DeER.........................  r8 = r8 + 0x2
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x91] = a1
    DeeE------------------------R  fallthrough
```

Gas simulation at offset 1591 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeE---------------------------------------R...........  r7 = r7 >> 0x1
    D=eeeeeeeeeeeeeeeeeeeeeeeeeE--------------R...........  u8 [r5 + 0x8f] = a0
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r8 = u8 [r5 + 0x90]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R...........  r7 = u8 [r5 + 0x7c]
    .D========================eE--------------R...........  r8 = r8 + 0xffffffffffffffff
    .D=========================eE-------------R...........  r9 = r8 & 0xff
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x90] = a1
    ..D=========================eeeeeeeeeeeeeeeeeeeeE----R  jump 1373 if r9 != 0
```

Gas simulation at offset 1621 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = u8 [r5 + 0x7d]
    DeE------------------------R  r7 = r7 & 0x1
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 124] = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 144] = 0x8
    .DeeeeeeeeeeeeeeeeeeeeE----R  jump 1649 if r7 == 0
```

Gas simulation at offset 1638 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 141] = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x8f] = a1
    DeeeeeeeeeeeeeeeE----------R  jump 1379
```

Gas simulation at offset 1649 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 141] = 0x1
    DeE------------------------R  r7 = r7 & 0x1
    D=eE-----------------------R  jump 1379 if r7 == 0
```

Gas simulation at offset 1661 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 1402
```

Gas simulation at offset 1664 with total cost of 3:

```
    DeER..  r7 = r7 + r8
    D=eER.  r7 = zext16 r7
    D==eER  jump 1777 if r7 <=u 2046
```

Gas simulation at offset 1674 with total cost of 2:

```
    DeER.  r7 = 0
    DeeER  fallthrough
```

Gas simulation at offset 1677 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r8 = u8 [r5 + 0x23]
    D=========================eE--------------R  jump 1889 if r8 == 0
```

Gas simulation at offset 1685 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r9 = u16 [r5 + 0x1e]
    DeE---------------------------------------R  r8 = 0
    D=========================eE--------------R  jump 1889 if r9 <u 8
```

Gas simulation at offset 1696 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r10 = u8 [r5 + 0x24]
    D=========================eE--------------R  jump 1889 if r10 == 0
```

Gas simulation at offset 1704 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r8 = u8 [r5 + 0x25]
    D=========================eE--------------R  jump 1928 if r8 == 0
```

Gas simulation at offset 1712 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r8 = u8 [r5 + 0x2d]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r10 = u8 [r5 + 0x27]
    D=========================eE--------------R  r8 = r8 & 0xf
    .D=========================eE-------------R  r8 = r9 >> r8
    .D========================eE--------------R  jump 1749 if r10 == 0
```

Gas simulation at offset 1728 with total cost of 45:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.....  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.....  r10 = u8 [r5 + 0x28]
    D=========================eeeeeeeeeeeeeeeeeeeeER  jump 1914 if r10 == 0
```

Gas simulation at offset 1736 with total cost of 22:

```
    DeER.....................  r8 = r9 - r8
    D=eER....................  r8 = zext16 r8
    D==eeeeeeeeeeeeeeeeeeeeER  jump 1760 if r8 >u 2046
```

Gas simulation at offset 1746 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 1928
```

Gas simulation at offset 1749 with total cost of 22:

```
    DeER.....................  r8 = r8 + r9
    D=eER....................  r8 = zext16 r8
    D==eeeeeeeeeeeeeeeeeeeeER  jump 1928 if r8 <=u 2046
```

Gas simulation at offset 1760 with total cost of 15:

```
    DeER..............  r8 = 0
    DeeeeeeeeeeeeeeeER  jump 1889
```

Gas simulation at offset 1764 with total cost of 4:

```
    DeER...  r7 = r7 ^ 0xffffffffffffffff
    D=eER..  r7 = r7 + r8
    D==eER.  r7 = zext16 r7
    D===eER  jump 1674 if r7 >u 2046
```

Gas simulation at offset 1777 with total cost of 109:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.....................................................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.....................................................................  r3 = u8 [r5 + 0]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.....................................................................  r8 = u8 [r5 + 0x11]
    DeE---------------------------------------R.....................................................................  r9 = 0x172d0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.....................................................................  r10 = u8 [r5 + 0x16]
    .DeE--------------------------------------R.....................................................................  r2 = r1 + 0x58
    .D========================eE--------------R.....................................................................  r8 = r8 << 0x3
    ..D========================eE-------------R.....................................................................  r8 = r8 + r9
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................................................  r9 = u8 [r8 + 0]
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................................................  r12 = u8 [r8 + 0x1]
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................................................  r6 = u8 [r8 + 0x2]
    ...D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................................................  r11 = u8 [r8 + 0x3]
    ...D=======================eE-------------------------R.........................................................  r10 = r10 + r2
    ...D=================================================eER........................................................  r12 = r12 << 0x8
    ...D=================================================eER........................................................  r6 = r6 << 0x10
    ....D================================================eER........................................................  r11 = r11 << 0x18
    ....D=================================================eER.......................................................  r9 = r9 | r12
    ....D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER................................  r12 = u8 [r8 + 0x4]
    ....D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER...............................  r7 = u8 [r8 + 0x5]
    .....D================================================eE------------------------R...............................  r11 = r11 | r6
    .....D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER..............................  r6 = u8 [r8 + 0x6]
    .....D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER..............................  r8 = u8 [r8 + 0x7]
    .....D=========================================================================eER..............................  r7 = r7 << 0x8
    ......D=========================================================================eER.............................  r7 = r7 | r12
    ......D=========================================================================eER.............................  r6 = r6 << 0x10
    ......D=========================================================================eER.............................  r8 = r8 << 0x18
    ......D==========================================================================eER............................  r8 = r8 | r6
    .......D======================================================================eE---R............................  r9 = r9 | r11
    .......D==========================================================================eER...........................  r7 = r7 | r8
    .......D==================eE--------------------------------------------------------R...........................  r8 = r5 - r3
    ........D==========================================================================eER..........................  r7 = r7 << 0x20
    ........D===========================================================================eER.........................  r7 = r7 | r9
    ...........................................D=========================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x58] = r7
    ...........................................D===================================eeeeeeeeeeeeeeeeeeeeeeeeeE------R  r7 = u8 [r10 + 0]
    ...........................................D=====================================eeeeeeeeeeeeeeeeeeeeeeeeeE----R  r8 = u8 [r8 + 0x4]
    ...........................................D==============================================================eeeE-R  r7 = r8 * r7
    ............................................D====================================eeeeeeeeeeeeeeeeeeeeeeeeeE----R  r8 = u8 [r5 + 0x23]
    ............................................D=============================================================eE---R  jump 1685 if r8 != 0
```

Gas simulation at offset 1889 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r9 = u16 [r5 + 0x70]
    D=========================eE--------------R  jump 2044 if r9 >=u 2
```

Gas simulation at offset 1898 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeE---------------------------------------R  r11 = 0x7
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r9 = u8 [r5 + 0x3d]
    DeE---------------------------------------R  r6 = 0
    .D========================eE--------------R  jump 2077 if r9 != 0
```

Gas simulation at offset 1911 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 2113
```

Gas simulation at offset 1914 with total cost of 23:

```
    DeER......................  r8 = r8 ^ 0xffffffffffffffff
    D=eER.....................  r8 = r8 + r9
    D==eER....................  r8 = zext16 r8
    D===eeeeeeeeeeeeeeeeeeeeER  jump 1760 if r8 >u 2046
```

Gas simulation at offset 1928 with total cost of 109:

```
    DeER............................................................................................................  r2 = r5 + 0x18
    DeeeeeeeeeeeeeeeeeeeeeeeeeER....................................................................................  r10 = u8 [r5 + 0x18]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER....................................................................................  r9 = u8 [r5 + 0x29]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER...................................................................................  r11 = u8 [r5 + 0x2e]
    .DeE------------------------R...................................................................................  r12 = 0x172d0
    .DeE------------------------R...................................................................................  r6 = r1 + 0x58
    ..D=======================eER...................................................................................  r9 = r9 << 0x3
    ..D========================eER..................................................................................  r3 = r6 + r11
    ..D========================eER..................................................................................  r9 = r9 + r12
    ...D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................................................  r12 = u8 [r9 + 0]
    ...D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................................................  r6 = u8 [r9 + 0x1]
    ...D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................................................  r8 = u8 [r9 + 0x2]
    ...D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................................................  r11 = u8 [r9 + 0x3]
    ....D=====================eE--------------------------R.........................................................  r2 = r2 - r10
    ....D================================================eER........................................................  r6 = r6 << 0x8
    ....D================================================eER........................................................  r8 = r8 << 0x10
    ....D================================================eER........................................................  r11 = r11 << 0x18
    .....D================================================eER.......................................................  r12 = r12 | r6
    .....D===============================================eeeeeeeeeeeeeeeeeeeeeeeeeER................................  r6 = u8 [r9 + 0x4]
    .....D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER...............................  r10 = u8 [r9 + 0x5]
    .....D================================================eE------------------------R...............................  r8 = r8 | r11
    ......D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER..............................  r11 = u8 [r9 + 0x6]
    ......D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER..............................  r9 = u8 [r9 + 0x7]
    ......D========================================================================eER..............................  r10 = r10 << 0x8
    ......D=========================================================================eER.............................  r10 = r10 | r6
    .......D========================================================================eER.............................  r11 = r11 << 0x10
    .......D========================================================================eER.............................  r9 = r9 << 0x18
    .......D=========================================================================eER............................  r9 = r9 | r11
    .......D======================================================================eE---R............................  r8 = r8 | r12
    ........D=========================================================================eER...........................  r9 = r9 | r10
    ........D==========================================================================eER..........................  r9 = r9 << 0x20
    ........D===========================================================================eER.........................  r8 = r8 | r9
    ........D============================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x58] = r8
    ............................D==================================================eeeeeeeeeeeeeeeeeeeeeeeeeE------R  r8 = u8 [r3 + 0]
    ............................D====================================================eeeeeeeeeeeeeeeeeeeeeeeeeE----R  r9 = u8 [r2 + 0x4]
    .............................D============================================================================eeeE-R  r8 = r9 * r8
    .............................D===================================================eeeeeeeeeeeeeeeeeeeeeeeeeE----R  r9 = u16 [r5 + 0x70]
    .............................D============================================================================eE---R  jump 1898 if r9 <u 2
```

Gas simulation at offset 2044 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r9 = u8 [r5 + 0x76]
    D=========================eE--------------R  jump 2065 if r9 >=u 16
```

Gas simulation at offset 2052 with total cost of 26:

```
    DeeER........................  r11 = 0xf - r9
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r9 = u8 [r5 + 0x3d]
    .DeE-----------------------R.  r6 = 0
    .D========================eER  jump 2077 if r9 != 0
```

Gas simulation at offset 2063 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 2113
```

Gas simulation at offset 2065 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeE---------------------------------------R  r11 = r9 + 0xfffffffffffffff0
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r9 = u8 [r5 + 0x3d]
    .DeE--------------------------------------R  r6 = 0
    .D========================eE--------------R  jump 2113 if r9 == 0
```

Gas simulation at offset 2077 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r9 = u8 [r5 + 0x3e]
    D=========================eE--------------R  jump 2113 if r9 == 0
```

Gas simulation at offset 2084 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r9 = u16 [r5 + 0x3a]
    D=========================eE--------------R  r9 = r9 & 0x1
    D==========================eE-------------R  jump 2440 if r9 != 0
```

Gas simulation at offset 2095 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  r9 = u8 [r5 + 0x30]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  r10 = u64 [r1 + 0x40]
    D=========================eE--------------R............  r9 = r10 - r9
    .D=========================eE-------------R............  r9 = r9 + 0x7ff
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u8 [r9 + 0x35]
    .DeeE-------------------------------------------------R  fallthrough
```

Gas simulation at offset 2113 with total cost of 50:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........  r10 = u8 [r5 + 0x91]
    DeE---------------------------------------R..........  r9 = r8 | r7
    .DeE--------------------------------------R..........  r9 = r9 & 0xff
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x50] = r10
    .D=eeeeeeeeeeeeeeeeeeeeE----------------------------R  jump 2291 if r9 == 0
```

Gas simulation at offset 2132 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x38] = r11
    DeE------------------------R  r7 = r7 & 0xff
    D=eeeeeeeeeeeeeeeeeeeeE----R  jump 2184 if r7 == 0
```

Gas simulation at offset 2142 with total cost of 14:

```
    DeER.............  i32 r9 = clz r7
    D=eeER...........  i32 r7 = r7 << r9
    .DeE-R...........  r9 = r9 << 0x17
    .D==eeER.........  i32 r10 = r7 >> 0x8
    ..D=eE-R.........  r11 = r7 >> 0x7
    ...D==eeER.......  r11 = r11 & ~r10
    ....D=eeER.......  i32 r10 = r10 - r9
    ....DeE--R.......  r7 = r7 << 0x18
    ....D===eER......  r11 = r11 & 0x1
    .....D===eeER....  i32 r7 = r7 - r11
    .....D=====eeER..  i32 r7 = r7 >> 0x1f
    ......D=eE----R..  r9 = r10 + 0x4e800000
    ......D======eeER  i32 r7 = r7 + r9
    .......DeeE-----R  fallthrough
```

Gas simulation at offset 2184 with total cost of 21:

```
    DeER....................  r8 = r8 & 0xff
    D=eeeeeeeeeeeeeeeeeeeeER  jump 2238 if r8 == 0
```

Gas simulation at offset 2191 with total cost of 22:

```
    DeER.....................  i32 r9 = clz r8
    D=eeER...................  i32 r8 = r8 << r9
    .DeE-R...................  r9 = r9 << 0x17
    .D==eeER.................  i32 r10 = r8 >> 0x8
    ..D=eE-R.................  r11 = r8 >> 0x7
    ...D==eeER...............  r11 = r11 & ~r10
    ....D=eeER...............  i32 r10 = r10 - r9
    ....DeE--R...............  r8 = r8 << 0x18
    ....D===eER..............  r11 = r11 & 0x1
    .....D===eeER............  i32 r8 = r8 - r11
    .....D=====eeER..........  i32 r8 = r8 >> 0x1f
    ......D=eE----R..........  r9 = r10 + 0x4e800000
    ......D======eeER........  i32 r8 = r8 + r9
    .......DeE------R........  r0 = 0x1c
    .......DeeeeeeeeeeeeeeeER  jump 33829
```

Gas simulation at offset 2238 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  r0 = 28, jump 33829
```

Gas simulation at offset 2243 with total cost of 16:

```
    DeeER..............  i32 r8 = r7 + 0
    DeE-R..............  r7 = 0x45fe0000
    .DeeeeeeeeeeeeeeeER  r0 = 30, jump 34745
```

Gas simulation at offset 2256 with total cost of 15:

```
    DeeER.............  i32 r7 = r7 + 0
    DeE-R.............  r8 = 0x42c80000
    DeeeeeeeeeeeeeeeER  r0 = 32, jump 33829
```

Gas simulation at offset 2269 with total cost of 16:

```
    DeeER..............  i32 r8 = r7 + 0
    DeE-R..............  r7 = 0x42bfc28f
    .DeeeeeeeeeeeeeeeER  r0 = 34, jump 34745
```

Gas simulation at offset 2282 with total cost of 25:

```
    D...........................  r9 = r7
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r10 = u64 [r1 + 0x50]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r11 = u64 [r1 + 0x38]
    DeeE-----------------------R  fallthrough
```

Gas simulation at offset 2291 with total cost of 23:

```
    DeER......................  r7 = r6 | r11
    D=eER.....................  r7 = r7 | r10
    D==eER....................  r7 = r7 & 0xff
    .D==eeeeeeeeeeeeeeeeeeeeER  jump 2613 if r7 == 0
```

Gas simulation at offset 2305 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x38] = r9
    DeE------------------------R  r7 = r11 & 0xff
    D=eeeeeeeeeeeeeeeeeeeeE----R  jump 2368 if r7 == 0
```

Gas simulation at offset 2315 with total cost of 22:

```
    DeER.....................  i32 r8 = clz r7
    D=eeER...................  i32 r7 = r7 << r8
    .DeE-R...................  r8 = r8 << 0x17
    .D==eeER.................  i32 r9 = r7 >> 0x8
    ..D=eE-R.................  r10 = r7 >> 0x7
    ...D==eeER...............  r10 = r10 & ~r9
    ....D=eeER...............  i32 r9 = r9 - r8
    ....DeE--R...............  r7 = r7 << 0x18
    ....D===eER..............  r10 = r10 & 0x1
    .....D===eeER............  i32 r7 = r7 - r10
    .....D=====eeER..........  i32 r7 = r7 >> 0x1f
    ......D=eE----R..........  r8 = r9 + 0x4e800000
    ......D======eeER........  i32 r7 = r7 + r8
    .......DeE------R........  r8 = 0x46008c00
    .......DeE------R........  r0 = 0x24
    .......DeeeeeeeeeeeeeeeER  jump 34745
```

Gas simulation at offset 2368 with total cost of 15:

```
    DeER..............  r8 = 0x46008c00
    DeeeeeeeeeeeeeeeER  r0 = 36, jump 34745
```

Gas simulation at offset 2379 with total cost of 27:

```
    DeeER.........................  i32 r7 = r7 + 0
    D==eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x30] = r7
    DeeeeeeeeeeeeeeeeeeeeE-------R  jump 2464 if r6 == 0
```

Gas simulation at offset 2387 with total cost of 23:

```
    DeER......................  i32 r7 = clz r6
    .DeeER....................  i32 r8 = r6 << r7
    ..DeER....................  r7 = r7 << 0x17
    ..D=eeER..................  i32 r9 = r8 >> 0x8
    ...DeE-R..................  r10 = r8 >> 0x7
    ....D=eeER................  r10 = r10 & ~r9
    .....DeeER................  i32 r9 = r9 - r7
    .....DeE-R................  r8 = r8 << 0x18
    .....D==eER...............  r10 = r10 & 0x1
    ......D==eeER.............  i32 r8 = r8 - r10
    ......D====eeER...........  i32 r8 = r8 >> 0x1f
    .......DeE----R...........  r7 = r9 + 0x4e800000
    .......D=====eeER.........  i32 r7 = r7 + r8
    ........DeE-----R.........  r8 = 0x463f4400
    ........DeE-----R.........  r0 = 0x26
    ........DeeeeeeeeeeeeeeeER  jump 34745
```

Gas simulation at offset 2440 with total cost of 50:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..........  unlikely
    DeE---------------------------------------R..........  r6 = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........  r10 = u8 [r5 + 0x91]
    .DeE--------------------------------------R..........  r9 = r8 | r7
    .D=eE-------------------------------------R..........  r9 = r9 & 0xff
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x50] = r10
    ..D=eeeeeeeeeeeeeeeeeeeeE---------------------------R  jump 2132 if r9 != 0
```

Gas simulation at offset 2461 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 2291
```

Gas simulation at offset 2464 with total cost of 15:

```
    DeER..............  r7 = 0
    DeER..............  r8 = 0x463f4400
    DeeeeeeeeeeeeeeeER  r0 = 38, jump 34745
```

Gas simulation at offset 2477 with total cost of 25:

```
    DeeER.......................  i32 r8 = r7 + 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u64 [r1 + 0x30]
    .DeeeeeeeeeeeeeeeE---------R  r0 = 40, jump 33829
```

Gas simulation at offset 2487 with total cost of 45:

```
    DeeER...........................................  i32 r6 = r7 + 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER....................  r8 = u64 [r1 + 0x50]
    .D========================eeeeeeeeeeeeeeeeeeeeER  jump 2548 if r8 == 0
```

Gas simulation at offset 2495 with total cost of 22:

```
    DeER.....................  i32 r7 = clz r8
    D=eeER...................  i32 r8 = r8 << r7
    .DeE-R...................  r7 = r7 << 0x17
    .D==eeER.................  i32 r9 = r8 >> 0x8
    ..D=eE-R.................  r10 = r8 >> 0x7
    ...D==eeER...............  r10 = r10 & ~r9
    ....D=eeER...............  i32 r9 = r9 - r7
    ....DeE--R...............  r8 = r8 << 0x18
    ....D===eER..............  r10 = r10 & 0x1
    .....D===eeER............  i32 r8 = r8 - r10
    .....D=====eeER..........  i32 r8 = r8 >> 0x1f
    ......D=eE----R..........  r7 = r9 + 0x4e800000
    ......D======eeER........  i32 r7 = r7 + r8
    .......DeE------R........  r8 = 0x46b0dc00
    .......DeE------R........  r0 = 0x2a
    .......DeeeeeeeeeeeeeeeER  jump 34745
```

Gas simulation at offset 2548 with total cost of 15:

```
    DeER..............  r7 = 0
    DeER..............  r8 = 0x46b0dc00
    DeeeeeeeeeeeeeeeER  r0 = 42, jump 34745
```

Gas simulation at offset 2561 with total cost of 16:

```
    DeeER..............  i32 r8 = r7 + 0
    D..................  r7 = r6
    .DeeeeeeeeeeeeeeeER  r0 = 44, jump 33829
```

Gas simulation at offset 2570 with total cost of 16:

```
    DeeER..............  i32 r8 = r7 + 0
    DeE-R..............  r7 = 0x3f800000
    .DeeeeeeeeeeeeeeeER  r0 = 46, jump 34745
```

Gas simulation at offset 2583 with total cost of 15:

```
    DeeER.............  i32 r7 = r7 + 0
    DeE-R.............  r8 = 0x42c80000
    DeeeeeeeeeeeeeeeER  r0 = 48, jump 33829
```

Gas simulation at offset 2596 with total cost of 16:

```
    DeeER..............  i32 r8 = r7 + 0
    DeE-R..............  r7 = 0x431fca3d
    .DeeeeeeeeeeeeeeeER  r0 = 50, jump 34745
```

Gas simulation at offset 2609 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r9 = u64 [r1 + 0x38]
    DeeE-----------------------R  fallthrough
```

Gas simulation at offset 2613 with total cost of 17:

```
    DeeER...............  i32 r9 = r9 + 0
    .DeeER..............  i32 r8 = r7 + 0
    .D..................  r7 = r9
    ..DeeeeeeeeeeeeeeeER  r0 = 52, jump 33829
```

Gas simulation at offset 2624 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = i32 [r5 + 0x64]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x18] = r7
    DeE------------------------R  r7 = 0x3f639ff9
    DeeeeeeeeeeeeeeeE----------R  r0 = 54, jump 34301
```

Gas simulation at offset 2641 with total cost of 50:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r8 = i32 [r5 + 0x58]
    D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x38] = r8
    DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  u64 [r1 + 0x30] = r7
    DeE-------------------------------------------------R  r7 = 0xffffffffbfe7002f
    .DeeeeeeeeeeeeeeeE----------------------------------R  r0 = 56, jump 34301
```

Gas simulation at offset 2661 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = i32 [r5 + 0x60]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x28] = r7
    DeE------------------------R  r7 = 0x3f8b0904
    D...........................  r8 = r6
    .DeeeeeeeeeeeeeeeE---------R  r0 = 58, jump 34301
```

Gas simulation at offset 2680 with total cost of 50:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r8 = i32 [r5 + 0x54]
    D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x50] = r8
    DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  u64 [r1 + 0x20] = r7
    DeE-------------------------------------------------R  r7 = 0xffffffffc0000000
    .DeeeeeeeeeeeeeeeE----------------------------------R  r0 = 60, jump 34301
```

Gas simulation at offset 2700 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x10] = r7
    DeE------------------------R  r7 = 0x3f79896a
    D...........................  r8 = r6
    DeeeeeeeeeeeeeeeE----------R  r0 = 62, jump 34301
```

Gas simulation at offset 2716 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = i32 [r5 + 0x5c]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0] = r7
    DeE------------------------R  r7 = 0x3f4eba39
    DeeeeeeeeeeeeeeeE----------R  r0 = 64, jump 34301
```

Gas simulation at offset 2732 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x8] = r7
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = i32 [r1 + 0x18]
    DeE------------------------R  r7 = 0x3cb94332
    DeeeeeeeeeeeeeeeE----------R  r0 = 66, jump 34301
```

Gas simulation at offset 2749 with total cost of 50:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r8 = i32 [r5 + 0x50]
    D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x18] = r8
    D....................................................  r6 = r7
    DeE-------------------------------------------------R  r7 = 0xffffffffbfe4746c
    .DeeeeeeeeeeeeeeeE----------------------------------R  r0 = 68, jump 34301
```

Gas simulation at offset 2768 with total cost of 16:

```
    DeER...............  r7 = r7 ^ 0xffffffff80000000
    DeeER..............  i32 r8 = r6 + 0
    .DeeER.............  i32 r7 = r7 + 0
    .DeeeeeeeeeeeeeeeER  r0 = 70, jump 33829
```

Gas simulation at offset 2783 with total cost of 28:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...  r8 = u64 [r1 + 0x8]
    D=========================eER..  r8 = r8 ^ 0xffffffff80000000
    DeeE------------------------R..  i32 r7 = r7 + 0
    .D=========================eeER  i32 r8 = r8 + 0
    .DeeeeeeeeeeeeeeeE------------R  r0 = 72, jump 33829
```

Gas simulation at offset 2801 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x8] = r7
    DeeE-----------------------R  i32 r8 = r7 + 0
    .DeE-----------------------R  r7 = 0x3d34a6a0
    .DeeeeeeeeeeeeeeeE---------R  r0 = 74, jump 34301
```

Gas simulation at offset 2817 with total cost of 25:

```
    D...........................  r6 = r7
    DeER........................  r7 = 0xffffffffbfeccd54
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = u64 [r1 + 0x50]
    DeeeeeeeeeeeeeeeE----------R  r0 = 76, jump 34301
```

Gas simulation at offset 2833 with total cost of 16:

```
    DeER...............  r7 = r7 ^ 0xffffffff80000000
    DeeER..............  i32 r8 = r6 + 0
    .DeeER.............  i32 r7 = r7 + 0
    .DeeeeeeeeeeeeeeeER  r0 = 78, jump 33829
```

Gas simulation at offset 2848 with total cost of 28:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...  r8 = u64 [r1 + 0]
    D=========================eER..  r8 = r8 ^ 0xffffffff80000000
    DeeE------------------------R..  i32 r7 = r7 + 0
    .D=========================eeER  i32 r8 = r8 + 0
    .DeeeeeeeeeeeeeeeE------------R  r0 = 80, jump 33829
```

Gas simulation at offset 2865 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0] = r7
    DeeE-----------------------R  i32 r8 = r7 + 0
    .DeE-----------------------R  r7 = 0x3f8b3765
    .DeeeeeeeeeeeeeeeE---------R  r0 = 82, jump 34301
```

Gas simulation at offset 2880 with total cost of 25:

```
    DeeER.......................  i32 r7 = r7 + 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = i32 [r1 + 0x10]
    DeeeeeeeeeeeeeeeE----------R  r0 = 84, jump 33829
```

Gas simulation at offset 2890 with total cost of 25:

```
    DeeER.......................  i32 r7 = r7 + 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = i32 [r1 + 0x20]
    DeeeeeeeeeeeeeeeE----------R  r0 = 86, jump 33829
```

Gas simulation at offset 2900 with total cost of 28:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...  r8 = u64 [r1 + 0x28]
    DeE------------------------R...  r6 = 0xffffffff80000000
    D=========================eER..  r8 = r8 ^ r6
    .DeeE-----------------------R..  i32 r7 = r7 + 0
    .D=========================eeER  i32 r8 = r8 + 0
    ..DeeeeeeeeeeeeeeeE-----------R  r0 = 88, jump 33829
```

Gas simulation at offset 2921 with total cost of 28:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...  r8 = u64 [r1 + 0x30]
    D=========================eER..  r8 = r8 ^ r6
    DeeE------------------------R..  i32 r7 = r7 + 0
    .D=========================eeER  i32 r8 = r8 + 0
    .DeeeeeeeeeeeeeeeE------------R  r0 = 90, jump 33829
```

Gas simulation at offset 2936 with total cost of 100:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r8 = u8 [r5 + 0x9a]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r9 = u64 [r1 + 0x8]
    D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  u32 [r5 + 0x50] = r9
    DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R..................................................  r9 = u64 [r1 + 0]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  u32 [r5 + 0x54] = r9
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE------------------------R..................................................  u32 [r5 + 0x58] = r7
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  r7 = u64 [r1 + 0x18]
    .D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u32 [r5 + 0x5c] = r7
    ..D========================eE------------------------------------------------R.........................  r8 = r8 + 0x1
    ..D=========================eE-----------------------------------------------R.........................  r9 = r8 & 0xff
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeE----------------------R.........................  r10 = u64 [r1 + 0x50]
    ...D==================================================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  u32 [r5 + 0x60] = r10
    ...D===============================================eeeeeeeeeeeeeeeeeeeeeeeeeE---R......................  r10 = u64 [r1 + 0x38]
    ...D========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r5 + 0x64] = r10
    ...D===============================================eeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  u8 [r5 + 0x9a] = a1
    ....D=======================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0x40]
    ....D=======================================================================eE------------------------R  jump 3028 if r9 <u 8
```

Gas simulation at offset 2990 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  r7 = i32 [r5 + 0x25c]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  u8 [r5 + 154] = 0
    .D========================eeE-------------R............  i32 r7 = r7 + 0x1
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r5 + 0x25c] = r7
    .D==========================eE------------------------R  jump 3028 if r7 <u 735
```

Gas simulation at offset 3011 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r7 = i32 [r5 + 0x258]
    D=========================eE--------------R...........  r7 = r7 + 0x1
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r5 + 0x258] = r7
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  u32 [r5 + 604] = 0
    .DeeE------------------------------------------------R  fallthrough
```

Gas simulation at offset 3028 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r7 = i16 [r5 + 0x94]
    DeE---------------------------------------R...........  r8 = 0xffff000000000000
    .D========================eE--------------R...........  r9 = r7 << 0x30
    .D=========================eE-------------R...........  r8 = r8 + r9
    .D========================eE--------------R...........  r7 = r7 + 0xffffffffffffffff
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x94] = r7
    ..D=========================eE-----------------------R  jump 3400 if r8 == 0
```

Gas simulation at offset 3060 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r8 = u8 [r5 + 0x92]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u8 [r5 + 0x93]
    DeE---------------------------------------R  r9 = 0x2
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R  u8 [r5 + 0x92] = a2
    .D========================eE--------------R  jump 3128 if r8 == r9
```

Gas simulation at offset 3079 with total cost of 56:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER................  unlikely
    DeE---------------------------------------R................  r8 = r8 & 0x1
    DeE---------------------------------------R................  r9 = 0x17bf4
    DeE---------------------------------------R................  r10 = 0x17c3c
    .DeE--------------------------------------R................  r11 = 0x1
    .DeeE-------------------------------------R................  r10 = r9 if r8 == 0
    ..DeeE------------------------------------R................  r7 = r11 & ~r7
    ...D=eE-----------------------------------R................  r9 = r7 << 0x3
    ...D==eE----------------------------------R................  r9 = r9 + r10
    ...D===eeeeeeeeeeeeeeeeeeeeeeeeeE---------R................  r9 = i16 [r9 + 0]
    ....DeE-----------------------------------R................  r8 = r8 ^ 0x9
    ....DeeeeeeeeeeeeeeeeeeeeeeeeeE-----------R................  u64 [r5 + 0x40] = r10
    ....D=eeeeeeeeeeeeeeeeeeeeeeeeeE----------R................  u64 [r5 + 0x48] = r8
    ....D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x94] = r9
    .....DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R  u8 [r5 + 0x99] = a0
    .....DeeE-------------------------------------------------R  fallthrough
```

Gas simulation at offset 3128 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u64 [r5 + 0x200]
    D=========================eE--------------R  jump 3236 if r7 != 0
```

Gas simulation at offset 3136 with total cost of 26:

```
    DeER.........................  r8 = 0x30a98
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x50] = r8
    D=eE------------------------R  r7 = r8 + 0x2750
    .D=eE-----------------------R  r7 = r7 & 0xfffffffffffffffc
    .DeE------------------------R  r8 = 0x1
    .DeeE-----------------------R  fallthrough
```

Gas simulation at offset 3155 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  u64 [0x30000] = r4
    DeE---------------------------------------R............  r4 = r8 << 0x20
    .DeE--------------------------------------R............  r4 = r4 >>a 0x20
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R............  r9 = i32 [r7 + 0]
    .D=========================eE-------------R............  r4 = r9 | r4
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r7 + 0] = r4
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r4 = u64 [0x30000]
    ..D========================eE-------------------------R  r9 = r9 & 0xff
    ..D=========================eE------------------------R  jump 3155 if r9 != 0
```

Gas simulation at offset 3186 with total cost of 15:

```
    DeER..............  r7 = 0xf00
    DeER..............  r8 = 0
    DeeeeeeeeeeeeeeeER  r0 = 92, jump 26592
```

Gas simulation at offset 3197 with total cost of 51:

```
    D.....................................................  r6 = r7
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r8 = u64 [r1 + 0x50]
    D=========================eER.........................  r7 = r8 + 0x2000
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 1872] = 0
    .DeE-------------------------------------------------R  jump 32329 if r6 == 0
```

Gas simulation at offset 3214 with total cost of 15:

```
    DeER..............  r9 = 0x1e000
    D.................  r7 = r6
    DeER..............  r8 = 0
    DeeeeeeeeeeeeeeeER  r0 = 94, jump 28080
```

Gas simulation at offset 3228 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r5 + 0x200] = r6
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0x40]
    DeeE-----------------------R  fallthrough
```

Gas simulation at offset 3236 with total cost of 74:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r7 = i16 [r5 + 0x220]
    DeE---------------------------------------R..................................  r8 = 0x18518
    D=========================eE--------------R..................................  r7 = r7 << 0x3
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R..................................  u64 [r1 + 0x48] = r8
    .D=========================eE-------------R..................................  r7 = r7 + r8
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r8 = u64 [r7 + 0]
    .D...........................................................................  r7 = r6
    ..D==================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 96, jump [r8 + 0]
```

Gas simulation at offset 3263 with total cost of 54:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.............................  r8 = u8 [r5 + 0x22e]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.............................  r7 = i16 [r5 + 0x220]
    D=========================eER............................  r9 = r8 << 0x1
    .D========================eER............................  r10 = r8 << 0x3
    .D=========================eER...........................  r9 = r10 - r9
    .DeE-------------------------R...........................  r10 = 0x172f0
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................  u64 [r1 + 0x50] = r10
    ..D=========================eER..........................  r9 = r9 + r10
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  r10 = u16 [r9 + 0x4]
    ..D=======================eE---------------------------R.  r7 = r7 + 0x1
    ...D=======================eE--------------------------R.  r11 = zext16 r7
    ...D=======================eeeeeeeeeeeeeeeeeeeeeeeeeE--R.  u16 [r5 + 0x220] = r7
    ...D==================================================eER  jump 3635 if r10 >=u r11
```

Gas simulation at offset 3307 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r7 = i16 [r5 + 0x21e]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r10 = u16 [r9 + 0]
    D=========================eE--------------R...........  r7 = r7 + 0x1
    .D=========================eE-------------R...........  r11 = zext16 r7
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x21e] = r7
    .D==========================eE-----------------------R  jump 3387 if r11 != r10
```

Gas simulation at offset 3326 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r9 = u8 [r5 + 0x22d]
    D=========================eE--------------R.............  r10 = r9 << 0x2
    .DeE--------------------------------------R.............  r7 = 0x17250
    .D=========================eE-------------R.............  r10 = r10 + r7
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  r12 = u8 [r10 + 0x3]
    ..DeE-------------------------------------------------R.  r11 = r8 + 0x1
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R.  u16 [r5 + 542] = 0
    ..D=eeeeeeeeeeeeeeeeeeeeeeeeeE------------------------R.  u8 [r5 + 0x22e] = a4
    ...D=================================================eER  jump 3444 if r8 >=u r12
```

Gas simulation at offset 3359 with total cost of 78:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER......................................  unlikely
    DeE---------------------------------------R......................................  r7 = r11 << 0x1
    DeE---------------------------------------R......................................  r11 = r11 << 0x3
    .DeE--------------------------------------R......................................  r11 = r11 - r7
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R......................................  r9 = u64 [r1 + 0x50]
    .D=========================eE-------------R......................................  r9 = r9 + r11
    .D==========================eE------------R......................................  r9 = r9 + 0x2
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r7 = u16 [r9 + 0]
    ..D===================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x220] = r7
    ..DeeeeeeeeeeeeeeeE-------------------------------------------------------------R  jump 3635
```

Gas simulation at offset 3387 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeE---------------------------------------R...........  r9 = r9 + 0x2
    D=eeeeeeeeeeeeeeeeeeeeeeeeeE--------------R...........  r7 = u16 [r9 + 0]
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x220] = r7
    .DeeeeeeeeeeeeeeeE-----------------------------------R  jump 3635
```

Gas simulation at offset 3400 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u8 [r5 + 0x99]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r8 = u64 [r5 + 0x48]
    D=========================eE--------------R  jump 5419 if r7 >=u r8
```

Gas simulation at offset 3412 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  r6 = u64 [r5 + 0x40]
    DeE---------------------------------------R............  r7 = r7 << 0x3
    D=========================eE--------------R............  r6 = r6 + r7
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  r7 = u8 [r6 + 0x6]
    .D==================================================eER  jump 3524 if r7 == 0
```

Gas simulation at offset 3428 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u8 [r5 + 0x7a]
    D=========================eE--------------R  jump 3499 if r7 == 0
```

Gas simulation at offset 3435 with total cost of 50:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........  r7 = u8 [r5 + 0x75]
    D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x74] = a0
    DeeeeeeeeeeeeeeeE-----------------------------------R  jump 3513
```

Gas simulation at offset 3444 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r8 = i16 [r5 + 0x21c]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r11 = u16 [r10 + 0]
    D=========================eE--------------R...........  r8 = r8 + 0x1
    .D=========================eE-------------R...........  r12 = zext16 r8
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x21c] = r8
    .D==========================eeeeeeeeeeeeeeeeeeeeE----R  jump 3602 if r12 != r11
```

Gas simulation at offset 3464 with total cost of 26:

```
    DeER.........................  r8 = r9 + 0x1
    DeER.........................  r10 = 0x7
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  u16 [r5 + 540] = 0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x22d] = a1
    .DeeeeeeeeeeeeeeeeeeeeE-----R  jump 3488 if r9 != r10
```

Gas simulation at offset 3481 with total cost of 25:

```
    DeER........................  r8 = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 557] = 0
    DeeE-----------------------R  fallthrough
```

Gas simulation at offset 3488 with total cost of 27:

```
    DeER..........................  r8 = r8 << 0x2
    D=eER.........................  r7 = r7 + r8
    D==eeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u8 [r7 + 0x2]
    DeeeeeeeeeeeeeeeE------------R  jump 3606
```

Gas simulation at offset 3499 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u8 [r5 + 0x74]
    D=========================eE--------------R  jump 3513 if r7 == 0
```

Gas simulation at offset 3506 with total cost of 26:

```
    DeER.........................  r7 = r7 + 0xffffffffffffffff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x74] = a0
    DeeE------------------------R  fallthrough
```

Gas simulation at offset 3513 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u8 [r5 + 0x77]
    D=========================eE--------------R  jump 3524 if r7 != 0
```

Gas simulation at offset 3520 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 122] = 0
    DeeE-----------------------R  fallthrough
```

Gas simulation at offset 3524 with total cost of 45:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.....  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.....  r7 = u8 [r6 + 0x5]
    D=========================eeeeeeeeeeeeeeeeeeeeER  jump 3549 if r7 == 0
```

Gas simulation at offset 3531 with total cost of 15:

```
    D.................  r7 = r5
    DeeeeeeeeeeeeeeeER  r0 = 98, jump 61
```

Gas simulation at offset 3538 with total cost of 26:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r7 = u64 [r1 + 0x48]
    D=========================eER  r7 = r7 + 0x19
    DeeeeeeeeeeeeeeeE-----------R  r0 = 100, jump 61
```

Gas simulation at offset 3549 with total cost of 26:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r7 = u8 [r6 + 0x7]
    D=========================eER  jump 5247 if r7 == 0
```

Gas simulation at offset 3556 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u8 [r5 + 0x2]
    D=========================eE--------------R  jump 3585 if r7 == 0
```

Gas simulation at offset 3563 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r7 = u8 [r5 + 0x3]
    DeE---------------------------------------R...........  r8 = 0xf
    D=========================eE--------------R...........  r7 = r7 + 0x1
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R...........  u8 [r5 + 2] = 0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R...........  u8 [r5 + 0x4] = a1
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x5] = a0
    .DeeeeeeeeeeeeeeeE-----------------------------------R  jump 5095
```

Gas simulation at offset 3585 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u8 [r5 + 0x5]
    D=========================eE--------------R  jump 3852 if r7 == 0
```

Gas simulation at offset 3593 with total cost of 26:

```
    DeER.........................  r7 = r7 + 0xffffffffffffffff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x5] = a0
    DeeeeeeeeeeeeeeeE-----------R  jump 5095
```

Gas simulation at offset 3602 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u8 [r10 + 0x2]
    DeeE-----------------------R  fallthrough
```

Gas simulation at offset 3606 with total cost of 78:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.....................................................  u8 [r5 + 0x22e] = a0
    DeE------------------------R.....................................................  r8 = r7 << 0x1
    DeE------------------------R.....................................................  r7 = r7 << 0x3
    .DeE-----------------------R.....................................................  r7 = r7 - r8
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER....................................................  r8 = u64 [r1 + 0x50]
    .D=========================eER...................................................  r7 = r7 + r8
    ..D=========================eER..................................................  r9 = r7 + 0x2
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r7 = u16 [r9 + 0]
    ..D===================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x220] = r7
    ...DeeE-------------------------------------------------------------------------R  fallthrough
```

Gas simulation at offset 3635 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r8 = u8 [r5 + 0x23b]
    D=========================eE--------------R  jump 3908 if r8 == 0
```

Gas simulation at offset 3644 with total cost of 73:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.................................  unlikely
    DeE---------------------------------------R.................................  r7 = sext16 r7
    D=eE--------------------------------------R.................................  r7 = r7 << 0x3
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.................................  r8 = u64 [r1 + 0x48]
    .D========================eE--------------R.................................  r7 = r7 + r8
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r8 = u64 [r7 + 0]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R......................  u8 [r5 + 571] = 0
    .D..........................................................................  r7 = r6
    ..D=================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 102, jump [r8 + 0]
```

Gas simulation at offset 3668 with total cost of 54:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.............................  r8 = u8 [r5 + 0x22e]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.............................  r7 = i16 [r5 + 0x220]
    D=========================eER............................  r9 = r8 << 0x1
    .D========================eER............................  r10 = r8 << 0x3
    .D=========================eER...........................  r9 = r10 - r9
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-R...........................  r10 = u64 [r1 + 0x50]
    ..D=========================eER..........................  r9 = r9 + r10
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  r10 = u16 [r9 + 0x4]
    ..D=======================eE---------------------------R.  r7 = r7 + 0x1
    ..D========================eE--------------------------R.  r11 = zext16 r7
    ...D=======================eeeeeeeeeeeeeeeeeeeeeeeeeE--R.  u16 [r5 + 0x220] = r7
    ...D==================================================eER  jump 3908 if r10 >=u r11
```

Gas simulation at offset 3707 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r7 = i16 [r5 + 0x21e]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r10 = u16 [r9 + 0]
    D=========================eE--------------R...........  r7 = r7 + 0x1
    .D=========================eE-------------R...........  r11 = zext16 r7
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x21e] = r7
    .D==========================eE-----------------------R  jump 3786 if r11 != r10
```

Gas simulation at offset 3726 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r9 = u8 [r5 + 0x22d]
    D=========================eE--------------R.............  r10 = r9 << 0x2
    .DeE--------------------------------------R.............  r7 = 0x17250
    .D=========================eE-------------R.............  r10 = r10 + r7
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  r12 = u8 [r10 + 0x3]
    ..DeE-------------------------------------------------R.  r11 = r8 + 0x1
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R.  u16 [r5 + 542] = 0
    ..D=eeeeeeeeeeeeeeeeeeeeeeeeeE------------------------R.  u8 [r5 + 0x22e] = a4
    ...D=================================================eER  jump 3798 if r8 >=u r12
```

Gas simulation at offset 3759 with total cost of 78:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER......................................  unlikely
    DeE---------------------------------------R......................................  r7 = r11 << 0x1
    DeE---------------------------------------R......................................  r11 = r11 << 0x3
    .DeE--------------------------------------R......................................  r11 = r11 - r7
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R......................................  r9 = u64 [r1 + 0x50]
    .D=========================eE-------------R......................................  r9 = r9 + r11
    .D==========================eE------------R......................................  r9 = r9 + 0x2
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r7 = u16 [r9 + 0]
    ..D===================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x220] = r7
    ..DeeeeeeeeeeeeeeeE-------------------------------------------------------------R  jump 3908
```

Gas simulation at offset 3786 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeE---------------------------------------R...........  r9 = r9 + 0x2
    D=eeeeeeeeeeeeeeeeeeeeeeeeeE--------------R...........  r7 = u16 [r9 + 0]
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x220] = r7
    .DeeeeeeeeeeeeeeeE-----------------------------------R  jump 3908
```

Gas simulation at offset 3798 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r8 = i16 [r5 + 0x21c]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r11 = u16 [r10 + 0]
    D=========================eE--------------R...........  r8 = r8 + 0x1
    .D=========================eE-------------R...........  r12 = zext16 r8
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x21c] = r8
    .D==========================eeeeeeeeeeeeeeeeeeeeE----R  jump 3875 if r12 != r11
```

Gas simulation at offset 3817 with total cost of 26:

```
    DeER.........................  r8 = r9 + 0x1
    DeER.........................  r10 = 0x7
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  u16 [r5 + 540] = 0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x22d] = a1
    .DeeeeeeeeeeeeeeeeeeeeE-----R  jump 3841 if r9 != r10
```

Gas simulation at offset 3834 with total cost of 25:

```
    DeER........................  r8 = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 557] = 0
    DeeE-----------------------R  fallthrough
```

Gas simulation at offset 3841 with total cost of 27:

```
    DeER..........................  r8 = r8 << 0x2
    D=eER.........................  r7 = r7 + r8
    D==eeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u8 [r7 + 0x2]
    DeeeeeeeeeeeeeeeE------------R  jump 3879
```

Gas simulation at offset 3852 with total cost of 50:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........  r8 = u8 [r5 + 0x3]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........  r7 = u8 [r5 + 0x4]
    D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x5] = a1
    .D========================eE------------------------R  jump 5083 if r7 == 0
```

Gas simulation at offset 3866 with total cost of 26:

```
    DeER.........................  r7 = r7 + 0xffffffffffffffff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x4] = a0
    DeeeeeeeeeeeeeeeE-----------R  jump 5095
```

Gas simulation at offset 3875 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u8 [r10 + 0x2]
    DeeE-----------------------R  fallthrough
```

Gas simulation at offset 3879 with total cost of 78:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.....................................................  u8 [r5 + 0x22e] = a0
    DeE------------------------R.....................................................  r8 = r7 << 0x1
    DeE------------------------R.....................................................  r7 = r7 << 0x3
    .DeE-----------------------R.....................................................  r7 = r7 - r8
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER....................................................  r8 = u64 [r1 + 0x50]
    .D=========================eER...................................................  r7 = r7 + r8
    ..D=========================eER..................................................  r9 = r7 + 0x2
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r7 = u16 [r9 + 0]
    ..D===================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x220] = r7
    ...DeeE-------------------------------------------------------------------------R  fallthrough
```

Gas simulation at offset 3908 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r8 = u64 [r5 + 0x200]
    D=========================eE--------------R  jump 4020 if r8 != 0
```

Gas simulation at offset 3916 with total cost of 26:

```
    DeER.........................  r8 = 0x30a98
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x38] = r8
    D=eE------------------------R  r7 = r8 + 0x2750
    .D=eE-----------------------R  r7 = r7 & 0xfffffffffffffffc
    .DeE------------------------R  r8 = 0x1
    .DeeE-----------------------R  fallthrough
```

Gas simulation at offset 3935 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  u64 [0x30000] = r4
    DeE---------------------------------------R............  r4 = r8 << 0x20
    .DeE--------------------------------------R............  r4 = r4 >>a 0x20
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R............  r9 = i32 [r7 + 0]
    .D=========================eE-------------R............  r4 = r9 | r4
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r7 + 0] = r4
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r4 = u64 [0x30000]
    ..D========================eE-------------------------R  r9 = r9 & 0xff
    ..D=========================eE------------------------R  jump 3935 if r9 != 0
```

Gas simulation at offset 3966 with total cost of 15:

```
    DeER..............  r7 = 0xf00
    DeER..............  r8 = 0
    DeeeeeeeeeeeeeeeER  r0 = 104, jump 26592
```

Gas simulation at offset 3977 with total cost of 51:

```
    D.....................................................  r6 = r7
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r8 = u64 [r1 + 0x38]
    D=========================eER.........................  r7 = r8 + 0x2000
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 1872] = 0
    .DeE-------------------------------------------------R  jump 32329 if r6 == 0
```

Gas simulation at offset 3994 with total cost of 15:

```
    DeER..............  r9 = 0x1e000
    D.................  r7 = r6
    DeER..............  r8 = 0
    DeeeeeeeeeeeeeeeER  r0 = 106, jump 28080
```

Gas simulation at offset 4008 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u16 [r5 + 0x220]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r5 + 0x200] = r6
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0x40]
    DeeE-----------------------R  fallthrough
```

Gas simulation at offset 4020 with total cost of 73:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.................................  unlikely
    DeE---------------------------------------R.................................  r7 = sext16 r7
    D=eE--------------------------------------R.................................  r7 = r7 << 0x3
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.................................  r8 = u64 [r1 + 0x48]
    .D========================eE--------------R.................................  r7 = r7 + r8
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r8 = u64 [r7 + 0]
    .D..........................................................................  r7 = r6
    .D==================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 108, jump [r8 + 0]
```

Gas simulation at offset 4040 with total cost of 54:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.............................  r8 = u8 [r5 + 0x22e]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.............................  r7 = i16 [r5 + 0x220]
    D=========================eER............................  r9 = r8 << 0x1
    .D========================eER............................  r10 = r8 << 0x3
    .D=========================eER...........................  r9 = r10 - r9
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-R...........................  r10 = u64 [r1 + 0x50]
    ..D=========================eER..........................  r9 = r9 + r10
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  r10 = u16 [r9 + 0x4]
    ..D=======================eE---------------------------R.  r7 = r7 + 0x1
    ..D========================eE--------------------------R.  r11 = zext16 r7
    ...D=======================eeeeeeeeeeeeeeeeeeeeeeeeeE--R.  u16 [r5 + 0x220] = r7
    ...D==================================================eER  jump 4257 if r10 >=u r11
```

Gas simulation at offset 4079 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r7 = i16 [r5 + 0x21e]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r10 = u16 [r9 + 0]
    D=========================eE--------------R...........  r7 = r7 + 0x1
    .D=========================eE-------------R...........  r11 = zext16 r7
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x21e] = r7
    .D==========================eE-----------------------R  jump 4158 if r11 != r10
```

Gas simulation at offset 4098 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r9 = u8 [r5 + 0x22d]
    D=========================eE--------------R.............  r10 = r9 << 0x2
    .DeE--------------------------------------R.............  r7 = 0x17250
    .D=========================eE-------------R.............  r10 = r10 + r7
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  r12 = u8 [r10 + 0x3]
    ..DeE-------------------------------------------------R.  r11 = r8 + 0x1
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R.  u16 [r5 + 542] = 0
    ..D=eeeeeeeeeeeeeeeeeeeeeeeeeE------------------------R.  u8 [r5 + 0x22e] = a4
    ...D=================================================eER  jump 4170 if r8 >=u r12
```

Gas simulation at offset 4131 with total cost of 78:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER......................................  unlikely
    DeE---------------------------------------R......................................  r7 = r11 << 0x1
    DeE---------------------------------------R......................................  r11 = r11 << 0x3
    .DeE--------------------------------------R......................................  r11 = r11 - r7
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R......................................  r9 = u64 [r1 + 0x50]
    .D=========================eE-------------R......................................  r9 = r9 + r11
    .D==========================eE------------R......................................  r9 = r9 + 0x2
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r7 = u16 [r9 + 0]
    ..D===================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x220] = r7
    ..DeeeeeeeeeeeeeeeE-------------------------------------------------------------R  jump 4257
```

Gas simulation at offset 4158 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeE---------------------------------------R...........  r9 = r9 + 0x2
    D=eeeeeeeeeeeeeeeeeeeeeeeeeE--------------R...........  r7 = u16 [r9 + 0]
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x220] = r7
    .DeeeeeeeeeeeeeeeE-----------------------------------R  jump 4257
```

Gas simulation at offset 4170 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r8 = i16 [r5 + 0x21c]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r11 = u16 [r10 + 0]
    D=========================eE--------------R...........  r8 = r8 + 0x1
    .D=========================eE-------------R...........  r12 = zext16 r8
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x21c] = r8
    .D==========================eeeeeeeeeeeeeeeeeeeeE----R  jump 4224 if r12 != r11
```

Gas simulation at offset 4189 with total cost of 26:

```
    DeER.........................  r8 = r9 + 0x1
    DeER.........................  r10 = 0x7
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  u16 [r5 + 540] = 0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x22d] = a1
    .DeeeeeeeeeeeeeeeeeeeeE-----R  jump 4213 if r9 != r10
```

Gas simulation at offset 4206 with total cost of 25:

```
    DeER........................  r8 = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 557] = 0
    DeeE-----------------------R  fallthrough
```

Gas simulation at offset 4213 with total cost of 27:

```
    DeER..........................  r8 = r8 << 0x2
    D=eER.........................  r7 = r7 + r8
    D==eeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u8 [r7 + 0x2]
    DeeeeeeeeeeeeeeeE------------R  jump 4228
```

Gas simulation at offset 4224 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u8 [r10 + 0x2]
    DeeE-----------------------R  fallthrough
```

Gas simulation at offset 4228 with total cost of 78:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.....................................................  u8 [r5 + 0x22e] = a0
    DeE------------------------R.....................................................  r8 = r7 << 0x1
    DeE------------------------R.....................................................  r7 = r7 << 0x3
    .DeE-----------------------R.....................................................  r7 = r7 - r8
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER....................................................  r8 = u64 [r1 + 0x50]
    .D=========================eER...................................................  r7 = r7 + r8
    ..D=========================eER..................................................  r9 = r7 + 0x2
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r7 = u16 [r9 + 0]
    ..D===================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x220] = r7
    ...DeeE-------------------------------------------------------------------------R  fallthrough
```

Gas simulation at offset 4257 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r8 = u8 [r5 + 0x23b]
    D=========================eE--------------R  jump 4507 if r8 == 0
```

Gas simulation at offset 4266 with total cost of 73:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.................................  unlikely
    DeE---------------------------------------R.................................  r7 = sext16 r7
    D=eE--------------------------------------R.................................  r7 = r7 << 0x3
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.................................  r8 = u64 [r1 + 0x48]
    .D========================eE--------------R.................................  r7 = r7 + r8
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r8 = u64 [r7 + 0]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R......................  u8 [r5 + 571] = 0
    .D..........................................................................  r7 = r6
    ..D=================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 110, jump [r8 + 0]
```

Gas simulation at offset 4290 with total cost of 54:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.............................  r8 = u8 [r5 + 0x22e]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.............................  r7 = i16 [r5 + 0x220]
    D=========================eER............................  r9 = r8 << 0x1
    .D========================eER............................  r10 = r8 << 0x3
    .D=========================eER...........................  r9 = r10 - r9
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-R...........................  r10 = u64 [r1 + 0x50]
    ..D=========================eER..........................  r9 = r9 + r10
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  r10 = u16 [r9 + 0x4]
    ..D=======================eE---------------------------R.  r7 = r7 + 0x1
    ..D========================eE--------------------------R.  r11 = zext16 r7
    ...D=======================eeeeeeeeeeeeeeeeeeeeeeeeeE--R.  u16 [r5 + 0x220] = r7
    ...D==================================================eER  jump 4507 if r10 >=u r11
```

Gas simulation at offset 4329 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r7 = i16 [r5 + 0x21e]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r10 = u16 [r9 + 0]
    D=========================eE--------------R...........  r7 = r7 + 0x1
    .D=========================eE-------------R...........  r11 = zext16 r7
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x21e] = r7
    .D==========================eE-----------------------R  jump 4408 if r11 != r10
```

Gas simulation at offset 4348 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r9 = u8 [r5 + 0x22d]
    D=========================eE--------------R.............  r10 = r9 << 0x2
    .DeE--------------------------------------R.............  r7 = 0x17250
    .D=========================eE-------------R.............  r10 = r10 + r7
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  r12 = u8 [r10 + 0x3]
    ..DeE-------------------------------------------------R.  r11 = r8 + 0x1
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R.  u16 [r5 + 542] = 0
    ..D=eeeeeeeeeeeeeeeeeeeeeeeeeE------------------------R.  u8 [r5 + 0x22e] = a4
    ...D=================================================eER  jump 4420 if r8 >=u r12
```

Gas simulation at offset 4381 with total cost of 78:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER......................................  unlikely
    DeE---------------------------------------R......................................  r7 = r11 << 0x1
    DeE---------------------------------------R......................................  r11 = r11 << 0x3
    .DeE--------------------------------------R......................................  r11 = r11 - r7
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R......................................  r9 = u64 [r1 + 0x50]
    .D=========================eE-------------R......................................  r9 = r9 + r11
    .D==========================eE------------R......................................  r9 = r9 + 0x2
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r7 = u16 [r9 + 0]
    ..D===================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x220] = r7
    ..DeeeeeeeeeeeeeeeE-------------------------------------------------------------R  jump 4507
```

Gas simulation at offset 4408 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeE---------------------------------------R...........  r9 = r9 + 0x2
    D=eeeeeeeeeeeeeeeeeeeeeeeeeE--------------R...........  r7 = u16 [r9 + 0]
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x220] = r7
    .DeeeeeeeeeeeeeeeE-----------------------------------R  jump 4507
```

Gas simulation at offset 4420 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r8 = i16 [r5 + 0x21c]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r11 = u16 [r10 + 0]
    D=========================eE--------------R...........  r8 = r8 + 0x1
    .D=========================eE-------------R...........  r12 = zext16 r8
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x21c] = r8
    .D==========================eeeeeeeeeeeeeeeeeeeeE----R  jump 4474 if r12 != r11
```

Gas simulation at offset 4439 with total cost of 26:

```
    DeER.........................  r8 = r9 + 0x1
    DeER.........................  r10 = 0x7
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  u16 [r5 + 540] = 0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x22d] = a1
    .DeeeeeeeeeeeeeeeeeeeeE-----R  jump 4463 if r9 != r10
```

Gas simulation at offset 4456 with total cost of 25:

```
    DeER........................  r8 = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 557] = 0
    DeeE-----------------------R  fallthrough
```

Gas simulation at offset 4463 with total cost of 27:

```
    DeER..........................  r8 = r8 << 0x2
    D=eER.........................  r7 = r7 + r8
    D==eeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u8 [r7 + 0x2]
    DeeeeeeeeeeeeeeeE------------R  jump 4478
```

Gas simulation at offset 4474 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u8 [r10 + 0x2]
    DeeE-----------------------R  fallthrough
```

Gas simulation at offset 4478 with total cost of 78:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.....................................................  u8 [r5 + 0x22e] = a0
    DeE------------------------R.....................................................  r8 = r7 << 0x1
    DeE------------------------R.....................................................  r7 = r7 << 0x3
    .DeE-----------------------R.....................................................  r7 = r7 - r8
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER....................................................  r8 = u64 [r1 + 0x50]
    .D=========================eER...................................................  r7 = r7 + r8
    ..D=========================eER..................................................  r9 = r7 + 0x2
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r7 = u16 [r9 + 0]
    ..D===================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x220] = r7
    ...DeeE-------------------------------------------------------------------------R  fallthrough
```

Gas simulation at offset 4507 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r8 = u64 [r5 + 0x200]
    D=========================eE--------------R  jump 4619 if r8 != 0
```

Gas simulation at offset 4515 with total cost of 26:

```
    DeER.........................  r8 = 0x30a98
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x38] = r8
    D=eE------------------------R  r7 = r8 + 0x2750
    .D=eE-----------------------R  r7 = r7 & 0xfffffffffffffffc
    .DeE------------------------R  r8 = 0x1
    .DeeE-----------------------R  fallthrough
```

Gas simulation at offset 4534 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  u64 [0x30000] = r4
    DeE---------------------------------------R............  r4 = r8 << 0x20
    .DeE--------------------------------------R............  r4 = r4 >>a 0x20
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R............  r9 = i32 [r7 + 0]
    .D=========================eE-------------R............  r4 = r9 | r4
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r7 + 0] = r4
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r4 = u64 [0x30000]
    ..D========================eE-------------------------R  r9 = r9 & 0xff
    ..D=========================eE------------------------R  jump 4534 if r9 != 0
```

Gas simulation at offset 4565 with total cost of 15:

```
    DeER..............  r7 = 0xf00
    DeER..............  r8 = 0
    DeeeeeeeeeeeeeeeER  r0 = 112, jump 26592
```

Gas simulation at offset 4576 with total cost of 51:

```
    D.....................................................  r6 = r7
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r8 = u64 [r1 + 0x38]
    D=========================eER.........................  r7 = r8 + 0x2000
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 1872] = 0
    .DeE-------------------------------------------------R  jump 32329 if r6 == 0
```

Gas simulation at offset 4593 with total cost of 15:

```
    DeER..............  r9 = 0x1e000
    D.................  r7 = r6
    DeER..............  r8 = 0
    DeeeeeeeeeeeeeeeER  r0 = 114, jump 28080
```

Gas simulation at offset 4607 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u16 [r5 + 0x220]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r5 + 0x200] = r6
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0x40]
    DeeE-----------------------R  fallthrough
```

Gas simulation at offset 4619 with total cost of 73:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.................................  unlikely
    DeE---------------------------------------R.................................  r7 = sext16 r7
    D=eE--------------------------------------R.................................  r7 = r7 << 0x3
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.................................  r8 = u64 [r1 + 0x48]
    .D========================eE--------------R.................................  r7 = r7 + r8
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r8 = u64 [r7 + 0]
    .D..........................................................................  r7 = r6
    .D==================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 116, jump [r8 + 0]
```

Gas simulation at offset 4639 with total cost of 54:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.............................  r8 = u8 [r5 + 0x22e]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.............................  r9 = i16 [r5 + 0x220]
    D=========================eER............................  r7 = r8 << 0x1
    .D========================eER............................  r10 = r8 << 0x3
    .D=========================eER...........................  r7 = r10 - r7
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-R...........................  r10 = u64 [r1 + 0x50]
    ..D=========================eER..........................  r7 = r7 + r10
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  r10 = u16 [r7 + 0x4]
    ..D=======================eE---------------------------R.  r9 = r9 + 0x1
    ..D========================eE--------------------------R.  r11 = zext16 r9
    ...D=======================eeeeeeeeeeeeeeeeeeeeeeeeeE--R.  u16 [r5 + 0x220] = r9
    ...D==================================================eER  jump 4837 if r10 >=u r11
```

Gas simulation at offset 4678 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r9 = i16 [r5 + 0x21e]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r10 = u16 [r7 + 0]
    D=========================eE--------------R...........  r9 = r9 + 0x1
    .D=========================eE-------------R...........  r11 = zext16 r9
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x21e] = r9
    .D==========================eE-----------------------R  jump 4826 if r11 != r10
```

Gas simulation at offset 4698 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r9 = u8 [r5 + 0x22d]
    D=========================eE--------------R.............  r10 = r9 << 0x2
    .DeE--------------------------------------R.............  r7 = 0x17250
    .D=========================eE-------------R.............  r10 = r10 + r7
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  r12 = u8 [r10 + 0x3]
    ..DeE-------------------------------------------------R.  r11 = r8 + 0x1
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R.  u16 [r5 + 542] = 0
    ..D=eeeeeeeeeeeeeeeeeeeeeeeeeE------------------------R.  u8 [r5 + 0x22e] = a4
    ...D=================================================eER  jump 4748 if r8 >=u r12
```

Gas simulation at offset 4731 with total cost of 27:

```
    DeER..........................  r7 = r11 << 0x1
    DeER..........................  r11 = r11 << 0x3
    D=eER.........................  r11 = r11 - r7
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r7 = u64 [r1 + 0x50]
    .D=========================eER  r7 = r7 + r11
    .DeeeeeeeeeeeeeeeE-----------R  jump 4826
```

Gas simulation at offset 4748 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r8 = i16 [r5 + 0x21c]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r11 = u16 [r10 + 0]
    D=========================eE--------------R...........  r8 = r8 + 0x1
    .D=========================eE-------------R...........  r12 = zext16 r8
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x21c] = r8
    .D==========================eeeeeeeeeeeeeeeeeeeeE----R  jump 4802 if r12 != r11
```

Gas simulation at offset 4767 with total cost of 26:

```
    DeER.........................  r8 = r9 + 0x1
    DeER.........................  r10 = 0x7
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  u16 [r5 + 540] = 0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x22d] = a1
    .DeeeeeeeeeeeeeeeeeeeeE-----R  jump 4791 if r9 != r10
```

Gas simulation at offset 4784 with total cost of 25:

```
    DeER........................  r8 = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 557] = 0
    DeeE-----------------------R  fallthrough
```

Gas simulation at offset 4791 with total cost of 27:

```
    DeER..........................  r8 = r8 << 0x2
    D=eER.........................  r7 = r7 + r8
    D==eeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u8 [r7 + 0x2]
    DeeeeeeeeeeeeeeeE------------R  jump 4806
```

Gas simulation at offset 4802 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u8 [r10 + 0x2]
    DeeE-----------------------R  fallthrough
```

Gas simulation at offset 4806 with total cost of 27:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..  u8 [r5 + 0x22e] = a0
    DeE------------------------R..  r8 = r7 << 0x1
    DeE------------------------R..  r7 = r7 << 0x3
    .DeE-----------------------R..  r7 = r7 - r8
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r8 = u64 [r1 + 0x50]
    .D=========================eER  r7 = r7 + r8
    .DeeE------------------------R  fallthrough
```

Gas simulation at offset 4826 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeE---------------------------------------R...........  r7 = r7 + 0x2
    D=eeeeeeeeeeeeeeeeeeeeeeeeeE--------------R...........  r9 = u16 [r7 + 0]
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x220] = r9
    .DeeE------------------------------------------------R  fallthrough
```

Gas simulation at offset 4837 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u8 [r5 + 0x23b]
    D=========================eE--------------R  jump 5068 if r7 == 0
```

Gas simulation at offset 4846 with total cost of 73:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.................................  unlikely
    DeE---------------------------------------R.................................  r7 = sext16 r9
    D=eE--------------------------------------R.................................  r7 = r7 << 0x3
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.................................  r8 = u64 [r1 + 0x48]
    .D========================eE--------------R.................................  r7 = r7 + r8
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r8 = u64 [r7 + 0]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R......................  u8 [r5 + 571] = 0
    .D..........................................................................  r7 = r6
    ..D=================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 118, jump [r8 + 0]
```

Gas simulation at offset 4870 with total cost of 54:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.............................  r8 = u8 [r5 + 0x22e]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.............................  r9 = i16 [r5 + 0x220]
    D=========================eER............................  r7 = r8 << 0x1
    .D========================eER............................  r10 = r8 << 0x3
    .D=========================eER...........................  r7 = r10 - r7
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-R...........................  r10 = u64 [r1 + 0x50]
    ..D=========================eER..........................  r7 = r7 + r10
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  r10 = u16 [r7 + 0x4]
    ..D=======================eE---------------------------R.  r9 = r9 + 0x1
    ..D========================eE--------------------------R.  r11 = zext16 r9
    ...D=======================eeeeeeeeeeeeeeeeeeeeeeeeeE--R.  u16 [r5 + 0x220] = r9
    ...D==================================================eER  jump 5068 if r10 >=u r11
```

Gas simulation at offset 4909 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r9 = i16 [r5 + 0x21e]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r10 = u16 [r7 + 0]
    D=========================eE--------------R...........  r9 = r9 + 0x1
    .D=========================eE-------------R...........  r11 = zext16 r9
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x21e] = r9
    .D==========================eE-----------------------R  jump 5057 if r11 != r10
```

Gas simulation at offset 4929 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r9 = u8 [r5 + 0x22d]
    D=========================eE--------------R.............  r10 = r9 << 0x2
    .DeE--------------------------------------R.............  r7 = 0x17250
    .D=========================eE-------------R.............  r10 = r10 + r7
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  r12 = u8 [r10 + 0x3]
    ..DeE-------------------------------------------------R.  r11 = r8 + 0x1
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R.  u16 [r5 + 542] = 0
    ..D=eeeeeeeeeeeeeeeeeeeeeeeeeE------------------------R.  u8 [r5 + 0x22e] = a4
    ...D=================================================eER  jump 4979 if r8 >=u r12
```

Gas simulation at offset 4962 with total cost of 27:

```
    DeER..........................  r7 = r11 << 0x1
    DeER..........................  r11 = r11 << 0x3
    D=eER.........................  r11 = r11 - r7
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r7 = u64 [r1 + 0x50]
    .D=========================eER  r7 = r7 + r11
    .DeeeeeeeeeeeeeeeE-----------R  jump 5057
```

Gas simulation at offset 4979 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r8 = i16 [r5 + 0x21c]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r11 = u16 [r10 + 0]
    D=========================eE--------------R...........  r8 = r8 + 0x1
    .D=========================eE-------------R...........  r12 = zext16 r8
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x21c] = r8
    .D==========================eeeeeeeeeeeeeeeeeeeeE----R  jump 5033 if r12 != r11
```

Gas simulation at offset 4998 with total cost of 26:

```
    DeER.........................  r8 = r9 + 0x1
    DeER.........................  r10 = 0x7
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  u16 [r5 + 540] = 0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x22d] = a1
    .DeeeeeeeeeeeeeeeeeeeeE-----R  jump 5022 if r9 != r10
```

Gas simulation at offset 5015 with total cost of 25:

```
    DeER........................  r8 = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 557] = 0
    DeeE-----------------------R  fallthrough
```

Gas simulation at offset 5022 with total cost of 27:

```
    DeER..........................  r8 = r8 << 0x2
    D=eER.........................  r7 = r7 + r8
    D==eeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u8 [r7 + 0x2]
    DeeeeeeeeeeeeeeeE------------R  jump 5037
```

Gas simulation at offset 5033 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u8 [r10 + 0x2]
    DeeE-----------------------R  fallthrough
```

Gas simulation at offset 5037 with total cost of 27:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..  u8 [r5 + 0x22e] = a0
    DeE------------------------R..  r8 = r7 << 0x1
    DeE------------------------R..  r7 = r7 << 0x3
    .DeE-----------------------R..  r7 = r7 - r8
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r8 = u64 [r1 + 0x50]
    .D=========================eER  r7 = r7 + r8
    .DeeE------------------------R  fallthrough
```

Gas simulation at offset 5057 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeE---------------------------------------R...........  r7 = r7 + 0x2
    D=eeeeeeeeeeeeeeeeeeeeeeeeeE--------------R...........  r7 = i16 [r7 + 0]
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x220] = r7
    .DeeE------------------------------------------------R  fallthrough
```

Gas simulation at offset 5068 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.......  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r0 = u64 [r1 + 0x70]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r5 = u64 [r1 + 0x68]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r6 = u64 [r1 + 0x60]
    .DeE--------------------------------------R.......  r1 = r1 + 0x78
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 5083 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u8 [r5 + 0x1]
    D=========================eE--------------R  jump 5095 if r7 == 0
```

Gas simulation at offset 5090 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 4] = 0xf
    DeeE-----------------------R  fallthrough
```

Gas simulation at offset 5095 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u8 [r5 + 0x1a]
    D=========================eE--------------R  jump 5123 if r7 == 0
```

Gas simulation at offset 5102 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r7 = u8 [r5 + 0x1b]
    DeE---------------------------------------R...........  r8 = 0xf
    D=========================eE--------------R...........  r7 = r7 + 0x1
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R...........  u8 [r5 + 26] = 0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R...........  u8 [r5 + 0x1c] = a1
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x1d] = a0
    .DeeeeeeeeeeeeeeeE-----------------------------------R  jump 5171
```

Gas simulation at offset 5123 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u8 [r5 + 0x1d]
    D=========================eE--------------R  jump 5138 if r7 == 0
```

Gas simulation at offset 5130 with total cost of 26:

```
    DeER.........................  r7 = r7 + 0xffffffffffffffff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x1d] = a0
    DeeeeeeeeeeeeeeeE-----------R  jump 5171
```

Gas simulation at offset 5138 with total cost of 50:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........  r8 = u8 [r5 + 0x1b]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........  r7 = u8 [r5 + 0x1c]
    D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x1d] = a1
    .D========================eE------------------------R  jump 5159 if r7 == 0
```

Gas simulation at offset 5151 with total cost of 26:

```
    DeER.........................  r7 = r7 + 0xffffffffffffffff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x1c] = a0
    DeeeeeeeeeeeeeeeE-----------R  jump 5171
```

Gas simulation at offset 5159 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u8 [r5 + 0x19]
    D=========================eE--------------R  jump 5171 if r7 == 0
```

Gas simulation at offset 5166 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 28] = 0xf
    DeeE-----------------------R  fallthrough
```

Gas simulation at offset 5171 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u8 [r5 + 0x32]
    D=========================eE--------------R  jump 5199 if r7 == 0
```

Gas simulation at offset 5178 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r7 = u8 [r5 + 0x33]
    DeE---------------------------------------R...........  r8 = 0xf
    D=========================eE--------------R...........  r7 = r7 + 0x1
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R...........  u8 [r5 + 50] = 0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R...........  u8 [r5 + 0x34] = a1
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x35] = a0
    .DeeeeeeeeeeeeeeeE-----------------------------------R  jump 5247
```

Gas simulation at offset 5199 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u8 [r5 + 0x35]
    D=========================eE--------------R  jump 5214 if r7 == 0
```

Gas simulation at offset 5206 with total cost of 26:

```
    DeER.........................  r7 = r7 + 0xffffffffffffffff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x35] = a0
    DeeeeeeeeeeeeeeeE-----------R  jump 5247
```

Gas simulation at offset 5214 with total cost of 50:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........  r8 = u8 [r5 + 0x33]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........  r7 = u8 [r5 + 0x34]
    D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x35] = a1
    .D========================eE------------------------R  jump 5235 if r7 == 0
```

Gas simulation at offset 5227 with total cost of 26:

```
    DeER.........................  r7 = r7 + 0xffffffffffffffff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x34] = a0
    DeeeeeeeeeeeeeeeE-----------R  jump 5247
```

Gas simulation at offset 5235 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u8 [r5 + 0x31]
    D=========================eE--------------R  jump 5247 if r7 == 0
```

Gas simulation at offset 5242 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 52] = 0xf
    DeeE-----------------------R  fallthrough
```

Gas simulation at offset 5247 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u8 [r6 + 0x4]
    D=========================eE--------------R  jump 5338 if r7 == 0
```

Gas simulation at offset 5254 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u8 [r5 + 0xa]
    D=========================eE--------------R  jump 5275 if r7 != 0
```

Gas simulation at offset 5261 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u8 [r5 + 0xc]
    D=========================eE--------------R  jump 5275 if r7 == 0
```

Gas simulation at offset 5268 with total cost of 26:

```
    DeER.........................  r7 = r7 + 0xffffffffffffffff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0xc] = a0
    DeeE------------------------R  fallthrough
```

Gas simulation at offset 5275 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u8 [r5 + 0x22]
    D=========================eE--------------R  jump 5296 if r7 != 0
```

Gas simulation at offset 5282 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u8 [r5 + 0x24]
    D=========================eE--------------R  jump 5296 if r7 == 0
```

Gas simulation at offset 5289 with total cost of 26:

```
    DeER.........................  r7 = r7 + 0xffffffffffffffff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x24] = a0
    DeeE------------------------R  fallthrough
```

Gas simulation at offset 5296 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u8 [r5 + 0x77]
    D=========================eE--------------R  jump 5317 if r7 != 0
```

Gas simulation at offset 5303 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u8 [r5 + 0x79]
    D=========================eE--------------R  jump 5317 if r7 == 0
```

Gas simulation at offset 5310 with total cost of 26:

```
    DeER.........................  r7 = r7 + 0xffffffffffffffff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x79] = a0
    DeeE------------------------R  fallthrough
```

Gas simulation at offset 5317 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u8 [r5 + 0x3c]
    D=========================eE--------------R  jump 5338 if r7 != 0
```

Gas simulation at offset 5324 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u8 [r5 + 0x3e]
    D=========================eE--------------R  jump 5338 if r7 == 0
```

Gas simulation at offset 5331 with total cost of 26:

```
    DeER.........................  r7 = r7 + 0xffffffffffffffff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x3e] = a0
    DeeE------------------------R  fallthrough
```

Gas simulation at offset 5338 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u8 [r6 + 0x3]
    D=========================eE--------------R  jump 5364 if r7 == 0
```

Gas simulation at offset 5345 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u8 [r5 + 0x97]
    D=========================eE--------------R  jump 5364 if r7 != 0
```

Gas simulation at offset 5353 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 152] = 0x1
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 623] = 0x1
    DeeE-----------------------R  fallthrough
```

Gas simulation at offset 5364 with total cost of 50:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........  r7 = u8 [r6 + 0x2]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........  r8 = u64 [r5 + 0x48]
    D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x99] = a0
    .D========================eE------------------------R  jump 5419 if r7 >=u r8
```

Gas simulation at offset 5378 with total cost of 76:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER....................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R....................................  r8 = u64 [r5 + 0x40]
    DeE---------------------------------------R....................................  r7 = r7 << 0x3
    D=========================eE--------------R....................................  r7 = r7 + r8
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r7 = i16 [r7 + 0]
    .D==================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x94] = r7
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------------------------------R  r6 = u64 [r1 + 0x40]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------------------------------R  r8 = u8 [r5 + 0x92]
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------------------------------R  r7 = u8 [r5 + 0x93]
    ..DeE-------------------------------------------------------------------------R  r9 = 0x2
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  u8 [r5 + 0x92] = a2
    ..D========================eE-------------------------------------------------R  jump 3079 if r8 != r9
```

Gas simulation at offset 5416 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 3128
```

Gas simulation at offset 5419 with total cost of 2:

```
    DeeER  trap
```

Gas simulation at offset 5420 with total cost of 27:

```
    DeER..........................  r9 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.  r9 = u8 [r9 + 0x284]
    D==========================eER  jump 5477 if r9 == 0
```

Gas simulation at offset 5431 with total cost of 61:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.....................  unlikely
    DeE---------------------------------------R.....................  r9 = r7 + r8
    D=eE--------------------------------------R.....................  r9 = r9 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeE-------------R.....................  r9 = u8 [r9 + 0x27f]
    .DeE--------------------------------------R.....................  r8 = r8 | 0xa80
    ..D=========================eeeE----------R.....................  r10 = r9 <u 0xc0
    ...D========================eE------------R.....................  r11 = r9 & 0x3f
    ...D===========================eeE--------R.....................  r11 = r9 if r10 != 0
    ....D============================eE-------R.....................  r10 = r11 & 0x30
    ....D============================eE-------R.....................  r9 = r11 & 0xcf
    .....D============================eE------R.....................  r10 = r10 + 0xffffffffffffffd0
    .....D=============================eeE----R.....................  r9 = r11 if r10 != 0
    ......DeE---------------------------------R.....................  r10 = r7 + r8
    ......D==============================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r10 + 0] = a2
    ......DeeeeeeeeeeeeeeeE----------------------------------------R  jump 5487
```

Gas simulation at offset 5477 with total cost of 27:

```
    DeER..........................  r8 = r8 | 0xa80
    D=eER.........................  r9 = r7 + r8
    D==eeeeeeeeeeeeeeeeeeeeeeeeeER  r9 = u8 [r9 + 0]
    .DeeE------------------------R  fallthrough
```

Gas simulation at offset 5487 with total cost of 27:

```
    DeER..........................  r8 = r8 + r7
    DeER..........................  r7 = r9 & 0x1
    DeER..........................  r9 = r9 >> 0x1
    .DeER.........................  r9 = r9 + 0x80
    .DeER.........................  r7 = r7 | 0x40
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r8 + 0] = a2
    .DeeeeeeeeeeeeeeeeeeeeeeE----R  jump [r0 + 0]
```

Gas simulation at offset 5507 with total cost of 29:

```
    DeER............................  r1 = r1 + 0xffffffffffffff90
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0x68] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0x60] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0x58] = r6
    .DeE------------------------R...  r7 = 0x30008
    .D=eE-----------------------R...  r5 = r7 + 0x7ff
    .D==eeeeeeeeeeeeeeeeeeeeeeeeeER.  r8 = u8 [r5 + 0x28b]
    ..D==========================eER  jump 6038 if r8 == 0
```

Gas simulation at offset 5536 with total cost of 76:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER....................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R....................................  r8 = i32 [r5 + 0x25d]
    D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u64 [r1 + 0x48] = r8
    DeE-------------------------------------------------R..........................  r7 = r7 + 0x8
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE------------------------R..........................  u64 [r1 + 0x50] = r7
    .DeE------------------------------------------------R..........................  r7 = 0x10140
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeE-----------------------R..........................  u64 [r1 + 0x30] = r7
    .DeE------------------------------------------------R..........................  r7 = 0x17cd8
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-----------------------R..........................  u64 [r1 + 0x20] = r7
    ..DeE-----------------------------------------------R..........................  r7 = 0x17d18
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u64 [r1 + 0x28] = r7
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER........................  u64 [r1 + 24] = 0xffff
    ...D========================eeeeeeeeeeeeeeeeeeeeeeeeeER........................  u64 [r1 + 16] = 0xfffb
    ...D===============================================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u64 [r1 + 8] = 0xfffe
    ...D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0] = 0xfffa
    ...DeeeeeeeeeeeeeeeE----------------------------------------------------------R  jump 5644
```

Gas simulation at offset 5599 with total cost of 75:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...................................  r7 = u8 [r5 + 0x26e]
    D=========================eE--------------R...................................  r7 = r7 ^ 0x80
    D==========================eE-------------R...................................  r7 = r7 << 0x3
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R...................................  r8 = u64 [r1 + 0x28]
    .D==========================eE------------R...................................  r7 = r7 + r8
    .D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r8 = u64 [r7 + 0]
    .D............................................................................  r7 = r6
    ..D===================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 120, jump [r8 + 0]
```

Gas simulation at offset 5625 with total cost of 2:

```
    DeER.  r8 = r7 & 0x1
    D=eER  jump 6074 if r8 != 0
```

Gas simulation at offset 5632 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = i32 [r5 + 0x25d]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r8 = u64 [r1 + 0x48]
    D=========================eE--------------R  jump 6042 if r7 != r8
```

Gas simulation at offset 5644 with total cost of 50:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........  r8 = u16 [r5 + 0x271]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........  r6 = u8 [r5 + 0x279]
    D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x269] = r8
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE------------------------R  r7 = u64 [r1 + 0x50]
    .DeeeeeeeeeeeeeeeE----------------------------------R  r0 = 122, jump 22578
```

Gas simulation at offset 5665 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x26e] = a0
    DeE------------------------R  jump 5680 if r6 == 0
```

Gas simulation at offset 5672 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u8 [r5 + 0x27a]
    D=========================eE--------------R  jump 5774 if r7 == 0
```

Gas simulation at offset 5680 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u8 [r5 + 0x278]
    D=========================eE--------------R  jump 5699 if r7 == 0
```

Gas simulation at offset 5688 with total cost of 46:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER......  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R......  r7 = u8 [r5 + 0x277]
    D=========================eE--------------R......  r7 = r7 & 0x4
    D==========================eeeeeeeeeeeeeeeeeeeeER  jump 5780 if r7 == 0
```

Gas simulation at offset 5699 with total cost of 1:

```
    DeER  jump 5707 if r6 != 0
```

Gas simulation at offset 5702 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 634] = 0
    DeeE-----------------------R  fallthrough
```

Gas simulation at offset 5707 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r7 = i16 [r5 + 0x271]
    D=========================eE--------------R...........  r7 = r7 + 0x1
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x271] = r7
    .D=========================eE------------------------R  r8 = zext16 r7
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r6 = u64 [r1 + 0x50]
    .D....................................................  r7 = r6
    .DeeeeeeeeeeeeeeeE-----------------------------------R  r0 = 124, jump 22578
```

Gas simulation at offset 5731 with total cost of 76:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...................................................  r8 = u8 [r5 + 0x26e]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...................................................  r9 = u64 [r1 + 0x30]
    D=========================eER..................................................  r8 = r8 + r9
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r8 = i8 [r8 + 0]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R.........................  u8 [r5 + 0x26d] = a0
    .D==================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x26f] = a1
    .D==================================================eE------------------------R  r7 = r8 & 0xff
    ..D=================================================eE------------------------R  jump 5980 if r8 <s 0
```

Gas simulation at offset 5759 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r8 = i16 [r5 + 0x271]
    D=========================eE--------------R...........  r8 = r8 + 0x1
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x271] = r8
    .DeeeeeeeeeeeeeeeE-----------------------------------R  jump 5986
```

Gas simulation at offset 5774 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 634] = 0x1
    DeeE-----------------------R  fallthrough
```

Gas simulation at offset 5780 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = u16 [r5 + 0x271]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0x50]
    D...........................  r7 = r6
    DeeeeeeeeeeeeeeeE----------R  r0 = 126, jump 22578
```

Gas simulation at offset 5794 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r7 = u8 [r5 + 0x277]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r8 = u8 [r5 + 0x276]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r9 = u8 [r5 + 0x272]
    D=========================eER.........................  r7 = r7 & 0xef
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x277] = a0
    .D========================eE-------------------------R  r8 = r8 | 0x100
    .D....................................................  r7 = r6
    .DeeeeeeeeeeeeeeeE-----------------------------------R  r0 = 128, jump 23116
```

Gas simulation at offset 5826 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r7 = u8 [r5 + 0x276]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r9 = u8 [r5 + 0x271]
    D=========================eER.........................  r7 = r7 + 0xffffffffffffffff
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x276] = a0
    .D=========================eE------------------------R  r7 = r7 & 0xff
    .D==========================eE-----------------------R  r8 = r7 | 0x100
    .D....................................................  r7 = r6
    ..DeeeeeeeeeeeeeeeE----------------------------------R  r0 = 130, jump 23116
```

Gas simulation at offset 5857 with total cost of 77:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER....................................................  r7 = u8 [r5 + 0x276]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER....................................................  r11 = u8 [r5 + 0x27a]
    D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER...........................  u64 [r1 + 0x38] = r11
    DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R...........................  r9 = u8 [r5 + 0x277]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE------------------------R...........................  r10 = u64 [r1 + 0x10]
    .D========================eE------------------------R...........................  r7 = r7 + 0xffffffffffffffff
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER...........................  r8 = u64 [r1 + 0x18]
    ..D================================================eeER.........................  r10 = r8 if r11 == 0
    ..D==================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x40] = r10
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R  u8 [r5 + 0x276] = a0
    ...D=======================eE--------------------------------------------------R  r7 = r7 & 0xff
    ...D========================eE-------------------------------------------------R  r8 = r7 | 0x100
    ...D............................................................................  r7 = r6
    ....DeeeeeeeeeeeeeeeE----------------------------------------------------------R  r0 = 132, jump 23116
```

Gas simulation at offset 5907 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER............................  r7 = u8 [r5 + 0x276]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER............................  r8 = u8 [r5 + 0x277]
    D=========================eER...........................  r7 = r7 + 0xffffffffffffffff
    D=========================eER...........................  r8 = r8 | 0x4
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER..  u8 [r5 + 0x276] = a0
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER..  u8 [r5 + 0x277] = a1
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R..  r8 = u64 [r1 + 0]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R..  r7 = u64 [r1 + 0x8]
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..  r9 = u64 [r1 + 0x38]
    ..D=================================================eeER  r8 = r7 if r9 == 0
    ..D.....................................................  r7 = r6
    ...DeeeeeeeeeeeeeeeE-----------------------------------R  r0 = 134, jump 22578
```

Gas simulation at offset 5948 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x271] = a0
    D...........................  r7 = r6
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = u64 [r1 + 0x40]
    DeeeeeeeeeeeeeeeE----------R  r0 = 136, jump 22578
```

Gas simulation at offset 5963 with total cost of 26:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  u8 [r5 + 0x272] = a0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r7 = i32 [r5 + 0x25d]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r8 = u64 [r1 + 0x48]
    D=========================eER  jump 5644 if r7 == r8
```

Gas simulation at offset 5978 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 6042
```

Gas simulation at offset 5980 with total cost of 1:

```
    DeER  jump 5599 if r7 == 128
```

Gas simulation at offset 5986 with total cost of 73:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.................................  unlikely
    DeE---------------------------------------R.................................  r7 = r7 & 0x7
    D=eE--------------------------------------R.................................  r7 = r7 << 0x3
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.................................  r8 = u64 [r1 + 0x20]
    .D========================eE--------------R.................................  r7 = r7 + r8
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r8 = u64 [r7 + 0]
    .D..........................................................................  r7 = r6
    .D==================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 138, jump [r8 + 0]
```

Gas simulation at offset 6008 with total cost of 27:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..  r7 = u8 [r5 + 0x26f]
    D=========================eER.  r7 = r7 & 0x40
    D==========================eER  jump 5599 if r7 == 0
```

Gas simulation at offset 6019 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = u16 [r5 + 0x26b]
    D...........................  r7 = r6
    DeeeeeeeeeeeeeeeE----------R  r0 = 140, jump 22578
```

Gas simulation at offset 6031 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x26d] = a0
    DeeeeeeeeeeeeeeeE----------R  jump 5599
```

Gas simulation at offset 6038 with total cost of 15:

```
    DeER..............  r9 = 0
    DeeeeeeeeeeeeeeeER  jump 6111
```

Gas simulation at offset 6042 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r9 = u16 [r5 + 0x281]
    D=========================eE--------------R  jump 6111 if r9 == 0
```

Gas simulation at offset 6050 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r8 = u16 [r5 + 0x283]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u8 [r5 + 0x285]
    DeE---------------------------------------R  r9 = r9 & 0x1
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R  u16 [r5 + 641] = 0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R  u8 [r5 + 651] = 0
    .D========================eE--------------R  jump 6107 if r9 != 0
```

Gas simulation at offset 6073 with total cost of 2:

```
    DeeER  trap
```

Gas simulation at offset 6074 with total cost of 28:

```
    DeER...........................  r7 = r7 << 0x10
    D=eER..........................  r8 = r7 >> 0x10
    .D=eER.........................  r7 = r8 >> 0x20
    .D=eER.........................  r8 = r8 >> 0x10
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER..  u16 [r5 + 641] = 0
    ..D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x283] = r8
    ..D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x285] = a0
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-R  u8 [r5 + 651] = 0
    ..DeE-------------------------R  r9 = 0x1
    ...DeeeeeeeeeeeeeeeE----------R  jump 6111
```

Gas simulation at offset 6107 with total cost of 2:

```
    DeER.  r9 = 0x1
    DeeER  fallthrough
```

Gas simulation at offset 6111 with total cost of 48:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER........  unlikely
    DeE---------------------------------------R........  r7 = r7 & 0xff
    DeE---------------------------------------R........  r8 = r8 << 0x30
    D=eE--------------------------------------R........  r7 = r7 << 0x20
    .DeE--------------------------------------R........  r8 = r8 >> 0x20
    .D=eE-------------------------------------R........  r7 = r7 | r8
    .D==eE------------------------------------R........  r7 = r7 | r9
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R........  r0 = u64 [r1 + 0x68]
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------R........  r5 = u64 [r1 + 0x60]
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------R........  r6 = u64 [r1 + 0x58]
    ..D==eE-----------------------------------R........  r1 = r1 + 0x70
    ..D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 6145 with total cost of 49:

```
    DeER................................................  r1 = r1 + 0xfffffffffffffff0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.......................  u64 [r1 + 0x8] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.......................  u64 [r1 + 0] = r6
    .DeE------------------------R.......................  r8 = r7 + 0x7ff
    .D=eE-----------------------R.......................  r8 = r8 + 0x1e1
    .D==eeeeeeeeeeeeeeeeeeeeeeeeeER.....................  r6 = u8 [r8 + 0x46]
    ..D==========================eER....................  r10 = r6 & 0x8
    ..D===========================eeeeeeeeeeeeeeeeeeeeER  jump 6186 if r10 != 0
```

Gas simulation at offset 6170 with total cost of 21:

```
    DeER....................  r3 = 0
    DeER....................  r2 = 0
    DeER....................  r9 = r6 & 0x10
    .DeER...................  r4 = 0x1
    .DeeeeeeeeeeeeeeeeeeeeER  jump 6270 if r9 != 0
```

Gas simulation at offset 6183 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 6567
```

Gas simulation at offset 6186 with total cost of 2:

```
    DeER.  r10 = r6 & 0x2
    D=eER  jump 6202 if r10 != 0
```

Gas simulation at offset 6192 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r10 = u16 [r8 + 0x30]
    DeE---------------------------------------R  r11 = 0x8
    D=========================eE--------------R  jump 6170 if r10 <u r11
```

Gas simulation at offset 6202 with total cost of 55:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...............  r10 = u8 [r8 + 0x42]
    DeE---------------------------------------R...............  r11 = 0xf
    .D========================eeE-------------R...............  r10 = r11 & ~r10
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R...............  r11 = u16 [r8 + 0x32]
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------R...............  r12 = u16 [r8 + 0x34]
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------R...............  r9 = u16 [r8 + 0x36]
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER....  r5 = u16 [r8 + 0x38]
    ...D========================eE-----------------------R....  r11 = r11 >> r10
    ...D========================eE-----------------------R....  r12 = r12 >> r10
    ....D=======================eE-----------------------R....  r9 = r9 >> r10
    .....D==============================================eER...  r10 = r5 >> r10
    .....D=======================eE-----------------------R...  r11 = r11 & 0x1
    ......D======================eE-----------------------R...  r9 = r9 & 0x1
    ......D======================eE-----------------------R...  r12 = r12 << 0x1
    ......D==============================================eER..  r10 = r10 << 0x1
    ......D=======================eE-----------------------R..  r12 = r12 & 0x2
    .......D==============================================eER.  r10 = r10 & 0x2
    .......D=======================eE-----------------------R.  r3 = r12 | r11
    ........D==============================================eER  r2 = r10 | r9
    ........D=====================eE-------------------------R  r9 = r6 & 0x10
    .........DeE---------------------------------------------R  r4 = 0x1
    .........D=====================eE------------------------R  jump 6567 if r9 == 0
```

Gas simulation at offset 6270 with total cost of 2:

```
    DeER.  r9 = r6 & 0x4
    D=eER  jump 6287 if r9 != 0
```

Gas simulation at offset 6276 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r9 = u16 [r8 + 0x30]
    DeE---------------------------------------R  r10 = 0x8
    D=========================eE--------------R  jump 6567 if r9 <u r10
```

Gas simulation at offset 6287 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r9 = u8 [r8 + 0x3]
    D=========================eE--------------R  jump 6309 if r9 != 0
```

Gas simulation at offset 6294 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r11 = u8 [r8 + 0]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r10 = u8 [r8 + 0x1]
    .D========================eE--------------R  r9 = r10 | r11
    .D=========================eE-------------R  r9 = sext8 r9
    .D==========================eE------------R  jump 6472 if r9 <s 0
```

Gas simulation at offset 6309 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r9 = u8 [r8 + 0x7]
    D=========================eE--------------R  jump 6332 if r9 != 0
```

Gas simulation at offset 6316 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r11 = u8 [r8 + 0x4]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r10 = u8 [r8 + 0x5]
    .D========================eE--------------R  r9 = r10 | r11
    .D=========================eE-------------R  r9 = sext8 r9
    .D==========================eE------------R  jump 6482 if r9 <s 0
```

Gas simulation at offset 6332 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r9 = u8 [r8 + 0xb]
    D=========================eE--------------R  jump 6355 if r9 != 0
```

Gas simulation at offset 6339 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r11 = u8 [r8 + 0x8]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r10 = u8 [r8 + 0x9]
    .D========================eE--------------R  r9 = r10 | r11
    .D=========================eE-------------R  r9 = sext8 r9
    .D==========================eE------------R  jump 6489 if r9 <s 0
```

Gas simulation at offset 6355 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r9 = u8 [r8 + 0xf]
    D=========================eE--------------R  jump 6377 if r9 != 0
```

Gas simulation at offset 6362 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r11 = u8 [r8 + 0xc]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r10 = u8 [r8 + 0xd]
    .D========================eE--------------R  r9 = r10 | r11
    .D=========================eE-------------R  r9 = sext8 r9
    .D==========================eE------------R  jump 6496 if r9 <s 0
```

Gas simulation at offset 6377 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r9 = u8 [r8 + 0x13]
    D=========================eE--------------R  jump 6399 if r9 != 0
```

Gas simulation at offset 6384 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r11 = u8 [r8 + 0x10]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r10 = u8 [r8 + 0x11]
    .D========================eE--------------R  r9 = r10 | r11
    .D=========================eE-------------R  r9 = sext8 r9
    .D==========================eE------------R  jump 6503 if r9 <s 0
```

Gas simulation at offset 6399 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r9 = u8 [r8 + 0x17]
    D=========================eE--------------R  jump 6421 if r9 != 0
```

Gas simulation at offset 6406 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r11 = u8 [r8 + 0x14]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r10 = u8 [r8 + 0x15]
    .D========================eE--------------R  r9 = r10 | r11
    .D=========================eE-------------R  r9 = sext8 r9
    .D==========================eE------------R  jump 6510 if r9 <s 0
```

Gas simulation at offset 6421 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r9 = u8 [r8 + 0x1b]
    D=========================eE--------------R  jump 6443 if r9 != 0
```

Gas simulation at offset 6428 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r11 = u8 [r8 + 0x18]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r10 = u8 [r8 + 0x19]
    .D========================eE--------------R  r9 = r10 | r11
    .D=========================eE-------------R  r9 = sext8 r9
    .D==========================eE------------R  jump 6517 if r9 <s 0
```

Gas simulation at offset 6443 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r9 = u8 [r8 + 0x1f]
    D=========================eE--------------R  jump 6567 if r9 != 0
```

Gas simulation at offset 6450 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r11 = u8 [r8 + 0x1c]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r10 = u8 [r8 + 0x1d]
    .D========================eE--------------R  r9 = r10 | r11
    .D=========================eE-------------R  r9 = sext8 r9
    .D==========================eE------------R  jump 6567 if r9 >=s 0
```

Gas simulation at offset 6465 with total cost of 15:

```
    DeER..............  r4 = 0
    DeER..............  r12 = r8 + 0x1c
    DeeeeeeeeeeeeeeeER  jump 6523
```

Gas simulation at offset 6472 with total cost of 15:

```
    DeER..............  r4 = 0x1000000
    D.................  r12 = r8
    DeeeeeeeeeeeeeeeER  jump 6523
```

Gas simulation at offset 6482 with total cost of 15:

```
    DeER..............  r4 = 0
    DeER..............  r12 = r8 + 0x4
    DeeeeeeeeeeeeeeeER  jump 6523
```

Gas simulation at offset 6489 with total cost of 15:

```
    DeER..............  r4 = 0
    DeER..............  r12 = r8 + 0x8
    DeeeeeeeeeeeeeeeER  jump 6523
```

Gas simulation at offset 6496 with total cost of 15:

```
    DeER..............  r4 = 0
    DeER..............  r12 = r8 + 0xc
    DeeeeeeeeeeeeeeeER  jump 6523
```

Gas simulation at offset 6503 with total cost of 15:

```
    DeER..............  r4 = 0
    DeER..............  r12 = r8 + 0x10
    DeeeeeeeeeeeeeeeER  jump 6523
```

Gas simulation at offset 6510 with total cost of 15:

```
    DeER..............  r4 = 0
    DeER..............  r12 = r8 + 0x14
    DeeeeeeeeeeeeeeeER  jump 6523
```

Gas simulation at offset 6517 with total cost of 2:

```
    DeER.  r4 = 0
    DeER.  r12 = r8 + 0x18
    DeeER  fallthrough
```

Gas simulation at offset 6523 with total cost of 31:

```
    DeER..............................  r11 = r11 >> 0x7
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......  r9 = u8 [r12 + 0x2]
    DeE------------------------R......  r10 = r10 >> 0x6
    D=eE-----------------------R......  r10 = r10 & 0x2
    .D=eE----------------------R......  r10 = r10 | r11
    .D========================eER.....  r11 = r9 & 0x3
    .D========================eER.....  r9 = r9 << 0x3a
    ..D========================eER....  r11 = r11 << 0x8
    ..D========================eER....  r9 = r9 >> 0x3f
    ..D=eE-----------------------R....  r10 = r10 << 0x10
    ..D=========================eER...  r11 = r11 | r4
    ...D=========================eER..  r9 = r9 | r11
    ...D==========================eER.  r9 = r9 | r10
    ...D===========================eER  r4 = r9 | 0x400
    ....DeeE-------------------------R  fallthrough
```

Gas simulation at offset 6567 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r9 = u16 [r8 + 0x30]
    D=========================eE--------------R  jump 6651 if r9 == 255
```

Gas simulation at offset 6576 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r9 = u16 [r8 + 0x2e]
    D=========================eE--------------R  jump 6651 if r9 == 0
```

Gas simulation at offset 6583 with total cost of 4:

```
    DeeER..  i32 r11 = r4 >> 0x10
    .D=eER.  r12 = r11 & 0xff
    ..DeeER  i32 r10 = r4 >> 0x8
    ..D=eER  jump 6627 if r12 == 0
```

Gas simulation at offset 6596 with total cost of 46:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER......  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R......  r9 = u8 [r8 + 0x5d]
    D=========================eE--------------R......  r9 = r9 & 0x1
    D==========================eeeeeeeeeeeeeeeeeeeeER  jump 6627 if r9 == 0
```

Gas simulation at offset 6606 with total cost of 20:

```
    DeeeeeeeeeeeeeeeeeeeeER  jump 6644 if r3 == 0
```

Gas simulation at offset 6609 with total cost of 3:

```
    DeeER.  i32 r9 = r4 >> 0x18
    D==eER  jump 6633 if r9 == 0
```

Gas simulation at offset 6615 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r9 = u8 [r8 + 0x47]
    D=========================eE--------------R...........  r9 = r9 | 0x40
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r8 + 0x47] = a2
    .DeeeeeeeeeeeeeeeE-----------------------------------R  jump 6633
```

Gas simulation at offset 6627 with total cost of 20:

```
    DeeeeeeeeeeeeeeeeeeeeER  jump 6644 if r3 == 0
```

Gas simulation at offset 6630 with total cost of 1:

```
    DeER  jump 6651 if r12 == 0
```

Gas simulation at offset 6633 with total cost of 16:

```
    DeER...............  r9 = r4 & 0x1
    D=eeER.............  r3 = r11 if r9 == 0
    .DeeER.............  r2 = r10 if r9 == 0
    .DeeeeeeeeeeeeeeeER  jump 6651
```

Gas simulation at offset 6644 with total cost of 3:

```
    DeeER.  r10 = 0 if r12 == 0
    D.....  r3 = r11
    .D....  r2 = r10
    .DeeER  fallthrough
```

Gas simulation at offset 6651 with total cost of 56:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER................  unlikely
    DeE---------------------------------------R................  r2 = r2 << 0x2
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R................  r9 = u64 [r8 + 0x20]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R................  r10 = u16 [r8 + 0x2c]
    .DeE--------------------------------------R................  r2 = r2 + r3
    .D=eE-------------------------------------R................  r11 = r2 & 0x1f
    .D==eE------------------------------------R................  r7 = r7 + r11
    ..D=======================eE--------------R................  r11 = r10 << 0x1
    ..D========================eE-------------R................  r9 = r9 + r11
    ..D==eE-----------------------------------R................  r7 = r7 + 0x7ff
    ...D==eeeeeeeeeeeeeeeeeeeeeeeeeE----------R................  r7 = u8 [r7 + 0x1a1]
    ...DeE------------------------------------R................  r6 = r6 << 0x1
    ...D=eE-----------------------------------R................  r11 = r6 & 0x1c0
    ....D=====================eE--------------R................  r10 = r10 + 0x1
    ....D==========================eE---------R................  r7 = r7 | r11
    ....D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r9 + 0] = r7
    ....D======================eeeeeeeeeeeeeeeeeeeeeeeeeE-----R  u16 [r8 + 0x2c] = r10
    .....DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R  r5 = u64 [r1 + 0x8]
    .....D======================eeeeeeeeeeeeeeeeeeeeeeeeeE----R  r6 = u64 [r1 + 0]
    .....D=========================eE-------------------------R  r1 = r1 + 0x10
    .....DeeeeeeeeeeeeeeeeeeeeeeE-----------------------------R  jump [r0 + 0]
```

Gas simulation at offset 6712 with total cost of 30:

```
    DeER.............................  r1 = r1 + 0xfffffffffffffff0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER....  u64 [r1 + 0x8] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER....  u64 [r1 + 0] = r5
    .DeE------------------------R....  r5 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  r10 = u16 [r5 + 0x209]
    ..D=========================eER..  r7 = r10 << 0x32
    ..D==========================eER.  r11 = r7 >> 0x3a
    ...DeE-------------------------R.  r12 = 0x3f
    ...D.............................  r9 = r8
    ...D==========================eER  jump 6779 if r11 >=u r12
```

Gas simulation at offset 6742 with total cost of 74:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r10 = u64 [r5 + 0x241]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r8 = u64 [r5 + 0x249]
    DeE---------------------------------------R..................................  r11 = 0x17c80
    .D========================eeE-------------R..................................  r11 = r8 if r10 != 0
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r11 = u64 [r11 + 0x50]
    ..DeE-------------------------------------------------R......................  r8 = r7 >> 0x32
    ..DeE-------------------------------------------------R......................  r7 = r5 + 0x27f
    ...D======================eeE-------------------------R......................  r7 = r10 if r10 != 0
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 142, jump [r11 + 0]
```

Gas simulation at offset 6777 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 6820
```

Gas simulation at offset 6779 with total cost of 28:

```
    DeER...........................  r11 = r10 & 0x1f
    DeER...........................  r7 = r9 & 0x3f
    .DeER..........................  r8 = r5 + 0x1a1
    .D=eER.........................  r9 = r8 + r11
    ..DeER.........................  r10 = r10 & 0x3
    ..D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r9 + 0] = a0
    ..D=eE------------------------R  jump 6820 if r10 != 0
```

Gas simulation at offset 6800 with total cost of 32:

```
    DeeeER.............................  r9 = r11 <u 0x10
    .DeE-R.............................  r10 = r11 + 0xfffffffffffffff0
    .DeE-R.............................  r11 = r11 | 0x10
    ..D=eeER...........................  r11 = r10 if r9 == 0
    ..D===eER..........................  r9 = zext16 r11
    ..D====eER.........................  r8 = r8 + r9
    ...D====eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r8 + 0] = a0
    ...DeeE---------------------------R  fallthrough
```

Gas simulation at offset 6820 with total cost of 56:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R................  r7 = u8 [r5 + 0x226]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R................  r8 = i16 [r5 + 0x209]
    DeE---------------------------------------R................  r9 = 0x20
    .D========================eE--------------R................  r7 = r7 & 0x4
    .DeE--------------------------------------R................  r10 = 0x1
    .D=========================eeE------------R................  r10 = r9 if r7 != 0
    ..D==========================eE-----------R................  r8 = r8 + r10
    ..D===========================eE----------R................  r8 = r8 << 0x31
    ..D============================eE---------R................  r8 = r8 >> 0x31
    ..D=============================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x209] = r8
    ...DeeeeeeeeeeeeeeeeeeeeeeeeeE----------------------------R  r0 = u64 [r1 + 0x8]
    ...DeeeeeeeeeeeeeeeeeeeeeeeeeE----------------------------R  r5 = u64 [r1 + 0]
    ...D======================eE------------------------------R  r1 = r1 + 0x10
    ...D=========================eeeeeeeeeeeeeeeeeeeeeeE------R  jump [r0 + 0]
```

Gas simulation at offset 6864 with total cost of 27:

```
    DeER..........................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.  r9 = u8 [r7 + 0x23a]
    D==========================eER  jump 6919 if r9 == 0
```

Gas simulation at offset 6875 with total cost of 53:

```
    DeER....................................................  r10 = r8 & 0x7
    DeER....................................................  r8 = r8 << 0x2
    D=eER...................................................  r10 = r10 << 0xc
    .DeER...................................................  r11 = r8 & 0xe0
    .D=eER..................................................  r10 = r10 | r11
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................  r11 = u16 [r7 + 0x20b]
    ..DeE-----------------------R...........................  r8 = r8 & 0x300
    ..D=eE----------------------R...........................  r8 = r8 | r10
    ..D========================eER..........................  r10 = r11 & 0xc1f
    ...D========================eER.........................  r8 = r8 | r10
    ...D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r7 + 0x20b] = r8
    ...DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  u8 [r7 + 570] = 0
    ...DeeeeeeeeeeeeeeeeeeeeeeE----------------------------R  jump [r0 + 0]
```

Gas simulation at offset 6919 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  r9 = u16 [r7 + 0x20b]
    D=========================eE--------------R............  r9 = r9 & 0x7fe0
    .DeE--------------------------------------R............  r10 = r8 & 0x7
    .DeE--------------------------------------R............  r8 = r8 >> 0x3
    .D=========================eE-------------R............  r8 = r8 | r9
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r7 + 0x20b] = r8
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  u8 [r7 + 0x223] = a3
    ..DeE-------------------------------------------------R  r9 = 0x1
    ..D=eeeeeeeeeeeeeeeeeeeeeeeeeE------------------------R  u8 [r7 + 0x23a] = a2
    ...DeeeeeeeeeeeeeeeeeeeeeeE---------------------------R  jump [r0 + 0]
```

Gas simulation at offset 6954 with total cost of 27:

```
    DeER..........................  r8 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.  r9 = u8 [r8 + 0x23d]
    D==========================eER  jump 7007 if r9 == 0
```

Gas simulation at offset 6965 with total cost of 77:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.....................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.....................................  r9 = u8 [r8 + 0x230]
    D=========================eE--------------R.....................................  r7 = r7 + r9
    D==========================eE-------------R.....................................  r7 = r7 + 0x7ff
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r7 = u8 [r7 + 0xa1]
    .D========================eE--------------------------R.........................  r9 = r9 + 0x1
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R.........................  u8 [r8 + 0x230] = a2
    .D===================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r8 + 0x232] = a0
    ..DeeE-------------------------------------------------------------------------R  fallthrough
```

Gas simulation at offset 6993 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r7 = u8 [r8 + 0x23d]
    D=========================eE--------------R...........  r7 = r7 ^ 0x1
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r8 + 0x23d] = a0
    .DeeeeeeeeeeeeeeeeeeeeeeE----------------------------R  jump [r0 + 0]
```

Gas simulation at offset 7007 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r9 = u8 [r8 + 0x237]
    D=========================eE--------------R  jump 7088 if r9 == 0
```

Gas simulation at offset 7015 with total cost of 2:

```
    DeER.  r10 = 0x1
    D=eER  jump 6993 if r9 != r10
```

Gas simulation at offset 7021 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  r9 = u8 [r8 + 0x231]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  r10 = u8 [r8 + 0x232]
    D=========================eE--------------R............  r7 = r7 + r9
    .D=========================eE-------------R............  r7 = r7 + 0x7ff
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x1c1] = a3
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R  r7 = u8 [r8 + 0x231]
    .D=========================eE-------------------------R  r7 = r7 + 0x1
    ..D=========================eE------------------------R  r9 = r7 & 0x3
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r8 + 0x231] = a0
    ..D==========================eE-----------------------R  jump 6993 if r9 != 0
```

Gas simulation at offset 7058 with total cost of 2:

```
    DeER.  r7 = r7 & 0xff
    DeER.  r9 = 0x20
    D=eER  jump 7218 if r7 != r9
```

Gas simulation at offset 7069 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  u8 [r8 + 567] = 0x2
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r7 = u8 [r8 + 0x23d]
    D=========================eE--------------R...........  r7 = r7 ^ 0x1
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r8 + 0x23d] = a0
    .DeeeeeeeeeeeeeeeeeeeeeeE----------------------------R  jump [r0 + 0]
```

Gas simulation at offset 7088 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  r10 = u8 [r8 + 0x231]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  r9 = u8 [r8 + 0x232]
    D=========================eE--------------R............  r7 = r7 + r10
    .D=========================eE-------------R............  r7 = r7 + 0x7ff
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x1c1] = a2
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R  r10 = u8 [r8 + 0x226]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R  r7 = u16 [r8 + 0x20f]
    ..D========================eE-------------------------R  r10 = r10 & 0x20
    ..D=========================eeeeeeeeeeeeeeeeeeeeE-----R  jump 7133 if r10 != 0
```

Gas simulation at offset 7122 with total cost of 20:

```
    DeeeeeeeeeeeeeeeeeeeeER  jump 7194 if r7 <u r9
```

Gas simulation at offset 7125 with total cost of 2:

```
    DeER.  r9 = r9 + 0x8
    D=eER  jump 7142 if r7 <u r9
```

Gas simulation at offset 7131 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 7194
```

Gas simulation at offset 7133 with total cost of 20:

```
    DeeeeeeeeeeeeeeeeeeeeER  jump 7194 if r7 <u r9
```

Gas simulation at offset 7136 with total cost of 2:

```
    DeER.  r9 = r9 + 0x10
    D=eER  jump 7194 if r7 >=u r9
```

Gas simulation at offset 7142 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u8 [r8 + 0x231]
    D=========================eE--------------R  jump 7166 if r7 != 0
```

Gas simulation at offset 7150 with total cost of 54:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..............  r9 = u8 [r8 + 0x230]
    D=========================eE--------------R..............  r9 = r9 + 0xffffffffffffffff
    .D=========================eeeE-----------R..............  r9 = r9 <u 0x1
    .D============================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r8 + 0x23f] = a2
    ..DeeE--------------------------------------------------R  fallthrough
```

Gas simulation at offset 7166 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeE---------------------------------------R............  r9 = 0x1
    D=eE--------------------------------------R............  r7 = r7 + r9
    D==eeeeeeeeeeeeeeeeeeeeeeeeeE-------------R............  u8 [r8 + 0x231] = a0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R............  u8 [r8 + 0x237] = a2
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R............  r7 = u8 [r8 + 0x23d]
    .D=========================eE-------------R............  r7 = r7 ^ r9
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r8 + 0x23d] = a0
    ..DeeeeeeeeeeeeeeeeeeeeeeE----------------------------R  jump [r0 + 0]
```

Gas simulation at offset 7194 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r7 = u8 [r8 + 0x230]
    D=========================eER.........................  r7 = r7 + 0x3
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r8 + 0x230] = a0
    DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R  r7 = u8 [r8 + 0x23d]
    .D========================eE-------------------------R  r7 = r7 ^ 0x1
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r8 + 0x23d] = a0
    .DeeeeeeeeeeeeeeeeeeeeeeE----------------------------R  jump [r0 + 0]
```

Gas simulation at offset 7218 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  u8 [r8 + 567] = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r7 = u8 [r8 + 0x23d]
    D=========================eE--------------R...........  r7 = r7 ^ 0x1
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r8 + 0x23d] = a0
    .DeeeeeeeeeeeeeeeeeeeeeeE----------------------------R  jump [r0 + 0]
```

Gas simulation at offset 7236 with total cost of 27:

```
    DeER..........................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.  r8 = u8 [r7 + 0x1e4]
    D==========================eER  jump 7368 if r8 == 0
```

Gas simulation at offset 7247 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeE---------------------------------------R  r8 = r8 + 0xffffffffffffffff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeE--------------R  u8 [r7 + 0x1e4] = a1
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r8 = u8 [r7 + 0x1e8]
    .D========================eE--------------R  jump 7399 if r8 == 0
```

Gas simulation at offset 7263 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeE---------------------------------------R  r8 = r8 + 0xffffffffffffffff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeE--------------R  u8 [r7 + 0x1e8] = a1
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r8 = u8 [r7 + 0x1ec]
    .D========================eE--------------R  jump 7430 if r8 == 0
```

Gas simulation at offset 7279 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeE---------------------------------------R  r8 = r8 + 0xffffffffffffffff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeE--------------R  u8 [r7 + 0x1ec] = a1
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r8 = u8 [r7 + 0x1f0]
    .D========================eE--------------R  jump 7461 if r8 == 0
```

Gas simulation at offset 7295 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeE---------------------------------------R  r8 = r8 + 0xffffffffffffffff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeE--------------R  u8 [r7 + 0x1f0] = a1
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r8 = u8 [r7 + 0x1f4]
    .D========================eE--------------R  jump 7492 if r8 == 0
```

Gas simulation at offset 7311 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeE---------------------------------------R  r8 = r8 + 0xffffffffffffffff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeE--------------R  u8 [r7 + 0x1f4] = a1
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r8 = u8 [r7 + 0x1f8]
    .D========================eE--------------R  jump 7523 if r8 == 0
```

Gas simulation at offset 7327 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeE---------------------------------------R  r8 = r8 + 0xffffffffffffffff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeE--------------R  u8 [r7 + 0x1f8] = a1
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r8 = u8 [r7 + 0x1fc]
    .D========================eE--------------R  jump 7554 if r8 == 0
```

Gas simulation at offset 7343 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeE---------------------------------------R  r8 = r8 + 0xffffffffffffffff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeE--------------R  u8 [r7 + 0x1fc] = a1
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r8 = u8 [r7 + 0x200]
    .D========================eE--------------R  jump 7585 if r8 == 0
```

Gas simulation at offset 7359 with total cost of 26:

```
    DeER.........................  r8 = r8 + 0xffffffffffffffff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x200] = a1
    DeeeeeeeeeeeeeeeeeeeeeeE----R  jump [r0 + 0]
```

Gas simulation at offset 7368 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r8 = u8 [r7 + 0x1e1]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r9 = u8 [r7 + 0x1e2]
    D=========================eE--------------R...........  r8 = r8 << 0x1
    .D========================eE--------------R...........  r9 = r9 << 0x1
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x1e1] = a1
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x1e2] = a2
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r8 = u8 [r7 + 0x1e8]
    ..D========================eE------------------------R  jump 7263 if r8 != 0
```

Gas simulation at offset 7399 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r8 = u8 [r7 + 0x1e5]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r9 = u8 [r7 + 0x1e6]
    D=========================eE--------------R...........  r8 = r8 << 0x1
    .D========================eE--------------R...........  r9 = r9 << 0x1
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x1e5] = a1
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x1e6] = a2
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r8 = u8 [r7 + 0x1ec]
    ..D========================eE------------------------R  jump 7279 if r8 != 0
```

Gas simulation at offset 7430 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r8 = u8 [r7 + 0x1e9]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r9 = u8 [r7 + 0x1ea]
    D=========================eE--------------R...........  r8 = r8 << 0x1
    .D========================eE--------------R...........  r9 = r9 << 0x1
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x1e9] = a1
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x1ea] = a2
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r8 = u8 [r7 + 0x1f0]
    ..D========================eE------------------------R  jump 7295 if r8 != 0
```

Gas simulation at offset 7461 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r8 = u8 [r7 + 0x1ed]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r9 = u8 [r7 + 0x1ee]
    D=========================eE--------------R...........  r8 = r8 << 0x1
    .D========================eE--------------R...........  r9 = r9 << 0x1
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x1ed] = a1
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x1ee] = a2
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r8 = u8 [r7 + 0x1f4]
    ..D========================eE------------------------R  jump 7311 if r8 != 0
```

Gas simulation at offset 7492 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r8 = u8 [r7 + 0x1f1]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r9 = u8 [r7 + 0x1f2]
    D=========================eE--------------R...........  r8 = r8 << 0x1
    .D========================eE--------------R...........  r9 = r9 << 0x1
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x1f1] = a1
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x1f2] = a2
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r8 = u8 [r7 + 0x1f8]
    ..D========================eE------------------------R  jump 7327 if r8 != 0
```

Gas simulation at offset 7523 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r8 = u8 [r7 + 0x1f5]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r9 = u8 [r7 + 0x1f6]
    D=========================eE--------------R...........  r8 = r8 << 0x1
    .D========================eE--------------R...........  r9 = r9 << 0x1
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x1f5] = a1
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x1f6] = a2
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r8 = u8 [r7 + 0x1fc]
    ..D========================eE------------------------R  jump 7343 if r8 != 0
```

Gas simulation at offset 7554 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r8 = u8 [r7 + 0x1f9]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r9 = u8 [r7 + 0x1fa]
    D=========================eE--------------R...........  r8 = r8 << 0x1
    .D========================eE--------------R...........  r9 = r9 << 0x1
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x1f9] = a1
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x1fa] = a2
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r8 = u8 [r7 + 0x200]
    ..D========================eE------------------------R  jump 7359 if r8 != 0
```

Gas simulation at offset 7585 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r8 = u8 [r7 + 0x1fd]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r9 = u8 [r7 + 0x1fe]
    D=========================eE--------------R...........  r8 = r8 << 0x1
    .D========================eE--------------R...........  r9 = r9 << 0x1
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x1fd] = a1
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x1fe] = a2
    .DeeeeeeeeeeeeeeeeeeeeeeE----------------------------R  jump [r0 + 0]
```

Gas simulation at offset 7610 with total cost of 77:

```
    DeER............................................................................  r1 = r1 + 0xfffffffffffffff0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...................................................  u64 [r1 + 0x8] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...................................................  u64 [r1 + 0] = r5
    .DeE------------------------R...................................................  r5 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  r9 = u8 [r5 + 0x227]
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  r10 = u8 [r5 + 0x23f]
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u8 [r5 + 560] = 0
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u8 [r5 + 561] = 0
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u8 [r5 + 567] = 0
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u8 [r5 + 573] = 0x1
    ...D================================================eER.........................  r9 = r9 & 0x10
    ...D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u8 [r5 + 0x23e] = a3
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 575] = 0
    ...D=================================================eeeeeeeeeeeeeeeeeeeeE-----R  jump 7666 if r9 == 0
```

Gas simulation at offset 7661 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 548] = 0
    DeeE-----------------------R  fallthrough
```

Gas simulation at offset 7666 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 525] = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 566] = 0
    DeeeeeeeeeeeeeeeE----------R  r0 = 146, jump 6145
```

Gas simulation at offset 7680 with total cost of 98:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.........................................................................  r7 = i16 [r5 + 0x211]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.........................................................................  r8 = i16 [r5 + 0x213]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.........................................................................  r9 = i16 [r5 + 0x215]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.........................................................................  r10 = i16 [r5 + 0x217]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER................................................  r11 = i16 [r5 + 0x219]
    .D========================eE------------------------R................................................  r8 = r8 << 0x1
    .D========================eE------------------------R................................................  r9 = r9 << 0x1
    .D========================eE------------------------R................................................  r10 = r10 << 0x1
    ..D========================eE-----------------------R................................................  r7 = r7 + 0x1
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER..............................................  u16 [r5 + 0x211] = r7
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R..............................................  u16 [r5 + 0x213] = r8
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R..............................................  u16 [r5 + 0x215] = r9
    ...D===============================================eeeeeeeeeeeeeeeeeeeeeeeeeER.......................  u16 [r5 + 0x217] = r10
    ...D================================================eE-----------------------R.......................  r11 = r11 << 0x1
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.....................  u16 [r5 + 0x219] = r11
    ...D================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-R.....................  r0 = u64 [r1 + 0x8]
    ....D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.....................  r5 = u64 [r1 + 0]
    ....D=======================================================================eE-R.....................  r1 = r1 + 0x10
    ....D========================================================================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 7745 with total cost of 28:

```
    DeER...........................  r1 = r1 + 0xffffffffffffffe8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0x10] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0x8] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0] = r6
    .D.............................  r5 = r7
    .DeE------------------------R..  r6 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER.  r8 = u8 [r6 + 0x23d]
    ..D=========================eER  jump 7773 if r8 == 0
```

Gas simulation at offset 7769 with total cost of 15:

```
    DeER..............  r8 = 0
    DeeeeeeeeeeeeeeeER  jump 7812
```

Gas simulation at offset 7773 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r8 = u8 [r6 + 0x231]
    D=========================eE--------------R.............  r8 = r8 + r5
    D==========================eE-------------R.............  r8 = r8 + 0x7ff
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u8 [r8 + 449] = 0xffffffffffffffff
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R.  r8 = u8 [r6 + 0x231]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R.  r9 = u8 [r6 + 0x23d]
    .D=========================eE-------------------------R.  r8 = r8 + 0x1
    ..D=========================eE------------------------R.  r8 = r8 & 0x1f
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x231] = a1
    ..D========================eE--------------------------R  r8 = r9 ^ 0x1
    ...DeeE------------------------------------------------R  fallthrough
```

Gas simulation at offset 7812 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER............................  r9 = u16 [r6 + 0x209]
    DeE------------------------R............................  r10 = 0x2000
    D=========================eER...........................  r9 = r9 << 0x34
    D==========================eER..........................  r9 = r9 >> 0x34
    .D==========================eER.........................  r9 = r9 | r10
    .DeE--------------------------R.........................  r8 = r8 & 0x1
    .D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r6 + 0x21b] = r9
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R  u8 [r6 + 0x23d] = a1
    ..D.....................................................  r7 = r5
    ..DeeeeeeeeeeeeeeeE------------------------------------R  r0 = 150, jump 7236
```

Gas simulation at offset 7848 with total cost of 15:

```
    D.................  r7 = r5
    DeeeeeeeeeeeeeeeER  r0 = 152, jump 6145
```

Gas simulation at offset 7856 with total cost of 100:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r7 = i16 [r6 + 0x211]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r8 = i16 [r6 + 0x213]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r9 = i16 [r6 + 0x215]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r10 = i16 [r6 + 0x217]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  r11 = i16 [r6 + 0x219]
    .D========================eE------------------------R..................................................  r8 = r8 << 0x1
    .D========================eE------------------------R..................................................  r9 = r9 << 0x1
    .D========================eE------------------------R..................................................  r10 = r10 << 0x1
    ..D========================eE-----------------------R..................................................  r7 = r7 + 0x1
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER................................................  u16 [r6 + 0x211] = r7
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R................................................  u16 [r6 + 0x213] = r8
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R................................................  u16 [r6 + 0x215] = r9
    ...D===============================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u16 [r6 + 0x217] = r10
    ...D================================================eE-----------------------R.........................  r11 = r11 << 0x1
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.......................  u16 [r6 + 0x219] = r11
    ...D================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-R.......................  r0 = u64 [r1 + 0x10]
    ....D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.......................  r5 = u64 [r1 + 0x8]
    ....D=======================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0]
    ....D========================================================================eE-----------------------R  r1 = r1 + 0x18
    ....D========================================================================eeeeeeeeeeeeeeeeeeeeeeE--R  jump [r0 + 0]
```

Gas simulation at offset 7924 with total cost of 28:

```
    DeER...........................  r1 = r1 + 0xffffffffffffffe8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0x10] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0x8] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0] = r6
    .D.............................  r5 = r7
    .DeE------------------------R..  r6 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER.  r7 = u8 [r6 + 0x23d]
    ..D=========================eER  jump 7982 if r7 == 0
```

Gas simulation at offset 7948 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r8 = u16 [r6 + 0x21b]
    D=========================eE--------------R  r9 = r8 >> 0x8
    .DeE--------------------------------------R  r10 = 0x3f
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R  u8 [r6 + 573] = 0
    .D=========================eE-------------R  jump 8040 if r9 <u r10
```

Gas simulation at offset 7966 with total cost of 28:

```
    DeER...........................  r8 = r8 & 0x1f
    D=eER..........................  r8 = r8 + r5
    D==eER.........................  r7 = r8 + 0x7ff
    .D==eeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u8 [r7 + 0x1a1]
    .DeeeeeeeeeeeeeeeE------------R  jump 8072
```

Gas simulation at offset 7982 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r7 = u8 [r6 + 0x231]
    D=========================eE--------------R.............  r7 = r7 + r5
    D==========================eE-------------R.............  r7 = r7 + 0x7ff
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u8 [r7 + 449] = 0xffffffffffffffff
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R.  r7 = u8 [r6 + 0x231]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R.  r8 = u8 [r6 + 0x23d]
    .D=========================eE-------------------------R.  r7 = r7 + 0x1
    ..D=========================eE------------------------R.  r7 = r7 & 0x1f
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x231] = a0
    ..D========================eE--------------------------R  r7 = r8 ^ 0x1
    ...DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r8 = u16 [r6 + 0x21b]
    ...D========================eE-------------------------R  r7 = r7 & 0x1
    ...D=========================eE------------------------R  r9 = r8 >> 0x8
    ....DeE------------------------------------------------R  r10 = 0x3f
    ....D========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x23d] = a0
    ....D=========================eE-----------------------R  jump 7966 if r9 >=u r10
```

Gas simulation at offset 8040 with total cost of 74:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r9 = u64 [r6 + 0x241]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r7 = u64 [r6 + 0x249]
    DeE---------------------------------------R..................................  r10 = 0x17c80
    .D========================eeE-------------R..................................  r10 = r7 if r9 != 0
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r10 = u64 [r10 + 0x48]
    ..DeE-------------------------------------------------R......................  r7 = r6 + 0x27f
    ..D=======================eeE-------------------------R......................  r7 = r9 if r9 != 0
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 156, jump [r10 + 0]
```

Gas simulation at offset 8072 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x22a] = a0
    D...........................  r7 = r5
    DeeeeeeeeeeeeeeeE----------R  r0 = 158, jump 7236
```

Gas simulation at offset 8084 with total cost of 15:

```
    D.................  r7 = r5
    DeeeeeeeeeeeeeeeER  r0 = 160, jump 6145
```

Gas simulation at offset 8092 with total cost of 100:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r7 = i16 [r6 + 0x211]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r8 = i16 [r6 + 0x213]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r9 = i16 [r6 + 0x215]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r10 = i16 [r6 + 0x217]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  r11 = i16 [r6 + 0x219]
    .D========================eE------------------------R..................................................  r8 = r8 << 0x1
    .D========================eE------------------------R..................................................  r9 = r9 << 0x1
    .D========================eE------------------------R..................................................  r10 = r10 << 0x1
    ..D========================eE-----------------------R..................................................  r7 = r7 + 0x1
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER................................................  u16 [r6 + 0x211] = r7
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R................................................  u16 [r6 + 0x213] = r8
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R................................................  u16 [r6 + 0x215] = r9
    ...D===============================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u16 [r6 + 0x217] = r10
    ...D================================================eE-----------------------R.........................  r11 = r11 << 0x1
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.......................  u16 [r6 + 0x219] = r11
    ...D================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-R.......................  r0 = u64 [r1 + 0x10]
    ....D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.......................  r5 = u64 [r1 + 0x8]
    ....D=======================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0]
    ....D========================================================================eE-----------------------R  r1 = r1 + 0x18
    ....D========================================================================eeeeeeeeeeeeeeeeeeeeeeE--R  jump [r0 + 0]
```

Gas simulation at offset 8160 with total cost of 28:

```
    DeER...........................  r1 = r1 + 0xffffffffffffffe8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0x10] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0x8] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0] = r6
    .D.............................  r5 = r7
    .DeE------------------------R..  r6 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER.  r8 = u8 [r6 + 0x23d]
    ..D=========================eER  jump 8188 if r8 == 0
```

Gas simulation at offset 8184 with total cost of 15:

```
    DeER..............  r9 = 0
    DeeeeeeeeeeeeeeeER  jump 8227
```

Gas simulation at offset 8188 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r8 = u8 [r6 + 0x231]
    D=========================eE--------------R.............  r8 = r8 + r5
    D==========================eE-------------R.............  r8 = r8 + 0x7ff
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u8 [r8 + 449] = 0xffffffffffffffff
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R.  r8 = u8 [r6 + 0x231]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R.  r9 = u8 [r6 + 0x23d]
    .D=========================eE-------------------------R.  r8 = r8 + 0x1
    ..D=========================eE------------------------R.  r8 = r8 & 0x1f
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x231] = a1
    ..D========================eE--------------------------R  r9 = r9 ^ 0x1
    ..DeeE-------------------------------------------------R  fallthrough
```

Gas simulation at offset 8227 with total cost of 46:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.....................  r8 = u16 [r6 + 0x209]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.....................  r11 = u16 [r6 + 0x211]
    DeE------------------------R.....................  r9 = r9 & 0x1
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER....................  u8 [r6 + 0x23d] = a2
    .D========================eER....................  r11 = r11 + 0xfffffffffffffeff
    .D========================eER....................  r9 = r8 >> 0x4
    .DeE------------------------R....................  r12 = 0x40
    ..D========================eER...................  r9 = r9 & 0x38
    ..D========================eeeeeeeeeeeeeeeeeeeeER  jump 8274 if r11 >=u r12
```

Gas simulation at offset 8258 with total cost of 16:

```
    DeER...............  r8 = r8 & 0xcff
    DeER...............  r10 = 0x2000
    D=eER..............  r8 = r8 | r10
    D==eER.............  r9 = r9 + r8
    .DeeeeeeeeeeeeeeeER  jump 8298
```

Gas simulation at offset 8274 with total cost of 4:

```
    DeER...  r10 = r8 & 0xc00
    DeER...  r8 = r8 << 0x3b
    D=eER..  r8 = r8 >> 0x3d
    .D=eER.  r8 = r8 | r10
    .DeE-R.  r10 = 0x23c0
    .D=eER.  r9 = r9 | r10
    .D==eER  r9 = r9 | r8
    ..DeeER  fallthrough
```

Gas simulation at offset 8298 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r6 + 0x21b] = r9
    D...........................  r7 = r5
    DeeeeeeeeeeeeeeeE----------R  r0 = 164, jump 7236
```

Gas simulation at offset 8310 with total cost of 15:

```
    D.................  r7 = r5
    DeeeeeeeeeeeeeeeER  r0 = 166, jump 6145
```

Gas simulation at offset 8318 with total cost of 100:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r7 = i16 [r6 + 0x211]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r8 = i16 [r6 + 0x213]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r9 = i16 [r6 + 0x215]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r10 = i16 [r6 + 0x217]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  r11 = i16 [r6 + 0x219]
    .D========================eE------------------------R..................................................  r8 = r8 << 0x1
    .D========================eE------------------------R..................................................  r9 = r9 << 0x1
    .D========================eE------------------------R..................................................  r10 = r10 << 0x1
    ..D========================eE-----------------------R..................................................  r7 = r7 + 0x1
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER................................................  u16 [r6 + 0x211] = r7
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R................................................  u16 [r6 + 0x213] = r8
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R................................................  u16 [r6 + 0x215] = r9
    ...D===============================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u16 [r6 + 0x217] = r10
    ...D================================================eE-----------------------R.........................  r11 = r11 << 0x1
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.......................  u16 [r6 + 0x219] = r11
    ...D================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-R.......................  r0 = u64 [r1 + 0x10]
    ....D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.......................  r5 = u64 [r1 + 0x8]
    ....D=======================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0]
    ....D========================================================================eE-----------------------R  r1 = r1 + 0x18
    ....D========================================================================eeeeeeeeeeeeeeeeeeeeeeE--R  jump [r0 + 0]
```

Gas simulation at offset 8386 with total cost of 28:

```
    DeER...........................  r1 = r1 + 0xffffffffffffffe8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0x10] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0x8] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0] = r6
    .D.............................  r5 = r7
    .DeE------------------------R..  r6 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER.  r7 = u8 [r6 + 0x23d]
    ..D=========================eER  jump 8444 if r7 == 0
```

Gas simulation at offset 8410 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r8 = u16 [r6 + 0x21b]
    D=========================eE--------------R  r9 = r8 >> 0x8
    .DeE--------------------------------------R  r10 = 0x3f
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R  u8 [r6 + 573] = 0
    .D=========================eE-------------R  jump 8502 if r9 <u r10
```

Gas simulation at offset 8428 with total cost of 28:

```
    DeER...........................  r8 = r8 & 0x1f
    D=eER..........................  r8 = r8 + r5
    D==eER.........................  r7 = r8 + 0x7ff
    .D==eeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u8 [r7 + 0x1a1]
    .DeeeeeeeeeeeeeeeE------------R  jump 8534
```

Gas simulation at offset 8444 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r7 = u8 [r6 + 0x231]
    D=========================eE--------------R.............  r7 = r7 + r5
    D==========================eE-------------R.............  r7 = r7 + 0x7ff
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u8 [r7 + 449] = 0xffffffffffffffff
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R.  r7 = u8 [r6 + 0x231]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R.  r8 = u8 [r6 + 0x23d]
    .D=========================eE-------------------------R.  r7 = r7 + 0x1
    ..D=========================eE------------------------R.  r7 = r7 & 0x1f
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x231] = a0
    ..D========================eE--------------------------R  r7 = r8 ^ 0x1
    ...DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r8 = u16 [r6 + 0x21b]
    ...D========================eE-------------------------R  r7 = r7 & 0x1
    ...D=========================eE------------------------R  r9 = r8 >> 0x8
    ....DeE------------------------------------------------R  r10 = 0x3f
    ....D========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x23d] = a0
    ....D=========================eE-----------------------R  jump 8428 if r9 >=u r10
```

Gas simulation at offset 8502 with total cost of 74:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r9 = u64 [r6 + 0x241]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r7 = u64 [r6 + 0x249]
    DeE---------------------------------------R..................................  r10 = 0x17c80
    .D========================eeE-------------R..................................  r10 = r7 if r9 != 0
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r10 = u64 [r10 + 0x48]
    ..DeE-------------------------------------------------R......................  r7 = r6 + 0x27f
    ..D=======================eeE-------------------------R......................  r7 = r9 if r9 != 0
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 170, jump [r10 + 0]
```

Gas simulation at offset 8534 with total cost of 55:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..............................  r8 = u8 [r6 + 0x209]
    D=========================eER.............................  r9 = r8 & 0x2
    D=========================eER.............................  r8 = r8 >> 0x4
    .D=========================eER............................  r8 = r8 & 0x4
    .D==========================eER...........................  r8 = r8 | r9
    .DeE--------------------------R...........................  r7 = r7 & 0xff
    ..D==========================eER..........................  r7 = r7 >> r8
    ..D===========================eER.........................  r7 = r7 & 0x3
    ..D============================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x22b] = a0
    ...D......................................................  r7 = r5
    ...DeeeeeeeeeeeeeeeE-------------------------------------R  r0 = 172, jump 7236
```

Gas simulation at offset 8572 with total cost of 15:

```
    D.................  r7 = r5
    DeeeeeeeeeeeeeeeER  r0 = 174, jump 6145
```

Gas simulation at offset 8580 with total cost of 100:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r7 = i16 [r6 + 0x211]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r8 = i16 [r6 + 0x213]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r9 = i16 [r6 + 0x215]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r10 = i16 [r6 + 0x217]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  r11 = i16 [r6 + 0x219]
    .D========================eE------------------------R..................................................  r8 = r8 << 0x1
    .D========================eE------------------------R..................................................  r9 = r9 << 0x1
    .D========================eE------------------------R..................................................  r10 = r10 << 0x1
    ..D========================eE-----------------------R..................................................  r7 = r7 + 0x1
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER................................................  u16 [r6 + 0x211] = r7
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R................................................  u16 [r6 + 0x213] = r8
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R................................................  u16 [r6 + 0x215] = r9
    ...D===============================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u16 [r6 + 0x217] = r10
    ...D================================================eE-----------------------R.........................  r11 = r11 << 0x1
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.......................  u16 [r6 + 0x219] = r11
    ...D================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-R.......................  r0 = u64 [r1 + 0x10]
    ....D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.......................  r5 = u64 [r1 + 0x8]
    ....D=======================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0]
    ....D========================================================================eE-----------------------R  r1 = r1 + 0x18
    ....D========================================================================eeeeeeeeeeeeeeeeeeeeeeE--R  jump [r0 + 0]
```

Gas simulation at offset 8648 with total cost of 28:

```
    DeER...........................  r1 = r1 + 0xffffffffffffffe8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0x10] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0x8] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0] = r6
    .D.............................  r5 = r7
    .DeE------------------------R..  r6 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER.  r8 = u8 [r6 + 0x23d]
    ..D=========================eER  jump 8676 if r8 == 0
```

Gas simulation at offset 8672 with total cost of 15:

```
    DeER..............  r8 = 0
    DeeeeeeeeeeeeeeeER  jump 8715
```

Gas simulation at offset 8676 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r8 = u8 [r6 + 0x231]
    D=========================eE--------------R.............  r8 = r8 + r5
    D==========================eE-------------R.............  r8 = r8 + 0x7ff
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u8 [r8 + 449] = 0xffffffffffffffff
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R.  r8 = u8 [r6 + 0x231]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R.  r9 = u8 [r6 + 0x23d]
    .D=========================eE-------------------------R.  r8 = r8 + 0x1
    ..D=========================eE------------------------R.  r8 = r8 & 0x1f
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x231] = a1
    ..D========================eE--------------------------R  r8 = r9 ^ 0x1
    ...DeeE------------------------------------------------R  fallthrough
```

Gas simulation at offset 8715 with total cost of 54:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.............................  r9 = u8 [r6 + 0x226]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.............................  r10 = u8 [r6 + 0x22a]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.............................  r11 = i16 [r6 + 0x209]
    D=========================eER............................  r9 = r9 & 0x10
    .D========================eER............................  r10 = r10 << 0x4
    .D=========================eER...........................  r9 = r9 << 0x8
    .D==========================eER..........................  r9 = r9 | r10
    .DeE--------------------------R..........................  r8 = r8 & 0x1
    ..D=======================eE--R..........................  r11 = r11 << 0x31
    ..D========================eE-R..........................  r11 = r11 >> 0x3d
    ..D==========================eER.........................  r9 = r9 | r11
    ..D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r6 + 0x21b] = r9
    ...DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R  u8 [r6 + 0x23d] = a1
    ...D.....................................................  r7 = r5
    ...DeeeeeeeeeeeeeeeE------------------------------------R  r0 = 178, jump 7236
```

Gas simulation at offset 8767 with total cost of 15:

```
    D.................  r7 = r5
    DeeeeeeeeeeeeeeeER  r0 = 180, jump 6145
```

Gas simulation at offset 8775 with total cost of 100:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r7 = i16 [r6 + 0x211]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r8 = i16 [r6 + 0x213]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r9 = i16 [r6 + 0x215]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r10 = i16 [r6 + 0x217]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  r11 = i16 [r6 + 0x219]
    .D========================eE------------------------R..................................................  r8 = r8 << 0x1
    .D========================eE------------------------R..................................................  r9 = r9 << 0x1
    .D========================eE------------------------R..................................................  r10 = r10 << 0x1
    ..D========================eE-----------------------R..................................................  r7 = r7 + 0x1
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER................................................  u16 [r6 + 0x211] = r7
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R................................................  u16 [r6 + 0x213] = r8
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R................................................  u16 [r6 + 0x215] = r9
    ...D===============================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u16 [r6 + 0x217] = r10
    ...D================================================eE-----------------------R.........................  r11 = r11 << 0x1
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.......................  u16 [r6 + 0x219] = r11
    ...D================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-R.......................  r0 = u64 [r1 + 0x10]
    ....D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.......................  r5 = u64 [r1 + 0x8]
    ....D=======================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0]
    ....D========================================================================eE-----------------------R  r1 = r1 + 0x18
    ....D========================================================================eeeeeeeeeeeeeeeeeeeeeeE--R  jump [r0 + 0]
```

Gas simulation at offset 8843 with total cost of 28:

```
    DeER...........................  r1 = r1 + 0xffffffffffffffe8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0x10] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0x8] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0] = r6
    .D.............................  r5 = r7
    .DeE------------------------R..  r6 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER.  r7 = u8 [r6 + 0x23d]
    ..D=========================eER  jump 8901 if r7 == 0
```

Gas simulation at offset 8867 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r8 = u16 [r6 + 0x21b]
    D=========================eE--------------R  r9 = r8 >> 0x8
    .DeE--------------------------------------R  r10 = 0x3f
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R  u8 [r6 + 573] = 0
    .D=========================eE-------------R  jump 8959 if r9 <u r10
```

Gas simulation at offset 8885 with total cost of 28:

```
    DeER...........................  r8 = r8 & 0x1f
    D=eER..........................  r8 = r8 + r5
    D==eER.........................  r7 = r8 + 0x7ff
    .D==eeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u8 [r7 + 0x1a1]
    .DeeeeeeeeeeeeeeeE------------R  jump 8991
```

Gas simulation at offset 8901 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r7 = u8 [r6 + 0x231]
    D=========================eE--------------R.............  r7 = r7 + r5
    D==========================eE-------------R.............  r7 = r7 + 0x7ff
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u8 [r7 + 449] = 0xffffffffffffffff
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R.  r7 = u8 [r6 + 0x231]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R.  r8 = u8 [r6 + 0x23d]
    .D=========================eE-------------------------R.  r7 = r7 + 0x1
    ..D=========================eE------------------------R.  r7 = r7 & 0x1f
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x231] = a0
    ..D========================eE--------------------------R  r7 = r8 ^ 0x1
    ...DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r8 = u16 [r6 + 0x21b]
    ...D========================eE-------------------------R  r7 = r7 & 0x1
    ...D=========================eE------------------------R  r9 = r8 >> 0x8
    ....DeE------------------------------------------------R  r10 = 0x3f
    ....D========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x23d] = a0
    ....D=========================eE-----------------------R  jump 8885 if r9 >=u r10
```

Gas simulation at offset 8959 with total cost of 74:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r9 = u64 [r6 + 0x241]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r7 = u64 [r6 + 0x249]
    DeE---------------------------------------R..................................  r10 = 0x17c80
    .D========================eeE-------------R..................................  r10 = r7 if r9 != 0
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r10 = u64 [r10 + 0x48]
    ..DeE-------------------------------------------------R......................  r7 = r6 + 0x27f
    ..D=======================eeE-------------------------R......................  r7 = r9 if r9 != 0
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 184, jump [r10 + 0]
```

Gas simulation at offset 8991 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x22c] = a0
    D...........................  r7 = r5
    DeeeeeeeeeeeeeeeE----------R  r0 = 186, jump 7236
```

Gas simulation at offset 9003 with total cost of 15:

```
    D.................  r7 = r5
    DeeeeeeeeeeeeeeeER  r0 = 188, jump 6145
```

Gas simulation at offset 9011 with total cost of 100:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r7 = i16 [r6 + 0x211]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r8 = i16 [r6 + 0x213]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r9 = i16 [r6 + 0x215]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r10 = i16 [r6 + 0x217]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  r11 = i16 [r6 + 0x219]
    .D========================eE------------------------R..................................................  r8 = r8 << 0x1
    .D========================eE------------------------R..................................................  r9 = r9 << 0x1
    .D========================eE------------------------R..................................................  r10 = r10 << 0x1
    ..D========================eE-----------------------R..................................................  r7 = r7 + 0x1
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER................................................  u16 [r6 + 0x211] = r7
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R................................................  u16 [r6 + 0x213] = r8
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R................................................  u16 [r6 + 0x215] = r9
    ...D===============================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u16 [r6 + 0x217] = r10
    ...D================================================eE-----------------------R.........................  r11 = r11 << 0x1
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.......................  u16 [r6 + 0x219] = r11
    ...D================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-R.......................  r0 = u64 [r1 + 0x10]
    ....D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.......................  r5 = u64 [r1 + 0x8]
    ....D=======================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0]
    ....D========================================================================eE-----------------------R  r1 = r1 + 0x18
    ....D========================================================================eeeeeeeeeeeeeeeeeeeeeeE--R  jump [r0 + 0]
```

Gas simulation at offset 9079 with total cost of 28:

```
    DeER...........................  r1 = r1 + 0xffffffffffffffe8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0x10] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0x8] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0] = r6
    .D.............................  r5 = r7
    .DeE------------------------R..  r6 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER.  r8 = u8 [r6 + 0x23d]
    ..D=========================eER  jump 9107 if r8 == 0
```

Gas simulation at offset 9103 with total cost of 15:

```
    DeER..............  r8 = 0
    DeeeeeeeeeeeeeeeER  jump 9146
```

Gas simulation at offset 9107 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r8 = u8 [r6 + 0x231]
    D=========================eE--------------R.............  r8 = r8 + r5
    D==========================eE-------------R.............  r8 = r8 + 0x7ff
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u8 [r8 + 449] = 0xffffffffffffffff
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R.  r8 = u8 [r6 + 0x231]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R.  r9 = u8 [r6 + 0x23d]
    .D=========================eE-------------------------R.  r8 = r8 + 0x1
    ..D=========================eE------------------------R.  r8 = r8 & 0x1f
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x231] = a1
    ..D========================eE--------------------------R  r8 = r9 ^ 0x1
    ...DeeE------------------------------------------------R  fallthrough
```

Gas simulation at offset 9146 with total cost of 54:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.............................  r9 = u8 [r6 + 0x22a]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.............................  r10 = u16 [r6 + 0x209]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.............................  r11 = u8 [r6 + 0x226]
    D=========================eER............................  r9 = r9 << 0x4
    .D========================eER............................  r10 = r10 >> 0xc
    .D=========================eER...........................  r9 = r9 | r10
    .DeE-------------------------R...........................  r8 = r8 & 0x1
    .D========================eE-R...........................  r11 = r11 & 0x10
    ..D========================eER...........................  r11 = r11 << 0x8
    ..D=========================eER..........................  r9 = r9 | r11
    ..D==========================eER.........................  r9 = r9 | 0x8
    ..D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r6 + 0x21b] = r9
    ...DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R  u8 [r6 + 0x23d] = a1
    ...D.....................................................  r7 = r5
    ...DeeeeeeeeeeeeeeeE------------------------------------R  r0 = 192, jump 7236
```

Gas simulation at offset 9198 with total cost of 15:

```
    D.................  r7 = r5
    DeeeeeeeeeeeeeeeER  r0 = 194, jump 6145
```

Gas simulation at offset 9206 with total cost of 100:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r7 = i16 [r6 + 0x211]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r8 = i16 [r6 + 0x213]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r9 = i16 [r6 + 0x215]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r10 = i16 [r6 + 0x217]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  r11 = i16 [r6 + 0x219]
    .D========================eE------------------------R..................................................  r8 = r8 << 0x1
    .D========================eE------------------------R..................................................  r9 = r9 << 0x1
    .D========================eE------------------------R..................................................  r10 = r10 << 0x1
    ..D========================eE-----------------------R..................................................  r7 = r7 + 0x1
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER................................................  u16 [r6 + 0x211] = r7
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R................................................  u16 [r6 + 0x213] = r8
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R................................................  u16 [r6 + 0x215] = r9
    ...D===============================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u16 [r6 + 0x217] = r10
    ...D================================================eE-----------------------R.........................  r11 = r11 << 0x1
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.......................  u16 [r6 + 0x219] = r11
    ...D================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-R.......................  r0 = u64 [r1 + 0x10]
    ....D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.......................  r5 = u64 [r1 + 0x8]
    ....D=======================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0]
    ....D========================================================================eE-----------------------R  r1 = r1 + 0x18
    ....D========================================================================eeeeeeeeeeeeeeeeeeeeeeE--R  jump [r0 + 0]
```

Gas simulation at offset 9274 with total cost of 28:

```
    DeER...........................  r1 = r1 + 0xffffffffffffffe8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0x10] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0x8] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0] = r6
    .D.............................  r5 = r7
    .DeE------------------------R..  r6 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER.  r7 = u8 [r6 + 0x23d]
    ..D=========================eER  jump 9346 if r7 == 0
```

Gas simulation at offset 9298 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r8 = u16 [r6 + 0x21b]
    D=========================eE--------------R  r9 = r8 >> 0x8
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R  u8 [r6 + 573] = 0
    .D=========================eE-------------R  jump 9402 if r9 <u 63
```

Gas simulation at offset 9314 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeE---------------------------------------R.............  r8 = r8 & 0x1f
    D=eE--------------------------------------R.............  r8 = r8 + r5
    .D=eE-------------------------------------R.............  r7 = r8 + 0x7ff
    .D==eeeeeeeeeeeeeeeeeeeeeeeeeE------------R.............  r7 = u8 [r7 + 0x1a1]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.............  r8 = u8 [r6 + 0x227]
    ..D========================eE-------------R.............  r8 = r8 & 0x18
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x22d] = a0
    ..D=========================eE-------------------------R  jump 9448 if r8 != 0
```

Gas simulation at offset 9343 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 9484
```

Gas simulation at offset 9346 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r7 = u8 [r6 + 0x231]
    D=========================eE--------------R.............  r7 = r7 + r5
    D==========================eE-------------R.............  r7 = r7 + 0x7ff
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u8 [r7 + 449] = 0xffffffffffffffff
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R.  r7 = u8 [r6 + 0x231]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R.  r8 = u8 [r6 + 0x23d]
    .D=========================eE-------------------------R.  r7 = r7 + 0x1
    ..D=========================eE------------------------R.  r7 = r7 & 0x1f
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x231] = a0
    ..D========================eE--------------------------R  r7 = r8 ^ 0x1
    ...DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r8 = u16 [r6 + 0x21b]
    ...D========================eE-------------------------R  r7 = r7 & 0x1
    ...D=========================eE------------------------R  r9 = r8 >> 0x8
    ....D========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x23d] = a0
    ....D=========================eE-----------------------R  jump 9314 if r9 >=u 63
```

Gas simulation at offset 9402 with total cost of 74:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r9 = u64 [r6 + 0x241]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r7 = u64 [r6 + 0x249]
    DeE---------------------------------------R..................................  r10 = 0x17c80
    .D========================eeE-------------R..................................  r10 = r7 if r9 != 0
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r10 = u64 [r10 + 0x48]
    ..DeE-------------------------------------------------R......................  r7 = r6 + 0x27f
    ..D=======================eeE-------------------------R......................  r7 = r9 if r9 != 0
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 198, jump [r10 + 0]
```

Gas simulation at offset 9434 with total cost of 27:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u8 [r6 + 0x227]
    D=========================eER.  r8 = r8 & 0x18
    DeeeeeeeeeeeeeeeeeeeeeeeeeE-R.  u8 [r6 + 0x22d] = a0
    D==========================eER  jump 9484 if r8 == 0
```

Gas simulation at offset 9448 with total cost of 46:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER......  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R......  r8 = u16 [r6 + 0x209]
    D=========================eE--------------R......  r9 = r8 & 0x1f
    .D========================eE--------------R......  r8 = r8 & 0xffffffffffffffe0
    .D=========================eeeeeeeeeeeeeeeeeeeeER  jump 9473 if r9 != 31
```

Gas simulation at offset 9463 with total cost of 26:

```
    DeER.........................  r8 = r8 ^ 0x400
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r6 + 0x209] = r8
    DeeeeeeeeeeeeeeeE-----------R  jump 9484
```

Gas simulation at offset 9473 with total cost of 27:

```
    DeER..........................  r8 = r8 | r9
    D=eER.........................  r8 = r8 + 0x1
    D==eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r6 + 0x209] = r8
    DeeE-------------------------R  fallthrough
```

Gas simulation at offset 9484 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r8 = u8 [r6 + 0x22b]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r9 = u8 [r6 + 0x22c]
    .D========================eE--------------R.............  r10 = r8 << 0x3f
    .D========================eE--------------R.............  r8 = r8 << 0x6
    .D=========================eE-------------R.............  r10 = r10 >>a 0x3f
    ..D========================eE-------------R.............  r8 = sext8 r8
    ..D=========================eE------------R.............  r8 = r8 >> 0x7
    ..D=======================eeeeeeeeeeeeeeeeeeeeeeeeeER...  u8 [r6 + 0x213] = a2
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-----------------------R...  u8 [r6 + 0x215] = a0
    ...D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u8 [r6 + 0x217] = a3
    ...D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x219] = a1
    ...D....................................................  r7 = r5
    ...DeeeeeeeeeeeeeeeE-----------------------------------R  r0 = 200, jump 7236
```

Gas simulation at offset 9531 with total cost of 15:

```
    D.................  r7 = r5
    DeeeeeeeeeeeeeeeER  r0 = 202, jump 6145
```

Gas simulation at offset 9539 with total cost of 100:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r7 = i16 [r6 + 0x211]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r8 = i16 [r6 + 0x213]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r9 = i16 [r6 + 0x215]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r10 = i16 [r6 + 0x217]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  r11 = i16 [r6 + 0x219]
    .D========================eE------------------------R..................................................  r8 = r8 << 0x1
    .D========================eE------------------------R..................................................  r9 = r9 << 0x1
    .D========================eE------------------------R..................................................  r10 = r10 << 0x1
    ..D========================eE-----------------------R..................................................  r7 = r7 + 0x1
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER................................................  u16 [r6 + 0x211] = r7
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R................................................  u16 [r6 + 0x213] = r8
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R................................................  u16 [r6 + 0x215] = r9
    ...D===============================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u16 [r6 + 0x217] = r10
    ...D================================================eE-----------------------R.........................  r11 = r11 << 0x1
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.......................  u16 [r6 + 0x219] = r11
    ...D================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-R.......................  r0 = u64 [r1 + 0x10]
    ....D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.......................  r5 = u64 [r1 + 0x8]
    ....D=======================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0]
    ....D========================================================================eE-----------------------R  r1 = r1 + 0x18
    ....D========================================================================eeeeeeeeeeeeeeeeeeeeeeE--R  jump [r0 + 0]
```

Gas simulation at offset 9607 with total cost of 26:

```
    DeER.........................  r1 = r1 + 0xffffffffffffffe8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x10] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x8] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0] = r6
    .D...........................  r5 = r7
    .DeE------------------------R  r6 = r7 + 0x7ff
    .DeeeeeeeeeeeeeeeE----------R  r0 = 206, jump 6954
```

Gas simulation at offset 9630 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER............................  r7 = u16 [r6 + 0x209]
    D=========================eER...........................  r7 = r7 << 0x34
    D==========================eER..........................  r7 = r7 >> 0x34
    D===========================eER.........................  r7 = r7 | 0x2000
    .D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r6 + 0x21b] = r7
    .D......................................................  r7 = r5
    .DeeeeeeeeeeeeeeeE-------------------------------------R  r0 = 208, jump 7236
```

Gas simulation at offset 9656 with total cost of 15:

```
    D.................  r7 = r5
    DeeeeeeeeeeeeeeeER  r0 = 210, jump 6145
```

Gas simulation at offset 9664 with total cost of 100:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r7 = i16 [r6 + 0x211]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r8 = i16 [r6 + 0x213]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r9 = i16 [r6 + 0x215]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r10 = i16 [r6 + 0x217]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  r11 = i16 [r6 + 0x219]
    .D========================eE------------------------R..................................................  r8 = r8 << 0x1
    .D========================eE------------------------R..................................................  r9 = r9 << 0x1
    .D========================eE------------------------R..................................................  r10 = r10 << 0x1
    ..D========================eE-----------------------R..................................................  r7 = r7 + 0x1
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER................................................  u16 [r6 + 0x211] = r7
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R................................................  u16 [r6 + 0x213] = r8
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R................................................  u16 [r6 + 0x215] = r9
    ...D===============================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u16 [r6 + 0x217] = r10
    ...D================================================eE-----------------------R.........................  r11 = r11 << 0x1
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.......................  u16 [r6 + 0x219] = r11
    ...D================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-R.......................  r0 = u64 [r1 + 0x10]
    ....D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.......................  r5 = u64 [r1 + 0x8]
    ....D=======================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0]
    ....D========================================================================eE-----------------------R  r1 = r1 + 0x18
    ....D========================================================================eeeeeeeeeeeeeeeeeeeeeeE--R  jump [r0 + 0]
```

Gas simulation at offset 9732 with total cost of 26:

```
    DeER.........................  r1 = r1 + 0xffffffffffffffe8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x10] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x8] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0] = r6
    .D...........................  r5 = r7
    .DeE------------------------R  r6 = r7 + 0x7ff
    .DeeeeeeeeeeeeeeeE----------R  r0 = 214, jump 6954
```

Gas simulation at offset 9755 with total cost of 27:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u16 [r6 + 0x21b]
    D=========================eER.  r7 = r8 >> 0x8
    DeE-------------------------R.  r9 = 0x3f
    .D=========================eER  jump 9802 if r7 >=u r9
```

Gas simulation at offset 9768 with total cost of 74:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r9 = u64 [r6 + 0x241]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r7 = u64 [r6 + 0x249]
    DeE---------------------------------------R..................................  r10 = 0x17c80
    .D========================eeE-------------R..................................  r10 = r7 if r9 != 0
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r10 = u64 [r10 + 0x48]
    ..DeE-------------------------------------------------R......................  r7 = r6 + 0x27f
    ..D=======================eeE-------------------------R......................  r7 = r9 if r9 != 0
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 216, jump [r10 + 0]
```

Gas simulation at offset 9800 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 9817
```

Gas simulation at offset 9802 with total cost of 28:

```
    DeER...........................  r8 = r8 & 0x1f
    D=eER..........................  r8 = r8 + r5
    D==eER.........................  r7 = r8 + 0x7ff
    .D==eeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u8 [r7 + 0x1a1]
    .DeeE-------------------------R  fallthrough
```

Gas simulation at offset 9817 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x22a] = a0
    D...........................  r7 = r5
    DeeeeeeeeeeeeeeeE----------R  r0 = 218, jump 7236
```

Gas simulation at offset 9829 with total cost of 15:

```
    D.................  r7 = r5
    DeeeeeeeeeeeeeeeER  r0 = 220, jump 6145
```

Gas simulation at offset 9837 with total cost of 100:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r7 = i16 [r6 + 0x211]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r8 = i16 [r6 + 0x213]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r9 = i16 [r6 + 0x215]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r10 = i16 [r6 + 0x217]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  r11 = i16 [r6 + 0x219]
    .D========================eE------------------------R..................................................  r8 = r8 << 0x1
    .D========================eE------------------------R..................................................  r9 = r9 << 0x1
    .D========================eE------------------------R..................................................  r10 = r10 << 0x1
    ..D========================eE-----------------------R..................................................  r7 = r7 + 0x1
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER................................................  u16 [r6 + 0x211] = r7
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R................................................  u16 [r6 + 0x213] = r8
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R................................................  u16 [r6 + 0x215] = r9
    ...D===============================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u16 [r6 + 0x217] = r10
    ...D================================================eE-----------------------R.........................  r11 = r11 << 0x1
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.......................  u16 [r6 + 0x219] = r11
    ...D================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-R.......................  r0 = u64 [r1 + 0x10]
    ....D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.......................  r5 = u64 [r1 + 0x8]
    ....D=======================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0]
    ....D========================================================================eE-----------------------R  r1 = r1 + 0x18
    ....D========================================================================eeeeeeeeeeeeeeeeeeeeeeE--R  jump [r0 + 0]
```

Gas simulation at offset 9905 with total cost of 27:

```
    DeER..........................  r1 = r1 + 0xffffffffffffffe0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.  u64 [r1 + 0x18] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.  u64 [r1 + 0x10] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.  u64 [r1 + 0x8] = r6
    .D............................  r5 = r7
    .DeE------------------------R.  r6 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0] = 0xc00
    ..D...........................  r7 = r5
    ..DeeeeeeeeeeeeeeeE----------R  r0 = 224, jump 6954
```

Gas simulation at offset 9935 with total cost of 46:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.....................  r7 = u16 [r6 + 0x211]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.....................  r8 = u16 [r6 + 0x209]
    D=========================eER....................  r9 = r7 + 0xfffffffffffffeff
    .D========================eER....................  r7 = r8 >> 0x4
    .DeE------------------------R....................  r10 = 0x40
    .D=========================eER...................  r7 = r7 & 0x38
    ..D========================eeeeeeeeeeeeeeeeeeeeER  jump 9980 if r9 >=u r10
```

Gas simulation at offset 9959 with total cost of 29:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER....  r9 = u64 [r1 + 0]
    D=========================eER...  r9 = r9 + 0xff
    D==========================eER..  r8 = r8 & r9
    DeE--------------------------R..  r9 = 0x2000
    .D==========================eER.  r8 = r8 + r9
    .D===========================eER  r7 = r7 + r8
    .DeeeeeeeeeeeeeeeE-------------R  jump 10005
```

Gas simulation at offset 9980 with total cost of 28:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...  r9 = u64 [r1 + 0]
    D=========================eER..  r9 = r9 & r8
    DeE-------------------------R..  r8 = r8 << 0x3b
    D=eE------------------------R..  r8 = r8 >> 0x3d
    .D=========================eER.  r8 = r8 | r9
    .DeE-------------------------R.  r9 = 0x23c0
    .D=eE------------------------R.  r7 = r7 | r9
    .D==========================eER  r7 = r7 | r8
    ..DeeE------------------------R  fallthrough
```

Gas simulation at offset 10005 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r6 + 0x21b] = r7
    D...........................  r7 = r5
    DeeeeeeeeeeeeeeeE----------R  r0 = 226, jump 7236
```

Gas simulation at offset 10017 with total cost of 15:

```
    D.................  r7 = r5
    DeeeeeeeeeeeeeeeER  r0 = 228, jump 6145
```

Gas simulation at offset 10025 with total cost of 100:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r7 = i16 [r6 + 0x211]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r8 = i16 [r6 + 0x213]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r9 = i16 [r6 + 0x215]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r10 = i16 [r6 + 0x217]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  r11 = i16 [r6 + 0x219]
    .D========================eE------------------------R..................................................  r8 = r8 << 0x1
    .D========================eE------------------------R..................................................  r9 = r9 << 0x1
    .D========================eE------------------------R..................................................  r10 = r10 << 0x1
    ..D========================eE-----------------------R..................................................  r7 = r7 + 0x1
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER................................................  u16 [r6 + 0x211] = r7
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R................................................  u16 [r6 + 0x213] = r8
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R................................................  u16 [r6 + 0x215] = r9
    ...D===============================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u16 [r6 + 0x217] = r10
    ...D================================================eE-----------------------R.........................  r11 = r11 << 0x1
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.......................  u16 [r6 + 0x219] = r11
    ...D================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-R.......................  r0 = u64 [r1 + 0x18]
    ....D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.......................  r5 = u64 [r1 + 0x10]
    ....D=======================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0x8]
    ....D========================================================================eE-----------------------R  r1 = r1 + 0x20
    ....D========================================================================eeeeeeeeeeeeeeeeeeeeeeE--R  jump [r0 + 0]
```

Gas simulation at offset 10094 with total cost of 26:

```
    DeER.........................  r1 = r1 + 0xffffffffffffffe8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x10] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x8] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0] = r6
    .D...........................  r5 = r7
    .DeE------------------------R  r6 = r7 + 0x7ff
    .DeeeeeeeeeeeeeeeE----------R  r0 = 232, jump 6954
```

Gas simulation at offset 10117 with total cost of 27:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u16 [r6 + 0x21b]
    D=========================eER.  r7 = r8 >> 0x8
    D==========================eER  jump 10162 if r7 >=u 63
```

Gas simulation at offset 10128 with total cost of 74:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r9 = u64 [r6 + 0x241]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r7 = u64 [r6 + 0x249]
    DeE---------------------------------------R..................................  r10 = 0x17c80
    .D========================eeE-------------R..................................  r10 = r7 if r9 != 0
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r10 = u64 [r10 + 0x48]
    ..DeE-------------------------------------------------R......................  r7 = r6 + 0x27f
    ..D=======================eeE-------------------------R......................  r7 = r9 if r9 != 0
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 234, jump [r10 + 0]
```

Gas simulation at offset 10160 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 10177
```

Gas simulation at offset 10162 with total cost of 28:

```
    DeER...........................  r8 = r8 & 0x1f
    D=eER..........................  r8 = r8 + r5
    D==eER.........................  r7 = r8 + 0x7ff
    .D==eeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u8 [r7 + 0x1a1]
    .DeeE-------------------------R  fallthrough
```

Gas simulation at offset 10177 with total cost of 55:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..............................  r8 = u8 [r6 + 0x209]
    D=========================eER.............................  r9 = r8 & 0x2
    D=========================eER.............................  r8 = r8 >> 0x4
    .D=========================eER............................  r8 = r8 & 0x4
    .D==========================eER...........................  r8 = r8 | r9
    .DeE--------------------------R...........................  r7 = r7 & 0xff
    ..D==========================eER..........................  r7 = r7 >> r8
    ..D===========================eER.........................  r7 = r7 & 0x3
    ..D============================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x22b] = a0
    ...D......................................................  r7 = r5
    ...DeeeeeeeeeeeeeeeE-------------------------------------R  r0 = 236, jump 7236
```

Gas simulation at offset 10215 with total cost of 15:

```
    D.................  r7 = r5
    DeeeeeeeeeeeeeeeER  r0 = 238, jump 6145
```

Gas simulation at offset 10223 with total cost of 100:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r7 = i16 [r6 + 0x211]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r8 = i16 [r6 + 0x213]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r9 = i16 [r6 + 0x215]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r10 = i16 [r6 + 0x217]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  r11 = i16 [r6 + 0x219]
    .D========================eE------------------------R..................................................  r8 = r8 << 0x1
    .D========================eE------------------------R..................................................  r9 = r9 << 0x1
    .D========================eE------------------------R..................................................  r10 = r10 << 0x1
    ..D========================eE-----------------------R..................................................  r7 = r7 + 0x1
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER................................................  u16 [r6 + 0x211] = r7
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R................................................  u16 [r6 + 0x213] = r8
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R................................................  u16 [r6 + 0x215] = r9
    ...D===============================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u16 [r6 + 0x217] = r10
    ...D================================================eE-----------------------R.........................  r11 = r11 << 0x1
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.......................  u16 [r6 + 0x219] = r11
    ...D================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-R.......................  r0 = u64 [r1 + 0x10]
    ....D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.......................  r5 = u64 [r1 + 0x8]
    ....D=======================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0]
    ....D========================================================================eE-----------------------R  r1 = r1 + 0x18
    ....D========================================================================eeeeeeeeeeeeeeeeeeeeeeE--R  jump [r0 + 0]
```

Gas simulation at offset 10291 with total cost of 26:

```
    DeER.........................  r1 = r1 + 0xffffffffffffffe8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x10] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x8] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0] = r6
    .D...........................  r5 = r7
    .DeE------------------------R  r6 = r7 + 0x7ff
    .DeeeeeeeeeeeeeeeE----------R  r0 = 242, jump 6954
```

Gas simulation at offset 10314 with total cost of 54:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.............................  r7 = u8 [r6 + 0x226]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.............................  r8 = u8 [r6 + 0x22a]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.............................  r9 = i16 [r6 + 0x209]
    D=========================eER............................  r7 = r7 & 0x10
    .D========================eER............................  r8 = r8 << 0x4
    .D========================eER............................  r9 = r9 << 0x31
    .D=========================eER...........................  r7 = r7 << 0x8
    .D==========================eER..........................  r7 = r7 | r8
    ..D========================eE-R..........................  r9 = r9 >> 0x3d
    ..D==========================eER.........................  r7 = r7 | r9
    ..D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r6 + 0x21b] = r7
    ..D......................................................  r7 = r5
    ...DeeeeeeeeeeeeeeeE------------------------------------R  r0 = 244, jump 7236
```

Gas simulation at offset 10359 with total cost of 15:

```
    D.................  r7 = r5
    DeeeeeeeeeeeeeeeER  r0 = 246, jump 6145
```

Gas simulation at offset 10367 with total cost of 100:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r7 = i16 [r6 + 0x211]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r8 = i16 [r6 + 0x213]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r9 = i16 [r6 + 0x215]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r10 = i16 [r6 + 0x217]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  r11 = i16 [r6 + 0x219]
    .D========================eE------------------------R..................................................  r8 = r8 << 0x1
    .D========================eE------------------------R..................................................  r9 = r9 << 0x1
    .D========================eE------------------------R..................................................  r10 = r10 << 0x1
    ..D========================eE-----------------------R..................................................  r7 = r7 + 0x1
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER................................................  u16 [r6 + 0x211] = r7
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R................................................  u16 [r6 + 0x213] = r8
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R................................................  u16 [r6 + 0x215] = r9
    ...D===============================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u16 [r6 + 0x217] = r10
    ...D================================================eE-----------------------R.........................  r11 = r11 << 0x1
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.......................  u16 [r6 + 0x219] = r11
    ...D================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-R.......................  r0 = u64 [r1 + 0x10]
    ....D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.......................  r5 = u64 [r1 + 0x8]
    ....D=======================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0]
    ....D========================================================================eE-----------------------R  r1 = r1 + 0x18
    ....D========================================================================eeeeeeeeeeeeeeeeeeeeeeE--R  jump [r0 + 0]
```

Gas simulation at offset 10435 with total cost of 26:

```
    DeER.........................  r1 = r1 + 0xffffffffffffffe8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x10] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x8] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0] = r6
    .D...........................  r5 = r7
    .DeE------------------------R  r6 = r7 + 0x7ff
    .DeeeeeeeeeeeeeeeE----------R  r0 = 250, jump 6954
```

Gas simulation at offset 10458 with total cost of 27:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u16 [r6 + 0x21b]
    D=========================eER.  r7 = r8 >> 0x8
    DeE-------------------------R.  r9 = 0x3f
    .D=========================eER  jump 10505 if r7 >=u r9
```

Gas simulation at offset 10471 with total cost of 74:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r9 = u64 [r6 + 0x241]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r7 = u64 [r6 + 0x249]
    DeE---------------------------------------R..................................  r10 = 0x17c80
    .D========================eeE-------------R..................................  r10 = r7 if r9 != 0
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r10 = u64 [r10 + 0x48]
    ..DeE-------------------------------------------------R......................  r7 = r6 + 0x27f
    ..D=======================eeE-------------------------R......................  r7 = r9 if r9 != 0
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 252, jump [r10 + 0]
```

Gas simulation at offset 10503 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 10520
```

Gas simulation at offset 10505 with total cost of 28:

```
    DeER...........................  r8 = r8 & 0x1f
    D=eER..........................  r8 = r8 + r5
    D==eER.........................  r7 = r8 + 0x7ff
    .D==eeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u8 [r7 + 0x1a1]
    .DeeE-------------------------R  fallthrough
```

Gas simulation at offset 10520 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x22c] = a0
    D...........................  r7 = r5
    DeeeeeeeeeeeeeeeE----------R  r0 = 254, jump 7236
```

Gas simulation at offset 10532 with total cost of 15:

```
    D.................  r7 = r5
    DeeeeeeeeeeeeeeeER  r0 = 256, jump 6145
```

Gas simulation at offset 10540 with total cost of 100:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r7 = i16 [r6 + 0x211]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r8 = i16 [r6 + 0x213]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r9 = i16 [r6 + 0x215]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r10 = i16 [r6 + 0x217]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  r11 = i16 [r6 + 0x219]
    .D========================eE------------------------R..................................................  r8 = r8 << 0x1
    .D========================eE------------------------R..................................................  r9 = r9 << 0x1
    .D========================eE------------------------R..................................................  r10 = r10 << 0x1
    ..D========================eE-----------------------R..................................................  r7 = r7 + 0x1
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER................................................  u16 [r6 + 0x211] = r7
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R................................................  u16 [r6 + 0x213] = r8
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R................................................  u16 [r6 + 0x215] = r9
    ...D===============================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u16 [r6 + 0x217] = r10
    ...D================================================eE-----------------------R.........................  r11 = r11 << 0x1
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.......................  u16 [r6 + 0x219] = r11
    ...D================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-R.......................  r0 = u64 [r1 + 0x10]
    ....D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.......................  r5 = u64 [r1 + 0x8]
    ....D=======================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0]
    ....D========================================================================eE-----------------------R  r1 = r1 + 0x18
    ....D========================================================================eeeeeeeeeeeeeeeeeeeeeeE--R  jump [r0 + 0]
```

Gas simulation at offset 10608 with total cost of 26:

```
    DeER.........................  r1 = r1 + 0xffffffffffffffe8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x10] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x8] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0] = r6
    .D...........................  r5 = r7
    .DeE------------------------R  r6 = r7 + 0x7ff
    .DeeeeeeeeeeeeeeeE----------R  r0 = 260, jump 6954
```

Gas simulation at offset 10631 with total cost of 54:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.............................  r7 = u8 [r6 + 0x226]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.............................  r8 = u8 [r6 + 0x22a]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.............................  r9 = u16 [r6 + 0x209]
    D=========================eER............................  r7 = r7 & 0x10
    .D========================eER............................  r8 = r8 << 0x4
    .D========================eER............................  r9 = r9 >> 0xc
    .D=========================eER...........................  r7 = r7 << 0x8
    .D=========================eER...........................  r8 = r8 | r9
    ..D=========================eER..........................  r7 = r7 | r8
    ..D==========================eER.........................  r7 = r7 | 0x8
    ..D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r6 + 0x21b] = r7
    ..D......................................................  r7 = r5
    ...DeeeeeeeeeeeeeeeE------------------------------------R  r0 = 262, jump 7236
```

Gas simulation at offset 10676 with total cost of 15:

```
    D.................  r7 = r5
    DeeeeeeeeeeeeeeeER  r0 = 264, jump 6145
```

Gas simulation at offset 10684 with total cost of 100:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r7 = i16 [r6 + 0x211]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r8 = i16 [r6 + 0x213]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r9 = i16 [r6 + 0x215]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r10 = i16 [r6 + 0x217]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  r11 = i16 [r6 + 0x219]
    .D========================eE------------------------R..................................................  r8 = r8 << 0x1
    .D========================eE------------------------R..................................................  r9 = r9 << 0x1
    .D========================eE------------------------R..................................................  r10 = r10 << 0x1
    ..D========================eE-----------------------R..................................................  r7 = r7 + 0x1
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER................................................  u16 [r6 + 0x211] = r7
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R................................................  u16 [r6 + 0x213] = r8
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R................................................  u16 [r6 + 0x215] = r9
    ...D===============================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u16 [r6 + 0x217] = r10
    ...D================================================eE-----------------------R.........................  r11 = r11 << 0x1
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.......................  u16 [r6 + 0x219] = r11
    ...D================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-R.......................  r0 = u64 [r1 + 0x10]
    ....D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.......................  r5 = u64 [r1 + 0x8]
    ....D=======================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0]
    ....D========================================================================eE-----------------------R  r1 = r1 + 0x18
    ....D========================================================================eeeeeeeeeeeeeeeeeeeeeeE--R  jump [r0 + 0]
```

Gas simulation at offset 10752 with total cost of 26:

```
    DeER.........................  r1 = r1 + 0xffffffffffffffe8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x10] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x8] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0] = r6
    .D...........................  r5 = r7
    .DeE------------------------R  r6 = r7 + 0x7ff
    .DeeeeeeeeeeeeeeeE----------R  r0 = 268, jump 6954
```

Gas simulation at offset 10775 with total cost of 27:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u16 [r6 + 0x21b]
    D=========================eER.  r7 = r8 >> 0x8
    D==========================eER  jump 10834 if r7 >=u 63
```

Gas simulation at offset 10786 with total cost of 74:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r9 = u64 [r6 + 0x241]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r7 = u64 [r6 + 0x249]
    DeE---------------------------------------R..................................  r10 = 0x17c80
    .D========================eeE-------------R..................................  r10 = r7 if r9 != 0
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r10 = u64 [r10 + 0x48]
    ..DeE-------------------------------------------------R......................  r7 = r6 + 0x27f
    ..D=======================eeE-------------------------R......................  r7 = r9 if r9 != 0
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 270, jump [r10 + 0]
```

Gas simulation at offset 10818 with total cost of 27:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u8 [r6 + 0x227]
    D=========================eER.  r8 = r8 & 0x18
    DeeeeeeeeeeeeeeeeeeeeeeeeeE-R.  u8 [r6 + 0x22d] = a0
    D==========================eER  jump 10863 if r8 != 0
```

Gas simulation at offset 10832 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 10899
```

Gas simulation at offset 10834 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeE---------------------------------------R.............  r8 = r8 & 0x1f
    D=eE--------------------------------------R.............  r8 = r8 + r5
    .D=eE-------------------------------------R.............  r7 = r8 + 0x7ff
    .D==eeeeeeeeeeeeeeeeeeeeeeeeeE------------R.............  r7 = u8 [r7 + 0x1a1]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.............  r8 = u8 [r6 + 0x227]
    ..D========================eE-------------R.............  r8 = r8 & 0x18
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x22d] = a0
    ..D=========================eE-------------------------R  jump 10899 if r8 == 0
```

Gas simulation at offset 10863 with total cost of 46:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER......  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R......  r8 = u16 [r6 + 0x209]
    D=========================eE--------------R......  r9 = r8 & 0x1f
    .D========================eE--------------R......  r8 = r8 & 0xffffffffffffffe0
    .D=========================eeeeeeeeeeeeeeeeeeeeER  jump 10888 if r9 != 31
```

Gas simulation at offset 10878 with total cost of 26:

```
    DeER.........................  r8 = r8 ^ 0x400
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r6 + 0x209] = r8
    DeeeeeeeeeeeeeeeE-----------R  jump 10899
```

Gas simulation at offset 10888 with total cost of 27:

```
    DeER..........................  r8 = r8 | r9
    D=eER.........................  r8 = r8 + 0x1
    D==eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r6 + 0x209] = r8
    DeeE-------------------------R  fallthrough
```

Gas simulation at offset 10899 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r8 = u8 [r6 + 0x22b]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r9 = u8 [r6 + 0x22c]
    .D========================eE--------------R.............  r10 = r8 << 0x3f
    .D========================eE--------------R.............  r8 = r8 << 0x6
    .D=========================eE-------------R.............  r10 = r10 >>a 0x3f
    ..D========================eE-------------R.............  r8 = sext8 r8
    ..D=========================eE------------R.............  r8 = r8 >> 0x7
    ..D=======================eeeeeeeeeeeeeeeeeeeeeeeeeER...  u8 [r6 + 0x213] = a2
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-----------------------R...  u8 [r6 + 0x215] = a0
    ...D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u8 [r6 + 0x217] = a3
    ...D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x219] = a1
    ...D....................................................  r7 = r5
    ...DeeeeeeeeeeeeeeeE-----------------------------------R  r0 = 272, jump 7236
```

Gas simulation at offset 10946 with total cost of 15:

```
    D.................  r7 = r5
    DeeeeeeeeeeeeeeeER  r0 = 274, jump 6145
```

Gas simulation at offset 10954 with total cost of 100:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r7 = i16 [r6 + 0x211]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r8 = i16 [r6 + 0x213]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r9 = i16 [r6 + 0x215]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r10 = i16 [r6 + 0x217]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  r11 = i16 [r6 + 0x219]
    .D========================eE------------------------R..................................................  r8 = r8 << 0x1
    .D========================eE------------------------R..................................................  r9 = r9 << 0x1
    .D========================eE------------------------R..................................................  r10 = r10 << 0x1
    ..D========================eE-----------------------R..................................................  r7 = r7 + 0x1
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER................................................  u16 [r6 + 0x211] = r7
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R................................................  u16 [r6 + 0x213] = r8
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R................................................  u16 [r6 + 0x215] = r9
    ...D===============================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u16 [r6 + 0x217] = r10
    ...D================================================eE-----------------------R.........................  r11 = r11 << 0x1
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.......................  u16 [r6 + 0x219] = r11
    ...D================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-R.......................  r0 = u64 [r1 + 0x10]
    ....D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.......................  r5 = u64 [r1 + 0x8]
    ....D=======================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0]
    ....D========================================================================eE-----------------------R  r1 = r1 + 0x18
    ....D========================================================================eeeeeeeeeeeeeeeeeeeeeeE--R  jump [r0 + 0]
```

Gas simulation at offset 11022 with total cost of 26:

```
    DeER.........................  r1 = r1 + 0xffffffffffffffe8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x10] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x8] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0] = r6
    .D...........................  r5 = r7
    .DeE------------------------R  r6 = r7 + 0x7ff
    .DeeeeeeeeeeeeeeeE----------R  r0 = 278, jump 6954
```

Gas simulation at offset 11045 with total cost of 27:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u16 [r6 + 0x21b]
    D=========================eER.  r7 = r8 >> 0x8
    D==========================eER  jump 11104 if r7 >=u 63
```

Gas simulation at offset 11056 with total cost of 74:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r9 = u64 [r6 + 0x241]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r7 = u64 [r6 + 0x249]
    DeE---------------------------------------R..................................  r10 = 0x17c80
    .D========================eeE-------------R..................................  r10 = r7 if r9 != 0
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r10 = u64 [r10 + 0x48]
    ..DeE-------------------------------------------------R......................  r7 = r6 + 0x27f
    ..D=======================eeE-------------------------R......................  r7 = r9 if r9 != 0
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 280, jump [r10 + 0]
```

Gas simulation at offset 11088 with total cost of 27:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u8 [r6 + 0x227]
    D=========================eER.  r8 = r8 & 0x18
    DeeeeeeeeeeeeeeeeeeeeeeeeeE-R.  u8 [r6 + 0x22d] = a0
    D==========================eER  jump 11133 if r8 != 0
```

Gas simulation at offset 11102 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 11169
```

Gas simulation at offset 11104 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeE---------------------------------------R.............  r8 = r8 & 0x1f
    D=eE--------------------------------------R.............  r8 = r8 + r5
    .D=eE-------------------------------------R.............  r7 = r8 + 0x7ff
    .D==eeeeeeeeeeeeeeeeeeeeeeeeeE------------R.............  r7 = u8 [r7 + 0x1a1]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.............  r8 = u8 [r6 + 0x227]
    ..D========================eE-------------R.............  r8 = r8 & 0x18
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x22d] = a0
    ..D=========================eE-------------------------R  jump 11169 if r8 == 0
```

Gas simulation at offset 11133 with total cost of 46:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER......  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R......  r9 = u16 [r6 + 0x209]
    D=========================eE--------------R......  r10 = r9 & 0x1f
    .D========================eE--------------R......  r9 = r9 & 0xffffffffffffffe0
    .D=========================eeeeeeeeeeeeeeeeeeeeER  jump 11158 if r10 != 31
```

Gas simulation at offset 11148 with total cost of 26:

```
    DeER.........................  r9 = r9 ^ 0x400
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r6 + 0x209] = r9
    DeeeeeeeeeeeeeeeE-----------R  jump 11169
```

Gas simulation at offset 11158 with total cost of 27:

```
    DeER..........................  r9 = r9 | r10
    D=eER.........................  r9 = r9 + 0x1
    D==eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r6 + 0x209] = r9
    DeeE-------------------------R  fallthrough
```

Gas simulation at offset 11169 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r9 = u8 [r6 + 0x22b]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r10 = u8 [r6 + 0x22c]
    .D========================eE--------------R.............  r11 = r9 << 0x3f
    .D========================eE--------------R.............  r9 = r9 << 0x6
    .D=========================eE-------------R.............  r11 = r11 >>a 0x3f
    ..D========================eE-------------R.............  r9 = sext8 r9
    ..D=========================eE------------R.............  r9 = r9 >> 0x7
    ..D=======================eeeeeeeeeeeeeeeeeeeeeeeeeER...  u8 [r6 + 0x213] = a3
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-----------------------R...  u8 [r6 + 0x215] = a0
    ...D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u8 [r6 + 0x217] = a4
    ...D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x219] = a2
    ...DeE-------------------------------------------------R  jump 11326 if r8 == 0
```

Gas simulation at offset 11211 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.......  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r7 = u16 [r6 + 0x209]
    DeE---------------------------------------R.......  r10 = 0x7
    .D========================eE--------------R.......  r9 = r7 << 0x31
    .D=========================eE-------------R.......  r9 = r9 >> 0x3d
    .DeE--------------------------------------R.......  r8 = 0x8c1f
    ..D=========================eeeeeeeeeeeeeeeeeeeeER  jump 11262 if r9 != r10
```

Gas simulation at offset 11233 with total cost of 22:

```
    DeER.....................  r9 = r7 >> 0x5
    D=eER....................  r10 = r9 & 0x1f
    .DeER....................  r11 = 0x1d
    .D=eeeeeeeeeeeeeeeeeeeeER  jump 11285 if r10 == r11
```

Gas simulation at offset 11245 with total cost of 21:

```
    DeER....................  r11 = 0x1f
    D=eeeeeeeeeeeeeeeeeeeeER  jump 11303 if r10 != r11
```

Gas simulation at offset 11251 with total cost of 26:

```
    DeER.........................  r7 = r7 & 0x8c1f
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r6 + 0x209] = r7
    DeeeeeeeeeeeeeeeE-----------R  jump 11326
```

Gas simulation at offset 11262 with total cost of 28:

```
    DeER...........................  r9 = r9 + 0x1
    DeER...........................  r8 = 0x8fff
    D=eER..........................  r7 = r7 & r8
    D=eER..........................  r9 = r9 << 0xc
    .D=eER.........................  r7 = r7 | r9
    .D==eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r6 + 0x209] = r7
    .DeeeeeeeeeeeeeeeE------------R  jump 11326
```

Gas simulation at offset 11285 with total cost of 27:

```
    DeER..........................  r7 = r7 & 0x8c1f
    DeER..........................  r8 = 0x800
    D=eER.........................  r7 = r7 ^ r8
    D==eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r6 + 0x209] = r7
    .DeeeeeeeeeeeeeeeE-----------R  jump 11326
```

Gas simulation at offset 11303 with total cost of 29:

```
    DeER............................  r9 = r9 << 0x5
    DeER............................  r7 = r7 & 0x8c1f
    D=eER...........................  r8 = r9 + 0x20
    .D=eER..........................  r8 = r8 & 0x3e0
    .D==eER.........................  r7 = r7 | r8
    .D===eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r6 + 0x209] = r7
    .DeeE--------------------------R  fallthrough
```

Gas simulation at offset 11326 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r7 = i16 [r6 + 0x211]
    D=========================eE--------------R...........  r7 = r7 + 0x1
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r6 + 0x211] = r7
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r0 = u64 [r1 + 0x10]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r5 = u64 [r1 + 0x8]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r6 = u64 [r1 + 0]
    .D=========================eE------------------------R  r1 = r1 + 0x18
    ..D========================eeeeeeeeeeeeeeeeeeeeeeE---R  jump [r0 + 0]
```

Gas simulation at offset 11351 with total cost of 54:

```
    DeER.....................................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER............................  r8 = u16 [r7 + 0x209]
    DeE-------------------------R............................  r9 = 0x1
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER............................  r11 = u8 [r7 + 0x227]
    .D=========================eER...........................  r12 = r8 << 0x34
    .D==========================eER..........................  r12 = r12 >> 0x34
    ..D==========================eER.........................  r10 = r12 | 0x2000
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE--R.........................  r12 = u8 [r7 + 0x1c1]
    ..D========================eE--R.........................  r11 = r11 & 0x18
    ...D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r7 + 0x21b] = r10
    ...DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R  u8 [r7 + 0x231] = a2
    ...D========================eeeeeeeeeeeeeeeeeeeeeeeeeE--R  u8 [r7 + 0x232] = a5
    ...D========================eeeeeeeeeeeeeeeeeeeeeeeeeE--R  u8 [r7 + 0x234] = a5
    ....D========================eE-------------------------R  jump 11423 if r11 == 0
```

Gas simulation at offset 11402 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  r9 = u16 [r7 + 0x20b]
    DeE---------------------------------------R............  r8 = r8 & 0xfffffffffffffbe0
    D=========================eE--------------R............  r9 = r9 & 0x41f
    .D=========================eE-------------R............  r8 = r8 | r9
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r7 + 0x209] = r8
    .DeeE-------------------------------------------------R  fallthrough
```

Gas simulation at offset 11423 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r8 = i16 [r7 + 0x211]
    D=========================eE--------------R...........  r8 = r8 + 0x1
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r7 + 0x211] = r8
    .DeeeeeeeeeeeeeeeeeeeeeeE----------------------------R  jump [r0 + 0]
```

Gas simulation at offset 11437 with total cost of 79:

```
    DeER..............................................................................  r1 = r1 + 0xfffffffffffffff0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.....................................................  u64 [r1 + 0x8] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.....................................................  u64 [r1 + 0] = r5
    .DeE------------------------R.....................................................  r5 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER....................................................  r9 = u8 [r5 + 0x231]
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER....................................................  r8 = u16 [r5 + 0x21b]
    ..DeE------------------------R....................................................  r10 = 0x3f
    ..D=========================eER...................................................  r11 = r7 + r9
    ..D==========================eER..................................................  r11 = r11 + 0x7ff
    ...D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r11 = u8 [r11 + 0x1c1]
    ...D========================eE--------------------------R.........................  r9 = r9 + 0x1
    ...D========================eE--------------------------R.........................  r12 = r8 >> 0x8
    ....D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R.........................  u8 [r5 + 0x231] = a2
    ....D==================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x232] = a4
    ....D==================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x233] = a4
    ....D========================eE--------------------------------------------------R  jump 11526 if r12 >=u r10
```

Gas simulation at offset 11492 with total cost of 74:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r9 = u64 [r5 + 0x241]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r7 = u64 [r5 + 0x249]
    DeE---------------------------------------R..................................  r10 = 0x17c80
    .D========================eeE-------------R..................................  r10 = r7 if r9 != 0
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r10 = u64 [r10 + 0x48]
    ..DeE-------------------------------------------------R......................  r7 = r5 + 0x27f
    ..D=======================eeE-------------------------R......................  r7 = r9 if r9 != 0
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 286, jump [r10 + 0]
```

Gas simulation at offset 11524 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 11541
```

Gas simulation at offset 11526 with total cost of 28:

```
    DeER...........................  r8 = r8 & 0x1f
    D=eER..........................  r7 = r7 + r8
    D==eER.........................  r7 = r7 + 0x7ff
    D===eeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u8 [r7 + 0x1a1]
    .DeeE-------------------------R  fallthrough
```

Gas simulation at offset 11541 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r8 = i16 [r5 + 0x211]
    D=========================eER.........................  r8 = r8 + 0x1
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x211] = r8
    DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R  u8 [r5 + 0x22a] = a0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r0 = u64 [r1 + 0x8]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r5 = u64 [r1 + 0]
    .D========================eE-------------------------R  r1 = r1 + 0x10
    .D=========================eeeeeeeeeeeeeeeeeeeeeeE---R  jump [r0 + 0]
```

Gas simulation at offset 11566 with total cost of 79:

```
    DeER..............................................................................  r8 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.....................................................  r10 = u16 [r8 + 0x209]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.....................................................  r4 = u16 [r8 + 0x211]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER.....................................................  r12 = u8 [r8 + 0x231]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER.....................................................  r11 = u8 [r8 + 0x236]
    .DeE------------------------R.....................................................  r2 = 0xc00
    .D=eE-----------------------R.....................................................  r3 = 0x40
    ..D========================eER....................................................  r9 = r7 + r12
    ..D========================eER....................................................  r11 = r11 << 0x2
    ..D=========================eER...................................................  r9 = r9 + 0x7ff
    ...D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r9 = u8 [r9 + 0x1c1]
    ...D=======================eE--------------------------R..........................  r12 = r12 + 0x1
    ...D========================eE-------------------------R..........................  r7 = r7 + r11
    ...D=========================eE------------------------R..........................  r7 = r7 + 0x7ff
    ....D=================================================eER.........................  r11 = r9 & 0xffffffffffffffe3
    ....D==================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x1e3] = a4
    .....D=====================eE----------------------------------------------------R  r7 = r4 + 0xfffffffffffffeff
    .....D======================eeeeeeeeeeeeeeeeeeeeeeeeeE---------------------------R  u8 [r8 + 0x231] = a5
    .....D================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-R  u8 [r8 + 0x232] = a2
    ......D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r8 + 0x235] = a4
    ......D=====================eE---------------------------------------------------R  r9 = r10 >> 0x4
    ......D======================eE--------------------------------------------------R  r11 = zext16 r7
    .......D======================eE-------------------------------------------------R  r7 = r9 & 0x38
    .......D======================eeeeeeeeeeeeeeeeeeeeE------------------------------R  jump 11678 if r11 >=u r3
```

Gas simulation at offset 11651 with total cost of 28:

```
    DeER...........................  r9 = r10 & 0xcff
    DeER...........................  r10 = 0x2000
    D=eER..........................  r9 = r9 | r10
    .D=eER.........................  r7 = r7 + r9
    .DeE-R.........................  r4 = r4 + 0x1
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER.  u16 [r8 + 0x211] = r4
    .D==eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r8 + 0x21b] = r7
    ..DeeeeeeeeeeeeeeeeeeeeeeE----R  jump [r0 + 0]
```

Gas simulation at offset 11678 with total cost of 29:

```
    DeER............................  r9 = r10 & 0xc00
    DeER............................  r10 = r10 << 0x3b
    D=eER...........................  r10 = r10 >> 0x3d
    .D=eER..........................  r9 = r9 | r10
    .DeE-R..........................  r10 = 0x23c0
    .D=eER..........................  r7 = r7 | r10
    .D==eER.........................  r7 = r7 | r9
    ..DeE-R.........................  r4 = r4 + 0x1
    ..D=eeeeeeeeeeeeeeeeeeeeeeeeeER.  u16 [r8 + 0x211] = r4
    ..D==eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r8 + 0x21b] = r7
    ..DeeeeeeeeeeeeeeeeeeeeeeE-----R  jump [r0 + 0]
```

Gas simulation at offset 11714 with total cost of 79:

```
    DeER..............................................................................  r1 = r1 + 0xfffffffffffffff0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.....................................................  u64 [r1 + 0x8] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.....................................................  u64 [r1 + 0] = r5
    .DeE------------------------R.....................................................  r5 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER....................................................  r8 = u8 [r5 + 0x231]
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER....................................................  r9 = u8 [r5 + 0x236]
    ..D=========================eER...................................................  r8 = r8 + r7
    ..D==========================eER..................................................  r8 = r8 + 0x7ff
    ..D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r10 = u8 [r8 + 0x1c1]
    ..D=========================eE--------------------------R.........................  r9 = r9 << 0x2
    ...D=========================eE-------------------------R.........................  r9 = r9 + r7
    ...D==========================eE------------------------R.........................  r8 = r9 + 0x7ff
    ...D===================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r8 + 0x1e4] = a3
    ....D======================eeeeeeeeeeeeeeeeeeeeeeeeeE----------------------------R  r8 = u16 [r5 + 0x21b]
    ....D===============================================eE---------------------------R  r9 = r8 >> 0x8
    ....DeE--------------------------------------------------------------------------R  r11 = 0x3f
    .....D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x232] = a3
    .....D===============================================eE--------------------------R  jump 11810 if r9 >=u r11
```

Gas simulation at offset 11776 with total cost of 74:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r9 = u64 [r5 + 0x241]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r7 = u64 [r5 + 0x249]
    DeE---------------------------------------R..................................  r10 = 0x17c80
    .D========================eeE-------------R..................................  r10 = r7 if r9 != 0
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r10 = u64 [r10 + 0x48]
    ..DeE-------------------------------------------------R......................  r7 = r5 + 0x27f
    ..D=======================eeE-------------------------R......................  r7 = r9 if r9 != 0
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 292, jump [r10 + 0]
```

Gas simulation at offset 11808 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 11825
```

Gas simulation at offset 11810 with total cost of 28:

```
    DeER...........................  r8 = r8 & 0x1f
    D=eER..........................  r7 = r7 + r8
    D==eER.........................  r7 = r7 + 0x7ff
    D===eeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u8 [r7 + 0x1a1]
    .DeeE-------------------------R  fallthrough
```

Gas simulation at offset 11825 with total cost of 55:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..............................  r8 = u8 [r5 + 0x209]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..............................  r9 = i16 [r5 + 0x211]
    D=========================eER.............................  r10 = r8 & 0x2
    .D========================eER.............................  r8 = r8 >> 0x4
    .D=========================eER............................  r8 = r8 & 0x4
    .D==========================eER...........................  r8 = r8 | r10
    .DeE--------------------------R...........................  r7 = r7 & 0xff
    ..D========================eE-R...........................  r9 = r9 + 0x1
    ..D==========================eER..........................  r7 = r7 >> r8
    ..D===========================eER.........................  r7 = r7 & 0x3
    ...D========================eeeeeeeeeeeeeeeeeeeeeeeeeER...  u16 [r5 + 0x211] = r9
    ...D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x22b] = a0
    ...DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------------------R  r0 = u64 [r1 + 0x8]
    ...DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------------------R  r5 = u64 [r1 + 0]
    ....D========================eE--------------------------R  r1 = r1 + 0x10
    ....D========================eeeeeeeeeeeeeeeeeeeeeeE-----R  jump [r0 + 0]
```

Gas simulation at offset 11876 with total cost of 78:

```
    DeER.............................................................................  r8 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER....................................................  r11 = u8 [r8 + 0x231]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER....................................................  r12 = u8 [r8 + 0x226]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER....................................................  r9 = u8 [r8 + 0x233]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER....................................................  r10 = i8 [r8 + 0x235]
    .D=========================eER...................................................  r7 = r7 + r11
    .D==========================eER..................................................  r7 = r7 + 0x7ff
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r7 = u8 [r7 + 0x1c1]
    ..D========================eE--------------------------R.........................  r11 = r12 & 0x20
    ..D===================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r8 + 0x232] = a0
    ...D========================eE--------------------------------------------------R  jump 11961 if r11 != 0
```

Gas simulation at offset 11917 with total cost of 55:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...............  r7 = i16 [r8 + 0x20f]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...............  r11 = u8 [r8 + 0x234]
    DeE---------------------------------------R...............  r10 = r10 >>a 0x3f
    .D========================eeE-------------R...............  i32 r7 = r7 - r11
    .D==========================eE------------R...............  r7 = r7 ^ r10
    .D===========================eE-----------R...............  r7 = r7 & 0x7
    ..DeE-------------------------------------R...............  r9 = r9 << 0x4
    ..D===========================eE----------R...............  r7 = r7 | r9
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------R...............  r9 = i16 [r8 + 0x211]
    ..D=========================eE------------R...............  r9 = r9 + 0x1
    ...D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER..  u16 [r8 + 0x211] = r9
    ...D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r8 + 0x21b] = a0
    ...DeeeeeeeeeeeeeeeeeeeeeeE------------------------------R  jump [r0 + 0]
```

Gas simulation at offset 11961 with total cost of 63:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.......................  unlikely
    DeeeE-------------------------------------R.......................  r7 = r10 <s 0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......................  r10 = i16 [r8 + 0x20f]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......................  r11 = u8 [r8 + 0x234]
    .DeE--------------------------------------R.......................  r9 = r9 & 0xe
    .DeE--------------------------------------R.......................  r12 = 0xfffffffffffffff8
    ..DeE-------------------------------------R.......................  r2 = 0x7
    ..D========================eeE------------R.......................  i32 r10 = r10 - r11
    ..D==========================eE-----------R.......................  r10 = r10 & 0xf
    ...D==========================eeeE--------R.......................  r11 = r10 <u 0x8
    ....D============================eeE------R.......................  r12 = 0 if r11 != 0
    ....D============================eE-------R.......................  r11 = r11 ^ r7
    .....D=============================eE-----R.......................  r10 = r10 + r12
    .....D============================eE------R.......................  r11 = r11 ^ 0x1
    .....D=============================eE-----R.......................  r9 = r9 | r11
    ......D=============================eE----R.......................  r11 = r2 - r10
    ......D=============================eeE---R.......................  r11 = r10 if r7 == 0
    .......D============================eE----R.......................  r7 = r9 << 0x4
    .......D==============================eE--R.......................  r7 = r7 + r11
    .......DeeeeeeeeeeeeeeeeeeeeeeeeeE--------R.......................  r9 = i16 [r8 + 0x211]
    ........D========================eE-------R.......................  r9 = r9 + 0x1
    ........D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER.....  u16 [r8 + 0x211] = r9
    ........D==============================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r8 + 0x21b] = a0
    ........DeeeeeeeeeeeeeeeeeeeeeeE---------------------------------R  jump [r0 + 0]
```

Gas simulation at offset 12033 with total cost of 79:

```
    DeER..............................................................................  r1 = r1 + 0xffffffffffffffe8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.....................................................  u64 [r1 + 0x10] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.....................................................  u64 [r1 + 0x8] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.....................................................  u64 [r1 + 0] = r6
    .D................................................................................  r5 = r7
    .DeE------------------------R.....................................................  r6 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER....................................................  r9 = u8 [r6 + 0x231]
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER............................  r7 = u8 [r6 + 0x226]
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER............................  r8 = u8 [r6 + 0x233]
    ..D=========================eE-----------------------R............................  r9 = r9 + r5
    ..D==========================eE----------------------R............................  r9 = r9 + 0x7ff
    ...D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r9 = u8 [r9 + 0x1c1]
    ...D================================================eE--R.........................  r10 = r7 & 0x20
    ...D===================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x232] = a2
    ....D===============================================eE---------------------------R  r9 = r8 << 0x4
    ....D================================================eE--------------------------R  jump 12143 if r10 != 0
```

Gas simulation at offset 12086 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeE---------------------------------------R  r7 = r7 & 0x8
    D=eE--------------------------------------R  r7 = r7 << 0x9
    D==eE-------------------------------------R  r7 = r7 | r9
    .D==eE------------------------------------R  r7 = r7 >> 0x8
    .D===eeeeeeeeeeeeeeeeeeeeeeeeeE-----------R  u8 [r6 + 0x21c] = a0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R  r8 = u16 [r6 + 0x21b]
    ..D========================eE-------------R  r7 = r8 >> 0x8
    ..DeE-------------------------------------R  r9 = 0x3f
    ..D=========================eE------------R  jump 12172 if r7 <u r9
```

Gas simulation at offset 12116 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.......  unlikely
    DeE---------------------------------------R.......  r8 = r8 & 0x1f
    D=eE--------------------------------------R.......  r8 = r8 + r5
    .D=eE-------------------------------------R.......  r7 = r8 + 0x7ff
    .D==eeeeeeeeeeeeeeeeeeeeeeeeeE------------R.......  r7 = u8 [r7 + 0x1a1]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......  r8 = u8 [r6 + 0x235]
    ..D========================eE-------------R.......  r8 = r8 & 0x40
    ..D=========================eeeeeeeeeeeeeeeeeeeeER  jump 12214 if r8 != 0
```

Gas simulation at offset 12141 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 12261
```

Gas simulation at offset 12143 with total cost of 29:

```
    DeER............................  r8 = r8 << 0xc
    D=eER...........................  r8 = r8 | r9
    D==eER..........................  r7 = r8 << 0x33
    .D==eER.........................  r7 = r7 >> 0x3b
    .D===eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x21c] = a0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE---R  r8 = u16 [r6 + 0x21b]
    ..D========================eE--R  r7 = r8 >> 0x8
    ..DeE--------------------------R  r9 = 0x3f
    ..D=========================eE-R  jump 12116 if r7 >=u r9
```

Gas simulation at offset 12172 with total cost of 74:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r9 = u64 [r6 + 0x241]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r7 = u64 [r6 + 0x249]
    DeE---------------------------------------R..................................  r10 = 0x17c80
    .D========================eeE-------------R..................................  r10 = r7 if r9 != 0
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r10 = u64 [r10 + 0x48]
    ..DeE-------------------------------------------------R......................  r7 = r6 + 0x27f
    ..D=======================eeE-------------------------R......................  r7 = r9 if r9 != 0
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 298, jump [r10 + 0]
```

Gas simulation at offset 12204 with total cost of 27:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u8 [r6 + 0x235]
    D=========================eER.  r8 = r8 & 0x40
    D==========================eER  jump 12261 if r8 == 0
```

Gas simulation at offset 12214 with total cost of 11:

```
    DeER..........  r8 = r7 & 0xff
    DeER..........  r9 = r7 << 0xb
    .DeER.........  r10 = r8 << 0x1
    .D=eER........  r9 = r9 | r10
    .DeE-R........  r10 = 0x22110
    ..DeER........  r7 = r7 << 0xf
    ..DeER........  r8 = r8 << 0x5
    ..D=eER.......  r7 = r7 | r8
    ..D=eER.......  r9 = r9 & r10
    ...D=eER......  r7 = r7 & 0x88440
    ...D==eER.....  r7 = r7 | r9
    ...D===eeeER..  r7 = r7 * 0x10101
    ....D=====eeER  i32 r7 = r7 >> 0x10
    ....DeeE-----R  fallthrough
```

Gas simulation at offset 12261 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r8 = u8 [r6 + 0x236]
    D=========================eE--------------R.............  r8 = r8 << 0x2
    D==========================eE-------------R.............  r8 = r8 + r5
    .D==========================eE------------R.............  r8 = r8 + 0x7ff
    .D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r8 + 0x1e1] = a0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------------------R  r7 = i16 [r6 + 0x211]
    .D=========================eE--------------------------R  r7 = r7 + 0x1
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R  u16 [r6 + 0x211] = r7
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R  r0 = u64 [r1 + 0x10]
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R  r5 = u64 [r1 + 0x8]
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R  r6 = u64 [r1 + 0]
    ...D========================eE-------------------------R  r1 = r1 + 0x18
    ...D========================eeeeeeeeeeeeeeeeeeeeeeE----R  jump [r0 + 0]
```

Gas simulation at offset 12304 with total cost of 78:

```
    DeER.............................................................................  r8 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER....................................................  r11 = u8 [r8 + 0x231]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER....................................................  r12 = u8 [r8 + 0x226]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER....................................................  r9 = u8 [r8 + 0x233]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER....................................................  r10 = i8 [r8 + 0x235]
    .D=========================eER...................................................  r7 = r7 + r11
    .D==========================eER..................................................  r7 = r7 + 0x7ff
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r7 = u8 [r7 + 0x1c1]
    ..D========================eE--------------------------R.........................  r11 = r12 & 0x20
    ..D===================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r8 + 0x232] = a0
    ...D========================eE--------------------------------------------------R  jump 12392 if r11 != 0
```

Gas simulation at offset 12345 with total cost of 56:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R................  r7 = i16 [r8 + 0x20f]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R................  r11 = u8 [r8 + 0x234]
    DeE---------------------------------------R................  r10 = r10 >>a 0x3f
    .D========================eeE-------------R................  i32 r7 = r7 - r11
    .D==========================eE------------R................  r7 = r7 ^ r10
    .D===========================eE-----------R................  r7 = r7 & 0x7
    ..DeE-------------------------------------R................  r9 = r9 << 0x4
    ..D===========================eE----------R................  r7 = r7 | r9
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------R................  r9 = i16 [r8 + 0x211]
    ..D============================eE---------R................  r7 = r7 + 0x8
    ...D========================eE------------R................  r9 = r9 + 0x1
    ...D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER...  u16 [r8 + 0x211] = r9
    ...D============================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r8 + 0x21b] = a0
    ...DeeeeeeeeeeeeeeeeeeeeeeE-------------------------------R  jump [r0 + 0]
```

Gas simulation at offset 12392 with total cost of 64:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER........................  unlikely
    DeeeE-------------------------------------R........................  r7 = r10 <s 0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R........................  r10 = i16 [r8 + 0x20f]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R........................  r11 = u8 [r8 + 0x234]
    .DeE--------------------------------------R........................  r9 = r9 & 0xe
    .DeE--------------------------------------R........................  r12 = 0xfffffffffffffff8
    ..DeE-------------------------------------R........................  r2 = 0x7
    ..D========================eeE------------R........................  i32 r10 = r10 - r11
    ..D==========================eE-----------R........................  r10 = r10 & 0xf
    ...D==========================eeeE--------R........................  r11 = r10 <u 0x8
    ....D============================eeE------R........................  r12 = 0 if r11 != 0
    ....D============================eE-------R........................  r11 = r11 ^ r7
    .....D=============================eE-----R........................  r10 = r10 + r12
    .....D============================eE------R........................  r11 = r11 ^ 0x1
    .....D=============================eE-----R........................  r9 = r9 | r11
    ......D=============================eE----R........................  r11 = r2 - r10
    ......D=============================eeE---R........................  r11 = r10 if r7 == 0
    .......D============================eE----R........................  r7 = r9 << 0x4
    .......D==============================eE--R........................  r7 = r7 + r11
    .......DeeeeeeeeeeeeeeeeeeeeeeeeeE--------R........................  r9 = i16 [r8 + 0x211]
    ........D==============================eE-R........................  r7 = r7 + 0x8
    ........D========================eE-------R........................  r9 = r9 + 0x1
    ........D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER......  u16 [r8 + 0x211] = r9
    ........D===============================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r8 + 0x21b] = a0
    .........DeeeeeeeeeeeeeeeeeeeeeeE---------------------------------R  jump [r0 + 0]
```

Gas simulation at offset 12467 with total cost of 79:

```
    DeER..............................................................................  r1 = r1 + 0xffffffffffffffe8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.....................................................  u64 [r1 + 0x10] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.....................................................  u64 [r1 + 0x8] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.....................................................  u64 [r1 + 0] = r6
    .D................................................................................  r5 = r7
    .DeE------------------------R.....................................................  r6 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER....................................................  r9 = u8 [r6 + 0x231]
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER............................  r8 = u8 [r6 + 0x226]
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER............................  r7 = u8 [r6 + 0x233]
    ..D=========================eE-----------------------R............................  r10 = r5 + r9
    ...D=========================eE----------------------R............................  r10 = r10 + 0x7ff
    ...D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r10 = u8 [r10 + 0x1c1]
    ...D========================eE--------------------------R.........................  r9 = r9 + 0x1
    ....D===============================================eE--R.........................  r11 = r8 & 0x20
    ....D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R.........................  u8 [r6 + 0x231] = a2
    ....D==================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x232] = a3
    .....D===============================================eeeeeeeeeeeeeeeeeeeeE-------R  jump 12538 if r11 != 0
```

Gas simulation at offset 12524 with total cost of 16:

```
    DeER...............  r8 = r8 & 0x8
    D=eER..............  r8 = r8 << 0x9
    DeE-R..............  r7 = r7 << 0x4
    D==eER.............  r7 = r7 | r8
    .DeeeeeeeeeeeeeeeER  jump 12607
```

Gas simulation at offset 12538 with total cost of 38:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.............  r8 = i16 [r6 + 0x20f]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.............  r9 = u8 [r6 + 0x234]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.............  r10 = i8 [r6 + 0x235]
    .DeE-----------------------R.............  r11 = r7 & 0x1
    .D=eE----------------------R.............  r7 = r7 & 0xfe
    .DeE-----------------------R.............  r12 = 0xfffffffffffffff8
    ..DeE----------------------R.............  r2 = 0x7
    ..D=eE---------------------R.............  r11 = r11 << 0xc
    ...D======================eeeER..........  r10 = r10 <s 0
    ....D=====================eeE-R..........  i32 r8 = r8 - r9
    ....D=======================eER..........  r8 = r8 & 0xf
    .....D=======================eeeER.......  r9 = r8 <u 0x8
    ......D=========================eeER.....  r12 = 0 if r9 != 0
    ......D=========================eE-R.....  r9 = r9 ^ r10
    .......D==========================eER....  r8 = r8 + r12
    .......D=========================eE-R....  r9 = r9 ^ 0x1
    .......D==========================eER....  r7 = r7 | r9
    ........D==========================eER...  r9 = r2 - r8
    ........D==========================eeER..  r9 = r8 if r10 == 0
    .........D=========================eE-R..  r7 = r7 << 0x4
    .........D===========================eER.  r9 = r9 + r11
    .........D============================eER  r7 = r7 + r9
    .........DeeE---------------------------R  fallthrough
```

Gas simulation at offset 12607 with total cost of 27:

```
    DeER..........................  r7 = r7 + 0x8
    D=eER.........................  r7 = r7 >> 0x8
    D==eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x21c] = a0
    DeeeeeeeeeeeeeeeeeeeeeeeeeE--R  r8 = u16 [r6 + 0x21b]
    .D========================eE-R  r7 = r8 >> 0x8
    .DeE-------------------------R  r9 = 0x3f
    .D=========================eER  jump 12674 if r7 >=u r9
```

Gas simulation at offset 12630 with total cost of 74:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r9 = u64 [r6 + 0x241]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r7 = u64 [r6 + 0x249]
    DeE---------------------------------------R..................................  r10 = 0x17c80
    .D========================eeE-------------R..................................  r10 = r7 if r9 != 0
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r10 = u64 [r10 + 0x48]
    ..DeE-------------------------------------------------R......................  r7 = r6 + 0x27f
    ..D=======================eeE-------------------------R......................  r7 = r9 if r9 != 0
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 304, jump [r10 + 0]
```

Gas simulation at offset 12662 with total cost of 46:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.....................  r8 = u8 [r6 + 0x235]
    D=========================eER....................  r8 = r8 & 0x40
    D==========================eeeeeeeeeeeeeeeeeeeeER  jump 12699 if r8 != 0
```

Gas simulation at offset 12672 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 12746
```

Gas simulation at offset 12674 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeE---------------------------------------R  r8 = r8 & 0x1f
    D=eE--------------------------------------R  r8 = r8 + r5
    .D=eE-------------------------------------R  r7 = r8 + 0x7ff
    .D==eeeeeeeeeeeeeeeeeeeeeeeeeE------------R  r7 = u8 [r7 + 0x1a1]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R  r8 = u8 [r6 + 0x235]
    ..D========================eE-------------R  r8 = r8 & 0x40
    ..D=========================eE------------R  jump 12746 if r8 == 0
```

Gas simulation at offset 12699 with total cost of 11:

```
    DeER..........  r8 = r7 & 0xff
    DeER..........  r9 = r7 << 0xb
    .DeER.........  r10 = r8 << 0x1
    .D=eER........  r9 = r9 | r10
    .DeE-R........  r10 = 0x22110
    ..DeER........  r7 = r7 << 0xf
    ..DeER........  r8 = r8 << 0x5
    ..D=eER.......  r7 = r7 | r8
    ..D=eER.......  r9 = r9 & r10
    ...D=eER......  r7 = r7 & 0x88440
    ...D==eER.....  r7 = r7 | r9
    ...D===eeeER..  r7 = r7 * 0x10101
    ....D=====eeER  i32 r7 = r7 >> 0x10
    ....DeeE-----R  fallthrough
```

Gas simulation at offset 12746 with total cost of 77:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.....................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.....................................  r8 = u8 [r6 + 0x236]
    D=========================eE--------------R.....................................  r8 = r8 << 0x2
    D==========================eE-------------R.....................................  r8 = r8 + r5
    .D==========================eE------------R.....................................  r8 = r8 + 0x7ff
    .D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER........................  u8 [r8 + 0x1e2] = a0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------------------R........................  r7 = u8 [r6 + 0x236]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------------------R........................  r8 = i16 [r6 + 0x211]
    ..D========================eE--------------------------R........................  r7 = r7 + 0x1
    ..D========================eE--------------------------R........................  r8 = r8 + 0x1
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R........................  u16 [r6 + 0x211] = r8
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R........................  u8 [r6 + 0x236] = a0
    ...DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R........................  r0 = u64 [r1 + 0x10]
    ...D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER........................  r5 = u64 [r1 + 0x8]
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0]
    ...D=================================================eE------------------------R  r1 = r1 + 0x18
    ....D========================eeeeeeeeeeeeeeeeeeeeeeE---------------------------R  jump [r0 + 0]
```

Gas simulation at offset 12800 with total cost of 78:

```
    DeER.............................................................................  r8 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER....................................................  r9 = u16 [r8 + 0x209]
    DeE-------------------------R....................................................  r10 = 0x2000
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER....................................................  r11 = i16 [r8 + 0x211]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER....................................................  r12 = u8 [r8 + 0x231]
    .D=========================eER...................................................  r9 = r9 << 0x34
    .D==========================eER..................................................  r9 = r9 >> 0x34
    ..D==========================eER.................................................  r9 = r9 | r10
    ..D========================eE--R.................................................  r7 = r7 + r12
    ..D========================eE--R.................................................  r12 = r12 + 0x1
    ..D========================eE--R.................................................  r11 = r11 + 0x1
    ...D========================eE-R.................................................  r7 = r7 + 0x7ff
    ...D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r7 = u8 [r7 + 0x1c1]
    ...D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R.........................  u16 [r8 + 0x211] = r11
    ...D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER........................  u16 [r8 + 0x21b] = r9
    ....D=======================eeeeeeeeeeeeeeeeeeeeeeeeeE--R........................  u8 [r8 + 0x231] = a5
    ....D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r8 + 0x232] = a0
    ....D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r8 + 0x234] = a0
    ....DeeeeeeeeeeeeeeeeeeeeeeE----------------------------------------------------R  jump [r0 + 0]
```

Gas simulation at offset 12868 with total cost of 79:

```
    DeER..............................................................................  r7 = r7 + 0x7ff
    DeER..............................................................................  r2 = 0x2000
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.....................................................  r3 = u16 [r7 + 0x209]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.....................................................  r4 = i16 [r7 + 0x211]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER.....................................................  r11 = i16 [r7 + 0x213]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER.....................................................  r12 = i16 [r7 + 0x215]
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER............................  r8 = i16 [r7 + 0x217]
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER............................  r9 = i16 [r7 + 0x219]
    ..D========================eE------------------------R............................  r3 = r3 << 0x34
    ..D=========================eE-----------------------R............................  r10 = r3 >> 0x34
    ..D==========================eE----------------------R............................  r10 = r10 | r2
    ...D================================================eER...........................  r9 = r9 << 0x1
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER..  u16 [r7 + 0x219] = r9
    ...D==========================eeeeeeeeeeeeeeeeeeeeeeeeeE-----------------------R..  u16 [r7 + 0x21b] = r10
    ...D=======================eE--------------------------------------------------R..  r11 = r11 << 0x1
    ....D=======================eE-------------------------------------------------R..  r12 = r12 << 0x1
    ....D===============================================eE-------------------------R..  r8 = r8 << 0x1
    ....D========================eE------------------------------------------------R..  r4 = r4 + 0x1
    ....D=========================eeeeeeeeeeeeeeeeeeeeeeeeeE-----------------------R..  u16 [r7 + 0x211] = r4
    .....D===============================================eeeeeeeeeeeeeeeeeeeeeeeeeER..  u16 [r7 + 0x213] = r11
    .....D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r7 + 0x215] = r12
    .....D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r7 + 0x217] = r8
    .....DeeeeeeeeeeeeeeeeeeeeeeE----------------------------------------------------R  jump [r0 + 0]
```

Gas simulation at offset 12950 with total cost of 29:

```
    DeER............................  r1 = r1 + 0xfffffffffffffff0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0x8] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0] = r5
    .DeE------------------------R...  r5 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u16 [r5 + 0x21b]
    ..D=========================eER.  r9 = r8 >> 0x8
    ..D==========================eER  jump 13007 if r9 >=u 63
```

Gas simulation at offset 12973 with total cost of 74:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r9 = u64 [r5 + 0x241]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r7 = u64 [r5 + 0x249]
    DeE---------------------------------------R..................................  r10 = 0x17c80
    .D========================eeE-------------R..................................  r10 = r7 if r9 != 0
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r10 = u64 [r10 + 0x48]
    ..DeE-------------------------------------------------R......................  r7 = r5 + 0x27f
    ..D=======================eeE-------------------------R......................  r7 = r9 if r9 != 0
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 312, jump [r10 + 0]
```

Gas simulation at offset 13005 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 13022
```

Gas simulation at offset 13007 with total cost of 28:

```
    DeER...........................  r8 = r8 & 0x1f
    D=eER..........................  r7 = r7 + r8
    D==eER.........................  r7 = r7 + 0x7ff
    D===eeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u8 [r7 + 0x1a1]
    .DeeE-------------------------R  fallthrough
```

Gas simulation at offset 13022 with total cost of 100:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r8 = i16 [r5 + 0x219]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r9 = i16 [r5 + 0x211]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r10 = i16 [r5 + 0x213]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r11 = i16 [r5 + 0x215]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  r12 = i16 [r5 + 0x217]
    .D========================eE------------------------R..................................................  r8 = r8 << 0x1
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER.................................................  u16 [r5 + 0x219] = r8
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R.................................................  u8 [r5 + 0x22a] = a0
    ..D=======================eE-------------------------R.................................................  r10 = r10 << 0x1
    ..D========================eE------------------------R.................................................  r11 = r11 << 0x1
    ..D================================================eER.................................................  r12 = r12 << 0x1
    ..D=========================eE-----------------------R.................................................  r9 = r9 + 0x1
    ...D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER...............................................  u16 [r5 + 0x211] = r9
    ...D===============================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u16 [r5 + 0x213] = r10
    ...D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER........................  u16 [r5 + 0x215] = r11
    ...D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER........................  u16 [r5 + 0x217] = r12
    ....D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r0 = u64 [r1 + 0x8]
    ....D=======================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  r5 = u64 [r1 + 0]
    ....D========================================================================eE-----------------------R  r1 = r1 + 0x10
    ....D==========================================================================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 13091 with total cost of 48:

```
    DeER...............................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r2 = u16 [r7 + 0x211]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r9 = u16 [r7 + 0x209]
    .D=========================eER.....................  r10 = r2 + 0xfffffffffffffeff
    .D=========================eER.....................  r12 = r9 >> 0x4
    ..D=========================eER....................  r8 = zext16 r10
    ..DeE-------------------------R....................  r3 = 0x40
    ..D=========================eER....................  r10 = r12 & 0x38
    ...D=========================eeeeeeeeeeeeeeeeeeeeER  jump 13134 if r8 >=u r3
```

Gas simulation at offset 13121 with total cost of 16:

```
    DeER...............  r8 = r9 & 0xcff
    D=eER..............  r8 = r8 | 0x2000
    .D=eER.............  r9 = r10 + r8
    .DeeeeeeeeeeeeeeeER  jump 13155
```

Gas simulation at offset 13134 with total cost of 4:

```
    DeER...  r11 = r9 & 0xc00
    DeER...  r9 = r9 << 0x3b
    D=eER..  r9 = r9 >> 0x3d
    .D=eER.  r9 = r9 | r11
    .DeE-R.  r8 = r10 | 0x23c0
    .D==eER  r9 = r9 | r8
    ..DeeER  fallthrough
```

Gas simulation at offset 13155 with total cost of 76:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...................................................  r8 = i16 [r7 + 0x219]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...................................................  r10 = i16 [r7 + 0x213]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...................................................  r11 = i16 [r7 + 0x215]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...................................................  r12 = i16 [r7 + 0x217]
    .D========================eER..................................................  r8 = r8 << 0x1
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u16 [r7 + 0x219] = r8
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R.........................  u16 [r7 + 0x21b] = r9
    .D========================eE-------------------------R.........................  r2 = r2 + 0x1
    ..D=======================eE-------------------------R.........................  r10 = r10 << 0x1
    ..D========================eE------------------------R.........................  r11 = r11 << 0x1
    ..D========================eE------------------------R.........................  r12 = r12 << 0x1
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER........................  u16 [r7 + 0x211] = r2
    ...D========================eeeeeeeeeeeeeeeeeeeeeeeeeER........................  u16 [r7 + 0x213] = r10
    ...D===============================================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u16 [r7 + 0x215] = r11
    ...D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r7 + 0x217] = r12
    ...DeeeeeeeeeeeeeeeeeeeeeeE---------------------------------------------------R  jump [r0 + 0]
```

Gas simulation at offset 13212 with total cost of 29:

```
    DeER............................  r1 = r1 + 0xfffffffffffffff0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0x8] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0] = r5
    .DeE------------------------R...  r5 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u16 [r5 + 0x21b]
    ..D=========================eER.  r9 = r8 >> 0x8
    ..D==========================eER  jump 13269 if r9 >=u 63
```

Gas simulation at offset 13235 with total cost of 74:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r9 = u64 [r5 + 0x241]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r7 = u64 [r5 + 0x249]
    DeE---------------------------------------R..................................  r10 = 0x17c80
    .D========================eeE-------------R..................................  r10 = r7 if r9 != 0
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r10 = u64 [r10 + 0x48]
    ..DeE-------------------------------------------------R......................  r7 = r5 + 0x27f
    ..D=======================eeE-------------------------R......................  r7 = r9 if r9 != 0
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 318, jump [r10 + 0]
```

Gas simulation at offset 13267 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 13284
```

Gas simulation at offset 13269 with total cost of 28:

```
    DeER...........................  r8 = r8 & 0x1f
    D=eER..........................  r7 = r7 + r8
    D==eER.........................  r7 = r7 + 0x7ff
    D===eeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u8 [r7 + 0x1a1]
    .DeeE-------------------------R  fallthrough
```

Gas simulation at offset 13284 with total cost of 123:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..................................................................................................  r10 = u8 [r5 + 0x209]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..................................................................................................  r2 = i16 [r5 + 0x211]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..................................................................................................  r3 = i16 [r5 + 0x213]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..................................................................................................  r11 = i16 [r5 + 0x215]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................................................................  r12 = i16 [r5 + 0x217]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................................................................  r9 = i16 [r5 + 0x219]
    .D========================eE------------------------R.........................................................................  r8 = r10 & 0x2
    ..D=======================eE------------------------R.........................................................................  r10 = r10 >> 0x4
    ..D========================eE-----------------------R.........................................................................  r10 = r10 & 0x4
    ..D=========================eE----------------------R.........................................................................  r8 = r8 | r10
    ..D========================eE-----------------------R.........................................................................  r7 = r7 & 0xff
    ...D=========================eE---------------------R.........................................................................  r7 = r7 >> r8
    ...D===============================================eER........................................................................  r9 = r9 << 0x1
    ...D==========================eE---------------------R........................................................................  r7 = r7 & 0x3
    ....D===============================================eeeeeeeeeeeeeeeeeeeeeeeeeER...............................................  u16 [r5 + 0x219] = r9
    ....D==========================eeeeeeeeeeeeeeeeeeeeeeeeeE---------------------R...............................................  u8 [r5 + 0x22b] = a0
    ....D=======================eE------------------------------------------------R...............................................  r3 = r3 << 0x1
    ....D========================eE-----------------------------------------------R...............................................  r11 = r11 << 0x1
    .....D=============================================eE-------------------------R...............................................  r12 = r12 << 0x1
    .....D========================eE----------------------------------------------R...............................................  r2 = r2 + 0x1
    .....D=========================eeeeeeeeeeeeeeeeeeeeeeeeeE---------------------R...............................................  u16 [r5 + 0x211] = r2
    .....D==============================================eeeeeeeeeeeeeeeeeeeeeeeeeER...............................................  u16 [r5 + 0x213] = r3
    ......D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER...........................................  u16 [r5 + 0x215] = r11
    ......D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER...........................................  u16 [r5 + 0x217] = r12
    ......D======================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r0 = u64 [r1 + 0x8]
    ......D======================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r5 = u64 [r1 + 0]
    .......D=========================================================================eE--------------------R......................  r1 = r1 + 0x10
    .......D==============================================================================================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 13379 with total cost of 104:

```
    DeER.......................................................................................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..............................................................................  r8 = u8 [r7 + 0x226]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..............................................................................  r9 = u8 [r7 + 0x22a]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..............................................................................  r2 = i16 [r7 + 0x217]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER..............................................................................  r3 = i16 [r7 + 0x219]
    .D=========================eER.............................................................................  r8 = r8 & 0x10
    .D=========================eER.............................................................................  r9 = r9 << 0x4
    .D==========================eER............................................................................  r8 = r8 << 0x8
    ..D==========================eER...........................................................................  r8 = r8 | r9
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.....................................................  r9 = i16 [r7 + 0x209]
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.....................................................  r12 = i16 [r7 + 0x211]
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER....................................................  r10 = i16 [r7 + 0x213]
    ...D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  r11 = i16 [r7 + 0x215]
    ...D================================================eE--R..................................................  r9 = r9 << 0x31
    ...D=================================================eE-R..................................................  r9 = r9 >> 0x3d
    ...D==================================================eER..................................................  r8 = r8 | r9
    ....D===============================================eE--R..................................................  r3 = r3 << 0x1
    ....D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER...........................  u16 [r7 + 0x219] = r3
    ....D==================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u16 [r7 + 0x21b] = r8
    ....D================================================eE--------------------------R.........................  r10 = r10 << 0x1
    .....D=================================================eE------------------------R.........................  r11 = r11 << 0x1
    .....D================================================eE-------------------------R.........................  r2 = r2 << 0x1
    .....D=================================================eE------------------------R.........................  r12 = r12 + 0x1
    .....D==================================================eeeeeeeeeeeeeeeeeeeeeeeeeER........................  u16 [r7 + 0x211] = r12
    ......D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER........................  u16 [r7 + 0x213] = r10
    ......D=======================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER..  u16 [r7 + 0x215] = r11
    ......D=========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r7 + 0x217] = r2
    ......DeeeeeeeeeeeeeeeeeeeeeeE----------------------------------------------------------------------------R  jump [r0 + 0]
```

Gas simulation at offset 13477 with total cost of 29:

```
    DeER............................  r1 = r1 + 0xfffffffffffffff0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0x8] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0] = r5
    .DeE------------------------R...  r5 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u16 [r5 + 0x21b]
    ..D=========================eER.  r9 = r8 >> 0x8
    ..D==========================eER  jump 13534 if r9 >=u 63
```

Gas simulation at offset 13500 with total cost of 74:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r9 = u64 [r5 + 0x241]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r7 = u64 [r5 + 0x249]
    DeE---------------------------------------R..................................  r10 = 0x17c80
    .D========================eeE-------------R..................................  r10 = r7 if r9 != 0
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r10 = u64 [r10 + 0x48]
    ..DeE-------------------------------------------------R......................  r7 = r5 + 0x27f
    ..D=======================eeE-------------------------R......................  r7 = r9 if r9 != 0
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 324, jump [r10 + 0]
```

Gas simulation at offset 13532 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 13549
```

Gas simulation at offset 13534 with total cost of 28:

```
    DeER...........................  r8 = r8 & 0x1f
    D=eER..........................  r7 = r7 + r8
    D==eER.........................  r7 = r7 + 0x7ff
    D===eeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u8 [r7 + 0x1a1]
    .DeeE-------------------------R  fallthrough
```

Gas simulation at offset 13549 with total cost of 100:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r8 = i16 [r5 + 0x219]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r9 = i16 [r5 + 0x211]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r10 = i16 [r5 + 0x213]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r11 = i16 [r5 + 0x215]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  r12 = i16 [r5 + 0x217]
    .D========================eE------------------------R..................................................  r8 = r8 << 0x1
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER.................................................  u16 [r5 + 0x219] = r8
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R.................................................  u8 [r5 + 0x22c] = a0
    ..D=======================eE-------------------------R.................................................  r10 = r10 << 0x1
    ..D========================eE------------------------R.................................................  r11 = r11 << 0x1
    ..D================================================eER.................................................  r12 = r12 << 0x1
    ..D=========================eE-----------------------R.................................................  r9 = r9 + 0x1
    ...D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER...............................................  u16 [r5 + 0x211] = r9
    ...D===============================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u16 [r5 + 0x213] = r10
    ...D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER........................  u16 [r5 + 0x215] = r11
    ...D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER........................  u16 [r5 + 0x217] = r12
    ....D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r0 = u64 [r1 + 0x8]
    ....D=======================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  r5 = u64 [r1 + 0]
    ....D========================================================================eE-----------------------R  r1 = r1 + 0x10
    ....D==========================================================================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 13618 with total cost of 104:

```
    DeER.......................................................................................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..............................................................................  r2 = i16 [r7 + 0x217]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..............................................................................  r4 = i16 [r7 + 0x219]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..............................................................................  r10 = u8 [r7 + 0x226]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER..............................................................................  r11 = u8 [r7 + 0x22a]
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER.....................................................  r12 = u16 [r7 + 0x209]
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER.....................................................  r3 = i16 [r7 + 0x211]
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER.....................................................  r8 = i16 [r7 + 0x213]
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.....................................................  r9 = i16 [r7 + 0x215]
    ..D=================================================eER....................................................  r11 = r11 << 0x4
    ..D=================================================eER....................................................  r12 = r12 >> 0xc
    ..D==================================================eER...................................................  r11 = r11 | r12
    ...D================================================eE-R...................................................  r10 = r10 & 0x10
    ...D=================================================eER...................................................  r10 = r10 << 0x8
    ...D==================================================eER..................................................  r10 = r10 | r11
    ...D================================================eE--R..................................................  r4 = r4 << 0x1
    ....D==================================================eER.................................................  r10 = r10 | 0x8
    ....D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER...........................  u16 [r7 + 0x219] = r4
    ....D===================================================eeeeeeeeeeeeeeeeeeeeeeeeeER........................  u16 [r7 + 0x21b] = r10
    ....D================================================eE---------------------------R........................  r8 = r8 << 0x1
    .....D================================================eE--------------------------R........................  r9 = r9 << 0x1
    .....D================================================eE--------------------------R........................  r2 = r2 << 0x1
    .....D=================================================eE-------------------------R........................  r3 = r3 + 0x1
    .....D==================================================eeeeeeeeeeeeeeeeeeeeeeeeeER........................  u16 [r7 + 0x211] = r3
    ......D================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-R........................  u16 [r7 + 0x213] = r8
    ......D=======================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER..  u16 [r7 + 0x215] = r9
    ......D=========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r7 + 0x217] = r2
    ......DeeeeeeeeeeeeeeeeeeeeeeE----------------------------------------------------------------------------R  jump [r0 + 0]
```

Gas simulation at offset 13716 with total cost of 29:

```
    DeER............................  r1 = r1 + 0xfffffffffffffff0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0x8] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0] = r5
    .DeE------------------------R...  r5 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u16 [r5 + 0x21b]
    ..D=========================eER.  r9 = r8 >> 0x8
    ..D==========================eER  jump 13787 if r9 >=u 63
```

Gas simulation at offset 13739 with total cost of 74:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r9 = u64 [r5 + 0x241]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r7 = u64 [r5 + 0x249]
    DeE---------------------------------------R..................................  r10 = 0x17c80
    .D========================eeE-------------R..................................  r10 = r7 if r9 != 0
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r10 = u64 [r10 + 0x48]
    ..DeE-------------------------------------------------R......................  r7 = r5 + 0x27f
    ..D=======================eeE-------------------------R......................  r7 = r9 if r9 != 0
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 330, jump [r10 + 0]
```

Gas simulation at offset 13771 with total cost of 27:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u8 [r5 + 0x227]
    D=========================eER.  r8 = r8 & 0x18
    DeeeeeeeeeeeeeeeeeeeeeeeeeE-R.  u8 [r5 + 0x22d] = a0
    D==========================eER  jump 13816 if r8 != 0
```

Gas simulation at offset 13785 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 13852
```

Gas simulation at offset 13787 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeE---------------------------------------R.............  r8 = r8 & 0x1f
    D=eE--------------------------------------R.............  r7 = r7 + r8
    D==eE-------------------------------------R.............  r7 = r7 + 0x7ff
    .D==eeeeeeeeeeeeeeeeeeeeeeeeeE------------R.............  r7 = u8 [r7 + 0x1a1]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.............  r8 = u8 [r5 + 0x227]
    .D=========================eE-------------R.............  r8 = r8 & 0x18
    .D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x22d] = a0
    ..D=========================eE-------------------------R  jump 13852 if r8 == 0
```

Gas simulation at offset 13816 with total cost of 46:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER......  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R......  r8 = u16 [r5 + 0x209]
    D=========================eE--------------R......  r9 = r8 & 0x1f
    .D========================eE--------------R......  r8 = r8 & 0xffffffffffffffe0
    .D=========================eeeeeeeeeeeeeeeeeeeeER  jump 13841 if r9 != 31
```

Gas simulation at offset 13831 with total cost of 26:

```
    DeER.........................  r8 = r8 ^ 0x400
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x209] = r8
    DeeeeeeeeeeeeeeeE-----------R  jump 13852
```

Gas simulation at offset 13841 with total cost of 27:

```
    DeER..........................  r8 = r8 | r9
    D=eER.........................  r8 = r8 + 0x1
    D==eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x209] = r8
    DeeE-------------------------R  fallthrough
```

Gas simulation at offset 13852 with total cost of 124:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER....................................................................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R....................................................................................  r2 = i16 [r5 + 0x211]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R....................................................................................  r9 = u16 [r5 + 0x213]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R....................................................................................  r3 = u16 [r5 + 0x219]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R....................................................................................  r11 = u8 [r5 + 0x22b]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..........................................................................  r12 = u8 [r5 + 0x22c]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..........................................................................  r8 = u16 [r5 + 0x215]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..........................................................................  r10 = u16 [r5 + 0x217]
    ..D========================eE-----------------------R..........................................................................  r9 = r9 & 0xffffffffffffff00
    ..D================================================eER.........................................................................  r9 = r9 | r12
    ..D=========================eE-----------------------R.........................................................................  r7 = r7 & 0xff
    ..D================================================eER.........................................................................  r8 = r8 & 0xffffffffffffff00
    ...D===============================================eER.........................................................................  r10 = r10 & 0xffffffffffffff00
    ...D================================================eER........................................................................  r7 = r7 | r8
    ...D=========================eE-----------------------R........................................................................  r8 = r11 << 0x3f
    ....D=========================eE----------------------R........................................................................  r8 = r8 >>a 0x3f
    ....D==========================eE---------------------R........................................................................  r8 = r8 & 0xff
    ....D===============================================eER........................................................................  r8 = r8 | r10
    .....D==========================eE--------------------R........................................................................  r10 = r3 & 0xffffffffffffff00
    .....D===========================eE-------------------R........................................................................  r11 = r11 << 0x6
    .....D============================eE------------------R........................................................................  r11 = sext8 r11
    ......D============================eE-----------------R........................................................................  r11 = r11 << 0x31
    ......D=============================eE----------------R........................................................................  r11 = r11 >> 0x38
    ......D==============================eE---------------R........................................................................  r10 = r10 | r11
    ......D===============================eE--------------R........................................................................  r2 = r2 + 0x1
    .......D============================================eER........................................................................  r9 = r9 << 0x1
    .......D=============================================eER.......................................................................  r7 = r7 << 0x1
    .......D=============================================eER.......................................................................  r8 = r8 << 0x1
    .......D===============================eeeeeeeeeeeeeeeeeeeeeeeeeER.............................................................  u16 [r5 + 0x211] = r2
    ........D============================================eeeeeeeeeeeeeeeeeeeeeeeeeER...............................................  u16 [r5 + 0x213] = r9
    ........D=============================================eeeeeeeeeeeeeeeeeeeeeeeeeER..............................................  u16 [r5 + 0x215] = r7
    ........D=============================================eeeeeeeeeeeeeeeeeeeeeeeeeER..............................................  u16 [r5 + 0x217] = r8
    ...........................................D====================eE--------------R..............................................  r10 = r10 << 0x1
    ...........................................D=====================eeeeeeeeeeeeeeeeeeeeeeeeeER...................................  u16 [r5 + 0x219] = r10
    ...........................................D==================================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r0 = u64 [r1 + 0x8]
    ...........................................D===================================eeeeeeeeeeeeeeeeeeeeeeeeeER.....................  r5 = u64 [r1 + 0]
    ............................................D==================================eE------------------------R.....................  r1 = r1 + 0x10
    .....................................................D=================================================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 13979 with total cost of 29:

```
    DeER............................  r1 = r1 + 0xfffffffffffffff0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0x8] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0] = r5
    .DeE------------------------R...  r5 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u16 [r5 + 0x21b]
    ..D=========================eER.  r9 = r8 >> 0x8
    ..D==========================eER  jump 14050 if r9 >=u 63
```

Gas simulation at offset 14002 with total cost of 74:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r9 = u64 [r5 + 0x241]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r7 = u64 [r5 + 0x249]
    DeE---------------------------------------R..................................  r10 = 0x17c80
    .D========================eeE-------------R..................................  r10 = r7 if r9 != 0
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r10 = u64 [r10 + 0x48]
    ..DeE-------------------------------------------------R......................  r7 = r5 + 0x27f
    ..D=======================eeE-------------------------R......................  r7 = r9 if r9 != 0
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 334, jump [r10 + 0]
```

Gas simulation at offset 14034 with total cost of 27:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u8 [r5 + 0x227]
    D=========================eER.  r8 = r8 & 0x18
    DeeeeeeeeeeeeeeeeeeeeeeeeeE-R.  u8 [r5 + 0x22d] = a0
    D==========================eER  jump 14079 if r8 != 0
```

Gas simulation at offset 14048 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 14115
```

Gas simulation at offset 14050 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeE---------------------------------------R.............  r8 = r8 & 0x1f
    D=eE--------------------------------------R.............  r7 = r7 + r8
    D==eE-------------------------------------R.............  r7 = r7 + 0x7ff
    .D==eeeeeeeeeeeeeeeeeeeeeeeeeE------------R.............  r7 = u8 [r7 + 0x1a1]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.............  r8 = u8 [r5 + 0x227]
    .D=========================eE-------------R.............  r8 = r8 & 0x18
    .D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x22d] = a0
    ..D=========================eE-------------------------R  jump 14115 if r8 == 0
```

Gas simulation at offset 14079 with total cost of 46:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER......  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R......  r8 = u16 [r5 + 0x209]
    D=========================eE--------------R......  r9 = r8 & 0x1f
    .D========================eE--------------R......  r8 = r8 & 0xffffffffffffffe0
    .D=========================eeeeeeeeeeeeeeeeeeeeER  jump 14104 if r9 != 31
```

Gas simulation at offset 14094 with total cost of 26:

```
    DeER.........................  r8 = r8 ^ 0x400
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x209] = r8
    DeeeeeeeeeeeeeeeE-----------R  jump 14115
```

Gas simulation at offset 14104 with total cost of 27:

```
    DeER..........................  r8 = r8 | r9
    D=eER.........................  r8 = r8 + 0x1
    D==eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x209] = r8
    DeeE-------------------------R  fallthrough
```

Gas simulation at offset 14115 with total cost of 98:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..........................................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........................................................  r8 = u8 [r5 + 0x22b]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........................................................  r9 = i16 [r5 + 0x211]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........................................................  r10 = u8 [r5 + 0x22c]
    .D========================eE--------------R..........................................................  r11 = r8 << 0x3f
    .D========================eE--------------R..........................................................  r8 = r8 << 0x6
    .D========================eE--------------R..........................................................  r9 = r9 + 0x1
    ..D========================eE-------------R..........................................................  r11 = r11 >>a 0x3f
    ..D========================eE-------------R..........................................................  r8 = sext8 r8
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER...............................................  u16 [r5 + 0x211] = r9
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER..............................................  u8 [r5 + 0x213] = a3
    ...DeeeeeeeeeeeeeeeeeeeeeeeeeE------------------------R..............................................  u8 [r5 + 0x215] = a0
    ...D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..............................................  u8 [r5 + 0x217] = a4
    ...D=========================eE-----------------------R..............................................  r8 = r8 >> 0x7
    ...D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER............................................  u8 [r5 + 0x219] = a1
    ....D===============================================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r0 = u64 [r1 + 0x8]
    ....D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.....................  r5 = u64 [r1 + 0]
    ....D================================================eE------------------------R.....................  r1 = r1 + 0x10
    ....D========================================================================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 14175 with total cost of 54:

```
    DeER.....................................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER............................  r8 = u16 [r7 + 0x209]
    DeE-------------------------R............................  r9 = 0x2000
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER............................  r10 = i16 [r7 + 0x211]
    .D=========================eER...........................  r8 = r8 << 0x34
    .D==========================eER..........................  r8 = r8 >> 0x34
    .D===========================eER.........................  r8 = r8 | r9
    .D=========================eE--R.........................  r10 = r10 + 0x1
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER..  u16 [r7 + 0x211] = r10
    ..D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r7 + 0x21b] = r8
    ..DeeeeeeeeeeeeeeeeeeeeeeE------------------------------R  jump [r0 + 0]
```

Gas simulation at offset 14213 with total cost of 29:

```
    DeER............................  r1 = r1 + 0xfffffffffffffff0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0x8] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0] = r5
    .DeE------------------------R...  r5 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u16 [r5 + 0x21b]
    ..D=========================eER.  r9 = r8 >> 0x8
    ..DeE-------------------------R.  r10 = 0x3f
    ..D==========================eER  jump 14272 if r9 >=u r10
```

Gas simulation at offset 14238 with total cost of 74:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r9 = u64 [r5 + 0x241]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r7 = u64 [r5 + 0x249]
    DeE---------------------------------------R..................................  r10 = 0x17c80
    .D========================eeE-------------R..................................  r10 = r7 if r9 != 0
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r10 = u64 [r10 + 0x48]
    ..DeE-------------------------------------------------R......................  r7 = r5 + 0x27f
    ..D=======================eeE-------------------------R......................  r7 = r9 if r9 != 0
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 340, jump [r10 + 0]
```

Gas simulation at offset 14270 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 14287
```

Gas simulation at offset 14272 with total cost of 28:

```
    DeER...........................  r8 = r8 & 0x1f
    D=eER..........................  r7 = r7 + r8
    D==eER.........................  r7 = r7 + 0x7ff
    D===eeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u8 [r7 + 0x1a1]
    .DeeE-------------------------R  fallthrough
```

Gas simulation at offset 14287 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r8 = i16 [r5 + 0x211]
    D=========================eER.........................  r8 = r8 + 0x1
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x211] = r8
    DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R  u8 [r5 + 0x22a] = a0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r0 = u64 [r1 + 0x8]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r5 = u64 [r1 + 0]
    .D========================eE-------------------------R  r1 = r1 + 0x10
    .D=========================eeeeeeeeeeeeeeeeeeeeeeE---R  jump [r0 + 0]
```

Gas simulation at offset 14312 with total cost of 29:

```
    DeER............................  r1 = r1 + 0xfffffffffffffff0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0x8] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0] = r5
    .DeE------------------------R...  r5 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u16 [r5 + 0x21b]
    ..D=========================eER.  r9 = r8 >> 0x8
    ..DeE-------------------------R.  r10 = 0x3f
    ..D==========================eER  jump 14371 if r9 >=u r10
```

Gas simulation at offset 14337 with total cost of 74:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r9 = u64 [r5 + 0x241]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r7 = u64 [r5 + 0x249]
    DeE---------------------------------------R..................................  r10 = 0x17c80
    .D========================eeE-------------R..................................  r10 = r7 if r9 != 0
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r10 = u64 [r10 + 0x48]
    ..DeE-------------------------------------------------R......................  r7 = r5 + 0x27f
    ..D=======================eeE-------------------------R......................  r7 = r9 if r9 != 0
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 344, jump [r10 + 0]
```

Gas simulation at offset 14369 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 14386
```

Gas simulation at offset 14371 with total cost of 28:

```
    DeER...........................  r8 = r8 & 0x1f
    D=eER..........................  r7 = r7 + r8
    D==eER.........................  r7 = r7 + 0x7ff
    D===eeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u8 [r7 + 0x1a1]
    .DeeE-------------------------R  fallthrough
```

Gas simulation at offset 14386 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r8 = i16 [r5 + 0x20f]
    D=========================eER.........................  r8 = r8 + 0x1
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x20f] = r8
    DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R  u16 [r5 + 529] = 0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  u8 [r5 + 0x22a] = a0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r0 = u64 [r1 + 0x8]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R  r5 = u64 [r1 + 0]
    .D=========================eE------------------------R  r1 = r1 + 0x10
    ..D========================eeeeeeeeeeeeeeeeeeeeeeE---R  jump [r0 + 0]
```

Gas simulation at offset 14415 with total cost of 77:

```
    DeER............................................................................  r1 = r1 + 0xfffffffffffffff0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...................................................  u64 [r1 + 0x8] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...................................................  u64 [r1 + 0] = r5
    .DeE------------------------R...................................................  r5 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  r9 = u8 [r5 + 0x227]
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  r10 = u8 [r5 + 0x23f]
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u8 [r5 + 560] = 0
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u8 [r5 + 561] = 0
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u8 [r5 + 567] = 0
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u8 [r5 + 573] = 0x1
    ...D================================================eER.........................  r9 = r9 & 0x10
    ...D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u8 [r5 + 0x23e] = a3
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 575] = 0
    ...D=================================================eeeeeeeeeeeeeeeeeeeeE-----R  jump 14481 if r9 == 0
```

Gas simulation at offset 14466 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 548] = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 566] = 0
    DeE------------------------R  r0 = 0x15c
    DeeeeeeeeeeeeeeeE----------R  jump 6145
```

Gas simulation at offset 14481 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 566] = 0
    DeeeeeeeeeeeeeeeE----------R  r0 = 348, jump 6145
```

Gas simulation at offset 14491 with total cost of 98:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.........................................................................  r7 = i16 [r5 + 0x211]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.........................................................................  r8 = i16 [r5 + 0x213]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.........................................................................  r9 = i16 [r5 + 0x215]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.........................................................................  r10 = i16 [r5 + 0x217]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER................................................  r11 = i16 [r5 + 0x219]
    .D========================eE------------------------R................................................  r8 = r8 << 0x1
    .D========================eE------------------------R................................................  r9 = r9 << 0x1
    .D========================eE------------------------R................................................  r10 = r10 << 0x1
    ..D========================eE-----------------------R................................................  r7 = r7 + 0x1
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER..............................................  u16 [r5 + 0x211] = r7
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R..............................................  u16 [r5 + 0x213] = r8
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R..............................................  u16 [r5 + 0x215] = r9
    ...D===============================================eeeeeeeeeeeeeeeeeeeeeeeeeER.......................  u16 [r5 + 0x217] = r10
    ...D================================================eE-----------------------R.......................  r11 = r11 << 0x1
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.....................  u16 [r5 + 0x219] = r11
    ...D================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-R.....................  r0 = u64 [r1 + 0x8]
    ....D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.....................  r5 = u64 [r1 + 0]
    ....D=======================================================================eE-R.....................  r1 = r1 + 0x10
    ....D========================================================================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 14556 with total cost of 26:

```
    DeER.........................  r1 = r1 + 0xffffffffffffffe8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x10] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x8] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0] = r6
    .D...........................  r5 = r7
    .DeE------------------------R  r6 = r7 + 0x7ff
    .DeeeeeeeeeeeeeeeE----------R  r0 = 352, jump 6954
```

Gas simulation at offset 14579 with total cost of 54:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.............................  r7 = u8 [r6 + 0x226]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.............................  r8 = u8 [r6 + 0x22a]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.............................  r9 = u16 [r6 + 0x209]
    D=========================eER............................  r7 = r7 & 0x10
    .D========================eER............................  r8 = r8 << 0x4
    .D========================eER............................  r9 = r9 >> 0xc
    .D=========================eER...........................  r7 = r7 << 0x8
    .D=========================eER...........................  r8 = r8 | r9
    ..D=========================eER..........................  r7 = r7 | r8
    ..D==========================eER.........................  r7 = r7 | 0x8
    ..D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r6 + 0x21b] = r7
    ..D......................................................  r7 = r5
    ...DeeeeeeeeeeeeeeeE------------------------------------R  r0 = 354, jump 7236
```

Gas simulation at offset 14624 with total cost of 15:

```
    D.................  r7 = r5
    DeeeeeeeeeeeeeeeER  r0 = 356, jump 6145
```

Gas simulation at offset 14632 with total cost of 122:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.................................................................................................  r7 = i16 [r6 + 0x211]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.................................................................................................  r8 = i16 [r6 + 0x213]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.................................................................................................  r9 = i16 [r6 + 0x215]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.................................................................................................  r10 = i16 [r6 + 0x217]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER........................................................................  r11 = i16 [r6 + 0x219]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER........................................................................  r12 = i32 [r6 + 0x255]
    .D========================eE------------------------R........................................................................  r8 = r8 << 0x1
    .D========================eE------------------------R........................................................................  r9 = r9 << 0x1
    ..D========================eE-----------------------R........................................................................  r10 = r10 << 0x1
    ..D========================eE-----------------------R........................................................................  r7 = r7 + 0x1
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................................................................  u16 [r6 + 0x211] = r7
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................................................................  u16 [r6 + 0x213] = r8
    ...D===============================================eeeeeeeeeeeeeeeeeeeeeeeeeER...............................................  u16 [r6 + 0x215] = r9
    ...D===============================================eeeeeeeeeeeeeeeeeeeeeeeeeER...............................................  u16 [r6 + 0x217] = r10
    ...D=================================================eE----------------------R...............................................  r11 = r11 << 0x1
    ...D=================================================eE----------------------R...............................................  r12 = r12 + 0x1
    ....D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER............................................  u16 [r6 + 0x219] = r11
    ....D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER............................................  u32 [r6 + 0x255] = r12
    ....D=======================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r0 = u64 [r1 + 0x10]
    ....D=======================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r5 = u64 [r1 + 0x8]
    .....D=========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER...................  r6 = u64 [r1 + 0]
    .....D=========================================================================eE------------------------R...................  r1 = r1 + 0x18
    .....D===============================================================================================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 14711 with total cost of 52:

```
    DeER...................................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r8 = i16 [r7 + 0x211]
    D==========================eER.........................  r8 = r8 + 0x1
    D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r7 + 0x211] = r8
    .DeeeeeeeeeeeeeeeeeeeeeeE-----------------------------R  jump [r0 + 0]
```

Gas simulation at offset 14728 with total cost of 52:

```
    DeER...................................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r8 = i16 [r7 + 0x20f]
    D==========================eER.........................  r8 = r8 + 0x1
    D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r7 + 0x20f] = r8
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R  u16 [r7 + 529] = 0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R  u8 [r7 + 569] = 0
    .DeeeeeeeeeeeeeeeeeeeeeeE-----------------------------R  jump [r0 + 0]
```

Gas simulation at offset 14753 with total cost of 27:

```
    DeER..........................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.  r8 = u8 [r7 + 0x239]
    D==========================eER  jump 14778 if r8 != 0
```

Gas simulation at offset 14764 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r8 = u8 [r7 + 0x228]
    D=========================eE--------------R...........  r8 = r8 | 0x80
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x228] = a1
    .DeeE------------------------------------------------R  fallthrough
```

Gas simulation at offset 14778 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r8 = i16 [r7 + 0x211]
    D=========================eE--------------R...........  r8 = r8 + 0x1
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r7 + 0x211] = r8
    .DeeeeeeeeeeeeeeeeeeeeeeE----------------------------R  jump [r0 + 0]
```

Gas simulation at offset 14792 with total cost of 54:

```
    DeER.....................................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER............................  r8 = u8 [r7 + 0x226]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER............................  r9 = u8 [r7 + 0x228]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER............................  r10 = i16 [r7 + 0x211]
    .D=========================eER...........................  r8 = r8 & r9
    .D=========================eER...........................  r10 = r10 + 0x1
    .D==========================eER..........................  r8 = r8 << 0x38
    .D===========================eER.........................  r8 = r8 >> 0x3f
    ..D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x271] = a1
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeE--R  u16 [r7 + 0x211] = r10
    ..DeeeeeeeeeeeeeeeeeeeeeeE------------------------------R  jump [r0 + 0]
```

Gas simulation at offset 14830 with total cost of 54:

```
    DeER.....................................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER............................  r8 = u8 [r7 + 0x226]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER............................  r9 = u8 [r7 + 0x228]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER............................  r10 = i16 [r7 + 0x20f]
    .D=========================eER...........................  r8 = r8 & r9
    .D=========================eER...........................  r10 = r10 + 0x1
    .D==========================eER..........................  r8 = r8 << 0x38
    .D===========================eER.........................  r8 = r8 >> 0x3f
    ..D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x271] = a1
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeE--R  u16 [r7 + 0x20f] = r10
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------------------R  u16 [r7 + 529] = 0
    ..DeeeeeeeeeeeeeeeeeeeeeeE------------------------------R  jump [r0 + 0]
```

Gas simulation at offset 14872 with total cost of 54:

```
    DeER.....................................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER............................  r8 = u8 [r7 + 0x226]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER............................  r9 = u8 [r7 + 0x228]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER............................  r10 = u8 [r7 + 0x238]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER............................  r11 = i16 [r7 + 0x20f]
    .D=========================eER...........................  r8 = r8 & r9
    .D=========================eER...........................  r9 = r10 ^ 0x1
    ..D========================eER...........................  r11 = r11 + 0x1
    ..D=========================eER..........................  r8 = r8 << 0x38
    ..D==========================eER.........................  r8 = r8 >> 0x3f
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER..  u16 [r7 + 0x20f] = r11
    ...D=======================eeeeeeeeeeeeeeeeeeeeeeeeeE-R..  u16 [r7 + 529] = 0
    ...D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..  u8 [r7 + 0x238] = a2
    ...D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x271] = a1
    ...DeeeeeeeeeeeeeeeeeeeeeeE-----------------------------R  jump [r0 + 0]
```

Gas simulation at offset 14925 with total cost of 102:

```
    DeER.....................................................................................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER............................................................................  r2 = i16 [r7 + 0x219]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER............................................................................  r3 = u8 [r7 + 0x226]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER............................................................................  r10 = u8 [r7 + 0x228]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER............................................................................  r11 = i16 [r7 + 0x211]
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER...................................................  r12 = i16 [r7 + 0x213]
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER...................................................  r8 = i16 [r7 + 0x215]
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER...................................................  r9 = i16 [r7 + 0x217]
    ..D========================eE------------------------R...................................................  r10 = r3 & r10
    ..D=================================================eER..................................................  r12 = r12 << 0x1
    ..D=================================================eER..................................................  r8 = r8 << 0x1
    ..D=================================================eER..................................................  r9 = r9 << 0x1
    ...D========================eE------------------------R..................................................  r11 = r11 + 0x1
    ...D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER.................................................  u16 [r7 + 0x211] = r11
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u16 [r7 + 0x213] = r12
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u16 [r7 + 0x215] = r8
    ....D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u16 [r7 + 0x217] = r9
    ....D=================================================eE-----------------------R.........................  r2 = r2 << 0x1
    ....D==================================================eE----------------------R.........................  r10 = r10 << 0x38
    ....D===================================================eE---------------------R.........................  r10 = r10 >> 0x3f
    .....D===================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.....................  u16 [r7 + 0x219] = r2
    .....D========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 552] = 0
    .....D========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 566] = 0
    .....D========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x271] = a3
    ......DeeeeeeeeeeeeeeeeeeeeeeE--------------------------------------------------------------------------R  jump [r0 + 0]
```

Gas simulation at offset 15015 with total cost of 105:

```
    DeER........................................................................................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...............................................................................  r2 = u16 [r7 + 0x209]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...............................................................................  r9 = i16 [r7 + 0x211]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...............................................................................  r10 = i16 [r7 + 0x213]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER...............................................................................  r11 = i16 [r7 + 0x215]
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................................................  r12 = i16 [r7 + 0x217]
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................................................  r3 = i16 [r7 + 0x219]
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................................................  r4 = u8 [r7 + 0x226]
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................................................  r8 = u8 [r7 + 0x228]
    ..D=================================================eER.....................................................  r10 = r10 << 0x1
    ..D=================================================eER.....................................................  r11 = r11 << 0x1
    ..D=================================================eER.....................................................  r12 = r12 << 0x1
    ...D================================================eER.....................................................  r9 = r9 + 0x1
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER............................  u16 [r7 + 0x211] = r9
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER............................  u16 [r7 + 0x213] = r10
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER............................  u16 [r7 + 0x215] = r11
    ....D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER............................  u16 [r7 + 0x217] = r12
    ....D=========================================================================eER...........................  r2 = r2 << 0x34
    ....D==========================================================================eER..........................  r10 = r2 >> 0x34
    .....D==========================================================================eER.........................  r9 = r10 | 0x2000
    .....D========================================================================eE--R.........................  r10 = r4 & r8
    ......D=======================================================================eE--R.........................  r8 = r8 & 0xbf
    ......D=======================================================================eE--R.........................  r3 = r3 << 0x1
    ......D========================================================================eE-R.........................  r10 = r10 >> 0x7
    ......D========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER..  u16 [r7 + 0x219] = r3
    .......D=========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r7 + 0x21b] = r9
    .......D=======================================================================eeeeeeeeeeeeeeeeeeeeeeeeeE--R  u8 [r7 + 0x228] = a1
    .......D========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-R  u8 [r7 + 0x271] = a3
    .......DeeeeeeeeeeeeeeeeeeeeeeE----------------------------------------------------------------------------R  jump [r0 + 0]
```

Gas simulation at offset 15120 with total cost of 29:

```
    DeER............................  r1 = r1 + 0xfffffffffffffff0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0x8] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0] = r5
    .DeE------------------------R...  r5 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u16 [r5 + 0x21b]
    ..D=========================eER.  r9 = r8 >> 0x8
    ..D==========================eER  jump 15177 if r9 >=u 63
```

Gas simulation at offset 15143 with total cost of 74:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r9 = u64 [r5 + 0x241]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r7 = u64 [r5 + 0x249]
    DeE---------------------------------------R..................................  r10 = 0x17c80
    .D========================eeE-------------R..................................  r10 = r7 if r9 != 0
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r10 = u64 [r10 + 0x48]
    ..DeE-------------------------------------------------R......................  r7 = r5 + 0x27f
    ..D=======================eeE-------------------------R......................  r7 = r9 if r9 != 0
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 376, jump [r10 + 0]
```

Gas simulation at offset 15175 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 15192
```

Gas simulation at offset 15177 with total cost of 28:

```
    DeER...........................  r8 = r8 & 0x1f
    D=eER..........................  r7 = r7 + r8
    D==eER.........................  r7 = r7 + 0x7ff
    D===eeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u8 [r7 + 0x1a1]
    .DeeE-------------------------R  fallthrough
```

Gas simulation at offset 15192 with total cost of 124:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...................................................................................................  r8 = u8 [r5 + 0x226]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...................................................................................................  r9 = u8 [r5 + 0x228]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...................................................................................................  r10 = i16 [r5 + 0x219]
    .D========================eER..................................................................................................  r2 = r8 & r9
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER..................................................................................................  r9 = i16 [r5 + 0x211]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..........................................................................  r11 = i16 [r5 + 0x213]
    ..D=======================eeeeeeeeeeeeeeeeeeeeeeeeeER..........................................................................  r12 = i16 [r5 + 0x215]
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................................................................  r8 = i16 [r5 + 0x217]
    ..D========================eE------------------------R.........................................................................  r10 = r10 << 0x1
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER........................................................................  u16 [r5 + 0x219] = r10
    ...D===============================================eeeeeeeeeeeeeeeeeeeeeeeeeER.................................................  u8 [r5 + 0x22a] = a0
    ...D===============================================eE------------------------R.................................................  r11 = r11 << 0x1
    ...D================================================eE-----------------------R.................................................  r12 = r12 << 0x1
    ...D================================================eE-----------------------R.................................................  r8 = r8 << 0x1
    ....D================================================eE----------------------R.................................................  r9 = r9 + 0x1
    ....D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER..............................................  u16 [r5 + 0x211] = r9
    ....D================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-R..............................................  u16 [r5 + 0x213] = r11
    ....D================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-R..............................................  u16 [r5 + 0x215] = r12
    .....D======================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER........................  u16 [r5 + 0x217] = r8
    .....D========================================================================eE----------------------R........................  r2 = r2 << 0x38
    .....D=========================================================================eE---------------------R........................  r7 = r2 >> 0x3f
    ......D=========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER....................  u8 [r5 + 0x271] = a0
    ......D=======================================================================eeeeeeeeeeeeeeeeeeeeeeeeeE--R....................  r0 = u64 [r1 + 0x8]
    ......D========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-R....................  r5 = u64 [r1 + 0]
    ......D==============================================================================================eE---R....................  r1 = r1 + 0x10
    .......D===============================================================================================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 15282 with total cost of 48:

```
    DeER...............................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r2 = u16 [r7 + 0x211]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r9 = u16 [r7 + 0x209]
    .D=========================eER.....................  r10 = r2 + 0xfffffffffffffeff
    .D=========================eER.....................  r12 = r9 >> 0x4
    ..D=========================eER....................  r8 = zext16 r10
    ..D=========================eER....................  r10 = r12 & 0x38
    ..D==========================eeeeeeeeeeeeeeeeeeeeER  jump 15323 if r8 >=u 64
```

Gas simulation at offset 15310 with total cost of 16:

```
    DeER...............  r8 = r9 & 0xcff
    D=eER..............  r8 = r8 | 0x2000
    .D=eER.............  r3 = r10 + r8
    .DeeeeeeeeeeeeeeeER  jump 15344
```

Gas simulation at offset 15323 with total cost of 4:

```
    DeER...  r11 = r9 & 0xc00
    DeER...  r9 = r9 << 0x3b
    D=eER..  r9 = r9 >> 0x3d
    .D=eER.  r9 = r9 | r11
    .DeE-R.  r8 = r10 | 0x23c0
    ..D=eER  r3 = r9 | r8
    ..DeeER  fallthrough
```

Gas simulation at offset 15344 with total cost of 103:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..............................................................................  r8 = i16 [r7 + 0x219]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..............................................................................  r10 = u8 [r7 + 0x226]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..............................................................................  r11 = u8 [r7 + 0x228]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..............................................................................  r12 = i16 [r7 + 0x213]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.....................................................  r9 = i16 [r7 + 0x215]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.....................................................  r4 = i16 [r7 + 0x217]
    .D========================eE------------------------R.....................................................  r10 = r10 & r11
    .D========================eE------------------------R.....................................................  r8 = r8 << 0x1
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER....................................................  u16 [r7 + 0x219] = r8
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER....................................................  u16 [r7 + 0x21b] = r3
    ..D================================================eER....................................................  r2 = r2 + 0x1
    ..D================================================eER....................................................  r12 = r12 << 0x1
    ...D================================================eER...................................................  r9 = r9 << 0x1
    ...D================================================eER...................................................  r4 = r4 << 0x1
    ...D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER...........................  u16 [r7 + 0x211] = r2
    ...D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER...........................  u16 [r7 + 0x213] = r12
    ....D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u16 [r7 + 0x215] = r9
    ....D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u16 [r7 + 0x217] = r4
    ....D========================================================================eER..........................  r10 = r10 << 0x38
    ....D=========================================================================eER.........................  r10 = r10 >> 0x3f
    .....D=========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x271] = a3
    .....DeeeeeeeeeeeeeeeeeeeeeeE----------------------------------------------------------------------------R  jump [r0 + 0]
```

Gas simulation at offset 15422 with total cost of 29:

```
    DeER............................  r1 = r1 + 0xfffffffffffffff0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0x8] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0] = r5
    .DeE------------------------R...  r5 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u16 [r5 + 0x21b]
    ..D=========================eER.  r9 = r8 >> 0x8
    ..D==========================eER  jump 15479 if r9 >=u 63
```

Gas simulation at offset 15445 with total cost of 74:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r9 = u64 [r5 + 0x241]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r7 = u64 [r5 + 0x249]
    DeE---------------------------------------R..................................  r10 = 0x17c80
    .D========================eeE-------------R..................................  r10 = r7 if r9 != 0
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r10 = u64 [r10 + 0x48]
    ..DeE-------------------------------------------------R......................  r7 = r5 + 0x27f
    ..D=======================eeE-------------------------R......................  r7 = r9 if r9 != 0
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 382, jump [r10 + 0]
```

Gas simulation at offset 15477 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 15494
```

Gas simulation at offset 15479 with total cost of 28:

```
    DeER...........................  r8 = r8 & 0x1f
    D=eER..........................  r7 = r7 + r8
    D==eER.........................  r7 = r7 + 0x7ff
    D===eeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u8 [r7 + 0x1a1]
    .DeeE-------------------------R  fallthrough
```

Gas simulation at offset 15494 with total cost of 127:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................................................................................................  r3 = i16 [r5 + 0x217]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................................................................................................  r2 = i16 [r5 + 0x219]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................................................................................................  r4 = u8 [r5 + 0x226]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................................................................................................  r11 = u8 [r5 + 0x228]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.............................................................................  r12 = i16 [r5 + 0x213]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.............................................................................  r8 = i16 [r5 + 0x215]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.............................................................................  r9 = u8 [r5 + 0x209]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.............................................................................  r10 = i16 [r5 + 0x211]
    ..D================================================eER............................................................................  r11 = r4 & r11
    ..D================================================eER............................................................................  r12 = r12 << 0x1
    ..D================================================eER............................................................................  r8 = r8 << 0x1
    ..D================================================eER............................................................................  r3 = r3 << 0x1
    ...D================================================eER...........................................................................  r10 = r10 + 0x1
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  u16 [r5 + 0x211] = r10
    ...D================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-R..................................................  u16 [r5 + 0x213] = r12
    ...D================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-R..................................................  u16 [r5 + 0x215] = r8
    ....D===============================================eeeeeeeeeeeeeeeeeeeeeeeeeE-R..................................................  u16 [r5 + 0x217] = r3
    ....D========================================================================eER..................................................  r8 = r9 & 0x2
    ....D========================================================================eER..................................................  r9 = r9 >> 0x4
    .....D========================================================================eER.................................................  r9 = r9 & 0x4
    .....D=========================================================================eER................................................  r8 = r8 | r9
    .....D=======================================================================eE--R................................................  r7 = r7 & 0xff
    ......D=========================================================================eER...............................................  r7 = r7 >> r8
    ......D=======================================================================eE--R...............................................  r2 = r2 << 0x1
    ......D=======================================================================eE--R...............................................  r11 = r11 << 0x38
    .......D=======================================================================eE-R...............................................  r11 = r11 >> 0x3f
    .......D=========================================================================eER..............................................  r7 = r7 & 0x3
    .......D=======================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER........................  u16 [r5 + 0x219] = r2
    .......D==========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.....................  u8 [r5 + 0x22b] = a0
    ........D=======================================================================eeeeeeeeeeeeeeeeeeeeeeeeeE--R.....................  u8 [r5 + 0x271] = a4
    ........D=====================================================================eeeeeeeeeeeeeeeeeeeeeeeeeE----R.....................  r0 = u64 [r1 + 0x8]
    ........D==============================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  r5 = u64 [r1 + 0]
    ............................D===========================================================================eE-----------------------R  r1 = r1 + 0x10
    ............................D==========================================================================eeeeeeeeeeeeeeeeeeeeeeE---R  jump [r0 + 0]
```

Gas simulation at offset 15610 with total cost of 126:

```
    DeER.............................................................................................................................  r1 = r1 + 0xfffffffffffffff8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER....................................................................................................  u64 [r1 + 0] = r5
    DeE-------------------------R....................................................................................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER....................................................................................................  r3 = u8 [r7 + 0x22a]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER....................................................................................................  r2 = i16 [r7 + 0x209]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER....................................................................................................  r10 = i16 [r7 + 0x211]
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r11 = i16 [r7 + 0x213]
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r12 = i16 [r7 + 0x215]
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r8 = i16 [r7 + 0x217]
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r4 = i16 [r7 + 0x219]
    ..D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  r9 = u8 [r7 + 0x226]
    ..D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  r5 = u8 [r7 + 0x228]
    ...D================================================eE------------------------R..................................................  r11 = r11 << 0x1
    ...D================================================eE------------------------R..................................................  r12 = r12 << 0x1
    ...D=================================================eE-----------------------R..................................................  r8 = r8 << 0x1
    ...D=================================================eE-----------------------R..................................................  r10 = r10 + 0x1
    ....D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER................................................  u16 [r7 + 0x211] = r10
    ....D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER................................................  u16 [r7 + 0x213] = r11
    ....D========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u16 [r7 + 0x215] = r12
    ....D========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u16 [r7 + 0x217] = r8
    .....D=========================================================================eE----------------------R.........................  r5 = r5 & r9
    .....D=========================================================================eE----------------------R.........................  r9 = r9 & 0x10
    .....D==========================================================================eE---------------------R.........................  r3 = r3 << 0x4
    .....D==========================================================================eE---------------------R.........................  r9 = r9 << 0x8
    ......D==========================================================================eE--------------------R.........................  r8 = r9 | r3
    ......D==========================================================================eE--------------------R.........................  r2 = r2 << 0x31
    ......D===========================================================================eE-------------------R.........................  r4 = r4 << 0x1
    .......D==========================================================================eE-------------------R.........................  r9 = r2 >> 0x3d
    .......D===========================================================================eE------------------R.........................  r5 = r5 >> 0x7
    .......D===========================================================================eE------------------R.........................  r8 = r8 | r9
    ........D===========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER..................  u16 [r7 + 0x219] = r4
    ........D===========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER..................  u16 [r7 + 0x21b] = r8
    ........D=============================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x271] = s0
    .............................D========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  r5 = u64 [r1 + 0]
    .............................D===============================================================================eE-----------------R  r1 = r1 + 0x8
    .............................DeeeeeeeeeeeeeeeeeeeeeeE---------------------------------------------------------------------------R  jump [r0 + 0]
```

Gas simulation at offset 15732 with total cost of 29:

```
    DeER............................  r1 = r1 + 0xfffffffffffffff0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0x8] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0] = r5
    .DeE------------------------R...  r5 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u16 [r5 + 0x21b]
    ..D=========================eER.  r9 = r8 >> 0x8
    ..D==========================eER  jump 15789 if r9 >=u 63
```

Gas simulation at offset 15755 with total cost of 74:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r9 = u64 [r5 + 0x241]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r7 = u64 [r5 + 0x249]
    DeE---------------------------------------R..................................  r10 = 0x17c80
    .D========================eeE-------------R..................................  r10 = r7 if r9 != 0
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r10 = u64 [r10 + 0x48]
    ..DeE-------------------------------------------------R......................  r7 = r5 + 0x27f
    ..D=======================eeE-------------------------R......................  r7 = r9 if r9 != 0
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 388, jump [r10 + 0]
```

Gas simulation at offset 15787 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 15804
```

Gas simulation at offset 15789 with total cost of 28:

```
    DeER...........................  r8 = r8 & 0x1f
    D=eER..........................  r7 = r7 + r8
    D==eER.........................  r7 = r7 + 0x7ff
    D===eeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u8 [r7 + 0x1a1]
    .DeeE-------------------------R  fallthrough
```

Gas simulation at offset 15804 with total cost of 124:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...................................................................................................  r8 = u8 [r5 + 0x226]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...................................................................................................  r9 = u8 [r5 + 0x228]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...................................................................................................  r10 = i16 [r5 + 0x219]
    .D========================eER..................................................................................................  r2 = r8 & r9
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER..................................................................................................  r9 = i16 [r5 + 0x211]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..........................................................................  r11 = i16 [r5 + 0x213]
    ..D=======================eeeeeeeeeeeeeeeeeeeeeeeeeER..........................................................................  r12 = i16 [r5 + 0x215]
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................................................................  r8 = i16 [r5 + 0x217]
    ..D========================eE------------------------R.........................................................................  r10 = r10 << 0x1
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER........................................................................  u16 [r5 + 0x219] = r10
    ...D===============================================eeeeeeeeeeeeeeeeeeeeeeeeeER.................................................  u8 [r5 + 0x22c] = a0
    ...D===============================================eE------------------------R.................................................  r11 = r11 << 0x1
    ...D================================================eE-----------------------R.................................................  r12 = r12 << 0x1
    ...D================================================eE-----------------------R.................................................  r8 = r8 << 0x1
    ....D================================================eE----------------------R.................................................  r9 = r9 + 0x1
    ....D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER..............................................  u16 [r5 + 0x211] = r9
    ....D================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-R..............................................  u16 [r5 + 0x213] = r11
    ....D================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-R..............................................  u16 [r5 + 0x215] = r12
    .....D======================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER........................  u16 [r5 + 0x217] = r8
    .....D========================================================================eE----------------------R........................  r2 = r2 << 0x38
    .....D=========================================================================eE---------------------R........................  r7 = r2 >> 0x3f
    ......D=========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER....................  u8 [r5 + 0x271] = a0
    ......D=======================================================================eeeeeeeeeeeeeeeeeeeeeeeeeE--R....................  r0 = u64 [r1 + 0x8]
    ......D========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-R....................  r5 = u64 [r1 + 0]
    ......D==============================================================================================eE---R....................  r1 = r1 + 0x10
    .......D===============================================================================================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 15894 with total cost of 107:

```
    DeER..........................................................................................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.................................................................................  r8 = u8 [r7 + 0x22a]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.................................................................................  r9 = u16 [r7 + 0x209]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.................................................................................  r4 = i16 [r7 + 0x211]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER.................................................................................  r11 = i16 [r7 + 0x213]
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER........................................................  r12 = i16 [r7 + 0x215]
    .D=========================eE------------------------R........................................................  r8 = r8 << 0x4
    .D=========================eE------------------------R........................................................  r9 = r9 >> 0xc
    ..D=========================eE-----------------------R........................................................  r2 = r8 | r9
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER........................................................  r9 = i16 [r7 + 0x217]
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER.......................................................  r3 = i16 [r7 + 0x219]
    ...D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................................................  r8 = u8 [r7 + 0x226]
    ...D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER...............................  r10 = u8 [r7 + 0x228]
    ...D================================================eE------------------------R...............................  r11 = r11 << 0x1
    ...D=================================================eE-----------------------R...............................  r12 = r12 << 0x1
    ....D================================================eE-----------------------R...............................  r9 = r9 << 0x1
    ....D=================================================eE----------------------R...............................  r4 = r4 + 0x1
    ....D==================================================eeeeeeeeeeeeeeeeeeeeeeeeeER............................  u16 [r7 + 0x211] = r4
    ....D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-R............................  u16 [r7 + 0x213] = r11
    .....D================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-R............................  u16 [r7 + 0x215] = r12
    .....D=======================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER......  u16 [r7 + 0x217] = r9
    .....D=========================================================================eE----------------------R......  r10 = r10 & r8
    .....D=========================================================================eE----------------------R......  r8 = r8 & 0x10
    ......D=========================================================================eE---------------------R......  r3 = r3 << 0x1
    ......D=========================================================================eE---------------------R......  r8 = r8 << 0x8
    ......D=========================================================================eE---------------------R......  r10 = r10 >> 0x7
    ......D==========================================================================eE--------------------R......  r8 = r8 | r2
    .......D==========================================================================eE-------------------R......  r8 = r8 | 0x8
    .......D=========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER..  u16 [r7 + 0x219] = r3
    .......D===========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r7 + 0x21b] = r8
    .......D=========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeE--R  u8 [r7 + 0x271] = a3
    ........DeeeeeeeeeeeeeeeeeeeeeeE-----------------------------------------------------------------------------R  jump [r0 + 0]
```

Gas simulation at offset 16006 with total cost of 29:

```
    DeER............................  r1 = r1 + 0xfffffffffffffff0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0x8] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0] = r5
    .DeE------------------------R...  r5 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u16 [r5 + 0x21b]
    ..D=========================eER.  r9 = r8 >> 0x8
    ..D==========================eER  jump 16077 if r9 >=u 63
```

Gas simulation at offset 16029 with total cost of 74:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r9 = u64 [r5 + 0x241]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r7 = u64 [r5 + 0x249]
    DeE---------------------------------------R..................................  r10 = 0x17c80
    .D========================eeE-------------R..................................  r10 = r7 if r9 != 0
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r10 = u64 [r10 + 0x48]
    ..DeE-------------------------------------------------R......................  r7 = r5 + 0x27f
    ..D=======================eeE-------------------------R......................  r7 = r9 if r9 != 0
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 394, jump [r10 + 0]
```

Gas simulation at offset 16061 with total cost of 27:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u8 [r5 + 0x227]
    D=========================eER.  r8 = r8 & 0x18
    DeeeeeeeeeeeeeeeeeeeeeeeeeE-R.  u8 [r5 + 0x22d] = a0
    D==========================eER  jump 16106 if r8 != 0
```

Gas simulation at offset 16075 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 16142
```

Gas simulation at offset 16077 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeE---------------------------------------R.............  r8 = r8 & 0x1f
    D=eE--------------------------------------R.............  r7 = r7 + r8
    D==eE-------------------------------------R.............  r7 = r7 + 0x7ff
    .D==eeeeeeeeeeeeeeeeeeeeeeeeeE------------R.............  r7 = u8 [r7 + 0x1a1]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.............  r8 = u8 [r5 + 0x227]
    .D=========================eE-------------R.............  r8 = r8 & 0x18
    .D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x22d] = a0
    ..D=========================eE-------------------------R  jump 16142 if r8 == 0
```

Gas simulation at offset 16106 with total cost of 46:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER......  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R......  r8 = u16 [r5 + 0x209]
    D=========================eE--------------R......  r9 = r8 & 0x1f
    .D========================eE--------------R......  r8 = r8 & 0xffffffffffffffe0
    .D=========================eeeeeeeeeeeeeeeeeeeeER  jump 16131 if r9 != 31
```

Gas simulation at offset 16121 with total cost of 26:

```
    DeER.........................  r8 = r8 ^ 0x400
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x209] = r8
    DeeeeeeeeeeeeeeeE-----------R  jump 16142
```

Gas simulation at offset 16131 with total cost of 27:

```
    DeER..........................  r8 = r8 | r9
    D=eER.........................  r8 = r8 + 0x1
    D==eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x209] = r8
    DeeE-------------------------R  fallthrough
```

Gas simulation at offset 16142 with total cost of 130:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..........................................................................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........................................................................................  r2 = u8 [r5 + 0x22c]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........................................................................................  r3 = u16 [r5 + 0x219]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........................................................................................  r10 = u8 [r5 + 0x226]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R..........................................................................................  r11 = u8 [r5 + 0x228]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER................................................................................  r12 = u8 [r5 + 0x22b]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER................................................................................  r4 = i16 [r5 + 0x211]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER................................................................................  r9 = u16 [r5 + 0x213]
    ..D========================eE-----------------------R................................................................................  r10 = r10 & r11
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER..............................................................................  r11 = u16 [r5 + 0x215]
    ..D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.......................................................  r8 = u16 [r5 + 0x217]
    ..D================================================eE------------------------R.......................................................  r9 = r9 & 0xffffffffffffff00
    ...D================================================eE-----------------------R.......................................................  r9 = r9 | r2
    ...D===============================================eE------------------------R.......................................................  r7 = r7 & 0xff
    ...D=================================================eE----------------------R.......................................................  r11 = r11 & 0xffffffffffffff00
    ...D========================================================================eER......................................................  r8 = r8 & 0xffffffffffffff00
    ....D=================================================eE----------------------R......................................................  r7 = r7 | r11
    ....D===============================================eE------------------------R......................................................  r11 = r12 << 0x3f
    ....D================================================eE-----------------------R......................................................  r11 = r11 >>a 0x3f
    .....D================================================eE----------------------R......................................................  r11 = r11 & 0xff
    .....D=======================================================================eER.....................................................  r8 = r8 | r11
    .....D===============================================eE------------------------R.....................................................  r11 = r3 & 0xffffffffffffff00
    ......D===============================================eE-----------------------R.....................................................  r12 = r12 << 0x6
    ......D================================================eE----------------------R.....................................................  r12 = sext8 r12
    ......D=================================================eE---------------------R.....................................................  r12 = r12 << 0x31
    ......D==================================================eE--------------------R.....................................................  r12 = r12 >> 0x38
    .......D==================================================eE-------------------R.....................................................  r11 = r11 | r12
    .......D===============================================eE----------------------R.....................................................  r4 = r4 + 0x1
    .......D===============================================eE----------------------R.....................................................  r10 = r10 << 0x38
    .......D================================================eE---------------------R.....................................................  r9 = r9 << 0x1
    ........D===============================================eE---------------------R.....................................................  r7 = r7 << 0x1
    ........D================================================eE--------------------R.....................................................  r10 = r10 >> 0x3f
    ...........................................D==================================eER....................................................  r8 = r8 << 0x1
    ...........................................D=============eeeeeeeeeeeeeeeeeeeeeeeeeER.................................................  u16 [r5 + 0x211] = r4
    ...........................................D==============eeeeeeeeeeeeeeeeeeeeeeeeeER................................................  u16 [r5 + 0x213] = r9
    ...........................................D===============eeeeeeeeeeeeeeeeeeeeeeeeeER...............................................  u16 [r5 + 0x215] = r7
    ............................................D==================================eeeeeeeeeeeeeeeeeeeeeeeeeER...........................  u16 [r5 + 0x217] = r8
    .....................................................D============================eE---------------------R...........................  r11 = r11 << 0x1
    .....................................................D=============================eeeeeeeeeeeeeeeeeeeeeeeeeER.......................  u16 [r5 + 0x219] = r11
    .....................................................D=============================eeeeeeeeeeeeeeeeeeeeeeeeeER.......................  u8 [r5 + 0x271] = a3
    .....................................................D==============================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r0 = u64 [r1 + 0x8]
    .......................................................D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER..  r5 = u64 [r1 + 0]
    ..............................................................................D=============================eE--------------------R..  r1 = r1 + 0x10
    ..............................................................................D==============================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 16290 with total cost of 105:

```
    DeER........................................................................................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...............................................................................  r3 = i16 [r7 + 0x217]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...............................................................................  r2 = i16 [r7 + 0x219]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...............................................................................  r10 = u8 [r7 + 0x226]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER...............................................................................  r11 = u8 [r7 + 0x228]
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................................................  r12 = i16 [r7 + 0x213]
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................................................  r8 = i16 [r7 + 0x215]
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................................................  r4 = u16 [r7 + 0x209]
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................................................  r9 = i16 [r7 + 0x211]
    ..D=================================================eER.....................................................  r10 = r10 & r11
    ..D=================================================eER.....................................................  r12 = r12 << 0x1
    ..D=================================================eER.....................................................  r8 = r8 << 0x1
    ...D================================================eER.....................................................  r3 = r3 << 0x1
    ...D=================================================eER....................................................  r9 = r9 + 0x1
    ...D==================================================eeeeeeeeeeeeeeeeeeeeeeeeeER...........................  u16 [r7 + 0x211] = r9
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-R...........................  u16 [r7 + 0x213] = r12
    ....D================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-R...........................  u16 [r7 + 0x215] = r8
    ....D================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-R...........................  u16 [r7 + 0x217] = r3
    ....D=========================================================================eER...........................  r4 = r4 << 0x34
    .....D=========================================================================eER..........................  r9 = r4 >> 0x34
    .....D==========================================================================eER.........................  r8 = r9 | 0x2000
    ......D=======================================================================eE--R.........................  r2 = r2 << 0x1
    ......D=======================================================================eE--R.........................  r10 = r10 << 0x38
    ......D========================================================================eE-R.........................  r10 = r10 >> 0x3f
    ......D========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER..  u16 [r7 + 0x219] = r2
    .......D=========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r7 + 0x21b] = r8
    .......D========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-R  u8 [r7 + 0x271] = a3
    .......DeeeeeeeeeeeeeeeeeeeeeeE----------------------------------------------------------------------------R  jump [r0 + 0]
```

Gas simulation at offset 16390 with total cost of 29:

```
    DeER............................  r1 = r1 + 0xfffffffffffffff0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0x8] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0] = r5
    .DeE------------------------R...  r5 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u16 [r5 + 0x21b]
    ..D=========================eER.  r9 = r8 >> 0x8
    ..D==========================eER  jump 16461 if r9 >=u 63
```

Gas simulation at offset 16413 with total cost of 74:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r9 = u64 [r5 + 0x241]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r7 = u64 [r5 + 0x249]
    DeE---------------------------------------R..................................  r10 = 0x17c80
    .D========================eeE-------------R..................................  r10 = r7 if r9 != 0
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r10 = u64 [r10 + 0x48]
    ..DeE-------------------------------------------------R......................  r7 = r5 + 0x27f
    ..D=======================eeE-------------------------R......................  r7 = r9 if r9 != 0
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 400, jump [r10 + 0]
```

Gas simulation at offset 16445 with total cost of 27:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u8 [r5 + 0x227]
    D=========================eER.  r8 = r8 & 0x18
    DeeeeeeeeeeeeeeeeeeeeeeeeeE-R.  u8 [r5 + 0x22d] = a0
    D==========================eER  jump 16490 if r8 != 0
```

Gas simulation at offset 16459 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 16526
```

Gas simulation at offset 16461 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeE---------------------------------------R.............  r8 = r8 & 0x1f
    D=eE--------------------------------------R.............  r7 = r7 + r8
    D==eE-------------------------------------R.............  r7 = r7 + 0x7ff
    .D==eeeeeeeeeeeeeeeeeeeeeeeeeE------------R.............  r7 = u8 [r7 + 0x1a1]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.............  r8 = u8 [r5 + 0x227]
    .D=========================eE-------------R.............  r8 = r8 & 0x18
    .D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x22d] = a0
    ..D=========================eE-------------------------R  jump 16526 if r8 == 0
```

Gas simulation at offset 16490 with total cost of 46:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER......  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R......  r9 = u16 [r5 + 0x209]
    D=========================eE--------------R......  r10 = r9 & 0x1f
    .D========================eE--------------R......  r9 = r9 & 0xffffffffffffffe0
    .D=========================eeeeeeeeeeeeeeeeeeeeER  jump 16515 if r10 != 31
```

Gas simulation at offset 16505 with total cost of 26:

```
    DeER.........................  r9 = r9 ^ 0x400
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x209] = r9
    DeeeeeeeeeeeeeeeE-----------R  jump 16526
```

Gas simulation at offset 16515 with total cost of 27:

```
    DeER..........................  r9 = r9 | r10
    D=eER.........................  r9 = r9 + 0x1
    D==eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x209] = r9
    DeeE-------------------------R  fallthrough
```

Gas simulation at offset 16526 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r9 = u8 [r5 + 0x22b]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r10 = u8 [r5 + 0x22c]
    .D========================eE--------------R.............  r11 = r9 << 0x3f
    .D========================eE--------------R.............  r9 = r9 << 0x6
    .D=========================eE-------------R.............  r11 = r11 >>a 0x3f
    ..D========================eE-------------R.............  r9 = sext8 r9
    ..D=========================eE------------R.............  r9 = r9 >> 0x7
    ..D=======================eeeeeeeeeeeeeeeeeeeeeeeeeER...  u8 [r5 + 0x213] = a3
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-----------------------R...  u8 [r5 + 0x215] = a0
    ...D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u8 [r5 + 0x217] = a4
    ...D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x219] = a2
    ...DeE-------------------------------------------------R  jump 16672 if r8 == 0
```

Gas simulation at offset 16568 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.......  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r7 = u16 [r5 + 0x209]
    DeE---------------------------------------R.......  r10 = 0x7
    .D========================eE--------------R.......  r9 = r7 << 0x31
    .D=========================eE-------------R.......  r9 = r9 >> 0x3d
    .D==========================eeeeeeeeeeeeeeeeeeeeER  jump 16614 if r9 != r10
```

Gas simulation at offset 16585 with total cost of 22:

```
    DeER.....................  r9 = r7 >> 0x5
    D=eER....................  r10 = r9 & 0x1f
    .DeER....................  r11 = 0x1d
    .D=eeeeeeeeeeeeeeeeeeeeER  jump 16634 if r10 == r11
```

Gas simulation at offset 16597 with total cost of 21:

```
    DeER....................  r11 = 0x1f
    D=eeeeeeeeeeeeeeeeeeeeER  jump 16649 if r10 != r11
```

Gas simulation at offset 16603 with total cost of 26:

```
    DeER.........................  r7 = r7 & 0x8c1f
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x209] = r7
    DeeeeeeeeeeeeeeeE-----------R  jump 16672
```

Gas simulation at offset 16614 with total cost of 28:

```
    DeER...........................  r9 = r9 + 0x1
    DeER...........................  r7 = r7 & 0x8fff
    D=eER..........................  r9 = r9 << 0xc
    D==eER.........................  r7 = r7 | r9
    .D==eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x209] = r7
    .DeeeeeeeeeeeeeeeE------------R  jump 16672
```

Gas simulation at offset 16634 with total cost of 27:

```
    DeER..........................  r7 = r7 & 0x8c1f
    D=eER.........................  r7 = r7 ^ 0x800
    D==eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x209] = r7
    DeeeeeeeeeeeeeeeE------------R  jump 16672
```

Gas simulation at offset 16649 with total cost of 29:

```
    DeER............................  r9 = r9 << 0x5
    DeER............................  r7 = r7 & 0x8c1f
    D=eER...........................  r8 = r9 + 0x20
    .D=eER..........................  r8 = r8 & 0x3e0
    .D==eER.........................  r7 = r7 | r8
    .D===eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x209] = r7
    .DeeE--------------------------R  fallthrough
```

Gas simulation at offset 16672 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r7 = u8 [r5 + 0x226]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r8 = u8 [r5 + 0x228]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r9 = i16 [r5 + 0x211]
    .D========================eE--------------R.............  r7 = r7 & r8
    .D========================eE--------------R.............  r9 = r9 + 0x1
    .D=========================eE-------------R.............  r7 = r7 << 0x38
    .D==========================eE------------R.............  r7 = r7 >> 0x3f
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x271] = a0
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE--R  u16 [r5 + 0x211] = r9
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R  r0 = u64 [r1 + 0x8]
    ..D=======================eeeeeeeeeeeeeeeeeeeeeeeeeE---R  r5 = u64 [r1 + 0]
    ...D========================eE-------------------------R  r1 = r1 + 0x10
    ...D========================eeeeeeeeeeeeeeeeeeeeeeE----R  jump [r0 + 0]
```

Gas simulation at offset 16715 with total cost of 54:

```
    DeER.....................................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER............................  r8 = u16 [r7 + 0x209]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER............................  r10 = u8 [r7 + 0x227]
    .D=========================eER...........................  r11 = r8 << 0x34
    .D==========================eER..........................  r11 = r11 >> 0x34
    ..D==========================eER.........................  r9 = r11 | 0x2000
    ..D========================eE--R.........................  r10 = r10 & 0x18
    ..D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r7 + 0x21b] = r9
    ...D========================eE--------------------------R  jump 16768 if r10 == 0
```

Gas simulation at offset 16747 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  r9 = u16 [r7 + 0x20b]
    DeE---------------------------------------R............  r8 = r8 & 0xfffffffffffffbe0
    D=========================eE--------------R............  r9 = r9 & 0x41f
    .D=========================eE-------------R............  r8 = r8 | r9
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r7 + 0x209] = r8
    .DeeE-------------------------------------------------R  fallthrough
```

Gas simulation at offset 16768 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r8 = u8 [r7 + 0x226]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r9 = u8 [r7 + 0x228]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r10 = i16 [r7 + 0x211]
    .D========================eE--------------R.............  r8 = r8 & r9
    .D========================eE--------------R.............  r10 = r10 + 0x1
    .D=========================eE-------------R.............  r8 = r8 << 0x38
    .D==========================eE------------R.............  r8 = r8 >> 0x3f
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x271] = a1
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE--R  u16 [r7 + 0x211] = r10
    ..DeeeeeeeeeeeeeeeeeeeeeeE-----------------------------R  jump [r0 + 0]
```

Gas simulation at offset 16803 with total cost of 29:

```
    DeER............................  r1 = r1 + 0xfffffffffffffff0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0x8] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0] = r5
    .DeE------------------------R...  r5 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u16 [r5 + 0x21b]
    ..D=========================eER.  r9 = r8 >> 0x8
    ..D==========================eER  jump 16860 if r9 >=u 63
```

Gas simulation at offset 16826 with total cost of 74:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r9 = u64 [r5 + 0x241]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r7 = u64 [r5 + 0x249]
    DeE---------------------------------------R..................................  r10 = 0x17c80
    .D========================eeE-------------R..................................  r10 = r7 if r9 != 0
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r10 = u64 [r10 + 0x48]
    ..DeE-------------------------------------------------R......................  r7 = r5 + 0x27f
    ..D=======================eeE-------------------------R......................  r7 = r9 if r9 != 0
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 406, jump [r10 + 0]
```

Gas simulation at offset 16858 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 16875
```

Gas simulation at offset 16860 with total cost of 28:

```
    DeER...........................  r8 = r8 & 0x1f
    D=eER..........................  r7 = r7 + r8
    D==eER.........................  r7 = r7 + 0x7ff
    D===eeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u8 [r7 + 0x1a1]
    .DeeE-------------------------R  fallthrough
```

Gas simulation at offset 16875 with total cost of 72:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...............................................  r8 = u8 [r5 + 0x226]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...............................................  r9 = u8 [r5 + 0x228]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...............................................  r10 = i16 [r5 + 0x211]
    D=========================eER..............................................  r8 = r8 & r9
    .D========================eER..............................................  r10 = r10 + 0x1
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER.....................  u16 [r5 + 0x211] = r10
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R.....................  u8 [r5 + 0x22a] = a0
    .D=========================eE------------------------R.....................  r8 = r8 << 0x38
    ..D=========================eE-----------------------R.....................  r8 = r8 >> 0x3f
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER...................  u8 [r5 + 0x271] = a1
    ..D=======================eeeeeeeeeeeeeeeeeeeeeeeeeE---R...................  r0 = u64 [r1 + 0x8]
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE--R...................  r5 = u64 [r1 + 0]
    ...D===============================================eE--R...................  r1 = r1 + 0x10
    ...D===============================================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 16921 with total cost of 48:

```
    DeER...............................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r2 = u16 [r7 + 0x211]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r9 = u16 [r7 + 0x209]
    DeE-------------------------R......................  r11 = 0xc00
    .D=========================eER.....................  r10 = r2 + 0xfffffffffffffeff
    .D=========================eER.....................  r12 = r9 >> 0x4
    ..D=========================eER....................  r8 = zext16 r10
    ..DeE-------------------------R....................  r3 = 0x40
    ..D=========================eER....................  r10 = r12 & 0x38
    ...D=========================eeeeeeeeeeeeeeeeeeeeER  jump 16968 if r8 >=u r3
```

Gas simulation at offset 16955 with total cost of 16:

```
    DeER...............  r8 = r9 & 0xcff
    D=eER..............  r8 = r8 | 0x2000
    .D=eER.............  r9 = r10 + r8
    .DeeeeeeeeeeeeeeeER  jump 16989
```

Gas simulation at offset 16968 with total cost of 4:

```
    DeER...  r11 = r9 & 0xc00
    DeER...  r9 = r9 << 0x3b
    D=eER..  r9 = r9 >> 0x3d
    .D=eER.  r9 = r9 | r11
    .DeE-R.  r8 = r10 | 0x23c0
    .D==eER  r9 = r9 | r8
    ..DeeER  fallthrough
```

Gas simulation at offset 16989 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER............................  r8 = u8 [r7 + 0x226]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER............................  r10 = u8 [r7 + 0x228]
    DeE------------------------R............................  r2 = r2 + 0x1
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...........................  u16 [r7 + 0x211] = r2
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................  u16 [r7 + 0x21b] = r9
    .D========================eER...........................  r8 = r8 & r10
    .D=========================eER..........................  r8 = r8 << 0x38
    .D==========================eER.........................  r8 = r8 >> 0x3f
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x271] = a1
    ..DeeeeeeeeeeeeeeeeeeeeeeE-----------------------------R  jump [r0 + 0]
```

Gas simulation at offset 17023 with total cost of 29:

```
    DeER............................  r1 = r1 + 0xfffffffffffffff0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0x8] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0] = r5
    .DeE------------------------R...  r5 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u16 [r5 + 0x21b]
    ..D=========================eER.  r9 = r8 >> 0x8
    ..D==========================eER  jump 17080 if r9 >=u 63
```

Gas simulation at offset 17046 with total cost of 74:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r9 = u64 [r5 + 0x241]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r7 = u64 [r5 + 0x249]
    DeE---------------------------------------R..................................  r10 = 0x17c80
    .D========================eeE-------------R..................................  r10 = r7 if r9 != 0
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r10 = u64 [r10 + 0x48]
    ..DeE-------------------------------------------------R......................  r7 = r5 + 0x27f
    ..D=======================eeE-------------------------R......................  r7 = r9 if r9 != 0
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 412, jump [r10 + 0]
```

Gas simulation at offset 17078 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 17095
```

Gas simulation at offset 17080 with total cost of 28:

```
    DeER...........................  r8 = r8 & 0x1f
    D=eER..........................  r7 = r7 + r8
    D==eER.........................  r7 = r7 + 0x7ff
    D===eeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u8 [r7 + 0x1a1]
    .DeeE-------------------------R  fallthrough
```

Gas simulation at offset 17095 with total cost of 76:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...................................................  r8 = u8 [r5 + 0x226]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...................................................  r9 = u8 [r5 + 0x228]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...................................................  r10 = u8 [r5 + 0x209]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...................................................  r11 = i16 [r5 + 0x211]
    .D========================eER..................................................  r8 = r8 & r9
    .D========================eER..................................................  r9 = r10 & 0x2
    .D========================eER..................................................  r10 = r10 >> 0x4
    ..D========================eER.................................................  r10 = r10 & 0x4
    ..D=========================eER................................................  r9 = r9 | r10
    ..D=======================eE--R................................................  r7 = r7 & 0xff
    ...D=========================eER...............................................  r7 = r7 >> r9
    ...D=======================eE--R...............................................  r11 = r11 + 0x1
    ...D=======================eE--R...............................................  r8 = r8 << 0x38
    ....D=======================eE-R...............................................  r8 = r8 >> 0x3f
    ....D=========================eER..............................................  r7 = r7 & 0x3
    ....D=======================eeeeeeeeeeeeeeeeeeeeeeeeeER........................  u16 [r5 + 0x211] = r11
    ....D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER.....................  u8 [r5 + 0x22b] = a0
    .....D=======================eeeeeeeeeeeeeeeeeeeeeeeeeE--R.....................  u8 [r5 + 0x271] = a1
    .....D=====================eeeeeeeeeeeeeeeeeeeeeeeeeE----R.....................  r0 = u64 [r1 + 0x8]
    .....D==============================================eeeeeeeeeeeeeeeeeeeeeeeeeER  r5 = u64 [r1 + 0]
    .....D===============================================eE-----------------------R  r1 = r1 + 0x10
    ......D=============================================eeeeeeeeeeeeeeeeeeeeeeE---R  jump [r0 + 0]
```

Gas simulation at offset 17167 with total cost of 47:

```
    DeER..............................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.....................  r8 = u8 [r7 + 0x226]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.....................  r10 = u8 [r7 + 0x233]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.....................  r9 = i8 [r7 + 0x235]
    .D=========================eER....................  r11 = r8 & 0x20
    .D==========================eeeeeeeeeeeeeeeeeeeeER  jump 17217 if r11 != 0
```

Gas simulation at offset 17189 with total cost of 30:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.....  r11 = i16 [r7 + 0x20f]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.....  r12 = u8 [r7 + 0x234]
    DeE------------------------R.....  r9 = r9 >>a 0x3f
    .D========================eeER...  i32 r11 = r11 - r12
    .D==========================eER..  r9 = r9 ^ r11
    .D===========================eER.  r9 = r9 & 0x7
    ..DeE--------------------------R.  r10 = r10 << 0x4
    ..D===========================eER  r9 = r9 | r10
    ..DeeeeeeeeeeeeeeeE-------------R  jump 17272
```

Gas simulation at offset 17217 with total cost of 38:

```
    DeeeER...................................  r9 = r9 <s 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.............  r11 = i16 [r7 + 0x20f]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER............  r12 = u8 [r7 + 0x234]
    .DeE------------------------R............  r2 = r10 & 0xe
    .DeE------------------------R............  r10 = 0xfffffffffffffff8
    ..DeE-----------------------R............  r3 = 0x7
    ..D========================eeER..........  i32 r11 = r11 - r12
    ..D==========================eER.........  r11 = r11 & 0xf
    ...D==========================eeeER......  r12 = r11 <u 0x8
    ....D============================eeER....  r10 = 0 if r12 != 0
    ....D============================eE-R....  r12 = r12 ^ r9
    .....D=============================eER...  r10 = r10 + r11
    .....D============================eE-R...  r11 = r12 ^ 0x1
    .....D=============================eER...  r11 = r2 | r11
    ......D=============================eER..  r12 = r3 - r10
    ......D=============================eeER.  r12 = r10 if r9 == 0
    .......D============================eE-R.  r9 = r11 << 0x4
    .......D==============================eER  r9 = r9 + r12
    .......DeeE-----------------------------R  fallthrough
```

Gas simulation at offset 17272 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................  r10 = u8 [r7 + 0x228]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................  r11 = i16 [r7 + 0x211]
    D=========================eER..........................  r8 = r8 & r10
    D=========================eER..........................  r11 = r11 + 0x1
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u16 [r7 + 0x211] = r11
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R.  u8 [r7 + 0x21b] = a2
    .D=========================eE------------------------R.  r8 = r8 >> 0x7
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x271] = a1
    ..DeeeeeeeeeeeeeeeeeeeeeeE----------------------------R  jump [r0 + 0]
```

Gas simulation at offset 17303 with total cost of 52:

```
    DeER...................................................  r1 = r1 + 0xffffffffffffffe8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u64 [r1 + 0x10] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u64 [r1 + 0x8] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u64 [r1 + 0] = r6
    .D.....................................................  r5 = r7
    .DeE------------------------R..........................  r6 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r8 = u8 [r6 + 0x226]
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  r9 = u8 [r6 + 0x233]
    ..D=========================eE-----------------------R.  r10 = r8 & 0x20
    ...D================================================eER  r7 = r9 << 0x4
    ...D=========================eE-----------------------R  jump 17392 if r10 != 0
```

Gas simulation at offset 17337 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeE---------------------------------------R  r8 = r8 & 0x8
    D=eE--------------------------------------R  r8 = r8 << 0x9
    D==eE-------------------------------------R  r7 = r7 | r8
    .D==eE------------------------------------R  r7 = r7 >> 0x8
    .D===eeeeeeeeeeeeeeeeeeeeeeeeeE-----------R  u8 [r6 + 0x21c] = a0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R  r8 = u16 [r6 + 0x21b]
    ..D========================eE-------------R  r7 = r8 >> 0x8
    ..D=========================eE------------R  jump 17420 if r7 <u 63
```

Gas simulation at offset 17365 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.......  unlikely
    DeE---------------------------------------R.......  r8 = r8 & 0x1f
    D=eE--------------------------------------R.......  r8 = r8 + r5
    .D=eE-------------------------------------R.......  r7 = r8 + 0x7ff
    .D==eeeeeeeeeeeeeeeeeeeeeeeeeE------------R.......  r7 = u8 [r7 + 0x1a1]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......  r8 = u8 [r6 + 0x235]
    ..D========================eE-------------R.......  r8 = r8 & 0x40
    ..D=========================eeeeeeeeeeeeeeeeeeeeER  jump 17462 if r8 != 0
```

Gas simulation at offset 17390 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 17509
```

Gas simulation at offset 17392 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeE---------------------------------------R  r9 = r9 << 0xc
    D=eE--------------------------------------R  r7 = r7 | r9
    D==eE-------------------------------------R  r7 = r7 << 0x33
    .D==eE------------------------------------R  r7 = r7 >> 0x3b
    .D===eeeeeeeeeeeeeeeeeeeeeeeeeE-----------R  u8 [r6 + 0x21c] = a0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R  r8 = u16 [r6 + 0x21b]
    ..D========================eE-------------R  r7 = r8 >> 0x8
    ..D=========================eE------------R  jump 17365 if r7 >=u 63
```

Gas simulation at offset 17420 with total cost of 74:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r9 = u64 [r6 + 0x241]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r7 = u64 [r6 + 0x249]
    DeE---------------------------------------R..................................  r10 = 0x17c80
    .D========================eeE-------------R..................................  r10 = r7 if r9 != 0
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r10 = u64 [r10 + 0x48]
    ..DeE-------------------------------------------------R......................  r7 = r6 + 0x27f
    ..D=======================eeE-------------------------R......................  r7 = r9 if r9 != 0
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 418, jump [r10 + 0]
```

Gas simulation at offset 17452 with total cost of 46:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.....................  r8 = u8 [r6 + 0x235]
    D=========================eER....................  r8 = r8 & 0x40
    D==========================eeeeeeeeeeeeeeeeeeeeER  jump 17509 if r8 == 0
```

Gas simulation at offset 17462 with total cost of 11:

```
    DeER..........  r8 = r7 & 0xff
    DeER..........  r9 = r7 << 0xb
    .DeER.........  r10 = r8 << 0x1
    .D=eER........  r9 = r9 | r10
    .DeE-R........  r10 = 0x22110
    ..DeER........  r7 = r7 << 0xf
    ..DeER........  r8 = r8 << 0x5
    ..D=eER.......  r7 = r7 | r8
    ..D=eER.......  r9 = r9 & r10
    ...D=eER......  r7 = r7 & 0x88440
    ...D==eER.....  r7 = r7 | r9
    ...D===eeeER..  r7 = r7 * 0x10101
    ....D=====eeER  i32 r7 = r7 >> 0x10
    ....DeeE-----R  fallthrough
```

Gas simulation at offset 17509 with total cost of 77:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER....................................................  r8 = u8 [r6 + 0x236]
    D=========================eER...................................................  r8 = r8 << 0x2
    D==========================eER..................................................  r8 = r8 + r5
    D===========================eER.................................................  r8 = r8 + 0x7ff
    .D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER........................  u8 [r8 + 0x1e1] = a0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------------------R........................  r7 = u8 [r6 + 0x226]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------------------R........................  r8 = u8 [r6 + 0x228]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------------------R........................  r9 = i16 [r6 + 0x211]
    ..D========================eE--------------------------R........................  r7 = r7 & r8
    ..D========================eE--------------------------R........................  r9 = r9 + 0x1
    ..D=========================eE-------------------------R........................  r7 = r7 << 0x38
    ..D==========================eE------------------------R........................  r7 = r7 >> 0x3f
    ...D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER.......................  u8 [r6 + 0x271] = a0
    ...D========================eeeeeeeeeeeeeeeeeeeeeeeeeE--R.......................  u16 [r6 + 0x211] = r9
    ...D=======================eeeeeeeeeeeeeeeeeeeeeeeeeE---R.......................  r0 = u64 [r1 + 0x10]
    ...D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.  r5 = u64 [r1 + 0x8]
    ....D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0]
    ....D=================================================eE-----------------------R  r1 = r1 + 0x18
    ....D===============================================eeeeeeeeeeeeeeeeeeeeeeE----R  jump [r0 + 0]
```

Gas simulation at offset 17572 with total cost of 47:

```
    DeER..............................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.....................  r8 = u8 [r7 + 0x226]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.....................  r10 = u8 [r7 + 0x233]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.....................  r9 = i8 [r7 + 0x235]
    .D=========================eER....................  r11 = r8 & 0x20
    .D==========================eeeeeeeeeeeeeeeeeeeeER  jump 17622 if r11 != 0
```

Gas simulation at offset 17594 with total cost of 30:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.....  r11 = i16 [r7 + 0x20f]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.....  r12 = u8 [r7 + 0x234]
    DeE------------------------R.....  r9 = r9 >>a 0x3f
    .D========================eeER...  i32 r11 = r11 - r12
    .D==========================eER..  r9 = r9 ^ r11
    .D===========================eER.  r9 = r9 & 0x7
    ..DeE--------------------------R.  r10 = r10 << 0x4
    ..D===========================eER  r9 = r9 | r10
    ..DeeeeeeeeeeeeeeeE-------------R  jump 17677
```

Gas simulation at offset 17622 with total cost of 38:

```
    DeeeER...................................  r9 = r9 <s 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.............  r11 = i16 [r7 + 0x20f]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER............  r12 = u8 [r7 + 0x234]
    .DeE------------------------R............  r2 = r10 & 0xe
    .DeE------------------------R............  r10 = 0xfffffffffffffff8
    ..DeE-----------------------R............  r3 = 0x7
    ..D========================eeER..........  i32 r11 = r11 - r12
    ..D==========================eER.........  r11 = r11 & 0xf
    ...D==========================eeeER......  r12 = r11 <u 0x8
    ....D============================eeER....  r10 = 0 if r12 != 0
    ....D============================eE-R....  r12 = r12 ^ r9
    .....D=============================eER...  r10 = r10 + r11
    .....D============================eE-R...  r11 = r12 ^ 0x1
    .....D=============================eER...  r11 = r2 | r11
    ......D=============================eER..  r12 = r3 - r10
    ......D=============================eeER.  r12 = r10 if r9 == 0
    .......D============================eE-R.  r9 = r11 << 0x4
    .......D==============================eER  r9 = r9 + r12
    .......DeeE-----------------------------R  fallthrough
```

Gas simulation at offset 17677 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................  r10 = u8 [r7 + 0x228]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................  r11 = i16 [r7 + 0x211]
    D=========================eER..........................  r8 = r8 & r10
    DeE-------------------------R..........................  r9 = r9 + 0x8
    .D========================eER..........................  r11 = r11 + 0x1
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u16 [r7 + 0x211] = r11
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R.  u8 [r7 + 0x21b] = a2
    .D=========================eE------------------------R.  r8 = r8 >> 0x7
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x271] = a1
    ..DeeeeeeeeeeeeeeeeeeeeeeE----------------------------R  jump [r0 + 0]
```

Gas simulation at offset 17711 with total cost of 51:

```
    DeER..................................................  r1 = r1 + 0xffffffffffffffe8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u64 [r1 + 0x10] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u64 [r1 + 0x8] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u64 [r1 + 0] = r6
    .D....................................................  r5 = r7
    .DeE------------------------R.........................  r6 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER........................  r8 = u8 [r6 + 0x226]
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u8 [r6 + 0x233]
    ..D=========================eE-----------------------R  r9 = r8 & 0x20
    ..D==========================eeeeeeeeeeeeeeeeeeeeE---R  jump 17756 if r9 != 0
```

Gas simulation at offset 17742 with total cost of 16:

```
    DeER...............  r8 = r8 & 0x8
    D=eER..............  r8 = r8 << 0x9
    DeE-R..............  r7 = r7 << 0x4
    D==eER.............  r7 = r7 | r8
    .DeeeeeeeeeeeeeeeER  jump 17825
```

Gas simulation at offset 17756 with total cost of 38:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.............  r8 = i16 [r6 + 0x20f]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.............  r9 = u8 [r6 + 0x234]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.............  r10 = i8 [r6 + 0x235]
    .DeE-----------------------R.............  r11 = r7 & 0x1
    .D=eE----------------------R.............  r7 = r7 & 0xfe
    .DeE-----------------------R.............  r12 = 0xfffffffffffffff8
    ..DeE----------------------R.............  r2 = 0x7
    ..D=eE---------------------R.............  r11 = r11 << 0xc
    ...D======================eeeER..........  r10 = r10 <s 0
    ....D=====================eeE-R..........  i32 r8 = r8 - r9
    ....D=======================eER..........  r8 = r8 & 0xf
    .....D=======================eeeER.......  r9 = r8 <u 0x8
    ......D=========================eeER.....  r12 = 0 if r9 != 0
    ......D=========================eE-R.....  r9 = r9 ^ r10
    .......D==========================eER....  r8 = r8 + r12
    .......D=========================eE-R....  r9 = r9 ^ 0x1
    .......D==========================eER....  r7 = r7 | r9
    ........D==========================eER...  r9 = r2 - r8
    ........D==========================eeER..  r9 = r8 if r10 == 0
    .........D=========================eE-R..  r7 = r7 << 0x4
    .........D===========================eER.  r9 = r9 + r11
    .........D============================eER  r7 = r7 + r9
    .........DeeE---------------------------R  fallthrough
```

Gas simulation at offset 17825 with total cost of 27:

```
    DeER..........................  r7 = r7 + 0x8
    D=eER.........................  r7 = r7 >> 0x8
    D==eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x21c] = a0
    DeeeeeeeeeeeeeeeeeeeeeeeeeE--R  r8 = u16 [r6 + 0x21b]
    .D========================eE-R  r7 = r8 >> 0x8
    .D=========================eER  jump 17890 if r7 >=u 63
```

Gas simulation at offset 17846 with total cost of 74:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r9 = u64 [r6 + 0x241]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r7 = u64 [r6 + 0x249]
    DeE---------------------------------------R..................................  r10 = 0x17c80
    .D========================eeE-------------R..................................  r10 = r7 if r9 != 0
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r10 = u64 [r10 + 0x48]
    ..DeE-------------------------------------------------R......................  r7 = r6 + 0x27f
    ..D=======================eeE-------------------------R......................  r7 = r9 if r9 != 0
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 424, jump [r10 + 0]
```

Gas simulation at offset 17878 with total cost of 46:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.....................  r8 = u8 [r6 + 0x235]
    D=========================eER....................  r8 = r8 & 0x40
    D==========================eeeeeeeeeeeeeeeeeeeeER  jump 17915 if r8 != 0
```

Gas simulation at offset 17888 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 17959
```

Gas simulation at offset 17890 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.......  unlikely
    DeE---------------------------------------R.......  r8 = r8 & 0x1f
    D=eE--------------------------------------R.......  r8 = r8 + r5
    .D=eE-------------------------------------R.......  r7 = r8 + 0x7ff
    .D==eeeeeeeeeeeeeeeeeeeeeeeeeE------------R.......  r7 = u8 [r7 + 0x1a1]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......  r8 = u8 [r6 + 0x235]
    ..D========================eE-------------R.......  r8 = r8 & 0x40
    ..D=========================eeeeeeeeeeeeeeeeeeeeER  jump 17959 if r8 == 0
```

Gas simulation at offset 17915 with total cost of 11:

```
    DeER..........  r8 = r7 & 0xff
    DeER..........  r9 = r7 << 0xb
    .DeER.........  r10 = r8 << 0x1
    .D=eER........  r9 = r9 | r10
    .DeE-R........  r7 = r7 << 0xf
    ..DeER........  r8 = r8 << 0x5
    ..D=eER.......  r7 = r7 | r8
    ..D=eER.......  r9 = r9 & 0x22110
    ..D==eER......  r7 = r7 & 0x88440
    ...D==eER.....  r7 = r7 | r9
    ...D===eeeER..  r7 = r7 * 0x10101
    ...D======eeER  i32 r7 = r7 >> 0x10
    ....DeeE-----R  fallthrough
```

Gas simulation at offset 17959 with total cost of 99:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................................................................  r8 = u8 [r6 + 0x236]
    D=========================eER.........................................................................  r8 = r8 << 0x2
    D==========================eER........................................................................  r8 = r8 + r5
    D===========================eER.......................................................................  r8 = r8 + 0x7ff
    .D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER..............................................  u8 [r8 + 0x1e2] = a0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------------------R..............................................  r7 = u8 [r6 + 0x226]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------------------R..............................................  r8 = u8 [r6 + 0x228]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------------------R..............................................  r9 = u8 [r6 + 0x236]
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE--R..............................................  r10 = i16 [r6 + 0x211]
    ..D========================eE--------------------------R..............................................  r7 = r7 & r8
    ..D========================eE--------------------------R..............................................  r9 = r9 + 0x1
    ..D=================================================eE-R..............................................  r10 = r10 + 0x1
    ...D========================eE-------------------------R..............................................  r7 = r7 << 0x38
    ...D=========================eE------------------------R..............................................  r7 = r7 >> 0x3f
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  u16 [r6 + 0x211] = r10
    ...D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R......................  u8 [r6 + 0x236] = a2
    ....D=========================eeeeeeeeeeeeeeeeeeeeeeeeeE-----------------------R......................  u8 [r6 + 0x271] = a0
    ....D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r0 = u64 [r1 + 0x10]
    ....D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.....................  r5 = u64 [r1 + 0x8]
    ....D==================================================eeeeeeeeeeeeeeeeeeeeeeeeeER....................  r6 = u64 [r1 + 0]
    .....D========================================================================eE-R....................  r1 = r1 + 0x18
    .....D========================================================================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 18033 with total cost of 54:

```
    DeER.....................................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER............................  r8 = u8 [r7 + 0x226]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER............................  r9 = u8 [r7 + 0x228]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER............................  r10 = u16 [r7 + 0x209]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER............................  r11 = i16 [r7 + 0x211]
    .D=========================eER...........................  r8 = r8 & r9
    .D=========================eER...........................  r10 = r10 << 0x34
    .D==========================eER..........................  r10 = r10 >> 0x34
    ..D==========================eER.........................  r9 = r10 | 0x2000
    ..D========================eE--R.........................  r11 = r11 + 0x1
    ..D=========================eE-R.........................  r8 = r8 << 0x38
    ...D=========================eER.........................  r8 = r8 >> 0x3f
    ...D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..  u16 [r7 + 0x211] = r11
    ...D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r7 + 0x21b] = r9
    ...D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x271] = a1
    ....DeeeeeeeeeeeeeeeeeeeeeeE----------------------------R  jump [r0 + 0]
```

Gas simulation at offset 18089 with total cost of 51:

```
    DeER..................................................  r1 = r1 + 0xffffffffffffffe8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u64 [r1 + 0x10] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u64 [r1 + 0x8] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u64 [r1 + 0] = r6
    .D....................................................  r5 = r7
    .DeE------------------------R.........................  r6 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER........................  r8 = u8 [r6 + 0x226]
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u8 [r6 + 0x233]
    ..D=========================eE-----------------------R  r9 = r8 & 0x20
    ..D==========================eeeeeeeeeeeeeeeeeeeeE---R  jump 18134 if r9 != 0
```

Gas simulation at offset 18120 with total cost of 16:

```
    DeER...............  r8 = r8 & 0x8
    D=eER..............  r8 = r8 << 0x9
    DeE-R..............  r7 = r7 << 0x4
    D==eER.............  r7 = r7 | r8
    .DeeeeeeeeeeeeeeeER  jump 18203
```

Gas simulation at offset 18134 with total cost of 38:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.............  r8 = i16 [r6 + 0x20f]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.............  r9 = u8 [r6 + 0x234]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.............  r10 = i8 [r6 + 0x235]
    .DeE-----------------------R.............  r11 = r7 & 0x1
    .D=eE----------------------R.............  r7 = r7 & 0xfe
    .DeE-----------------------R.............  r12 = 0xfffffffffffffff8
    ..DeE----------------------R.............  r2 = 0x7
    ..D=eE---------------------R.............  r11 = r11 << 0xc
    ...D======================eeeER..........  r10 = r10 <s 0
    ....D=====================eeE-R..........  i32 r8 = r8 - r9
    ....D=======================eER..........  r8 = r8 & 0xf
    .....D=======================eeeER.......  r9 = r8 <u 0x8
    ......D=========================eeER.....  r12 = 0 if r9 != 0
    ......D=========================eE-R.....  r9 = r9 ^ r10
    .......D==========================eER....  r8 = r8 + r12
    .......D=========================eE-R....  r9 = r9 ^ 0x1
    .......D==========================eER....  r7 = r7 | r9
    ........D==========================eER...  r9 = r2 - r8
    ........D==========================eeER..  r9 = r8 if r10 == 0
    .........D=========================eE-R..  r7 = r7 << 0x4
    .........D===========================eER.  r9 = r9 + r11
    .........D============================eER  r7 = r7 + r9
    .........DeeE---------------------------R  fallthrough
```

Gas simulation at offset 18203 with total cost of 27:

```
    DeER..........................  r7 = r7 + 0x8
    D=eER.........................  r7 = r7 >> 0x8
    D==eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x21c] = a0
    DeeeeeeeeeeeeeeeeeeeeeeeeeE--R  r8 = u16 [r6 + 0x21b]
    .D========================eE-R  r7 = r8 >> 0x8
    .D=========================eER  jump 18268 if r7 >=u 63
```

Gas simulation at offset 18224 with total cost of 74:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r9 = u64 [r6 + 0x241]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r7 = u64 [r6 + 0x249]
    DeE---------------------------------------R..................................  r10 = 0x17c80
    .D========================eeE-------------R..................................  r10 = r7 if r9 != 0
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r10 = u64 [r10 + 0x48]
    ..DeE-------------------------------------------------R......................  r7 = r6 + 0x27f
    ..D=======================eeE-------------------------R......................  r7 = r9 if r9 != 0
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 430, jump [r10 + 0]
```

Gas simulation at offset 18256 with total cost of 46:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.....................  r8 = u8 [r6 + 0x235]
    D=========================eER....................  r8 = r8 & 0x40
    D==========================eeeeeeeeeeeeeeeeeeeeER  jump 18293 if r8 != 0
```

Gas simulation at offset 18266 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 18340
```

Gas simulation at offset 18268 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeE---------------------------------------R  r8 = r8 & 0x1f
    D=eE--------------------------------------R  r8 = r8 + r5
    .D=eE-------------------------------------R  r7 = r8 + 0x7ff
    .D==eeeeeeeeeeeeeeeeeeeeeeeeeE------------R  r7 = u8 [r7 + 0x1a1]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R  r8 = u8 [r6 + 0x235]
    ..D========================eE-------------R  r8 = r8 & 0x40
    ..D=========================eE------------R  jump 18340 if r8 == 0
```

Gas simulation at offset 18293 with total cost of 11:

```
    DeER..........  r8 = r7 & 0xff
    DeER..........  r9 = r7 << 0xb
    .DeER.........  r10 = r8 << 0x1
    .D=eER........  r9 = r9 | r10
    .DeE-R........  r10 = 0x22110
    ..DeER........  r7 = r7 << 0xf
    ..DeER........  r8 = r8 << 0x5
    ..D=eER.......  r7 = r7 | r8
    ..D=eER.......  r9 = r9 & r10
    ...D=eER......  r7 = r7 & 0x88440
    ...D==eER.....  r7 = r7 | r9
    ...D===eeeER..  r7 = r7 * 0x10101
    ....D=====eeER  i32 r7 = r7 >> 0x10
    ....DeeE-----R  fallthrough
```

Gas simulation at offset 18340 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r8 = u8 [r6 + 0x236]
    D=========================eE--------------R.............  r8 = r8 << 0x2
    D==========================eE-------------R.............  r8 = r8 + r5
    .D==========================eE------------R.............  r8 = r8 + 0x7ff
    .D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r8 + 0x1e2] = a0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------------------R  r7 = u8 [r6 + 0x236]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------------------R  r8 = u8 [r6 + 0x227]
    ..D========================eE--------------------------R  r7 = r7 + 0x1
    ..D========================eE--------------------------R  r8 = r8 & 0x18
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R  u8 [r6 + 0x236] = a0
    ..D=========================eE-------------------------R  jump 18409 if r8 == 0
```

Gas simulation at offset 18380 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  r7 = u16 [r6 + 0x209]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  r8 = u16 [r6 + 0x20b]
    DeE---------------------------------------R............  r10 = 0x841f
    .D========================eE--------------R............  r7 = r7 & r10
    .D========================eE--------------R............  r8 = r8 & 0x7be0
    .D=========================eE-------------R............  r7 = r7 | r8
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r6 + 0x209] = r7
    ..DeeE------------------------------------------------R  fallthrough
```

Gas simulation at offset 18409 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r7 = u8 [r6 + 0x226]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r8 = u8 [r6 + 0x228]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r9 = i16 [r6 + 0x211]
    .D========================eE--------------R.............  r7 = r7 & r8
    .D========================eE--------------R.............  r9 = r9 + 0x1
    .D=========================eE-------------R.............  r7 = r7 << 0x38
    .D==========================eE------------R.............  r7 = r7 >> 0x3f
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x271] = a0
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE--R  u16 [r6 + 0x211] = r9
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R  r0 = u64 [r1 + 0x10]
    ..D=======================eeeeeeeeeeeeeeeeeeeeeeeeeE---R  r5 = u64 [r1 + 0x8]
    ...D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R  r6 = u64 [r1 + 0]
    ...D===============================================eE--R  r1 = r1 + 0x18
    ...D========================eeeeeeeeeeeeeeeeeeeeeeE----R  jump [r0 + 0]
```

Gas simulation at offset 18455 with total cost of 54:

```
    DeER.....................................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER............................  r8 = u16 [r7 + 0x209]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER............................  r10 = u8 [r7 + 0x227]
    .D=========================eER...........................  r11 = r8 << 0x34
    .D==========================eER..........................  r11 = r11 >> 0x34
    ..D==========================eER.........................  r9 = r11 | 0x2000
    ..D========================eE--R.........................  r10 = r10 & 0x18
    ..D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r7 + 0x21b] = r9
    ...D========================eE--------------------------R  jump 18512 if r10 == 0
```

Gas simulation at offset 18487 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  r9 = u16 [r7 + 0x20b]
    DeE---------------------------------------R............  r11 = 0x841f
    D=eE--------------------------------------R............  r8 = r8 & r11
    .D========================eE--------------R............  r9 = r9 & 0x7be0
    .D=========================eE-------------R............  r8 = r8 | r9
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r7 + 0x209] = r8
    .DeeE-------------------------------------------------R  fallthrough
```

Gas simulation at offset 18512 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r8 = u8 [r7 + 0x226]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r9 = u8 [r7 + 0x228]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r10 = i16 [r7 + 0x211]
    .D========================eE--------------R.............  r8 = r8 & r9
    .D========================eE--------------R.............  r10 = r10 + 0x1
    .D=========================eE-------------R.............  r8 = r8 << 0x38
    .D==========================eE------------R.............  r8 = r8 >> 0x3f
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x271] = a1
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE--R  u16 [r7 + 0x211] = r10
    ..DeeeeeeeeeeeeeeeeeeeeeeE-----------------------------R  jump [r0 + 0]
```

Gas simulation at offset 18547 with total cost of 29:

```
    DeER............................  r1 = r1 + 0xfffffffffffffff0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0x8] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0] = r5
    .DeE------------------------R...  r5 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u16 [r5 + 0x21b]
    ..D=========================eER.  r9 = r8 >> 0x8
    ..DeE-------------------------R.  r10 = 0x3f
    ..D==========================eER  jump 18620 if r9 >=u r10
```

Gas simulation at offset 18572 with total cost of 74:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r9 = u64 [r5 + 0x241]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r7 = u64 [r5 + 0x249]
    DeE---------------------------------------R..................................  r10 = 0x17c80
    .D========================eeE-------------R..................................  r10 = r7 if r9 != 0
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r10 = u64 [r10 + 0x48]
    ..DeE-------------------------------------------------R......................  r7 = r5 + 0x27f
    ..D=======================eeE-------------------------R......................  r7 = r9 if r9 != 0
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 436, jump [r10 + 0]
```

Gas simulation at offset 18604 with total cost of 27:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u8 [r5 + 0x227]
    D=========================eER.  r8 = r8 & 0x18
    DeeeeeeeeeeeeeeeeeeeeeeeeeE-R.  u8 [r5 + 0x22a] = a0
    D==========================eER  jump 18649 if r8 != 0
```

Gas simulation at offset 18618 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 18678
```

Gas simulation at offset 18620 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeE---------------------------------------R.............  r8 = r8 & 0x1f
    D=eE--------------------------------------R.............  r7 = r7 + r8
    D==eE-------------------------------------R.............  r7 = r7 + 0x7ff
    .D==eeeeeeeeeeeeeeeeeeeeeeeeeE------------R.............  r7 = u8 [r7 + 0x1a1]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.............  r8 = u8 [r5 + 0x227]
    .D=========================eE-------------R.............  r8 = r8 & 0x18
    .D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x22a] = a0
    ..D=========================eE-------------------------R  jump 18678 if r8 == 0
```

Gas simulation at offset 18649 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  r7 = u16 [r5 + 0x209]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  r8 = u16 [r5 + 0x20b]
    DeE---------------------------------------R............  r10 = 0x841f
    .D========================eE--------------R............  r7 = r7 & r10
    .D========================eE--------------R............  r8 = r8 & 0x7be0
    .D=========================eE-------------R............  r7 = r7 | r8
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x209] = r7
    ..DeeE------------------------------------------------R  fallthrough
```

Gas simulation at offset 18678 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r7 = u8 [r5 + 0x226]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r8 = u8 [r5 + 0x228]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r9 = i16 [r5 + 0x211]
    .D========================eE--------------R.............  r7 = r7 & r8
    .D========================eE--------------R.............  r9 = r9 + 0x1
    .D=========================eE-------------R.............  r7 = r7 << 0x38
    .D==========================eE------------R.............  r7 = r7 >> 0x3f
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x271] = a0
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE--R  u16 [r5 + 0x211] = r9
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R  r0 = u64 [r1 + 0x8]
    ..D=======================eeeeeeeeeeeeeeeeeeeeeeeeeE---R  r5 = u64 [r1 + 0]
    ...D========================eE-------------------------R  r1 = r1 + 0x10
    ...D========================eeeeeeeeeeeeeeeeeeeeeeE----R  jump [r0 + 0]
```

Gas simulation at offset 18721 with total cost of 29:

```
    DeER............................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  r2 = u16 [r7 + 0x211]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  r9 = u16 [r7 + 0x209]
    .D=========================eER..  r10 = r2 + 0xfffffffffffffeff
    .D=========================eER..  r12 = r9 >> 0x4
    ..D=========================eER.  r8 = zext16 r10
    ..DeE-------------------------R.  r3 = 0x40
    ..D=========================eER.  r10 = r12 & 0x38
    ...D=========================eER  jump 18782 if r8 >=u r3
```

Gas simulation at offset 18751 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeE---------------------------------------R  r8 = r9 & 0xcff
    DeE---------------------------------------R  r11 = 0x2000
    .DeE--------------------------------------R  r8 = r8 | r11
    .D=eE-------------------------------------R  r10 = r10 + r8
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R  r8 = u8 [r7 + 0x227]
    .D=========================eE-------------R  r8 = r8 & 0x18
    ..D=eeeeeeeeeeeeeeeeeeeeeeeeeE------------R  u16 [r7 + 0x21b] = r10
    ..D=========================eE------------R  jump 18820 if r8 != 0
```

Gas simulation at offset 18780 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 18848
```

Gas simulation at offset 18782 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeE---------------------------------------R  r11 = r9 & 0xc00
    .DeE--------------------------------------R  r8 = r9 << 0x3b
    .D=eE-------------------------------------R  r8 = r8 >> 0x3d
    .D==eE------------------------------------R  r8 = r8 | r11
    ..DeE-------------------------------------R  r11 = 0x23c0
    ..D=eE------------------------------------R  r10 = r10 | r11
    ..D==eE-----------------------------------R  r10 = r10 | r8
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------R  r8 = u8 [r7 + 0x227]
    ...D========================eE------------R  r8 = r8 & 0x18
    ...D==eeeeeeeeeeeeeeeeeeeeeeeeeE----------R  u16 [r7 + 0x21b] = r10
    ...D=========================eE-----------R  jump 18848 if r8 == 0
```

Gas simulation at offset 18820 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  r8 = u16 [r7 + 0x20b]
    DeE---------------------------------------R............  r11 = 0x841f
    D=eE--------------------------------------R............  r9 = r9 & r11
    .DeE--------------------------------------R............  r10 = 0x7be0
    .D========================eE--------------R............  r8 = r8 & r10
    .D=========================eE-------------R............  r8 = r8 | r9
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r7 + 0x209] = r8
    ..DeeE------------------------------------------------R  fallthrough
```

Gas simulation at offset 18848 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r8 = u8 [r7 + 0x226]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r9 = u8 [r7 + 0x228]
    DeE---------------------------------------R.............  r2 = r2 + 0x1
    .D========================eE--------------R.............  r8 = r8 & r9
    .D=========================eE-------------R.............  r8 = r8 << 0x38
    .D==========================eE------------R.............  r8 = r8 >> 0x3f
    .D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x271] = a1
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R  u16 [r7 + 0x211] = r2
    ..DeeeeeeeeeeeeeeeeeeeeeeE-----------------------------R  jump [r0 + 0]
```

Gas simulation at offset 18879 with total cost of 29:

```
    DeER............................  r1 = r1 + 0xfffffffffffffff0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0x8] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0] = r5
    .DeE------------------------R...  r5 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u16 [r5 + 0x21b]
    ..D=========================eER.  r9 = r8 >> 0x8
    ..D==========================eER  jump 18936 if r9 >=u 63
```

Gas simulation at offset 18902 with total cost of 74:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r9 = u64 [r5 + 0x241]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r7 = u64 [r5 + 0x249]
    DeE---------------------------------------R..................................  r10 = 0x17c80
    .D========================eeE-------------R..................................  r10 = r7 if r9 != 0
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r10 = u64 [r10 + 0x48]
    ..DeE-------------------------------------------------R......................  r7 = r5 + 0x27f
    ..D=======================eeE-------------------------R......................  r7 = r9 if r9 != 0
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 442, jump [r10 + 0]
```

Gas simulation at offset 18934 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 18951
```

Gas simulation at offset 18936 with total cost of 28:

```
    DeER...........................  r8 = r8 & 0x1f
    D=eER..........................  r7 = r7 + r8
    D==eER.........................  r7 = r7 + 0x7ff
    D===eeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u8 [r7 + 0x1a1]
    .DeeE-------------------------R  fallthrough
```

Gas simulation at offset 18951 with total cost of 55:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..............................  r8 = u16 [r5 + 0x209]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..............................  r9 = u8 [r5 + 0x227]
    D=========================eER.............................  r10 = r8 & 0x2
    .D========================eER.............................  r11 = r8 >> 0x4
    .D=========================eER............................  r11 = r11 & 0x4
    .D==========================eER...........................  r10 = r10 | r11
    ..DeE-------------------------R...........................  r7 = r7 & 0xff
    ..D==========================eER..........................  r7 = r7 >> r10
    ..D===========================eER.........................  r7 = r7 & 0x3
    ...D======================eE----R.........................  r9 = r9 & 0x18
    ...D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x22b] = a0
    ...D=======================eE----------------------------R  jump 19016 if r9 == 0
```

Gas simulation at offset 18991 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  r7 = u16 [r5 + 0x20b]
    DeE---------------------------------------R............  r10 = 0x841f
    D=eE--------------------------------------R............  r8 = r8 & r10
    .D========================eE--------------R............  r7 = r7 & 0x7be0
    .D=========================eE-------------R............  r7 = r7 | r8
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x209] = r7
    .DeeE-------------------------------------------------R  fallthrough
```

Gas simulation at offset 19016 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r7 = u8 [r5 + 0x226]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r8 = u8 [r5 + 0x228]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r9 = i16 [r5 + 0x211]
    .D========================eE--------------R.............  r7 = r7 & r8
    .D========================eE--------------R.............  r9 = r9 + 0x1
    .D=========================eE-------------R.............  r7 = r7 << 0x38
    .D==========================eE------------R.............  r7 = r7 >> 0x3f
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x271] = a0
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE--R  u16 [r5 + 0x211] = r9
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R  r0 = u64 [r1 + 0x8]
    ..D=======================eeeeeeeeeeeeeeeeeeeeeeeeeE---R  r5 = u64 [r1 + 0]
    ...D========================eE-------------------------R  r1 = r1 + 0x10
    ...D========================eeeeeeeeeeeeeeeeeeeeeeE----R  jump [r0 + 0]
```

Gas simulation at offset 19059 with total cost of 28:

```
    DeER...........................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u8 [r7 + 0x226]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  r10 = u8 [r7 + 0x233]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  r9 = i8 [r7 + 0x235]
    .D=========================eER.  r11 = r8 & 0x20
    .D==========================eER  jump 19124 if r11 != 0
```

Gas simulation at offset 19081 with total cost of 55:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...............  r11 = i16 [r7 + 0x20f]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...............  r12 = u8 [r7 + 0x234]
    DeE---------------------------------------R...............  r9 = r9 >>a 0x3f
    .D========================eeE-------------R...............  i32 r11 = r11 - r12
    .D==========================eE------------R...............  r9 = r9 ^ r11
    .D===========================eE-----------R...............  r9 = r9 & 0x7
    ..DeE-------------------------------------R...............  r10 = r10 << 0x4
    ..D===========================eE----------R...............  r9 = r9 | r10
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------R...............  r10 = u8 [r7 + 0x227]
    ..D=========================eE------------R...............  r10 = r10 & 0x18
    ...D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x21b] = a2
    ...D=========================eE--------------------------R  jump 19193 if r10 != 0
```

Gas simulation at offset 19122 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 19225
```

Gas simulation at offset 19124 with total cost of 63:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.......................  unlikely
    DeeeE-------------------------------------R.......................  r9 = r9 <s 0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......................  r11 = i16 [r7 + 0x20f]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......................  r12 = u8 [r7 + 0x234]
    .DeE--------------------------------------R.......................  r2 = r10 & 0xe
    ..DeE-------------------------------------R.......................  r10 = 0xfffffffffffffff8
    ..DeE-------------------------------------R.......................  r3 = 0x7
    ..D========================eeE------------R.......................  i32 r11 = r11 - r12
    ...D=========================eE-----------R.......................  r11 = r11 & 0xf
    ...D==========================eeeE--------R.......................  r12 = r11 <u 0x8
    ....D============================eeE------R.......................  r10 = 0 if r12 != 0
    ....D============================eE-------R.......................  r12 = r12 ^ r9
    .....D=============================eE-----R.......................  r10 = r10 + r11
    .....D============================eE------R.......................  r11 = r12 ^ 0x1
    .....D=============================eE-----R.......................  r11 = r2 | r11
    ......D=============================eE----R.......................  r12 = r3 - r10
    ......D=============================eeE---R.......................  r12 = r10 if r9 == 0
    .......D============================eE----R.......................  r9 = r11 << 0x4
    .......D==============================eE--R.......................  r9 = r9 + r12
    .......DeeeeeeeeeeeeeeeeeeeeeeeeeE--------R.......................  r10 = u8 [r7 + 0x227]
    ........D========================eE-------R.......................  r10 = r10 & 0x18
    ........D==============================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x21b] = a2
    ........D=========================eE-----------------------------R  jump 19225 if r10 == 0
```

Gas simulation at offset 19193 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  r9 = u16 [r7 + 0x209]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  r10 = u16 [r7 + 0x20b]
    DeE---------------------------------------R............  r12 = 0x841f
    .DeE--------------------------------------R............  r11 = 0x7be0
    .D========================eE--------------R............  r9 = r9 & r12
    .D========================eE--------------R............  r10 = r10 & r11
    .D=========================eE-------------R............  r9 = r9 | r10
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r7 + 0x209] = r9
    ..DeeE------------------------------------------------R  fallthrough
```

Gas simulation at offset 19225 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  r9 = u8 [r7 + 0x228]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  r10 = i16 [r7 + 0x211]
    D=========================eE--------------R............  r8 = r8 & r9
    .D========================eE--------------R............  r10 = r10 + 0x1
    .D=========================eE-------------R............  r8 = r8 >> 0x7
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x271] = a1
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R  u16 [r7 + 0x211] = r10
    ..DeeeeeeeeeeeeeeeeeeeeeeE----------------------------R  jump [r0 + 0]
```

Gas simulation at offset 19253 with total cost of 52:

```
    DeER...................................................  r1 = r1 + 0xffffffffffffffe8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u64 [r1 + 0x10] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u64 [r1 + 0x8] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u64 [r1 + 0] = r6
    .D.....................................................  r5 = r7
    .DeE------------------------R..........................  r6 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r8 = u8 [r6 + 0x226]
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  r9 = u8 [r6 + 0x233]
    ..D=========================eE-----------------------R.  r10 = r8 & 0x20
    ...D================================================eER  r7 = r9 << 0x4
    ...D=========================eE-----------------------R  jump 19342 if r10 != 0
```

Gas simulation at offset 19287 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeE---------------------------------------R  r8 = r8 & 0x8
    D=eE--------------------------------------R  r8 = r8 << 0x9
    D==eE-------------------------------------R  r7 = r7 | r8
    .D==eE------------------------------------R  r7 = r7 >> 0x8
    .D===eeeeeeeeeeeeeeeeeeeeeeeeeE-----------R  u8 [r6 + 0x21c] = a0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R  r8 = u16 [r6 + 0x21b]
    ..D========================eE-------------R  r7 = r8 >> 0x8
    ..D=========================eE------------R  jump 19370 if r7 <u 63
```

Gas simulation at offset 19315 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.......  unlikely
    DeE---------------------------------------R.......  r8 = r8 & 0x1f
    D=eE--------------------------------------R.......  r8 = r8 + r5
    .D=eE-------------------------------------R.......  r7 = r8 + 0x7ff
    .D==eeeeeeeeeeeeeeeeeeeeeeeeeE------------R.......  r7 = u8 [r7 + 0x1a1]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......  r8 = u8 [r6 + 0x235]
    ..D========================eE-------------R.......  r8 = r8 & 0x40
    ..D=========================eeeeeeeeeeeeeeeeeeeeER  jump 19412 if r8 != 0
```

Gas simulation at offset 19340 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 19459
```

Gas simulation at offset 19342 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeE---------------------------------------R  r9 = r9 << 0xc
    D=eE--------------------------------------R  r7 = r7 | r9
    D==eE-------------------------------------R  r7 = r7 << 0x33
    .D==eE------------------------------------R  r7 = r7 >> 0x3b
    .D===eeeeeeeeeeeeeeeeeeeeeeeeeE-----------R  u8 [r6 + 0x21c] = a0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R  r8 = u16 [r6 + 0x21b]
    ..D========================eE-------------R  r7 = r8 >> 0x8
    ..D=========================eE------------R  jump 19315 if r7 >=u 63
```

Gas simulation at offset 19370 with total cost of 74:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r9 = u64 [r6 + 0x241]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r7 = u64 [r6 + 0x249]
    DeE---------------------------------------R..................................  r10 = 0x17c80
    .D========================eeE-------------R..................................  r10 = r7 if r9 != 0
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r10 = u64 [r10 + 0x48]
    ..DeE-------------------------------------------------R......................  r7 = r6 + 0x27f
    ..D=======================eeE-------------------------R......................  r7 = r9 if r9 != 0
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 448, jump [r10 + 0]
```

Gas simulation at offset 19402 with total cost of 27:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u8 [r6 + 0x235]
    D=========================eER.  r8 = r8 & 0x40
    D==========================eER  jump 19459 if r8 == 0
```

Gas simulation at offset 19412 with total cost of 11:

```
    DeER..........  r8 = r7 & 0xff
    DeER..........  r9 = r7 << 0xb
    .DeER.........  r10 = r8 << 0x1
    .D=eER........  r9 = r9 | r10
    .DeE-R........  r10 = 0x22110
    ..DeER........  r7 = r7 << 0xf
    ..DeER........  r8 = r8 << 0x5
    ..D=eER.......  r7 = r7 | r8
    ..D=eER.......  r9 = r9 & r10
    ...D=eER......  r7 = r7 & 0x88440
    ...D==eER.....  r7 = r7 | r9
    ...D===eeeER..  r7 = r7 * 0x10101
    ....D=====eeER  i32 r7 = r7 >> 0x10
    ....DeeE-----R  fallthrough
```

Gas simulation at offset 19459 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r8 = u8 [r6 + 0x236]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r9 = u8 [r6 + 0x227]
    D=========================eE--------------R.............  r8 = r8 << 0x2
    .D=========================eE-------------R.............  r8 = r8 + r5
    .D==========================eE------------R.............  r8 = r8 + 0x7ff
    .D========================eE--------------R.............  r9 = r9 & 0x18
    .D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r8 + 0x1e1] = a0
    ..D========================eE--------------------------R  jump 19517 if r9 == 0
```

Gas simulation at offset 19488 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  r7 = u16 [r6 + 0x209]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  r8 = u16 [r6 + 0x20b]
    DeE---------------------------------------R............  r10 = 0x841f
    .D========================eE--------------R............  r7 = r7 & r10
    .D========================eE--------------R............  r8 = r8 & 0x7be0
    .D=========================eE-------------R............  r7 = r7 | r8
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r6 + 0x209] = r7
    ..DeeE------------------------------------------------R  fallthrough
```

Gas simulation at offset 19517 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r7 = u8 [r6 + 0x226]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r8 = u8 [r6 + 0x228]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r9 = i16 [r6 + 0x211]
    .D========================eE--------------R.............  r7 = r7 & r8
    .D========================eE--------------R.............  r9 = r9 + 0x1
    .D=========================eE-------------R.............  r7 = r7 << 0x38
    .D==========================eE------------R.............  r7 = r7 >> 0x3f
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x271] = a0
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE--R  u16 [r6 + 0x211] = r9
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R  r0 = u64 [r1 + 0x10]
    ..D=======================eeeeeeeeeeeeeeeeeeeeeeeeeE---R  r5 = u64 [r1 + 0x8]
    ...D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R  r6 = u64 [r1 + 0]
    ...D===============================================eE--R  r1 = r1 + 0x18
    ...D========================eeeeeeeeeeeeeeeeeeeeeeE----R  jump [r0 + 0]
```

Gas simulation at offset 19563 with total cost of 28:

```
    DeER...........................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u8 [r7 + 0x226]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  r10 = u8 [r7 + 0x233]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  r9 = i8 [r7 + 0x235]
    .D=========================eER.  r11 = r8 & 0x20
    .D==========================eER  jump 19631 if r11 != 0
```

Gas simulation at offset 19585 with total cost of 56:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R................  r11 = i16 [r7 + 0x20f]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R................  r12 = u8 [r7 + 0x234]
    DeE---------------------------------------R................  r9 = r9 >>a 0x3f
    .D========================eeE-------------R................  i32 r11 = r11 - r12
    .D==========================eE------------R................  r9 = r9 ^ r11
    .D===========================eE-----------R................  r9 = r9 & 0x7
    ..DeE-------------------------------------R................  r10 = r10 << 0x4
    ..D===========================eE----------R................  r9 = r9 | r10
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------R................  r10 = u8 [r7 + 0x227]
    ..D============================eE---------R................  r9 = r9 + 0x8
    ...D========================eE------------R................  r10 = r10 & 0x18
    ...D============================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x21b] = a2
    ...D=========================eE---------------------------R  jump 19703 if r10 != 0
```

Gas simulation at offset 19629 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 19735
```

Gas simulation at offset 19631 with total cost of 64:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER........................  unlikely
    DeeeE-------------------------------------R........................  r9 = r9 <s 0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R........................  r11 = i16 [r7 + 0x20f]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R........................  r12 = u8 [r7 + 0x234]
    .DeE--------------------------------------R........................  r2 = r10 & 0xe
    ..DeE-------------------------------------R........................  r10 = 0xfffffffffffffff8
    ..DeE-------------------------------------R........................  r3 = 0x7
    ..D========================eeE------------R........................  i32 r11 = r11 - r12
    ...D=========================eE-----------R........................  r11 = r11 & 0xf
    ...D==========================eeeE--------R........................  r12 = r11 <u 0x8
    ....D============================eeE------R........................  r10 = 0 if r12 != 0
    ....D============================eE-------R........................  r12 = r12 ^ r9
    .....D=============================eE-----R........................  r10 = r10 + r11
    .....D============================eE------R........................  r11 = r12 ^ 0x1
    .....D=============================eE-----R........................  r11 = r2 | r11
    ......D=============================eE----R........................  r12 = r3 - r10
    ......D=============================eeE---R........................  r12 = r10 if r9 == 0
    .......D============================eE----R........................  r9 = r11 << 0x4
    .......D==============================eE--R........................  r9 = r9 + r12
    .......DeeeeeeeeeeeeeeeeeeeeeeeeeE--------R........................  r10 = u8 [r7 + 0x227]
    ........D==============================eE-R........................  r9 = r9 + 0x8
    ........D========================eE-------R........................  r10 = r10 & 0x18
    ........D===============================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x21b] = a2
    ........D=========================eE------------------------------R  jump 19735 if r10 == 0
```

Gas simulation at offset 19703 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  r9 = u16 [r7 + 0x209]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  r10 = u16 [r7 + 0x20b]
    DeE---------------------------------------R............  r12 = 0x841f
    .DeE--------------------------------------R............  r11 = 0x7be0
    .D========================eE--------------R............  r9 = r9 & r12
    .D========================eE--------------R............  r10 = r10 & r11
    .D=========================eE-------------R............  r9 = r9 | r10
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r7 + 0x209] = r9
    ..DeeE------------------------------------------------R  fallthrough
```

Gas simulation at offset 19735 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  r9 = u8 [r7 + 0x228]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  r10 = i16 [r7 + 0x211]
    D=========================eE--------------R............  r8 = r8 & r9
    .D========================eE--------------R............  r10 = r10 + 0x1
    .D=========================eE-------------R............  r8 = r8 >> 0x7
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x271] = a1
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R  u16 [r7 + 0x211] = r10
    ..DeeeeeeeeeeeeeeeeeeeeeeE----------------------------R  jump [r0 + 0]
```

Gas simulation at offset 19763 with total cost of 29:

```
    DeER............................  r1 = r1 + 0xfffffffffffffff0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0x8] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0] = r5
    .DeE------------------------R...  r5 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u16 [r5 + 0x21b]
    ..D=========================eER.  r9 = r8 >> 0x8
    ..D==========================eER  jump 19834 if r9 >=u 63
```

Gas simulation at offset 19786 with total cost of 74:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r9 = u64 [r5 + 0x241]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r7 = u64 [r5 + 0x249]
    DeE---------------------------------------R..................................  r10 = 0x17c80
    .D========================eeE-------------R..................................  r10 = r7 if r9 != 0
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r10 = u64 [r10 + 0x48]
    ..DeE-------------------------------------------------R......................  r7 = r5 + 0x27f
    ..D=======================eeE-------------------------R......................  r7 = r9 if r9 != 0
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 454, jump [r10 + 0]
```

Gas simulation at offset 19818 with total cost of 27:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..  r2 = u8 [r5 + 0x227]
    D=========================eER.  r9 = r2 & 0x18
    DeeeeeeeeeeeeeeeeeeeeeeeeeE-R.  u8 [r5 + 0x22d] = a0
    .D=========================eER  jump 19863 if r9 != 0
```

Gas simulation at offset 19832 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 19899
```

Gas simulation at offset 19834 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeE---------------------------------------R.............  r8 = r8 & 0x1f
    D=eE--------------------------------------R.............  r7 = r7 + r8
    D==eE-------------------------------------R.............  r7 = r7 + 0x7ff
    .D==eeeeeeeeeeeeeeeeeeeeeeeeeE------------R.............  r7 = u8 [r7 + 0x1a1]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.............  r2 = u8 [r5 + 0x227]
    .D=========================eE-------------R.............  r9 = r2 & 0x18
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x22d] = a0
    ..D=========================eE-------------------------R  jump 19899 if r9 == 0
```

Gas simulation at offset 19863 with total cost of 46:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER......  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R......  r9 = u16 [r5 + 0x209]
    D=========================eE--------------R......  r10 = r9 & 0x1f
    .D========================eE--------------R......  r9 = r9 & 0xffffffffffffffe0
    .D=========================eeeeeeeeeeeeeeeeeeeeER  jump 19888 if r10 != 31
```

Gas simulation at offset 19878 with total cost of 26:

```
    DeER.........................  r9 = r9 ^ 0x400
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x209] = r9
    DeeeeeeeeeeeeeeeE-----------R  jump 19899
```

Gas simulation at offset 19888 with total cost of 27:

```
    DeER..........................  r9 = r9 | r10
    D=eER.........................  r9 = r9 + 0x1
    D==eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x209] = r9
    DeeE-------------------------R  fallthrough
```

Gas simulation at offset 19899 with total cost of 123:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...................................................................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...................................................................................  r3 = i16 [r5 + 0x211]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...................................................................................  r10 = u8 [r5 + 0x226]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...................................................................................  r11 = u8 [r5 + 0x228]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R...................................................................................  r12 = u8 [r5 + 0x22b]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................................................................  r8 = u8 [r5 + 0x22c]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................................................................  r9 = u8 [r5 + 0x238]
    .D========================eE------------------------R.........................................................................  r10 = r10 & r11
    ..D========================eE-----------------------R.........................................................................  r2 = r2 << 0x3c
    ..D=========================eE----------------------R.........................................................................  r11 = r2 >> 0x3f
    ..D================================================eER........................................................................  r9 = r9 & r11
    ...D=======================eE------------------------R........................................................................  r11 = r12 << 0x3f
    ...D========================eE-----------------------R........................................................................  r3 = r3 + 0x1
    ...D=========================eE----------------------R........................................................................  r11 = r11 >>a 0x3f
    ....D========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................................................................  u16 [r5 + 0x211] = r3
    ....D==============================================eeeeeeeeeeeeeeeeeeeeeeeeeER................................................  u8 [r5 + 0x213] = a1
    ....D=========================eeeeeeeeeeeeeeeeeeeeeeeeeE---------------------R................................................  u8 [r5 + 0x215] = a0
    ....D===============================================eeeeeeeeeeeeeeeeeeeeeeeeeER...............................................  u8 [r5 + 0x217] = a4
    .....D================================================eE----------------------R...............................................  r12 = r12 << 0x6
    .....D=================================================eE---------------------R...............................................  r7 = sext8 r12
    .....D=================================================eE---------------------R...............................................  r10 = r10 << 0x38
    .....D==================================================eE--------------------R...............................................  r7 = r7 >> 0x7
    ......D=================================================eE--------------------R...............................................  r10 = r10 >> 0x3f
    ......D==================================================eeeeeeeeeeeeeeeeeeeeeeeeeER..........................................  u8 [r5 + 0x219] = a0
    ......D==================================================eeeeeeeeeeeeeeeeeeeeeeeeeER..........................................  u8 [r5 + 0x23b] = a2
    ......D=====================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.......................  u8 [r5 + 0x271] = a3
    .......D=====================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r0 = u64 [r1 + 0x8]
    .......D==========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.................  r5 = u64 [r1 + 0]
    .......D==========================================================================eE------------------------R.................  r1 = r1 + 0x10
    .......D==============================================================================================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 19997 with total cost of 29:

```
    DeER............................  r1 = r1 + 0xfffffffffffffff0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0x8] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0] = r5
    .DeE------------------------R...  r5 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u16 [r5 + 0x21b]
    ..D=========================eER.  r9 = r8 >> 0x8
    ..DeE-------------------------R.  r10 = 0x3f
    ..D==========================eER  jump 20056 if r9 >=u r10
```

Gas simulation at offset 20022 with total cost of 74:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r9 = u64 [r5 + 0x241]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r7 = u64 [r5 + 0x249]
    DeE---------------------------------------R..................................  r10 = 0x17c80
    .D========================eeE-------------R..................................  r10 = r7 if r9 != 0
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r10 = u64 [r10 + 0x48]
    ..DeE-------------------------------------------------R......................  r7 = r5 + 0x27f
    ..D=======================eeE-------------------------R......................  r7 = r9 if r9 != 0
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeER  r0 = 458, jump [r10 + 0]
```

Gas simulation at offset 20054 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 20071
```

Gas simulation at offset 20056 with total cost of 28:

```
    DeER...........................  r8 = r8 & 0x1f
    D=eER..........................  r7 = r7 + r8
    D==eER.........................  r7 = r7 + 0x7ff
    D===eeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u8 [r7 + 0x1a1]
    .DeeE-------------------------R  fallthrough
```

Gas simulation at offset 20071 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER............................  r8 = u8 [r5 + 0x226]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER............................  r9 = u8 [r5 + 0x228]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER............................  u8 [r5 + 0x22a] = a0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER............................  r7 = u8 [r5 + 0x23b]
    .D========================eER...........................  r8 = r8 & r9
    .D=========================eER..........................  r8 = r8 << 0x38
    .D==========================eER.........................  r8 = r8 >> 0x3f
    .D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x271] = a1
    ..D=======================eE---------------------------R  jump 20111 if r7 == 0
```

Gas simulation at offset 20103 with total cost of 26:

```
    DeER.........................  r7 = 0x1
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x23c] = a0
    DeeE------------------------R  fallthrough
```

Gas simulation at offset 20111 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.......  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  u16 [r5 + 527] = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  u16 [r5 + 529] = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r0 = u64 [r1 + 0x8]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......  r5 = u64 [r1 + 0]
    .D========================eE--------------R.......  r1 = r1 + 0x10
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 20130 with total cost of 22:

```
    DeER.....................  r7 = 0
    DeeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 20134 with total cost of 22:

```
    DeeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 20136 with total cost of 22:

```
    DeeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 20138 with total cost of 52:

```
    DeER...................................................  r1 = r1 + 0xffffffffffffffd0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u64 [r1 + 0x28] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u64 [r1 + 0x20] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u64 [r1 + 0x18] = r6
    .D.....................................................  r5 = r7
    .DeE------------------------R..........................  r6 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r7 = u8 [r6 + 0x265]
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x10] = r7
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R  r8 = u16 [r6 + 0x269]
    ..D....................................................  r7 = r5
    ..DeeeeeeeeeeeeeeeE-----------------------------------R  r0 = 468, jump 22578
```

Gas simulation at offset 20175 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r8 = i16 [r6 + 0x269]
    DeE------------------------R..........................  r9 = r7 << 0x8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u64 [r1 + 0] = r9
    .D========================eER.........................  r8 = r8 + 0x1
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r6 + 0x269] = r8
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r7 = u64 [r1 + 0x10]
    .D=========================eE------------------------R  r7 = r7 | r9
    ..D=========================eE-----------------------R  r8 = zext16 r7
    ..D...................................................  r7 = r5
    ..DeeeeeeeeeeeeeeeE----------------------------------R  r0 = 470, jump 22578
```

Gas simulation at offset 20207 with total cost of 29:

```
    DeER............................  r7 = r7 & 0xff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0x8] = r7
    DeeeeeeeeeeeeeeeeeeeeeeeeeE-R...  r7 = u64 [r1 + 0x10]
    D=========================eER...  r7 = r7 + 0x1
    .D=========================eER..  r7 = r7 & 0xff
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-R..  r8 = u64 [r1 + 0]
    .D==========================eER.  r7 = r7 | r8
    .D===========================eER  r8 = zext16 r7
    ..D.............................  r7 = r5
    ..DeeeeeeeeeeeeeeeE------------R  r0 = 472, jump 22578
```

Gas simulation at offset 20239 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER............................  r8 = u16 [r6 + 0x261]
    DeE------------------------R............................  r7 = r7 << 0x8
    DeeeeeeeeeeeeeeeeeeeeeeeeeER............................  r9 = u64 [r1 + 0x8]
    D=========================eER...........................  r9 = r9 | r7
    .D=========================eER..........................  r7 = zext16 r9
    .D==========================eER.........................  r7 = r7 ^ r8
    ..D==========================eeeER......................  r7 = r7 <u 0x1
    ..D=======================eE-----R......................  r8 = r8 << 0x20
    ...D============================eER.....................  r7 = r7 << 0x10
    ...D=============================eER....................  r7 = r7 | r8
    ...D=======================eeeeeeeeeeeeeeeeeeeeeeeeeER..  u16 [r6 + 0x269] = r9
    ...DeeeeeeeeeeeeeeeeeeeeeeeeeE-----------------------R..  r0 = u64 [r1 + 0x28]
    ....DeeeeeeeeeeeeeeeeeeeeeeeeeE----------------------R..  r5 = u64 [r1 + 0x20]
    ....D========================eeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0x18]
    ....D=========================eE-----------------------R  r1 = r1 + 0x30
    ....D========================eeeeeeeeeeeeeeeeeeeeeeE---R  jump [r0 + 0]
```

Gas simulation at offset 20287 with total cost of 51:

```
    DeER..................................................  r1 = r1 + 0xffffffffffffffe8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u64 [r1 + 0x10] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u64 [r1 + 0x8] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u64 [r1 + 0] = r6
    .DeE------------------------R.........................  r5 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER........................  r6 = u8 [r5 + 0x265]
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = u16 [r5 + 0x269]
    ..DeeeeeeeeeeeeeeeE----------------------------------R  r0 = 476, jump 22578
```

Gas simulation at offset 20316 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER............................  r8 = u16 [r5 + 0x261]
    DeE------------------------R............................  r7 = r7 << 0x8
    D=eE-----------------------R............................  r6 = r6 | r7
    D==eE----------------------R............................  r7 = zext16 r6
    .D========================eER...........................  r7 = r7 ^ r8
    .D=========================eeeER........................  r7 = r7 <u 0x1
    ..D=========================eE-R........................  r8 = r8 << 0x20
    ..D===========================eER.......................  r7 = r7 << 0x10
    ..D============================eER......................  r7 = r7 | r8
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE----R......................  u16 [r5 + 0x269] = r6
    ...DeeeeeeeeeeeeeeeeeeeeeeeeeE---R......................  r0 = u64 [r1 + 0x10]
    ...DeeeeeeeeeeeeeeeeeeeeeeeeeE---R......................  r5 = u64 [r1 + 0x8]
    ...D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0]
    ...D=========================eE------------------------R  r1 = r1 + 0x18
    ....D========================eeeeeeeeeeeeeeeeeeeeeeE---R  jump [r0 + 0]
```

Gas simulation at offset 20360 with total cost of 52:

```
    DeER...................................................  r1 = r1 + 0xffffffffffffffe0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u64 [r1 + 0x18] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u64 [r1 + 0x10] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u64 [r1 + 0x8] = r6
    .DeE------------------------R..........................  r6 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r8 = u8 [r6 + 0x267]
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  r9 = u8 [r6 + 0x265]
    ..D=========================eE-----------------------R.  r10 = r8 & 0x7
    ..DeE------------------------------------------------R.  r2 = 0x7
    ...D================================================eER  r5 = r9 + 0x1
    ...D=========================eE-----------------------R  jump 20420 if r10 == r2
```

Gas simulation at offset 20396 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = u16 [r6 + 0x263]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0] = r7
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u64 [r1 + 0]
    DeeeeeeeeeeeeeeeE----------R  r0 = 480, jump 23116
```

Gas simulation at offset 20410 with total cost of 25:

```
    DeER........................  r2 = 0x7
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u64 [r1 + 0]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = u8 [r6 + 0x267]
    DeeE-----------------------R  fallthrough
```

Gas simulation at offset 20420 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r10 = u8 [r6 + 0x26f]
    DeE---------------------------------------R.............  r11 = r5 & 0x80
    .DeE--------------------------------------R.............  r9 = r5 & 0xff
    ..DeeeE-----------------------------------R.............  r12 = r9 <u 0x1
    ..D===eE----------------------------------R.............  r12 = r12 << 0x1
    ...D======================eE--------------R.............  r10 = r10 & 0x7d
    ...D=======================eE-------------R.............  r10 = r10 | r11
    ...D========================eE------------R.............  r10 = r10 | r12
    ....DeE-----------------------------------R.............  r11 = r8 & 0x7
    ....D========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x26f] = a3
    ....D=eeeeeeeeeeeeeeeeeeeeE----------------------------R  jump 20487 if r11 != 7
```

Gas simulation at offset 20459 with total cost of 2:

```
    DeER.  r8 = r8 & 0x18
    D=eER  jump 20513 if r8 != 8
```

Gas simulation at offset 20466 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.......  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  u8 [r6 + 0x26c] = s0
    DeE---------------------------------------R.......  r7 = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r0 = u64 [r1 + 0x18]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......  r5 = u64 [r1 + 0x10]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......  r6 = u64 [r1 + 0x8]
    .D========================eE--------------R.......  r1 = r1 + 0x20
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 20487 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = u16 [r6 + 0x263]
    DeeeeeeeeeeeeeeeE----------R  r0 = 482, jump 23116
```

Gas simulation at offset 20497 with total cost of 47:

```
    DeER..............................................  r7 = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r0 = u64 [r1 + 0x18]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r5 = u64 [r1 + 0x10]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r6 = u64 [r1 + 0x8]
    .DeE-----------------------R......................  r1 = r1 + 0x20
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 20513 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.......  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  u8 [r6 + 0x26d] = s0
    DeE---------------------------------------R.......  r7 = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r0 = u64 [r1 + 0x18]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......  r5 = u64 [r1 + 0x10]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......  r6 = u64 [r1 + 0x8]
    .D========================eE--------------R.......  r1 = r1 + 0x20
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 20534 with total cost of 58:

```
    DeER.........................................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER................................  r8 = u8 [r7 + 0x265]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER................................  r9 = u8 [r7 + 0x26b]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER................................  r10 = u8 [r7 + 0x26f]
    .D=========================eER...............................  r11 = r9 - r8
    .D=========================eER...............................  r10 = r10 & 0x7c
    .D=========================eER...............................  r8 = r8 ^ r9
    ..D=========================eeeER............................  r9 = r11 <u 0x100
    ..D=========================eE--R............................  r11 = r11 & 0x80
    ...D========================eeeER............................  r8 = r8 <u 0x1
    ...D===========================eER...........................  r8 = r8 << 0x1
    ....D==========================eER...........................  r9 = r9 | r10
    ....D===========================eER..........................  r8 = r8 | r9
    ....D============================eER.........................  r8 = r8 | r11
    ....D=============================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x26f] = a1
    .....DeE----------------------------------------------------R  r7 = 0
    .....DeeeeeeeeeeeeeeeeeeeeeeE-------------------------------R  jump [r0 + 0]
```

Gas simulation at offset 20590 with total cost of 58:

```
    DeER.........................................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER................................  r8 = u8 [r7 + 0x265]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER................................  r9 = u8 [r7 + 0x26c]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER................................  r10 = u8 [r7 + 0x26f]
    .D=========================eER...............................  r11 = r9 - r8
    .D=========================eER...............................  r10 = r10 & 0x7c
    .D=========================eER...............................  r8 = r8 ^ r9
    ..D=========================eeeER............................  r9 = r11 <u 0x100
    ..D=========================eE--R............................  r11 = r11 & 0x80
    ...D========================eeeER............................  r8 = r8 <u 0x1
    ...D===========================eER...........................  r8 = r8 << 0x1
    ....D==========================eER...........................  r9 = r9 | r10
    ....D===========================eER..........................  r8 = r8 | r9
    ....D============================eER.........................  r8 = r8 | r11
    ....D=============================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x26f] = a1
    .....DeE----------------------------------------------------R  r7 = 0
    .....DeeeeeeeeeeeeeeeeeeeeeeE-------------------------------R  jump [r0 + 0]
```

Gas simulation at offset 20646 with total cost of 58:

```
    DeER.........................................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER................................  r8 = u8 [r7 + 0x265]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER................................  r9 = u8 [r7 + 0x26d]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER................................  r10 = u8 [r7 + 0x26f]
    .D=========================eER...............................  r11 = r9 - r8
    .D=========================eER...............................  r10 = r10 & 0x7c
    .D=========================eER...............................  r8 = r8 ^ r9
    ..D=========================eeeER............................  r9 = r11 <u 0x100
    ..D=========================eE--R............................  r11 = r11 & 0x80
    ...D========================eeeER............................  r8 = r8 <u 0x1
    ...D===========================eER...........................  r8 = r8 << 0x1
    ....D==========================eER...........................  r9 = r9 | r10
    ....D===========================eER..........................  r8 = r8 | r9
    ....D============================eER.........................  r8 = r8 | r11
    ....D=============================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x26f] = a1
    .....DeE----------------------------------------------------R  r7 = 0
    .....DeeeeeeeeeeeeeeeeeeeeeeE-------------------------------R  jump [r0 + 0]
```

Gas simulation at offset 20702 with total cost of 56:

```
    DeER.......................................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..............................  r8 = u8 [r7 + 0x26f]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..............................  r9 = u8 [r7 + 0x265]
    D==========================eER.............................  r8 = r8 & 0x7d
    .D=========================eER.............................  r10 = r9 & 0x80
    ..D========================eeeER...........................  r11 = r9 <u 0x1
    ..D===========================eER..........................  r11 = r11 << 0x1
    ...D========================eE--R..........................  r8 = r8 | r10
    ...D===========================eER.........................  r8 = r8 | r11
    ...D=======================eeeeeeeeeeeeeeeeeeeeeeeeeER.....  u8 [r7 + 0x26b] = a2
    ...D============================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x26f] = a1
    ....DeE---------------------------------------------------R  r7 = 0
    ....DeeeeeeeeeeeeeeeeeeeeeeE------------------------------R  jump [r0 + 0]
```

Gas simulation at offset 20745 with total cost of 56:

```
    DeER.......................................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..............................  r8 = u8 [r7 + 0x26f]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..............................  r9 = u8 [r7 + 0x265]
    D==========================eER.............................  r8 = r8 & 0x7d
    .D=========================eER.............................  r10 = r9 & 0x80
    ..D========================eeeER...........................  r11 = r9 <u 0x1
    ..D===========================eER..........................  r11 = r11 << 0x1
    ...D========================eE--R..........................  r8 = r8 | r10
    ...D===========================eER.........................  r8 = r8 | r11
    ...D=======================eeeeeeeeeeeeeeeeeeeeeeeeeER.....  u8 [r7 + 0x26c] = a2
    ...D============================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x26f] = a1
    ....DeE---------------------------------------------------R  r7 = 0
    ....DeeeeeeeeeeeeeeeeeeeeeeE------------------------------R  jump [r0 + 0]
```

Gas simulation at offset 20788 with total cost of 56:

```
    DeER.......................................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..............................  r8 = u8 [r7 + 0x26f]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..............................  r9 = u8 [r7 + 0x265]
    D==========================eER.............................  r8 = r8 & 0x7d
    .D=========================eER.............................  r10 = r9 & 0x80
    ..D========================eeeER...........................  r11 = r9 <u 0x1
    ..D===========================eER..........................  r11 = r11 << 0x1
    ...D========================eE--R..........................  r8 = r8 | r10
    ...D===========================eER.........................  r8 = r8 | r11
    ...D=======================eeeeeeeeeeeeeeeeeeeeeeeeeER.....  u8 [r7 + 0x26d] = a2
    ...D============================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x26f] = a1
    ....DeE---------------------------------------------------R  r7 = 0
    ....DeeeeeeeeeeeeeeeeeeeeeeE------------------------------R  jump [r0 + 0]
```

Gas simulation at offset 20831 with total cost of 26:

```
    DeER.........................  r1 = r1 + 0xfffffffffffffff8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0] = r0
    DeE-------------------------R  r9 = r7 + 0x7ff
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = u16 [r9 + 0x263]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER  r9 = u8 [r9 + 0x26b]
    .DeeeeeeeeeeeeeeeE----------R  r0 = 498, jump 23116
```

Gas simulation at offset 20854 with total cost of 47:

```
    DeER..............................................  r7 = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r0 = u64 [r1 + 0]
    DeE------------------------R......................  r1 = r1 + 0x8
    D=========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 20863 with total cost of 26:

```
    DeER.........................  r1 = r1 + 0xfffffffffffffff8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0] = r0
    DeE-------------------------R  r9 = r7 + 0x7ff
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = u16 [r9 + 0x263]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER  r9 = u8 [r9 + 0x26c]
    .DeeeeeeeeeeeeeeeE----------R  r0 = 502, jump 23116
```

Gas simulation at offset 20886 with total cost of 47:

```
    DeER..............................................  r7 = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r0 = u64 [r1 + 0]
    DeE------------------------R......................  r1 = r1 + 0x8
    D=========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 20895 with total cost of 26:

```
    DeER.........................  r1 = r1 + 0xfffffffffffffff8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0] = r0
    DeE-------------------------R  r9 = r7 + 0x7ff
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = u16 [r9 + 0x263]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER  r9 = u8 [r9 + 0x26d]
    .DeeeeeeeeeeeeeeeE----------R  r0 = 506, jump 23116
```

Gas simulation at offset 20918 with total cost of 47:

```
    DeER..............................................  r7 = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r0 = u64 [r1 + 0]
    DeE------------------------R......................  r1 = r1 + 0x8
    D=========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 20927 with total cost of 52:

```
    DeER...................................................  r1 = r1 + 0xffffffffffffffe0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u64 [r1 + 0x18] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u64 [r1 + 0x10] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u64 [r1 + 0x8] = r6
    .DeE------------------------R..........................  r6 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r8 = u8 [r6 + 0x267]
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  r9 = u8 [r6 + 0x265]
    ..D=========================eE-----------------------R.  r10 = r8 & 0x7
    ..DeE------------------------------------------------R.  r2 = 0x7
    ...D================================================eER  r5 = r9 + 0xffffffffffffffff
    ...D=========================eE-----------------------R  jump 20987 if r10 == r2
```

Gas simulation at offset 20963 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = u16 [r6 + 0x263]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0] = r7
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u64 [r1 + 0]
    DeeeeeeeeeeeeeeeE----------R  r0 = 510, jump 23116
```

Gas simulation at offset 20977 with total cost of 25:

```
    DeER........................  r2 = 0x7
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u64 [r1 + 0]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = u8 [r6 + 0x267]
    DeeE-----------------------R  fallthrough
```

Gas simulation at offset 20987 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r10 = u8 [r6 + 0x26f]
    DeE---------------------------------------R.............  r11 = r5 & 0x80
    .DeE--------------------------------------R.............  r9 = r5 & 0xff
    ..DeeeE-----------------------------------R.............  r12 = r9 <u 0x1
    ..D===eE----------------------------------R.............  r12 = r12 << 0x1
    ...D======================eE--------------R.............  r10 = r10 & 0x7d
    ...D=======================eE-------------R.............  r10 = r10 | r11
    ...D========================eE------------R.............  r10 = r10 | r12
    ....DeE-----------------------------------R.............  r11 = r8 & 0x7
    ....D========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x26f] = a3
    ....D=eeeeeeeeeeeeeeeeeeeeE----------------------------R  jump 21054 if r11 != 7
```

Gas simulation at offset 21026 with total cost of 2:

```
    DeER.  r8 = r8 & 0x18
    D=eER  jump 21080 if r8 != 8
```

Gas simulation at offset 21033 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.......  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  u8 [r6 + 0x26c] = s0
    DeE---------------------------------------R.......  r7 = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r0 = u64 [r1 + 0x18]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......  r5 = u64 [r1 + 0x10]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......  r6 = u64 [r1 + 0x8]
    .D========================eE--------------R.......  r1 = r1 + 0x20
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 21054 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = u16 [r6 + 0x263]
    DeeeeeeeeeeeeeeeE----------R  r0 = 512, jump 23116
```

Gas simulation at offset 21064 with total cost of 47:

```
    DeER..............................................  r7 = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r0 = u64 [r1 + 0x18]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r5 = u64 [r1 + 0x10]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r6 = u64 [r1 + 0x8]
    .DeE-----------------------R......................  r1 = r1 + 0x20
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 21080 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.......  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  u8 [r6 + 0x26d] = s0
    DeE---------------------------------------R.......  r7 = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r0 = u64 [r1 + 0x18]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......  r5 = u64 [r1 + 0x10]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......  r6 = u64 [r1 + 0x8]
    .D========================eE--------------R.......  r1 = r1 + 0x20
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 21101 with total cost of 27:

```
    DeER..........................  r1 = r1 + 0xfffffffffffffff8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.  u64 [r1 + 0] = r0
    DeE-------------------------R.  r8 = r7 + 0x7ff
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r9 = u8 [r8 + 0x26b]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r10 = u8 [r8 + 0x26c]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r8 = u16 [r8 + 0x263]
    .D=========================eER  r9 = r9 & r10
    ..DeeeeeeeeeeeeeeeE----------R  r0 = 516, jump 23116
```

Gas simulation at offset 21131 with total cost of 47:

```
    DeER..............................................  r7 = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r0 = u64 [r1 + 0]
    DeE------------------------R......................  r1 = r1 + 0x8
    D=========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 21140 with total cost of 56:

```
    DeER.......................................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..............................  r8 = u8 [r7 + 0x26f]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..............................  r9 = u8 [r7 + 0x265]
    D==========================eER.............................  r8 = r8 & 0x7d
    .D=========================eER.............................  r10 = r9 & 0x80
    ..D========================eeeER...........................  r11 = r9 <u 0x1
    ..D===========================eER..........................  r11 = r11 << 0x1
    ...D========================eE--R..........................  r8 = r8 | r10
    ...D===========================eER.........................  r8 = r8 | r11
    ...D=======================eeeeeeeeeeeeeeeeeeeeeeeeeER.....  u8 [r7 + 0x26b] = a2
    ...D========================eeeeeeeeeeeeeeeeeeeeeeeeeER....  u8 [r7 + 0x26c] = a2
    ....D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x26f] = a1
    ....DeE---------------------------------------------------R  r7 = 0
    ....DeeeeeeeeeeeeeeeeeeeeeeE------------------------------R  jump [r0 + 0]
```

Gas simulation at offset 21187 with total cost of 52:

```
    DeER...................................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r8 = u8 [r7 + 0x26f]
    D==========================eER.........................  r8 = r8 & 0xfe
    D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x26f] = a1
    .DeE--------------------------------------------------R  r7 = 0
    .DeeeeeeeeeeeeeeeeeeeeeeE-----------------------------R  jump [r0 + 0]
```

Gas simulation at offset 21207 with total cost of 52:

```
    DeER...................................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r8 = u8 [r7 + 0x26f]
    D==========================eER.........................  r8 = r8 | 0x1
    D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x26f] = a1
    .DeE--------------------------------------------------R  r7 = 0
    .DeeeeeeeeeeeeeeeeeeeeeeE-----------------------------R  jump [r0 + 0]
```

Gas simulation at offset 21226 with total cost of 52:

```
    DeER...................................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r8 = u8 [r7 + 0x26f]
    D==========================eER.........................  r8 = r8 & 0xf7
    D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x26f] = a1
    .DeE--------------------------------------------------R  r7 = 0
    .DeeeeeeeeeeeeeeeeeeeeeeE-----------------------------R  jump [r0 + 0]
```

Gas simulation at offset 21246 with total cost of 52:

```
    DeER...................................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r8 = u8 [r7 + 0x26f]
    D==========================eER.........................  r8 = r8 | 0x8
    D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x26f] = a1
    .DeE--------------------------------------------------R  r7 = 0
    .DeeeeeeeeeeeeeeeeeeeeeeE-----------------------------R  jump [r0 + 0]
```

Gas simulation at offset 21265 with total cost of 52:

```
    DeER...................................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r8 = u8 [r7 + 0x26f]
    D==========================eER.........................  r8 = r8 & 0xbf
    D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x26f] = a1
    .DeE--------------------------------------------------R  r7 = 0
    .DeeeeeeeeeeeeeeeeeeeeeeE-----------------------------R  jump [r0 + 0]
```

Gas simulation at offset 21285 with total cost of 52:

```
    DeER...................................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r8 = u8 [r7 + 0x26f]
    D==========================eER.........................  r8 = r8 & 0xfb
    D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x26f] = a1
    .DeE--------------------------------------------------R  r7 = 0
    .DeeeeeeeeeeeeeeeeeeeeeeE-----------------------------R  jump [r0 + 0]
```

Gas simulation at offset 21305 with total cost of 52:

```
    DeER...................................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r8 = u8 [r7 + 0x26f]
    D==========================eER.........................  r8 = r8 | 0x4
    D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x26f] = a1
    .DeE--------------------------------------------------R  r7 = 0
    .DeeeeeeeeeeeeeeeeeeeeeeE-----------------------------R  jump [r0 + 0]
```

Gas simulation at offset 21324 with total cost of 28:

```
    DeER...........................  r1 = r1 + 0xffffffffffffffe0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0x18] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0x10] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0x8] = r6
    .DeE------------------------R..  r6 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER.  r8 = i8 [r6 + 0x26f]
    .D==========================eER  jump 21364 if r8 <s 0
```

Gas simulation at offset 21347 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.......  unlikely
    DeE---------------------------------------R.......  r7 = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r0 = u64 [r1 + 0x18]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r5 = u64 [r1 + 0x10]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......  r6 = u64 [r1 + 0x8]
    .DeE--------------------------------------R.......  r1 = r1 + 0x20
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 21364 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = u16 [r6 + 0x269]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0] = r7
    DeeeeeeeeeeeeeeeE----------R  r0 = 536, jump 22578
```

Gas simulation at offset 21376 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r5 = i8 [r6 + 0x265]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r7 = u16 [r6 + 0x269]
    D=========================eER.....................  r5 = r5 + r7
    D=========================eER.....................  r7 = r7 & 0xffffffffffffff00
    .D=========================eER....................  r8 = r5 & 0xff00
    .D==========================eeeeeeeeeeeeeeeeeeeeER  jump 21414 if r7 == r8
```

Gas simulation at offset 21399 with total cost of 25:

```
    DeER........................  r8 = r5 & 0xff
    D=eER.......................  r8 = r8 | r7
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u64 [r1 + 0]
    .DeeeeeeeeeeeeeeeE---------R  r0 = 538, jump 22578
```

Gas simulation at offset 21414 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  u16 [r6 + 0x269] = r5
    DeE------------------------R......................  r7 = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r0 = u64 [r1 + 0x18]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r5 = u64 [r1 + 0x10]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER.....................  r6 = u64 [r1 + 0x8]
    .D========================eER.....................  r1 = r1 + 0x20
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 21434 with total cost of 29:

```
    DeER............................  r1 = r1 + 0xffffffffffffffe0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0x18] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0x10] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0x8] = r6
    .DeE------------------------R...  r6 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u8 [r6 + 0x26f]
    .D==========================eER.  r8 = r8 & 0x2
    ..D==========================eER  jump 21515 if r8 == 0
```

Gas simulation at offset 21460 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = u16 [r6 + 0x269]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0] = r7
    DeeeeeeeeeeeeeeeE----------R  r0 = 542, jump 22578
```

Gas simulation at offset 21472 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r5 = i8 [r6 + 0x265]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r7 = u16 [r6 + 0x269]
    D=========================eER.....................  r5 = r5 + r7
    D=========================eER.....................  r7 = r7 & 0xffffffffffffff00
    .D=========================eER....................  r8 = r5 & 0xff00
    .D==========================eeeeeeeeeeeeeeeeeeeeER  jump 21510 if r7 == r8
```

Gas simulation at offset 21495 with total cost of 25:

```
    DeER........................  r8 = r5 & 0xff
    D=eER.......................  r8 = r8 | r7
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u64 [r1 + 0]
    .DeeeeeeeeeeeeeeeE---------R  r0 = 544, jump 22578
```

Gas simulation at offset 21510 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r6 + 0x269] = r5
    DeeE-----------------------R  fallthrough
```

Gas simulation at offset 21515 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.......  unlikely
    DeE---------------------------------------R.......  r7 = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r0 = u64 [r1 + 0x18]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r5 = u64 [r1 + 0x10]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......  r6 = u64 [r1 + 0x8]
    .DeE--------------------------------------R.......  r1 = r1 + 0x20
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 21532 with total cost of 29:

```
    DeER............................  r1 = r1 + 0xffffffffffffffe0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0x18] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0x10] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0x8] = r6
    .DeE------------------------R...  r6 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u8 [r6 + 0x26f]
    .D==========================eER.  r8 = r8 & 0x1
    ..D==========================eER  jump 21613 if r8 == 0
```

Gas simulation at offset 21558 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = u16 [r6 + 0x269]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0] = r7
    DeeeeeeeeeeeeeeeE----------R  r0 = 548, jump 22578
```

Gas simulation at offset 21570 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r5 = i8 [r6 + 0x265]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r7 = u16 [r6 + 0x269]
    D=========================eER.....................  r5 = r5 + r7
    D=========================eER.....................  r7 = r7 & 0xffffffffffffff00
    .D=========================eER....................  r8 = r5 & 0xff00
    .D==========================eeeeeeeeeeeeeeeeeeeeER  jump 21608 if r7 == r8
```

Gas simulation at offset 21593 with total cost of 25:

```
    DeER........................  r8 = r5 & 0xff
    D=eER.......................  r8 = r8 | r7
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u64 [r1 + 0]
    .DeeeeeeeeeeeeeeeE---------R  r0 = 550, jump 22578
```

Gas simulation at offset 21608 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r6 + 0x269] = r5
    DeeE-----------------------R  fallthrough
```

Gas simulation at offset 21613 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.......  unlikely
    DeE---------------------------------------R.......  r7 = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r0 = u64 [r1 + 0x18]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r5 = u64 [r1 + 0x10]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......  r6 = u64 [r1 + 0x8]
    .DeE--------------------------------------R.......  r1 = r1 + 0x20
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 21630 with total cost of 28:

```
    DeER...........................  r1 = r1 + 0xffffffffffffffe0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0x18] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0x10] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0x8] = r6
    .DeE------------------------R..  r6 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER.  r8 = i8 [r6 + 0x26f]
    .D==========================eER  jump 21708 if r8 <s 0
```

Gas simulation at offset 21653 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = u16 [r6 + 0x269]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0] = r7
    DeeeeeeeeeeeeeeeE----------R  r0 = 554, jump 22578
```

Gas simulation at offset 21665 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r5 = i8 [r6 + 0x265]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r7 = u16 [r6 + 0x269]
    D=========================eER.....................  r5 = r5 + r7
    D=========================eER.....................  r7 = r7 & 0xffffffffffffff00
    .D=========================eER....................  r8 = r5 & 0xff00
    .D==========================eeeeeeeeeeeeeeeeeeeeER  jump 21703 if r7 == r8
```

Gas simulation at offset 21688 with total cost of 25:

```
    DeER........................  r8 = r5 & 0xff
    D=eER.......................  r8 = r8 | r7
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u64 [r1 + 0]
    .DeeeeeeeeeeeeeeeE---------R  r0 = 556, jump 22578
```

Gas simulation at offset 21703 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r6 + 0x269] = r5
    DeeE-----------------------R  fallthrough
```

Gas simulation at offset 21708 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.......  unlikely
    DeE---------------------------------------R.......  r7 = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r0 = u64 [r1 + 0x18]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r5 = u64 [r1 + 0x10]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......  r6 = u64 [r1 + 0x8]
    .DeE--------------------------------------R.......  r1 = r1 + 0x20
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 21725 with total cost of 29:

```
    DeER............................  r1 = r1 + 0xffffffffffffffe0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0x18] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0x10] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0x8] = r6
    .DeE------------------------R...  r6 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u8 [r6 + 0x26f]
    .D==========================eER.  r8 = r8 & 0x2
    ..D==========================eER  jump 21806 if r8 != 0
```

Gas simulation at offset 21751 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = u16 [r6 + 0x269]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0] = r7
    DeeeeeeeeeeeeeeeE----------R  r0 = 560, jump 22578
```

Gas simulation at offset 21763 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r5 = i8 [r6 + 0x265]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r7 = u16 [r6 + 0x269]
    D=========================eER.....................  r5 = r5 + r7
    D=========================eER.....................  r7 = r7 & 0xffffffffffffff00
    .D=========================eER....................  r8 = r5 & 0xff00
    .D==========================eeeeeeeeeeeeeeeeeeeeER  jump 21801 if r7 == r8
```

Gas simulation at offset 21786 with total cost of 25:

```
    DeER........................  r8 = r5 & 0xff
    D=eER.......................  r8 = r8 | r7
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u64 [r1 + 0]
    .DeeeeeeeeeeeeeeeE---------R  r0 = 562, jump 22578
```

Gas simulation at offset 21801 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r6 + 0x269] = r5
    DeeE-----------------------R  fallthrough
```

Gas simulation at offset 21806 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.......  unlikely
    DeE---------------------------------------R.......  r7 = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r0 = u64 [r1 + 0x18]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r5 = u64 [r1 + 0x10]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......  r6 = u64 [r1 + 0x8]
    .DeE--------------------------------------R.......  r1 = r1 + 0x20
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 21823 with total cost of 29:

```
    DeER............................  r1 = r1 + 0xffffffffffffffe0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0x18] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0x10] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0x8] = r6
    .DeE------------------------R...  r6 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u8 [r6 + 0x26f]
    .D==========================eER.  r8 = r8 & 0x1
    ..D==========================eER  jump 21904 if r8 != 0
```

Gas simulation at offset 21849 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = u16 [r6 + 0x269]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0] = r7
    DeeeeeeeeeeeeeeeE----------R  r0 = 566, jump 22578
```

Gas simulation at offset 21861 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r5 = i8 [r6 + 0x265]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r7 = u16 [r6 + 0x269]
    D=========================eER.....................  r5 = r5 + r7
    D=========================eER.....................  r7 = r7 & 0xffffffffffffff00
    .D=========================eER....................  r8 = r5 & 0xff00
    .D==========================eeeeeeeeeeeeeeeeeeeeER  jump 21899 if r7 == r8
```

Gas simulation at offset 21884 with total cost of 25:

```
    DeER........................  r8 = r5 & 0xff
    D=eER.......................  r8 = r8 | r7
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u64 [r1 + 0]
    .DeeeeeeeeeeeeeeeE---------R  r0 = 568, jump 22578
```

Gas simulation at offset 21899 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r6 + 0x269] = r5
    DeeE-----------------------R  fallthrough
```

Gas simulation at offset 21904 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.......  unlikely
    DeE---------------------------------------R.......  r7 = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r0 = u64 [r1 + 0x18]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r5 = u64 [r1 + 0x10]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......  r6 = u64 [r1 + 0x8]
    .DeE--------------------------------------R.......  r1 = r1 + 0x20
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 21921 with total cost of 29:

```
    DeER............................  r1 = r1 + 0xffffffffffffffe0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0x18] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0x10] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0x8] = r6
    .DeE------------------------R...  r6 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u8 [r6 + 0x26f]
    .D==========================eER.  r8 = r8 & 0x40
    ..D==========================eER  jump 22002 if r8 == 0
```

Gas simulation at offset 21947 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = u16 [r6 + 0x269]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0] = r7
    DeeeeeeeeeeeeeeeE----------R  r0 = 572, jump 22578
```

Gas simulation at offset 21959 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r5 = i8 [r6 + 0x265]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r7 = u16 [r6 + 0x269]
    D=========================eER.....................  r5 = r5 + r7
    D=========================eER.....................  r7 = r7 & 0xffffffffffffff00
    .D=========================eER....................  r8 = r5 & 0xff00
    .D==========================eeeeeeeeeeeeeeeeeeeeER  jump 21997 if r7 == r8
```

Gas simulation at offset 21982 with total cost of 25:

```
    DeER........................  r8 = r5 & 0xff
    D=eER.......................  r8 = r8 | r7
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u64 [r1 + 0]
    .DeeeeeeeeeeeeeeeE---------R  r0 = 574, jump 22578
```

Gas simulation at offset 21997 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r6 + 0x269] = r5
    DeeE-----------------------R  fallthrough
```

Gas simulation at offset 22002 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.......  unlikely
    DeE---------------------------------------R.......  r7 = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r0 = u64 [r1 + 0x18]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r5 = u64 [r1 + 0x10]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......  r6 = u64 [r1 + 0x8]
    .DeE--------------------------------------R.......  r1 = r1 + 0x20
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 22019 with total cost of 29:

```
    DeER............................  r1 = r1 + 0xffffffffffffffe0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0x18] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0x10] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  u64 [r1 + 0x8] = r6
    .DeE------------------------R...  r6 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u8 [r6 + 0x26f]
    .D==========================eER.  r8 = r8 & 0x40
    ..D==========================eER  jump 22100 if r8 != 0
```

Gas simulation at offset 22045 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = u16 [r6 + 0x269]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0] = r7
    DeeeeeeeeeeeeeeeE----------R  r0 = 578, jump 22578
```

Gas simulation at offset 22057 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r5 = i8 [r6 + 0x265]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r7 = u16 [r6 + 0x269]
    D=========================eER.....................  r5 = r5 + r7
    D=========================eER.....................  r7 = r7 & 0xffffffffffffff00
    .D=========================eER....................  r8 = r5 & 0xff00
    .D==========================eeeeeeeeeeeeeeeeeeeeER  jump 22095 if r7 == r8
```

Gas simulation at offset 22080 with total cost of 25:

```
    DeER........................  r8 = r5 & 0xff
    D=eER.......................  r8 = r8 | r7
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u64 [r1 + 0]
    .DeeeeeeeeeeeeeeeE---------R  r0 = 580, jump 22578
```

Gas simulation at offset 22095 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r6 + 0x269] = r5
    DeeE-----------------------R  fallthrough
```

Gas simulation at offset 22100 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.......  unlikely
    DeE---------------------------------------R.......  r7 = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r0 = u64 [r1 + 0x18]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r5 = u64 [r1 + 0x10]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......  r6 = u64 [r1 + 0x8]
    .DeE--------------------------------------R.......  r1 = r1 + 0x20
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 22117 with total cost of 22:

```
    DeeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 22119 with total cost of 51:

```
    DeER..................................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r8 = u8 [r7 + 0x265]
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r7 + 0x263] = r8
    DeeeeeeeeeeeeeeeeeeeeeeE-----------------------------R  jump [r0 + 0]
```

Gas simulation at offset 22133 with total cost of 27:

```
    DeER..........................  r1 = r1 + 0xffffffffffffffe8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.  u64 [r1 + 0x10] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.  u64 [r1 + 0x8] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.  u64 [r1 + 0] = r6
    .D............................  r5 = r7
    .DeE------------------------R.  r6 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = u16 [r6 + 0x269]
    ..DeeeeeeeeeeeeeeeE----------R  r0 = 588, jump 22578
```

Gas simulation at offset 22160 with total cost of 61:

```
    D...............................................................  r8 = r7
    D...............................................................  r7 = r5
    DeeeeeeeeeeeeeeeeeeeeeeeeeER....................................  r9 = i16 [r6 + 0x269]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER....................................  r10 = u8 [r6 + 0x267]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER...................................  r11 = u8 [r6 + 0x265]
    .D========================eER...................................  r9 = r9 + 0x1
    .D========================eER...................................  r12 = r10 & 0x18
    ..D========================eER..................................  r12 = r12 + 0xfffffffffffffff8
    ..D=========================eeeER...............................  r12 = r12 <u 0x1
    ...D===========================eER..............................  r12 = r5 - r12
    ...D============================eER.............................  r12 = r12 + 0x7ff
    ...D=============================eeeeeeeeeeeeeeeeeeeeeeeeeER....  r5 = u8 [r12 + 0x26d]
    ...D=======================eeeeeeeeeeeeeeeeeeeeeeeeeE------R....  u16 [r6 + 0x269] = r9
    ....DeE----------------------------------------------------R....  r8 = r8 << 0x8
    ....D======================eE------------------------------R....  r11 = r11 | r8
    ....D=====================================================eER...  r5 = r5 + r11
    .....D=====================================================eER..  r9 = r5 & 0xff
    .....D======================================================eER.  r8 = r8 | r9
    ......D===================eE----------------------------------R.  r9 = r10 & 0x20
    ......D======================================================eER  r8 = zext16 r8
    ......D====================eeeeeeeeeeeeeeeeeeeeE---------------R  jump 22250 if r9 != 0
```

Gas simulation at offset 22227 with total cost of 2:

```
    DeER.  r9 = zext16 r5
    D=eER  jump 22250 if r8 != r9
```

Gas simulation at offset 22232 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.......  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  u16 [r6 + 0x263] = r5
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r0 = u64 [r1 + 0x10]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r5 = u64 [r1 + 0x8]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......  r6 = u64 [r1 + 0]
    .D========================eE--------------R.......  r1 = r1 + 0x18
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 22250 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  r0 = 590, jump 22578
```

Gas simulation at offset 22256 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  u16 [r6 + 0x263] = r5
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r0 = u64 [r1 + 0x10]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r5 = u64 [r1 + 0x8]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r6 = u64 [r1 + 0]
    .D========================eER.....................  r1 = r1 + 0x18
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 22273 with total cost of 27:

```
    DeER..........................  r1 = r1 + 0xffffffffffffffe8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.  u64 [r1 + 0x10] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.  u64 [r1 + 0x8] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.  u64 [r1 + 0] = r6
    .D............................  r5 = r7
    .DeE------------------------R.  r6 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = u8 [r6 + 0x265]
    ..DeeeeeeeeeeeeeeeE----------R  r0 = 594, jump 22578
```

Gas simulation at offset 22300 with total cost of 84:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................  r7 = u8 [r6 + 0x267]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................  r8 = u8 [r6 + 0x265]
    D=========================eER..........................................................  r7 = r7 & 0x18
    D==========================eER.........................................................  r7 = r7 + 0xfffffffffffffff8
    .D==========================eeeER......................................................  r7 = r7 <u 0x1
    .D=============================eER.....................................................  r5 = r5 - r7
    ..D=============================eER....................................................  r7 = r5 + 0x7ff
    ..D==============================eeeeeeeeeeeeeeeeeeeeeeeeeER...........................  r7 = u8 [r7 + 0x26d]
    ..D=======================================================eER..........................  r7 = r7 + r8
    ...D=======================================================eER.........................  r7 = r7 & 0xff
    ...D========================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r6 + 0x263] = r7
    ...DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------------------------------------R  r0 = u64 [r1 + 0x10]
    ...DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------------------------------------R  r5 = u64 [r1 + 0x8]
    ....D=====================eeeeeeeeeeeeeeeeeeeeeeeeeE----------------------------------R  r6 = u64 [r1 + 0]
    ....D========================eE-------------------------------------------------------R  r1 = r1 + 0x18
    ....D========================eeeeeeeeeeeeeeeeeeeeeeE----------------------------------R  jump [r0 + 0]
```

Gas simulation at offset 22352 with total cost of 53:

```
    DeER....................................................  r1 = r1 + 0xffffffffffffffd8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...........................  u64 [r1 + 0x20] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...........................  u64 [r1 + 0x18] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...........................  u64 [r1 + 0x10] = r6
    .D......................................................  r5 = r7
    .DeE------------------------R...........................  r6 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r8 = u8 [r6 + 0x265]
    ..D=========================eER.........................  r7 = r8 + 0x1
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x8] = r7
    ..D.....................................................  r7 = r5
    ...DeeeeeeeeeeeeeeeE-----------------------------------R  r0 = 598, jump 22578
```

Gas simulation at offset 22388 with total cost of 26:

```
    DeER.........................  r7 = r7 & 0xff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0] = r7
    DeeeeeeeeeeeeeeeeeeeeeeeeeE-R  r8 = u8 [r1 + 0x8]
    D............................  r7 = r5
    .DeeeeeeeeeeeeeeeE----------R  r0 = 600, jump 22578
```

Gas simulation at offset 22405 with total cost of 31:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......  u64 [r1 + 0x8] = r6
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......  r6 = u8 [r6 + 0x26d]
    DeE------------------------R......  r7 = r7 << 0x8
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......  r8 = u64 [r1 + 0]
    .D========================eER.....  r8 = r8 | r7
    .D=========================eER....  r6 = r6 + r8
    .D==========================eER...  r9 = zext16 r6
    ..D=========================eER...  r8 = r6 & 0xff
    ..D==========================eER..  r7 = r7 | r8
    ..D===========================eER.  r8 = zext16 r7
    ...D===========================eER  jump 22451 if r8 != r9
```

Gas simulation at offset 22437 with total cost of 71:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...............................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...............................  r7 = u64 [r1 + 0x8]
    D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER.....................  r7 = u8 [r7 + 0x267]
    D==================================================eER....................  r7 = r7 & 0x20
    .D==================================================eeeeeeeeeeeeeeeeeeeeER  jump 22458 if r7 == 0
```

Gas simulation at offset 22451 with total cost of 15:

```
    D.................  r7 = r5
    DeeeeeeeeeeeeeeeER  r0 = 602, jump 22578
```

Gas simulation at offset 22458 with total cost of 50:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r7 = u64 [r1 + 0x8]
    D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r7 + 0x263] = r6
    DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r0 = u64 [r1 + 0x20]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r5 = u64 [r1 + 0x18]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE------------------------R  r6 = u64 [r1 + 0x10]
    .D========================eE------------------------R  r1 = r1 + 0x28
    .D========================eeeeeeeeeeeeeeeeeeeeeeE---R  jump [r0 + 0]
```

Gas simulation at offset 22479 with total cost of 52:

```
    DeER...................................................  r1 = r1 + 0xffffffffffffffd8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u64 [r1 + 0x20] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u64 [r1 + 0x18] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u64 [r1 + 0x10] = r6
    .D.....................................................  r5 = r7
    .DeE------------------------R..........................  r7 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u64 [r1 + 0x8] = r7
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  r8 = u8 [r7 + 0x265]
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  r7 = u8 [r7 + 0x26c]
    ..D=================================================eER  r6 = r7 + r8
    ..D....................................................  r7 = r5
    ...DeeeeeeeeeeeeeeeE----------------------------------R  r0 = 606, jump 22578
```

Gas simulation at offset 22518 with total cost of 15:

```
    DeER..............  r8 = r6 & 0xff
    D.................  r7 = r5
    DeeeeeeeeeeeeeeeER  r0 = 608, jump 22578
```

Gas simulation at offset 22529 with total cost of 26:

```
    DeER.........................  r7 = r7 & 0xff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0] = r7
    DeE-------------------------R  r7 = r6 + 0x1
    .DeE------------------------R  r8 = r7 & 0xff
    .D...........................  r7 = r5
    .DeeeeeeeeeeeeeeeE----------R  r0 = 610, jump 22578
```

Gas simulation at offset 22549 with total cost of 51:

```
    DeER..................................................  r7 = r7 << 0x8
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r8 = u64 [r1 + 0]
    D=========================eER.........................  r7 = r7 | r8
    DeeeeeeeeeeeeeeeeeeeeeeeeeE-R.........................  r8 = u64 [r1 + 0x8]
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r8 + 0x263] = r7
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r0 = u64 [r1 + 0x20]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r5 = u64 [r1 + 0x18]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R  r6 = u64 [r1 + 0x10]
    ..D========================eE------------------------R  r1 = r1 + 0x28
    ..D========================eeeeeeeeeeeeeeeeeeeeeeE---R  jump [r0 + 0]
```

Gas simulation at offset 22578 with total cost of 27:

```
    DeER..........................  r1 = r1 + 0xffffffffffffffa8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.  u64 [r1 + 0x50] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.  u64 [r1 + 0x48] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.  u64 [r1 + 0x40] = r6
    .D............................  r5 = r8
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER.  u64 [r1 + 0x30] = r7
    .D=========================eER  r6 = r7 + 0x7ff
    ..DeeeeeeeeeeeeeeeE----------R  r0 = 612, jump 1045
```

Gas simulation at offset 22605 with total cost of 26:

```
    D............................  r8 = r5
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r7 = u8 [r6 + 0x277]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  u64 [r1 + 56] = 0x1
    D=========================eER  jump 22631 if r7 != 0
```

Gas simulation at offset 22618 with total cost of 45:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.....  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.....  r7 = u8 [r6 + 0x278]
    D=========================eeeeeeeeeeeeeeeeeeeeER  jump 23098 if r7 == 0
```

Gas simulation at offset 22627 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 56] = 0
    DeeE-----------------------R  fallthrough
```

Gas simulation at offset 22631 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r5 = u64 [r1 + 0x30]
    D...........................  r7 = r5
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x8] = r8
    DeeeeeeeeeeeeeeeE----------R  r0 = 614, jump 385
```

Gas simulation at offset 22645 with total cost of 15:

```
    D.................  r7 = r5
    DeeeeeeeeeeeeeeeER  r0 = 616, jump 1045
```

Gas simulation at offset 22653 with total cost of 27:

```
    DeER..........................  r2 = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 24] = 0
    DeE------------------------R..  r7 = r6 + 0xa1
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER.  u64 [r1 + 0] = r7
    .DeE------------------------R.  r7 = 0xffff000000000000
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x20] = r7
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x28] = r6
    ..DeeeeeeeeeeeeeeeE----------R  jump 22739
```

Gas simulation at offset 22682 with total cost of 57:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.................  r10 = u64 [r1 + 0x38]
    D=========================eE--------------R.................  r8 = r10 & 0xff
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.................  r9 = i16 [r6 + 0x275]
    .D=========================eeeE-----------R.................  r8 = r8 >u 0
    ..D===========================eE----------R.................  r8 = r8 + 0x1
    ..D============================eeE--------R.................  r10 = r8 if r7 != 0
    ..D==============================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x38] = r10
    ...DeeeeeeeeeeeeeeeeeeeeeeeeeE-----------------------------R  r7 = u64 [r1 + 0x18]
    ...D=========================eE----------------------------R  r9 = r9 + r7
    ...D==========================eE---------------------------R  r8 = zext16 r9
    ...DeeeeeeeeeeeeeeeeeeeeeeeeeE-----------------------------R  r5 = u64 [r1 + 0x30]
    ....D.......................................................  r7 = r5
    ....DeeeeeeeeeeeeeeeE--------------------------------------R  r0 = 618, jump 385
```

Gas simulation at offset 22724 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x10] = r7
    D...........................  r7 = r5
    DeeeeeeeeeeeeeeeE----------R  r0 = 620, jump 1045
```

Gas simulation at offset 22735 with total cost of 2:

```
    DeER.  r2 = 0x1
    DeeER  fallthrough
```

Gas simulation at offset 22739 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u8 [r6 + 0x277]
    DeE---------------------------------------R  r9 = 0
    D=========================eE--------------R  jump 22768 if r7 == 0
```

Gas simulation at offset 22749 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r8 = u8 [r1 + 0x38]
    D=========================eE--------------R  jump 22768 if r8 != 2
```

Gas simulation at offset 22757 with total cost of 29:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER....  r8 = u8 [r6 + 0x251]
    D=========================eER...  r8 = r8 & 0x1
    .D=========================eeeER  r9 = r8 <u 0x1
    .DeeE--------------------------R  fallthrough
```

Gas simulation at offset 22768 with total cost of 48:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R........  r12 = u8 [r6 + 0x278]
    .D========================eeE-------------R........  r10 = r2 | ~r12
    .D==========================eE------------R........  r10 = r10 & 0x1
    ..D==========================eeeeeeeeeeeeeeeeeeeeER  jump 22799 if r10 == 0
```

Gas simulation at offset 22782 with total cost of 21:

```
    DeER....................  r10 = 0
    DeER....................  r11 = r2 & r12
    D=eeeeeeeeeeeeeeeeeeeeER  jump 22815 if r11 != 0
```

Gas simulation at offset 22790 with total cost of 20:

```
    DeeeeeeeeeeeeeeeeeeeeER  jump 22818 if r9 != 0
```

Gas simulation at offset 22793 with total cost of 1:

```
    DeER  jump 22682 if r10 != 0
```

Gas simulation at offset 22796 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 22946
```

Gas simulation at offset 22799 with total cost of 29:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER....  r10 = u8 [r6 + 0x251]
    D=========================eER...  r10 = r10 & 0x1
    .D=========================eeeER  r10 = r10 <u 0x1
    ..DeE--------------------------R  r11 = r2 & r12
    ..D=eeeeeeeeeeeeeeeeeeeeE------R  jump 22790 if r11 == 0
```

Gas simulation at offset 22815 with total cost of 20:

```
    DeeeeeeeeeeeeeeeeeeeeER  jump 22931 if r9 == 0
```

Gas simulation at offset 22818 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = u16 [r6 + 0x273]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r5 = u64 [r1 + 0x30]
    D...........................  r7 = r5
    D...........................  r6 = r2
    .DeeeeeeeeeeeeeeeE---------R  r0 = 622, jump 385
```

Gas simulation at offset 22835 with total cost of 15:

```
    D.................  r8 = r5
    D.................  r5 = r7
    D.................  r7 = r8
    DeeeeeeeeeeeeeeeER  r0 = 624, jump 1045
```

Gas simulation at offset 22847 with total cost of 77:

```
    D...............................................................................  r2 = r6
    DeeeeeeeeeeeeeeeeeeeeeeeeeER....................................................  r6 = u64 [r1 + 0x28]
    D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER...........................  r7 = i16 [r6 + 0x87]
    D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER...........................  r8 = i16 [r6 + 0x85]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER...........................  u8 [r6 + 631] = 0
    .D=================================================eER..........................  r7 = r7 + 0x1
    .D=================================================eER..........................  r9 = r8 << 0x30
    ..D================================================eER..........................  r8 = r8 + 0xffffffffffffffff
    ..D=================================================eER.........................  r7 = r7 | 0x8000
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R.........................  r10 = u64 [r1 + 0x20]
    ..D=================================================eER.........................  r9 = r9 + r10
    ...D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u8 [r6 + 125] = 0x1
    ...D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u8 [r6 + 0x7e] = s0
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r6 + 0x85] = r8
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r6 + 0x87] = r7
    ....D================================================eE------------------------R  jump 22739 if r9 != 0
```

Gas simulation at offset 22903 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u8 [r6 + 0x8d]
    D=========================eE--------------R  jump 23004 if r7 == 0
```

Gas simulation at offset 22911 with total cost of 50:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........  r7 = i16 [r6 + 0x83]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........  r8 = i16 [r6 + 0x81]
    D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r6 + 0x85] = r7
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r6 + 0x87] = r8
    .DeeeeeeeeeeeeeeeE----------------------------------R  jump 22739
```

Gas simulation at offset 22931 with total cost of 1:

```
    DeER  jump 22682 if r10 != 0
```

Gas simulation at offset 22935 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r9 = u32 [r6 + 0x251]
    D=========================eE--------------R  r9 = r9 & 0x1
    D==========================eE-------------R  jump 23021 if r9 != 0
```

Gas simulation at offset 22946 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = u64 [r1 + 0x8]
    DeE------------------------R  jump 22956 if r7 != 0
```

Gas simulation at offset 22952 with total cost of 1:

```
    DeER  jump 23098 if r12 == 0
```

Gas simulation at offset 22956 with total cost of 57:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.................  r10 = u64 [r1 + 0x38]
    D=========================eE--------------R.................  r9 = r10 & 0xff
    .D=========================eeeE-----------R.................  r9 = r9 >u 0
    .D============================eE----------R.................  r9 = r9 + 0x1
    ..D============================eeE--------R.................  r10 = r9 if r7 != 0
    ..D==============================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x38] = r10
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE------------------------------R  r5 = u64 [r1 + 0x30]
    ...D........................................................  r7 = r5
    ...D........................................................  r6 = r2
    ...DeeeeeeeeeeeeeeeE---------------------------------------R  r0 = 626, jump 385
```

Gas simulation at offset 22988 with total cost of 15:

```
    D.................  r7 = r5
    DeeeeeeeeeeeeeeeER  r0 = 628, jump 1045
```

Gas simulation at offset 22996 with total cost of 25:

```
    D...........................  r2 = r6
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0x28]
    DeeeeeeeeeeeeeeeE----------R  jump 22739
```

Gas simulation at offset 23004 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u8 [r6 + 0x8c]
    D=========================eE--------------R  jump 22739 if r7 == 0
```

Gas simulation at offset 23013 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 143] = 0x1
    DeeeeeeeeeeeeeeeE----------R  jump 22739
```

Gas simulation at offset 23021 with total cost of 57:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.................  r9 = u64 [r1 + 0x38]
    D=========================eE--------------R.................  r8 = r9 & 0xff
    .D=========================eeeE-----------R.................  r8 = r8 >u 0
    .D============================eE----------R.................  r8 = r8 + 0x1
    ..D============================eeE--------R.................  r9 = r8 if r7 != 0
    ..D==============================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x38] = r9
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE------------------------------R  r5 = u64 [r1 + 0x18]
    ...D========================eE-----------------------------R  r7 = r5 & 0xff
    ...DeeeeeeeeeeeeeeeeeeeeeeeeeE-----------------------------R  r8 = u64 [r1 + 0]
    ...D=========================eE----------------------------R  r7 = r7 + r8
    ....DeeeeeeeeeeeeeeeeeeeeeeeeeE----------------------------R  r8 = u64 [r1 + 0x10]
    ....D=========================eeeeeeeeeeeeeeeeeeeeeeeeeE---R  u8 [r7 + 0] = a1
    ....D========================eeeeeeeeeeeeeeeeeeeeeeeeeE----R  r7 = u64 [r1 + 0x30]
    ....DeeeeeeeeeeeeeeeE--------------------------------------R  r0 = 630, jump 1045
```

Gas simulation at offset 23066 with total cost of 26:

```
    DeER.........................  r2 = 0
    DeER.........................  r5 = r5 + 0x1
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x18] = r5
    D=eE------------------------R  r7 = zext16 r5
    .DeE------------------------R  r8 = 0x100
    .D=eE-----------------------R  jump 22739 if r7 != r8
```

Gas simulation at offset 23084 with total cost of 25:

```
    DeER........................  r2 = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 632] = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 24] = 0x100
    DeeeeeeeeeeeeeeeE----------R  jump 22739
```

Gas simulation at offset 23098 with total cost of 26:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r7 = u64 [r1 + 0x30]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r0 = u64 [r1 + 0x50]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r5 = u64 [r1 + 0x48]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r6 = u64 [r1 + 0x40]
    .D========================eER  r1 = r1 + 0x58
    .DeeeeeeeeeeeeeeeE----------R  jump 385
```

Gas simulation at offset 23116 with total cost of 53:

```
    DeER....................................................  r1 = r1 + 0xffffffffffffffd0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...........................  u64 [r1 + 0x28] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...........................  u64 [r1 + 0x20] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...........................  u64 [r1 + 0x18] = r6
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................  u64 [r1 + 0x10] = r9
    .D......................................................  r5 = r8
    .D......................................................  r6 = r7
    .D=========================eER..........................  r7 = r7 + 0x7ff
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u64 [r1 + 0] = r7
    ..D=========================eE------------------------R.  r7 = r7 + 0x1
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x8] = r7
    ..D.....................................................  r7 = r6
    ...DeeeeeeeeeeeeeeeE-----------------------------------R  r0 = 632, jump 1045
```

Gas simulation at offset 23155 with total cost of 51:

```
    D.....................................................  r8 = r5
    DeER..................................................  r7 = r5 >> 0xd
    D=eER.................................................  r7 = r7 << 0x2
    .DeER.................................................  r9 = 0x100a0
    .D=eER................................................  r7 = r7 + r9
    .D==eeeeeeeeeeeeeeeeeeeeeeeeeER.......................  r7 = i32 [r7 + 0]
    .D===========================eER......................  r7 = r7 + r9
    ..D===========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r7 + 0]
```

Gas simulation at offset 23178 with total cost of 77:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER....................................................  r7 = u64 [r1 + 0x8]
    D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER...........................  r10 = u64 [r7 + 0x240]
    D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER...........................  r7 = u64 [r7 + 0x248]
    DeE-------------------------------------------------R...........................  r9 = 0x17c80
    .D=================================================eeER.........................  r9 = r7 if r10 != 0
    .D===================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  r12 = u64 [r9 + 0x20]
    .DeeE--------------------------------------------------------------------------R  fallthrough
```

Gas simulation at offset 23201 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r7 = u64 [r1 + 0]
    D=========================eER.........................  r7 = r7 + 0x27f
    DeeE------------------------R.........................  r7 = r10 if r10 != 0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r9 = u64 [r1 + 0x10]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r0 = u64 [r1 + 0x28]
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER........................  r5 = u64 [r1 + 0x20]
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0x18]
    ..D========================eE------------------------R  r1 = r1 + 0x30
    ..DeeeeeeeeeeeeeeeeeeeeeeE---------------------------R  jump [r12 + 0]
```

Gas simulation at offset 23227 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r5 = u64 [r1 + 0]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r9 = u64 [r1 + 0x10]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r11 = u64 [r1 + 0x8]
    .DeE-----------------------R  r12 = r8 >> 0x5
    .DeE-----------------------R  r10 = 0x201
    .D=eE----------------------R  jump 23444 if r12 >=u r10
```

Gas simulation at offset 23246 with total cost of 2:

```
    D....  r7 = r6
    DeER.  r6 = r8 & 0x1f
    DeER.  r8 = 0x17
    .DeER  jump 23362 if r8 <u r6
```

Gas simulation at offset 23257 with total cost of 50:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..........  unlikely
    D....................................................  r12 = r9
    DeE---------------------------------------R..........  r6 = r6 << 0x2
    DeE---------------------------------------R..........  r9 = 0x100c0
    .DeE--------------------------------------R..........  r6 = r6 + r9
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeE-------------R..........  r8 = i32 [r6 + 0]
    .D==========================eE------------R..........  r8 = r8 + r9
    .D===========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r8 + 0]
```

Gas simulation at offset 23278 with total cost of 75:

```
    DeER..........................................................................  r7 = r12 & 0xf
    DeER..........................................................................  r8 = r12 << 0x3b
    .DeER.........................................................................  r9 = r12 << 0x3a
    .DeER.........................................................................  r10 = r12 >> 0x6
    ..DeER........................................................................  r8 = r8 >> 0x3f
    ..DeER........................................................................  r9 = r9 >> 0x3f
    ..D=eeeeeeeeeeeeeeeeeeeeeeeeeER...............................................  u8 [r11 + 0] = a1
    ..D=eeeeeeeeeeeeeeeeeeeeeeeeeER...............................................  u8 [r11 + 0x1] = a2
    ...DeeeeeeeeeeeeeeeeeeeeeeeeeER...............................................  u8 [r11 + 0x3] = a0
    ...DeeeeeeeeeeeeeeeeeeeeeeeeeER...............................................  u8 [r11 + 0xa] = a2
    ...D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  u8 [r11 + 0x11] = a3
    ...D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r0 = u64 [r1 + 0x28]
    ....D========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r5 = u64 [r1 + 0x20]
    ....D========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r6 = u64 [r1 + 0x18]
    ....D=================================================eER.....................  r1 = r1 + 0x30
    ....D=================================================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 23324 with total cost of 77:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER....................................................  r7 = u64 [r1 + 0x8]
    D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER...........................  r10 = u64 [r7 + 0x240]
    D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER...........................  r7 = u64 [r7 + 0x248]
    DeE-------------------------------------------------R...........................  r9 = 0x17c80
    .D=================================================eeER.........................  r9 = r7 if r10 != 0
    .D===================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  r12 = u64 [r9 + 0x30]
    .DeeeeeeeeeeeeeeeE-------------------------------------------------------------R  jump 23201
```

Gas simulation at offset 23349 with total cost of 50:

```
    DeER.................................................  r7 = r8 & 0x7ff
    D=eER................................................  r7 = r7 + r6
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r8 = u64 [r1 + 0x10]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0] = a1
    .DeeE-----------------------------------------------R  fallthrough
```

Gas simulation at offset 23362 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r0 = u64 [r1 + 0x28]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r5 = u64 [r1 + 0x20]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r6 = u64 [r1 + 0x18]
    DeE------------------------R......................  r1 = r1 + 0x30
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 23376 with total cost of 51:

```
    D.....................................................  r5 = r6
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r9 = u64 [r1 + 0x8]
    DeE------------------------R..........................  r6 = r8 & 0x7
    .DeE-----------------------R..........................  r6 = r6 << 0x2
    .DeE-----------------------R..........................  r7 = 0x10120
    .D=eE----------------------R..........................  r6 = r6 + r7
    .D==eeeeeeeeeeeeeeeeeeeeeeeeeER.......................  r8 = i32 [r6 + 0]
    ..D==========================eER......................  r7 = r7 + r8
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE--R......................  r8 = u64 [r1 + 0x10]
    ..D===========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r7 + 0]
```

Gas simulation at offset 23405 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................  r7 = u16 [r9 + 0x20a]
    D=========================eER..........................  r7 = r7 & 0x73ff
    DeE-------------------------R..........................  r10 = r8 & 0x3
    .DeE------------------------R..........................  r10 = r10 << 0xa
    .D=========================eER.........................  r7 = r7 | r10
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r9 + 0x20a] = r7
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R  u8 [r9 + 0x225] = a1
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r0 = u64 [r1 + 0x28]
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r5 = u64 [r1 + 0x20]
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R  r6 = u64 [r1 + 0x18]
    ..D=========================eE------------------------R  r1 = r1 + 0x30
    ...D========================eeeeeeeeeeeeeeeeeeeeeeE---R  jump [r0 + 0]
```

Gas simulation at offset 23444 with total cost of 74:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r6 = u64 [r11 + 0x240]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..................................  r7 = u64 [r11 + 0x248]
    DeE---------------------------------------R..................................  r10 = 0x17c80
    .D========================eeE-------------R..................................  r10 = r7 if r6 != 0
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r12 = u64 [r10 + 0x40]
    ..DeE-------------------------------------------------R......................  r7 = r5 + 0x27f
    ..D=======================eeE-------------------------R......................  r7 = r6 if r6 != 0
    ...DeeeeeeeeeeeeeeeeeeeeeeeeeE------------------------R......................  r0 = u64 [r1 + 0x28]
    ...DeeeeeeeeeeeeeeeeeeeeeeeeeE------------------------R......................  r5 = u64 [r1 + 0x20]
    ...D========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r6 = u64 [r1 + 0x18]
    ...D=========================eE-----------------------R......................  r1 = r1 + 0x30
    ....D================================================eeeeeeeeeeeeeeeeeeeeeeER  jump [r12 + 0]
```

Gas simulation at offset 23485 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER............................  r7 = u8 [r9 + 0x223]
    D=========================eER...........................  r5 = r5 + r7
    D==========================eER..........................  r7 = r7 + 0x1
    .D==========================eER.........................  r10 = r5 + 0x7ff
    .D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r10 + 0xa1] = a1
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R  u8 [r9 + 0x223] = a0
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R  r0 = u64 [r1 + 0x28]
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R  r5 = u64 [r1 + 0x20]
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R  r6 = u64 [r1 + 0x18]
    ..D=========================eE-------------------------R  r1 = r1 + 0x30
    ...D========================eeeeeeeeeeeeeeeeeeeeeeE----R  jump [r0 + 0]
```

Gas simulation at offset 23521 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  u8 [r9 + 0x226] = a1
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r0 = u64 [r1 + 0x28]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r5 = u64 [r1 + 0x20]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r6 = u64 [r1 + 0x18]
    .D========================eER.....................  r1 = r1 + 0x30
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 23539 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  u8 [r9 + 0x223] = a1
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r0 = u64 [r1 + 0x28]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r5 = u64 [r1 + 0x20]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r6 = u64 [r1 + 0x18]
    .D========================eER.....................  r1 = r1 + 0x30
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 23557 with total cost of 25:

```
    D...........................  r7 = r5
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r0 = u64 [r1 + 0x28]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r5 = u64 [r1 + 0x20]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0x18]
    .DeE-----------------------R  r1 = r1 + 0x30
    .DeeeeeeeeeeeeeeeE---------R  jump 6712
```

Gas simulation at offset 23574 with total cost of 25:

```
    D...........................  r7 = r5
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r0 = u64 [r1 + 0x28]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r5 = u64 [r1 + 0x20]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0x18]
    .DeE-----------------------R  r1 = r1 + 0x30
    .DeeeeeeeeeeeeeeeE---------R  jump 6864
```

Gas simulation at offset 23591 with total cost of 26:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r7 = u8 [r9 + 0x239]
    D=========================eER  jump 23635 if r7 == 0
```

Gas simulation at offset 23598 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  r7 = u8 [r9 + 0x20b]
    D=========================eE--------------R............  r7 = r7 << 0x8
    D==========================eE-------------R............  r7 = r7 | r8
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r9 + 0x208] = r7
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r9 + 0x20a] = r7
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R  u8 [r9 + 569] = 0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R  r0 = u64 [r1 + 0x28]
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r5 = u64 [r1 + 0x20]
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R  r6 = u64 [r1 + 0x18]
    ..D========================eE-------------------------R  r1 = r1 + 0x30
    ..D========================eeeeeeeeeeeeeeeeeeeeeeE----R  jump [r0 + 0]
```

Gas simulation at offset 23635 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeE---------------------------------------R...........  r7 = r8 & 0x3f
    DeE---------------------------------------R...........  r8 = 0x1
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R...........  u8 [r9 + 0x20b] = a0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R...........  u8 [r9 + 0x239] = a1
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R...........  r0 = u64 [r1 + 0x28]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R...........  r5 = u64 [r1 + 0x20]
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0x18]
    ..D========================eE------------------------R  r1 = r1 + 0x30
    ..D========================eeeeeeeeeeeeeeeeeeeeeeE---R  jump [r0 + 0]
```

Gas simulation at offset 23664 with total cost of 51:

```
    DeER..................................................  r7 = r12 << 0x8
    DeER..................................................  r8 = 0x1
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u16 [r11 + 0x274] = r7
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u8 [r11 + 0x277] = a1
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r0 = u64 [r1 + 0x28]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r5 = u64 [r1 + 0x20]
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0x18]
    ..D========================eE------------------------R  r1 = r1 + 0x30
    ..D========================eeeeeeeeeeeeeeeeeeeeeeE---R  jump [r0 + 0]
```

Gas simulation at offset 23692 with total cost of 28:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...  r7 = i32 [r11 + 0x250]
    DeE------------------------R...  r8 = r12 >> 0x7
    .DeE-----------------------R...  r9 = r12 << 0x39
    .D=eE----------------------R...  r9 = r9 >> 0x3f
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER..  u8 [r11 + 0x96] = a1
    ..D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r11 + 0x97] = a2
    ..D=eE------------------------R  jump 23730 if r9 == 0
```

Gas simulation at offset 23716 with total cost of 50:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........  r9 = u8 [r11 + 0x8e]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........  u8 [r11 + 152] = 0
    D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r11 + 0x26f] = a2
    .DeeE-----------------------------------------------R  fallthrough
```

Gas simulation at offset 23730 with total cost of 50:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..........  unlikely
    DeE---------------------------------------R..........  r7 = r7 & 0x1
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........  u8 [r11 + 0x92] = a1
    D=eeeeeeeeeeeeeeeeeeeeeeeeeE--------------R..........  u8 [r11 + 0x93] = a0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R..........  r0 = u64 [r1 + 0x28]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R..........  r5 = u64 [r1 + 0x20]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0x18]
    .D=========================eE-----------------------R  r1 = r1 + 0x30
    ..D========================eeeeeeeeeeeeeeeeeeeeeeE--R  jump [r0 + 0]
```

Gas simulation at offset 23756 with total cost of 26:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r7 = u8 [r11 + 0x3d]
    D=========================eER  jump 23780 if r7 == 0
```

Gas simulation at offset 23762 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeE---------------------------------------R............  r7 = r12 >> 0x3
    DeE---------------------------------------R............  r8 = 0x17290
    .DeE--------------------------------------R............  r7 = r7 + r8
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeE-------------R............  r7 = u8 [r7 + 0]
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r11 + 0x3e] = a0
    .DeeE-------------------------------------------------R  fallthrough
```

Gas simulation at offset 23780 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.......  unlikely
    DeE---------------------------------------R.......  r7 = 0x1
    D=eeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......  u8 [r11 + 0x32] = a0
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r0 = u64 [r1 + 0x28]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......  r5 = u64 [r1 + 0x20]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......  r6 = u64 [r1 + 0x18]
    .D========================eE--------------R.......  r1 = r1 + 0x30
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 23801 with total cost of 26:

```
    DeER.........................  r7 = r5 + 0x71
    D............................  r8 = r12
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r0 = u64 [r1 + 0x28]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER  r5 = u64 [r1 + 0x20]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0x18]
    .DeE------------------------R  r1 = r1 + 0x30
    .DeeeeeeeeeeeeeeeE----------R  jump 207
```

Gas simulation at offset 23821 with total cost of 53:

```
    DeER....................................................  r7 = r12 & 0xf
    DeER....................................................  r8 = 0x172b0
    D=eER...................................................  r7 = r7 << 0x1
    .D=eER..................................................  r7 = r7 + r8
    .D==eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r7 = i16 [r7 + 0]
    .DeE--------------------------R.........................  r8 = r12 >> 0x7
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r11 + 0x36] = r7
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R  u8 [r11 + 0x3f] = a1
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R  r0 = u64 [r1 + 0x28]
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R  r5 = u64 [r1 + 0x20]
    ...D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R  r6 = u64 [r1 + 0x18]
    ...D========================eE-------------------------R  r1 = r1 + 0x30
    ...D========================eeeeeeeeeeeeeeeeeeeeeeE----R  jump [r0 + 0]
```

Gas simulation at offset 23860 with total cost of 25:

```
    D...........................  r8 = r12
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r0 = u64 [r1 + 0x28]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r5 = u64 [r1 + 0x20]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0x18]
    .DeE-----------------------R  r1 = r1 + 0x30
    .DeeeeeeeeeeeeeeeE---------R  jump 263
```

Gas simulation at offset 23877 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  u8 [r11 + 0x6] = a5
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r0 = u64 [r1 + 0x28]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r5 = u64 [r1 + 0x20]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r6 = u64 [r1 + 0x18]
    .D========================eER.....................  r1 = r1 + 0x30
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 23894 with total cost of 78:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.....................................................  r8 = u8 [r11 + 0x2b]
    DeE------------------------R.....................................................  r9 = r12 >> 0x7
    .DeE-----------------------R.....................................................  r10 = r12 << 0x3c
    .D=eE----------------------R.....................................................  r10 = r10 >> 0x3f
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER....................................................  u8 [r11 + 0x25] = a2
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeER...................................................  u8 [r11 + 38] = 0x1
    ..D=eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  u8 [r11 + 0x27] = a3
    ..D=======================eeeeeeeeeeeeeeeeeeeeeeeeeER............................  u8 [r11 + 0x2a] = a1
    ...D=======================eE-----------------------R............................  r7 = r12 << 0x39
    ...D========================eE----------------------R............................  r8 = r12 & 0x7
    ....D=======================eE----------------------R............................  r7 = r7 >> 0x3d
    ....D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u8 [r11 + 0x2c] = a0
    ....D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u8 [r11 + 0x2d] = a1
    ....D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r0 = u64 [r1 + 0x28]
    .....D=============================================eeeeeeeeeeeeeeeeeeeeeeeeeER...  r5 = u64 [r1 + 0x20]
    .....D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0x18]
    .....D================================================eE------------------------R  r1 = r1 + 0x30
    .....D================================================eeeeeeeeeeeeeeeeeeeeeeE---R  jump [r0 + 0]
```

Gas simulation at offset 23948 with total cost of 74:

```
    DeER.........................................................................  r7 = r12 << 0x3a
    DeER.........................................................................  r8 = r12 & 0xf
    .DeER........................................................................  r9 = r12 << 0x3b
    .DeER........................................................................  r7 = r7 >> 0x3f
    .D=eER.......................................................................  r9 = r9 >> 0x3f
    ..D=eeeeeeeeeeeeeeeeeeeeeeeeeER..............................................  u8 [r11 + 0x30] = a2
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-R..............................................  u8 [r11 + 0x31] = a0
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-R..............................................  u8 [r11 + 0x33] = a1
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-R..............................................  u8 [r11 + 0x3c] = a0
    ...D========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r0 = u64 [r1 + 0x28]
    ...D========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r5 = u64 [r1 + 0x20]
    ...D========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r6 = u64 [r1 + 0x18]
    ...D=========================eE-----------------------R......................  r1 = r1 + 0x30
    ....D================================================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 23989 with total cost of 78:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.....................................................  r8 = u8 [r11 + 0x13]
    DeE------------------------R.....................................................  r9 = r12 >> 0x7
    .DeE-----------------------R.....................................................  r10 = r12 << 0x3c
    .D=eE----------------------R.....................................................  r10 = r10 >> 0x3f
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER....................................................  u8 [r11 + 0xd] = a2
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeER...................................................  u8 [r11 + 14] = 0x1
    ..D=eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  u8 [r11 + 0xf] = a3
    ..D=======================eeeeeeeeeeeeeeeeeeeeeeeeeER............................  u8 [r11 + 0x12] = a1
    ...D=======================eE-----------------------R............................  r7 = r12 << 0x39
    ...D========================eE----------------------R............................  r8 = r12 & 0x7
    ....D=======================eE----------------------R............................  r7 = r7 >> 0x3d
    ....D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u8 [r11 + 0x14] = a0
    ....D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u8 [r11 + 0x15] = a1
    ....D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r0 = u64 [r1 + 0x28]
    .....D=============================================eeeeeeeeeeeeeeeeeeeeeeeeeER...  r5 = u64 [r1 + 0x20]
    .....D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0x18]
    .....D================================================eE------------------------R  r1 = r1 + 0x30
    .....D================================================eeeeeeeeeeeeeeeeeeeeeeE---R  jump [r0 + 0]
```

Gas simulation at offset 24043 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  u8 [r11 + 0x1e] = a5
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r0 = u64 [r1 + 0x28]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r5 = u64 [r1 + 0x20]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r6 = u64 [r1 + 0x18]
    .D========================eER.....................  r1 = r1 + 0x30
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 24060 with total cost of 26:

```
    DeER.........................  r7 = r5 + 0x19
    D............................  r8 = r12
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r0 = u64 [r1 + 0x28]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER  r5 = u64 [r1 + 0x20]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0x18]
    .DeE------------------------R  r1 = r1 + 0x30
    .DeeeeeeeeeeeeeeeE----------R  jump 0
```

Gas simulation at offset 24080 with total cost of 55:

```
    DeER......................................................  r7 = r12 & 0xf
    DeER......................................................  r8 = 0x17270
    D=eER.....................................................  r7 = r7 << 0x1
    .D=eER....................................................  r7 = r7 + r8
    .D==eeeeeeeeeeeeeeeeeeeeeeeeeER...........................  r7 = u16 [r7 + 0]
    .DeE--------------------------R...........................  r8 = r12 >> 0x7
    ..DeE-------------------------R...........................  r9 = r12 << 0x39
    ..D=eE------------------------R...........................  r9 = r9 >> 0x3f
    ..D==========================eER..........................  r7 = r7 >> 0x1
    ...D==========================eER.........................  r7 = r7 + 0xffffffffffffffff
    ...D===========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r11 + 0x7e] = r7
    ...DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------------------R  u8 [r11 + 0x8b] = a1
    ...D=eeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R  u8 [r11 + 0x8c] = a2
    ....DeE--------------------------------------------------R  jump 23362 if r8 != 0
```

Gas simulation at offset 24126 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.......  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  u8 [r11 + 142] = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r0 = u64 [r1 + 0x28]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r5 = u64 [r1 + 0x20]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......  r6 = u64 [r1 + 0x18]
    .D========================eE--------------R.......  r1 = r1 + 0x30
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 24145 with total cost of 47:

```
    DeER..............................................  r7 = r12 & 0x7f
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.....................  u8 [r11 + 0x91] = a0
    DeeeeeeeeeeeeeeeeeeeeeeeeeE-R.....................  r0 = u64 [r1 + 0x28]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER.....................  r5 = u64 [r1 + 0x20]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER.....................  r6 = u64 [r1 + 0x18]
    .D========================eER.....................  r1 = r1 + 0x30
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 24166 with total cost of 26:

```
    D............................  r7 = r11
    D............................  r8 = r12
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r0 = u64 [r1 + 0x28]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r5 = u64 [r1 + 0x20]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0x18]
    .DeE------------------------R  r1 = r1 + 0x30
    .DeeeeeeeeeeeeeeeE----------R  jump 0
```

Gas simulation at offset 24185 with total cost of 75:

```
    DeER..........................................................................  r7 = r12 & 0xf
    DeER..........................................................................  r8 = r12 << 0x3b
    .DeER.........................................................................  r9 = r12 << 0x3a
    .DeER.........................................................................  r10 = r12 >> 0x6
    ..DeER........................................................................  r8 = r8 >> 0x3f
    ..DeER........................................................................  r9 = r9 >> 0x3f
    ..D=eeeeeeeeeeeeeeeeeeeeeeeeeER...............................................  u8 [r11 + 0x18] = a1
    ..D=eeeeeeeeeeeeeeeeeeeeeeeeeER...............................................  u8 [r11 + 0x19] = a2
    ...DeeeeeeeeeeeeeeeeeeeeeeeeeER...............................................  u8 [r11 + 0x1b] = a0
    ...DeeeeeeeeeeeeeeeeeeeeeeeeeER...............................................  u8 [r11 + 0x22] = a2
    ...D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  u8 [r11 + 0x29] = a3
    ...D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r0 = u64 [r1 + 0x28]
    ....D========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r5 = u64 [r1 + 0x20]
    ....D========================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r6 = u64 [r1 + 0x18]
    ....D=================================================eER.....................  r1 = r1 + 0x30
    ....D=================================================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 24232 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  u8 [r11 + 0x70] = a5
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r0 = u64 [r1 + 0x28]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r5 = u64 [r1 + 0x20]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r6 = u64 [r1 + 0x18]
    .D========================eER.....................  r1 = r1 + 0x30
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 24249 with total cost of 51:

```
    DeER..................................................  r7 = r12 >> 0x7
    DeER..................................................  r8 = r12 & 0x7f
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u8 [r11 + 0x75] = a1
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u8 [r11 + 0x77] = a0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r0 = u64 [r1 + 0x28]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r5 = u64 [r1 + 0x20]
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0x18]
    ..D========================eE------------------------R  r1 = r1 + 0x30
    ..D========================eeeeeeeeeeeeeeeeeeeeeeE---R  jump [r0 + 0]
```

Gas simulation at offset 24275 with total cost of 48:

```
    DeER...............................................  r7 = r12 << 0x4
    D=eER..............................................  r7 = r7 + 0x1
    D==eeeeeeeeeeeeeeeeeeeeeeeeeER.....................  u16 [r11 + 0x82] = r7
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-R.....................  r0 = u64 [r1 + 0x28]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-R.....................  r5 = u64 [r1 + 0x20]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-R.....................  r6 = u64 [r1 + 0x18]
    .D=========================eER.....................  r1 = r1 + 0x30
    ..D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 24299 with total cost of 48:

```
    DeER...............................................  r7 = r12 | 0x300
    D=eER..............................................  r7 = r7 << 0x6
    D==eeeeeeeeeeeeeeeeeeeeeeeeeER.....................  u16 [r11 + 0x80] = r7
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-R.....................  r0 = u64 [r1 + 0x28]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-R.....................  r5 = u64 [r1 + 0x20]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-R.....................  r6 = u64 [r1 + 0x18]
    .D=========================eER.....................  r1 = r1 + 0x30
    ..D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 24324 with total cost of 26:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r7 = u8 [r11 + 0x283]
    D=========================eER  jump 24395 if r7 == 0
```

Gas simulation at offset 24331 with total cost of 59:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...................  r7 = u8 [r11 + 0x27e]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...................  r8 = u8 [r11 + 0x27f]
    .D========================eeeE------------R...................  r9 = r7 <u 0xc0
    ..D=======================eE--------------R...................  r10 = r7 & 0x3f
    ..D==========================eeE----------R...................  r10 = r7 if r9 != 0
    ...D======================eeeE------------R...................  r7 = r8 <u 0xc0
    ....D=====================eE--------------R...................  r9 = r8 & 0x3f
    ....D========================eeE----------R...................  r9 = r8 if r7 != 0
    .....D=========================eE---------R...................  r7 = r10 & 0x30
    .....D=========================eE---------R...................  r8 = r10 & 0xcf
    ......D=========================eE--------R...................  r7 = r7 + 0xffffffffffffffd0
    ......D==========================eeE------R...................  r8 = r10 if r7 != 0
    .......D=======================eE---------R...................  r7 = r9 & 0x30
    .......D=======================eE---------R...................  r10 = r9 & 0xcf
    ........D=======================eE--------R...................  r7 = r7 + 0xffffffffffffffd0
    ........D========================eeE------R...................  r10 = r9 if r7 != 0
    ........D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r11 + 0x280] = a1
    .........D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r11 + 0x281] = a3
    .........DeeE------------------------------------------------R  fallthrough
```

Gas simulation at offset 24395 with total cost of 47:

```
    DeER..............................................  r7 = r12 & 0x1
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.....................  u8 [r11 + 0x283] = a0
    DeeeeeeeeeeeeeeeeeeeeeeeeeE-R.....................  r0 = u64 [r1 + 0x28]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER.....................  r5 = u64 [r1 + 0x20]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER.....................  r6 = u64 [r1 + 0x18]
    .D========================eER.....................  r1 = r1 + 0x30
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 24416 with total cost of 27:

```
    DeER..........................  r1 = r1 + 0xfffffffffffffff0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.  u64 [r1 + 0x8] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.  u64 [r1 + 0] = r5
    .DeE------------------------R.  r5 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = u16 [r5 + 0x269]
    .DeeeeeeeeeeeeeeeE-----------R  r0 = 706, jump 22578
```

Gas simulation at offset 24438 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r8 = u8 [r5 + 0x265]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r9 = i16 [r5 + 0x269]
    DeE------------------------R..........................  r7 = r7 << 0x8
    D=========================eER.........................  r7 = r7 | r8
    .D========================eER.........................  r9 = r9 + 0x1
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x263] = r7
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r5 + 0x269] = r9
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r0 = u64 [r1 + 0x8]
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE------------------------R  r5 = u64 [r1 + 0]
    ..D========================eE------------------------R  r1 = r1 + 0x10
    ..D========================eeeeeeeeeeeeeeeeeeeeeeE---R  jump [r0 + 0]
```

Gas simulation at offset 24473 with total cost of 80:

```
    DeER...............................................................................  r8 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER......................................................  r9 = u8 [r8 + 0x267]
    D==========================eER.....................................................  r9 = r9 << 0x3b
    .D==========================eER....................................................  r9 = r9 >> 0x3e
    .D===========================eER...................................................  r7 = r7 + r9
    .D============================eER..................................................  r7 = r7 + 0x7ff
    .D=============================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r7 = u8 [r7 + 0x26b]
    ..D=====================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r8 + 0x265] = a0
    ..DeeeeeeeeeeeeeeeeeeeeeeE--------------------------------------------------------R  jump [r0 + 0]
```

Gas simulation at offset 24504 with total cost of 60:

```
    DeER...........................................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..................................  r8 = u8 [r7 + 0x26b]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..................................  r9 = u8 [r7 + 0x26f]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..................................  r10 = u8 [r7 + 0x265]
    .D=========================eER.................................  r11 = r9 & 0x1
    .D=========================eER.................................  r12 = r10 + r8
    ..D========================eER.................................  r2 = r9 & 0x3c
    ..D========================eER.................................  r10 = r10 ^ r8
    ..D=========================eER................................  r11 = r11 + r12
    ...D========================eeeER..............................  r3 = r10 <u 0x80
    ....D========================eE-R..............................  r12 = r11 & 0xff
    ....D========================eE-R..............................  r9 = r11 & 0x80
    .....D=======================eeeER.............................  r10 = r11 <u 0x100
    .....D========================eE-R.............................  r8 = r8 ^ r11
    ......D=======================eeeER............................  r12 = r12 <u 0x1
    ......D=========================eER............................  r10 = r10 ^ 0x1
    .......D=======================eE-R............................  r8 = r8 << 0x38
    .......D=======================eE-R............................  r9 = r9 | r2
    .......D=========================eER...........................  r12 = r12 << 0x1
    .......D========================eE-R...........................  r8 = r8 >> 0x3f
    ........D========================eER...........................  r9 = r9 | r10
    ........D========================eER...........................  r8 = r3 & r8
    ........D=========================eER..........................  r9 = r9 | r12
    ........D=========================eER..........................  r8 = r8 << 0x6
    .........D=========================eER.........................  r8 = r8 | r9
    .........D======================eeeeeeeeeeeeeeeeeeeeeeeeeER....  u8 [r7 + 0x26b] = a4
    .........D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x26f] = a1
    .........DeE--------------------------------------------------R  r7 = 0
    ..........DeeeeeeeeeeeeeeeeeeeeeeE----------------------------R  jump [r0 + 0]
```

Gas simulation at offset 24599 with total cost of 57:

```
    DeER........................................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...............................  r8 = u8 [r7 + 0x265]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...............................  r9 = u8 [r7 + 0x26b]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...............................  r10 = u8 [r7 + 0x26f]
    .D=========================eER..............................  r8 = r8 & r9
    .D=========================eER..............................  r9 = r10 & 0x7d
    ..D=========================eER.............................  r10 = r8 & 0x80
    ..D==========================eER............................  r9 = r9 | r10
    ...D========================eeeER...........................  r10 = r8 <u 0x1
    ...D===========================eER..........................  r10 = r10 << 0x1
    ....D===========================eER.........................  r9 = r9 | r10
    ....D=======================eeeeeeeeeeeeeeeeeeeeeeeeeER.....  u8 [r7 + 0x26b] = a1
    ....D============================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x26f] = a2
    ....DeE----------------------------------------------------R  r7 = 0
    .....DeeeeeeeeeeeeeeeeeeeeeeE------------------------------R  jump [r0 + 0]
```

Gas simulation at offset 24649 with total cost of 52:

```
    DeER...................................................  r1 = r1 + 0xffffffffffffffd8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u64 [r1 + 0x20] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u64 [r1 + 0x18] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u64 [r1 + 0x10] = r6
    .DeE------------------------R..........................  r6 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r8 = u8 [r6 + 0x267]
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  r10 = u8 [r6 + 0x265]
    ..D=========================eE-----------------------R.  r9 = r8 & 0x7
    ..DeE------------------------------------------------R.  r3 = 0x7
    ...D================================================eER  r5 = r10 << 0x1
    ...D=========================eE-----------------------R  jump 24718 if r9 == r3
```

Gas simulation at offset 24685 with total cost of 26:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r8 = u16 [r6 + 0x263]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  u64 [r1 + 0x8] = r7
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r7 = u64 [r1 + 0x8]
    D............................  r9 = r10
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0] = r10
    .DeeeeeeeeeeeeeeeE----------R  r0 = 716, jump 23116
```

Gas simulation at offset 24705 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r10 = u64 [r1 + 0]
    DeE------------------------R  r3 = 0x7
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u64 [r1 + 0x8]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = u8 [r6 + 0x267]
    .DeeE----------------------R  fallthrough
```

Gas simulation at offset 24718 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r2 = u8 [r6 + 0x26f]
    DeE---------------------------------------R.............  r10 = r10 >> 0x7
    .DeE--------------------------------------R.............  r11 = r5 & 0x80
    .DeE--------------------------------------R.............  r9 = r5 & 0xff
    ..DeeeE-----------------------------------R.............  r12 = r9 <u 0x1
    ..DeE-------------------------------------R.............  r11 = r11 | r10
    ...D==eE----------------------------------R.............  r12 = r12 << 0x1
    ...D======================eE--------------R.............  r10 = r2 & 0x7c
    ...D=======================eE-------------R.............  r10 = r10 | r11
    ....D=======================eE------------R.............  r10 = r10 | r12
    ....DeE-----------------------------------R.............  r8 = r8 & 0x7
    ....D========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x26f] = a3
    ....D=eE-----------------------------------------------R  jump 24784 if r8 != 7
```

Gas simulation at offset 24763 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.......  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  u8 [r6 + 0x26b] = s0
    DeE---------------------------------------R.......  r7 = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r0 = u64 [r1 + 0x20]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......  r5 = u64 [r1 + 0x18]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......  r6 = u64 [r1 + 0x10]
    .D========================eE--------------R.......  r1 = r1 + 0x28
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 24784 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = u16 [r6 + 0x263]
    DeeeeeeeeeeeeeeeE----------R  r0 = 718, jump 23116
```

Gas simulation at offset 24794 with total cost of 47:

```
    DeER..............................................  r7 = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r0 = u64 [r1 + 0x20]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r5 = u64 [r1 + 0x18]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r6 = u64 [r1 + 0x10]
    .DeE-----------------------R......................  r1 = r1 + 0x28
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 24810 with total cost of 59:

```
    DeER..........................................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.................................  r8 = u8 [r7 + 0x26b]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.................................  r9 = u8 [r7 + 0x26c]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.................................  r10 = u8 [r7 + 0x26f]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER.................................  r11 = u8 [r7 + 0x265]
    .D=========================eER................................  r8 = r8 & r9
    .D=========================eER................................  r9 = r10 & 0x7c
    ..D=========================eER...............................  r8 = r8 - r11
    ..D==========================eeeER............................  r10 = r8 <u 0x100
    ...D=========================eE--R............................  r11 = r8 & 0xff
    ...D=========================eE--R............................  r12 = r8 & 0x80
    ....D=========================eeeER...........................  r11 = r11 <u 0x1
    ....D===========================eER...........................  r9 = r9 | r10
    .....D===========================eER..........................  r11 = r11 << 0x1
    .....D===========================eER..........................  r9 = r9 | r12
    .....D============================eER.........................  r9 = r9 | r11
    .....D=======================eeeeeeeeeeeeeeeeeeeeeeeeeER......  u8 [r7 + 0x26c] = a1
    ......D============================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x26f] = a2
    ......DeE----------------------------------------------------R  r7 = 0
    ......DeeeeeeeeeeeeeeeeeeeeeeE-------------------------------R  jump [r0 + 0]
```

Gas simulation at offset 24878 with total cost of 57:

```
    DeER........................................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...............................  r8 = u8 [r7 + 0x265]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...............................  r9 = u8 [r7 + 0x26b]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...............................  r10 = u8 [r7 + 0x26f]
    .D=========================eER..............................  r9 = r9 & r8
    .D=========================eER..............................  r10 = r10 & 0x3d
    .D=========================eER..............................  r8 = r8 & 0xc0
    ..D=========================eeeER...........................  r9 = r9 <u 0x1
    ..D============================eER..........................  r9 = r9 << 0x1
    ...D========================eE---R..........................  r8 = r8 | r10
    ...D============================eER.........................  r8 = r8 | r9
    ...D=============================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x26f] = a1
    ...DeE-----------------------------------------------------R  r7 = 0
    ....DeeeeeeeeeeeeeeeeeeeeeeE-------------------------------R  jump [r0 + 0]
```

Gas simulation at offset 24924 with total cost of 53:

```
    DeER....................................................  r1 = r1 + 0xffffffffffffffd8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...........................  u64 [r1 + 0x20] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...........................  u64 [r1 + 0x18] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...........................  u64 [r1 + 0x10] = r6
    .D......................................................  r5 = r7
    .DeE------------------------R...........................  r6 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r7 = u8 [r6 + 0x26f]
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u8 [r6 + 0x26e]
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..  r9 = u8 [r6 + 0x26a]
    ..D=========================eE-----------------------R..  r7 = r7 | 0x10
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x26f] = a0
    ...D================================================eE-R  r8 = r8 | 0x100
    ...D....................................................  r7 = r5
    ...DeeeeeeeeeeeeeeeE-----------------------------------R  r0 = 726, jump 23116
```

Gas simulation at offset 24973 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r7 = u8 [r6 + 0x26e]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r9 = u8 [r6 + 0x269]
    D=========================eER.........................  r7 = r7 + 0xffffffffffffffff
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x26e] = a0
    .D=========================eE------------------------R  r7 = r7 & 0xff
    .D==========================eE-----------------------R  r8 = r7 | 0x100
    .D....................................................  r7 = r5
    ..DeeeeeeeeeeeeeeeE----------------------------------R  r0 = 728, jump 23116
```

Gas simulation at offset 25004 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................  r7 = u8 [r6 + 0x26e]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................  r9 = u8 [r6 + 0x26f]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................  r11 = u8 [r6 + 0x271]
    D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0] = r11
    .DeE------------------------------------------------R..  r10 = 0xfffb
    .D========================eeE-----------------------R..  r10 = 0xffff if r11 == 0
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x8] = r10
    ..D=======================eE--------------------------R  r7 = r7 + 0xffffffffffffffff
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-R  u8 [r6 + 0x26e] = a0
    ..D========================eE-------------------------R  r7 = r7 & 0xff
    ...D========================eE------------------------R  r8 = r7 | 0x100
    ...D...................................................  r7 = r5
    ...DeeeeeeeeeeeeeeeE----------------------------------R  r0 = 730, jump 23116
```

Gas simulation at offset 25054 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r7 = u8 [r6 + 0x26e]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r8 = u8 [r6 + 0x26f]
    D=========================eER.........................  r7 = r7 + 0xffffffffffffffff
    D=========================eER.........................  r8 = r8 | 0x4
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x26e] = a0
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x26f] = a1
    .DeE-------------------------------------------------R  r8 = 0xfffa
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r9 = u64 [r1 + 0]
    ..D========================eeE-----------------------R  r8 = 0xfffe if r9 == 0
    ..D...................................................  r7 = r5
    ...DeeeeeeeeeeeeeeeE---------------------------------R  r0 = 732, jump 22578
```

Gas simulation at offset 25096 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x269] = a0
    D...........................  r7 = r5
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = u64 [r1 + 0x8]
    DeeeeeeeeeeeeeeeE----------R  r0 = 734, jump 22578
```

Gas simulation at offset 25111 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  u8 [r6 + 0x26a] = a0
    DeE------------------------R......................  r7 = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r0 = u64 [r1 + 0x20]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r5 = u64 [r1 + 0x18]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER.....................  r6 = u64 [r1 + 0x10]
    .D========================eER.....................  r1 = r1 + 0x28
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 25131 with total cost of 57:

```
    DeER........................................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...............................  r8 = u8 [r7 + 0x265]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...............................  r9 = u8 [r7 + 0x26b]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...............................  r10 = u8 [r7 + 0x26f]
    .D=========================eER..............................  r8 = r8 ^ r9
    .D=========================eER..............................  r9 = r10 & 0x7d
    ..D=========================eER.............................  r10 = r8 & 0x80
    ..D==========================eER............................  r9 = r9 | r10
    ...D========================eeeER...........................  r10 = r8 <u 0x1
    ...D===========================eER..........................  r10 = r10 << 0x1
    ....D===========================eER.........................  r9 = r9 | r10
    ....D=======================eeeeeeeeeeeeeeeeeeeeeeeeeER.....  u8 [r7 + 0x26b] = a1
    ....D============================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x26f] = a2
    ....DeE----------------------------------------------------R  r7 = 0
    .....DeeeeeeeeeeeeeeeeeeeeeeE------------------------------R  jump [r0 + 0]
```

Gas simulation at offset 25181 with total cost of 76:

```
    DeER...........................................................................  r1 = r1 + 0xffffffffffffffd8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  u64 [r1 + 0x20] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  u64 [r1 + 0x18] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  u64 [r1 + 0x10] = r6
    .D.............................................................................  r5 = r7
    .DeE------------------------R..................................................  r6 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER.................................................  r7 = u8 [r6 + 0x26e]
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r8 = u8 [r6 + 0x265]
    ..D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x8] = r8
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r8 = u16 [r6 + 0x269]
    ..D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0] = r8
    ...D========================eE------------------------------------------------R  r8 = r7 | 0x100
    ...D...........................................................................  r7 = r5
    ...DeeeeeeeeeeeeeeeE----------------------------------------------------------R  r0 = 740, jump 22578
```

Gas simulation at offset 25228 with total cost of 26:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r7 = u8 [r6 + 0x26e]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r9 = u8 [r6 + 0x26a]
    D=========================eER  r8 = r7 | 0x100
    .D...........................  r7 = r5
    .DeeeeeeeeeeeeeeeE----------R  r0 = 742, jump 23116
```

Gas simulation at offset 25248 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r7 = u8 [r6 + 0x26e]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r9 = u8 [r6 + 0x269]
    D=========================eER.........................  r7 = r7 + 0xffffffffffffffff
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x26e] = a0
    .D=========================eE------------------------R  r7 = r7 & 0xff
    .D==========================eE-----------------------R  r8 = r7 | 0x100
    .D....................................................  r7 = r5
    ..DeeeeeeeeeeeeeeeE----------------------------------R  r0 = 744, jump 23116
```

Gas simulation at offset 25279 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r7 = u8 [r6 + 0x26e]
    D=========================eER.........................  r7 = r7 + 0xffffffffffffffff
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x26e] = a0
    D.....................................................  r7 = r5
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r8 = u64 [r1 + 0]
    .DeeeeeeeeeeeeeeeE-----------------------------------R  r0 = 746, jump 22578
```

Gas simulation at offset 25300 with total cost of 51:

```
    DeER..................................................  r7 = r7 << 0x8
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r8 = u64 [r1 + 0x8]
    D=========================eER.........................  r7 = r7 | r8
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r6 + 0x269] = r7
    .DeE-------------------------------------------------R  r7 = 0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r0 = u64 [r1 + 0x20]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r5 = u64 [r1 + 0x18]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r6 = u64 [r1 + 0x10]
    ..D========================eE------------------------R  r1 = r1 + 0x28
    ..D========================eeeeeeeeeeeeeeeeeeeeeeE---R  jump [r0 + 0]
```

Gas simulation at offset 25329 with total cost of 51:

```
    DeER..................................................  r1 = r1 + 0xffffffffffffffe0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u64 [r1 + 0x18] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u64 [r1 + 0x10] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u64 [r1 + 0x8] = r6
    .DeE------------------------R.........................  r6 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER........................  r8 = u8 [r6 + 0x267]
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  r5 = u8 [r6 + 0x265]
    ..D=========================eE-----------------------R  r9 = r8 & 0x7
    ..DeE------------------------------------------------R  r11 = 0x7
    ..D==========================eE----------------------R  jump 25388 if r9 == r11
```

Gas simulation at offset 25362 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = u16 [r6 + 0x263]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0] = r7
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u64 [r1 + 0]
    D...........................  r9 = r5
    .DeeeeeeeeeeeeeeeE---------R  r0 = 750, jump 23116
```

Gas simulation at offset 25378 with total cost of 25:

```
    DeER........................  r11 = 0x7
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u64 [r1 + 0]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = u8 [r6 + 0x267]
    DeeE-----------------------R  fallthrough
```

Gas simulation at offset 25388 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.............  unlikely
    DeE---------------------------------------R.............  r9 = r5 >> 0x1
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.............  r10 = u8 [r6 + 0x26f]
    .DeE--------------------------------------R.............  r2 = r5 & 0x1
    ..DeeeE-----------------------------------R.............  r12 = r5 <u 0x2
    ..D===eE----------------------------------R.............  r12 = r12 << 0x1
    ...D======================eE--------------R.............  r10 = r10 & 0x7c
    ...D=======================eE-------------R.............  r10 = r2 | r10
    ...D========================eE------------R.............  r10 = r10 | r12
    ...DeE------------------------------------R.............  r8 = r8 & 0x7
    ....D========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x26f] = a3
    ....DeE------------------------------------------------R  jump 25446 if r8 != 7
```

Gas simulation at offset 25425 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.......  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  u8 [r6 + 0x26b] = a2
    DeE---------------------------------------R.......  r7 = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r0 = u64 [r1 + 0x18]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......  r5 = u64 [r1 + 0x10]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......  r6 = u64 [r1 + 0x8]
    .D========================eE--------------R.......  r1 = r1 + 0x20
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 25446 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = u16 [r6 + 0x263]
    DeeeeeeeeeeeeeeeE----------R  r0 = 752, jump 23116
```

Gas simulation at offset 25456 with total cost of 47:

```
    DeER..............................................  r7 = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r0 = u64 [r1 + 0x18]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r5 = u64 [r1 + 0x10]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r6 = u64 [r1 + 0x8]
    .DeE-----------------------R......................  r1 = r1 + 0x20
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 25472 with total cost of 22:

```
    DeER.....................  r7 = 0
    DeeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 25476 with total cost of 57:

```
    DeER........................................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...............................  r8 = u8 [r7 + 0x265]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...............................  r9 = u8 [r7 + 0x26b]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...............................  r10 = u8 [r7 + 0x26f]
    .D=========================eER..............................  r8 = r8 | r9
    .D=========================eER..............................  r9 = r10 & 0x7d
    ..D=========================eER.............................  r10 = r8 & 0x80
    ..D==========================eER............................  r9 = r9 | r10
    ...D========================eeeER...........................  r10 = r8 <u 0x1
    ...D===========================eER..........................  r10 = r10 << 0x1
    ....D===========================eER.........................  r9 = r9 | r10
    ....D=======================eeeeeeeeeeeeeeeeeeeeeeeeeER.....  u8 [r7 + 0x26b] = a1
    ....D============================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x26f] = a2
    ....DeE----------------------------------------------------R  r7 = 0
    .....DeeeeeeeeeeeeeeeeeeeeeeE------------------------------R  jump [r0 + 0]
```

Gas simulation at offset 25526 with total cost of 28:

```
    DeER...........................  r1 = r1 + 0xfffffffffffffff0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0x8] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0] = r5
    .DeE------------------------R..  r5 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER.  r8 = u8 [r5 + 0x26e]
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER.  r9 = u8 [r5 + 0x26b]
    ..D=========================eER  r8 = r8 | 0x100
    ..DeeeeeeeeeeeeeeeE-----------R  r0 = 760, jump 23116
```

Gas simulation at offset 25556 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r7 = u8 [r5 + 0x26e]
    D=========================eER.........................  r7 = r7 + 0xffffffffffffffff
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x26e] = a0
    DeE--------------------------------------------------R  r7 = 0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r0 = u64 [r1 + 0x8]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r5 = u64 [r1 + 0]
    .DeE-------------------------------------------------R  r1 = r1 + 0x10
    .D=========================eeeeeeeeeeeeeeeeeeeeeeE---R  jump [r0 + 0]
```

Gas simulation at offset 25579 with total cost of 53:

```
    DeER....................................................  r1 = r1 + 0xfffffffffffffff0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...........................  u64 [r1 + 0x8] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...........................  u64 [r1 + 0] = r5
    .DeE------------------------R...........................  r5 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r8 = u8 [r5 + 0x26f]
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r10 = u8 [r5 + 0x26e]
    ..D=========================eER.........................  r9 = r8 | 0x10
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x26f] = a2
    ...D========================eE-------------------------R  r8 = r10 | 0x100
    ...DeeeeeeeeeeeeeeeE-----------------------------------R  r0 = 764, jump 23116
```

Gas simulation at offset 25616 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r7 = u8 [r5 + 0x26e]
    D=========================eER.........................  r7 = r7 + 0xffffffffffffffff
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r5 + 0x26e] = a0
    DeE--------------------------------------------------R  r7 = 0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r0 = u64 [r1 + 0x8]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r5 = u64 [r1 + 0]
    .DeE-------------------------------------------------R  r1 = r1 + 0x10
    .D=========================eeeeeeeeeeeeeeeeeeeeeeE---R  jump [r0 + 0]
```

Gas simulation at offset 25639 with total cost of 28:

```
    DeER...........................  r1 = r1 + 0xffffffffffffffe8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0x10] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0x8] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0] = r6
    .D.............................  r5 = r7
    .DeE------------------------R..  r6 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER.  r7 = u8 [r6 + 0x26e]
    ..D=========================eER  r8 = r7 | 0x100
    ..D............................  r7 = r5
    ..DeeeeeeeeeeeeeeeE-----------R  r0 = 768, jump 22578
```

Gas simulation at offset 25672 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r7 = u8 [r6 + 0x26e]
    D=========================eER.........................  r7 = r7 + 0x1
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x26e] = a0
    D==========================eE------------------------R  r7 = r7 & 0xff
    .D==========================eE-----------------------R  r8 = r7 | 0x100
    .D....................................................  r7 = r5
    .DeeeeeeeeeeeeeeeE-----------------------------------R  r0 = 770, jump 22578
```

Gas simulation at offset 25699 with total cost of 53:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER............................  r8 = u8 [r6 + 0x26f]
    DeE------------------------R............................  r9 = r7 & 0x80
    D=========================eER...........................  r8 = r8 & 0x7d
    .D=========================eER..........................  r8 = r8 | r9
    .DeE-------------------------R..........................  r9 = r7 & 0xff
    ..DeeeE----------------------R..........................  r9 = r9 <u 0x1
    ..D===eE---------------------R..........................  r9 = r9 << 0x1
    ...D========================eER.........................  r8 = r8 | r9
    ...DeeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u8 [r6 + 0x26b] = a0
    ...D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x26f] = a1
    ...DeE-------------------------------------------------R  r7 = 0
    ....DeeeeeeeeeeeeeeeeeeeeeeeeeE------------------------R  r0 = u64 [r1 + 0x10]
    ....D==eeeeeeeeeeeeeeeeeeeeeeeeeE----------------------R  r5 = u64 [r1 + 0x8]
    ....D========================eeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0]
    ....D=========================eE-----------------------R  r1 = r1 + 0x18
    .....D========================eeeeeeeeeeeeeeeeeeeeeeE--R  jump [r0 + 0]
```

Gas simulation at offset 25749 with total cost of 28:

```
    DeER...........................  r1 = r1 + 0xffffffffffffffe8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0x10] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0x8] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0] = r6
    .D.............................  r5 = r7
    .DeE------------------------R..  r6 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER.  r7 = u8 [r6 + 0x26e]
    ..D=========================eER  r8 = r7 | 0x100
    ..D............................  r7 = r5
    ..DeeeeeeeeeeeeeeeE-----------R  r0 = 774, jump 22578
```

Gas simulation at offset 25782 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r7 = u8 [r6 + 0x26e]
    D=========================eER.........................  r7 = r7 + 0x1
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x26e] = a0
    D==========================eE------------------------R  r7 = r7 & 0xff
    .D==========================eE-----------------------R  r8 = r7 | 0x100
    .D....................................................  r7 = r5
    .DeeeeeeeeeeeeeeeE-----------------------------------R  r0 = 776, jump 22578
```

Gas simulation at offset 25809 with total cost of 47:

```
    DeER..............................................  r7 = r7 | 0x20
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.....................  u8 [r6 + 0x26f] = a0
    DeE-------------------------R.....................  r7 = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeE-R.....................  r0 = u64 [r1 + 0x10]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER.....................  r5 = u64 [r1 + 0x8]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER.....................  r6 = u64 [r1 + 0]
    .D========================eER.....................  r1 = r1 + 0x18
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 25831 with total cost of 53:

```
    DeER....................................................  r1 = r1 + 0xffffffffffffffd0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...........................  u64 [r1 + 0x28] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...........................  u64 [r1 + 0x20] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...........................  u64 [r1 + 0x18] = r6
    .DeE------------------------R...........................  r6 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r9 = u8 [r6 + 0x26f]
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u8 [r6 + 0x267]
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..  r5 = u8 [r6 + 0x265]
    ..D=========================eE-----------------------R..  r11 = r9 & 0x1
    ...D================================================eER.  r10 = r8 & 0x7
    ...DeE------------------------------------------------R.  r2 = 0x7
    ....D===============================================eER.  r12 = r5 << 0x1
    ....D================================================eER  jump 25918 if r10 == r2
```

Gas simulation at offset 25874 with total cost of 50:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........  r8 = u16 [r6 + 0x263]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........  u64 [r1 + 0x10] = r7
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........  r7 = u64 [r1 + 0x10]
    .D...................................................  r9 = r5
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R..........  u64 [r1 + 0x8] = r12
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0] = r11
    .DeeeeeeeeeeeeeeeE----------------------------------R  r0 = 780, jump 23116
```

Gas simulation at offset 25898 with total cost of 50:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r11 = u64 [r1 + 0]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r12 = u64 [r1 + 0x8]
    DeE------------------------R.........................  r2 = 0x7
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r7 = u64 [r1 + 0x10]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER........................  r8 = u8 [r6 + 0x267]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER  r9 = u8 [r6 + 0x26f]
    .DeeE-----------------------------------------------R  fallthrough
```

Gas simulation at offset 25918 with total cost of 32:

```
    DeER...............................  r10 = r11 | r12
    DeER...............................  r11 = r9 & 0x7c
    .DeER..............................  r5 = r5 >> 0x7
    .DeER..............................  r12 = r12 & 0x80
    .DeER..............................  r9 = r10 & 0xff
    ..DeER.............................  r12 = r12 | r5
    ..DeeeER...........................  r5 = r9 <u 0x1
    ...DeE-R...........................  r11 = r11 | r12
    ...D==eER..........................  r5 = r5 << 0x1
    ...D===eER.........................  r11 = r11 | r5
    ...DeE---R.........................  r8 = r8 & 0x7
    ....D===eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x26f] = a4
    ....DeE---------------------------R  jump 25982 if r8 != 7
```

Gas simulation at offset 25961 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.......  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  u8 [r6 + 0x26b] = a3
    DeE---------------------------------------R.......  r7 = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r0 = u64 [r1 + 0x28]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......  r5 = u64 [r1 + 0x20]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......  r6 = u64 [r1 + 0x18]
    .D========================eE--------------R.......  r1 = r1 + 0x30
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 25982 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = u16 [r6 + 0x263]
    DeeeeeeeeeeeeeeeE----------R  r0 = 782, jump 23116
```

Gas simulation at offset 25992 with total cost of 47:

```
    DeER..............................................  r7 = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r0 = u64 [r1 + 0x28]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r5 = u64 [r1 + 0x20]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r6 = u64 [r1 + 0x18]
    .DeE-----------------------R......................  r1 = r1 + 0x30
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 26008 with total cost of 72:

```
    DeER.......................................................................  r1 = r1 + 0xffffffffffffffd8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..............................................  u64 [r1 + 0x20] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..............................................  u64 [r1 + 0x18] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..............................................  u64 [r1 + 0x10] = r6
    .DeE------------------------R..............................................  r6 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER.............................................  r5 = u8 [r6 + 0x265]
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER.....................  r9 = u8 [r6 + 0x26f]
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.....................  r8 = u8 [r6 + 0x267]
    ..D=========================eE-----------------------R.....................  r10 = r5 >> 0x1
    ...D================================================eER....................  r11 = r9 << 0x7
    ...D================================================eER....................  r12 = r8 & 0x7
    ....DeE-----------------------------------------------R....................  r3 = 0x7
    ....D================================================eER...................  r11 = r11 | r10
    ....D================================================eeeeeeeeeeeeeeeeeeeeER  jump 26091 if r12 == r3
```

Gas simulation at offset 26054 with total cost of 26:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r8 = u16 [r6 + 0x263]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  u64 [r1 + 0x8] = r7
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r7 = u64 [r1 + 0x8]
    D............................  r9 = r5
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0] = r11
    .DeeeeeeeeeeeeeeeE----------R  r0 = 786, jump 23116
```

Gas simulation at offset 26074 with total cost of 26:

```
    DeER.........................  r3 = 0x7
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r11 = u64 [r1 + 0]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r7 = u64 [r1 + 0x8]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r8 = u8 [r6 + 0x267]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER  r9 = u8 [r6 + 0x26f]
    .DeeE-----------------------R  fallthrough
```

Gas simulation at offset 26091 with total cost of 32:

```
    DeER...............................  r2 = r9 & 0x7c
    DeER...............................  r5 = r5 & 0x1
    .DeER..............................  r10 = r11 & 0x80
    .DeER..............................  r9 = r11 & 0xff
    ..DeeeER...........................  r12 = r9 <u 0x1
    ..DeE--R...........................  r10 = r10 | r5
    ...D==eER..........................  r12 = r12 << 0x1
    ...DeE--R..........................  r10 = r10 | r2
    ...D===eER.........................  r10 = r10 | r12
    ...DeE---R.........................  r8 = r8 & 0x7
    ....D===eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x26f] = a3
    ....DeE---------------------------R  jump 26152 if r8 != 7
```

Gas simulation at offset 26131 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.......  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  u8 [r6 + 0x26b] = a4
    DeE---------------------------------------R.......  r7 = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r0 = u64 [r1 + 0x20]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......  r5 = u64 [r1 + 0x18]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......  r6 = u64 [r1 + 0x10]
    .D========================eE--------------R.......  r1 = r1 + 0x28
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 26152 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = u16 [r6 + 0x263]
    DeeeeeeeeeeeeeeeE----------R  r0 = 788, jump 23116
```

Gas simulation at offset 26162 with total cost of 47:

```
    DeER..............................................  r7 = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r0 = u64 [r1 + 0x20]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r5 = u64 [r1 + 0x18]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r6 = u64 [r1 + 0x10]
    .DeE-----------------------R......................  r1 = r1 + 0x28
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 26178 with total cost of 28:

```
    DeER...........................  r1 = r1 + 0xffffffffffffffe8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0x10] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0x8] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0] = r6
    .D.............................  r5 = r7
    .DeE------------------------R..  r6 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER.  r7 = u8 [r6 + 0x26e]
    ..D=========================eER  r8 = r7 | 0x100
    ..D............................  r7 = r5
    ..DeeeeeeeeeeeeeeeE-----------R  r0 = 792, jump 22578
```

Gas simulation at offset 26211 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r7 = u8 [r6 + 0x26e]
    D=========================eER.........................  r7 = r7 + 0x1
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x26e] = a0
    D==========================eE------------------------R  r7 = r7 & 0xff
    .D==========================eE-----------------------R  r8 = r7 | 0x100
    .D....................................................  r7 = r5
    .DeeeeeeeeeeeeeeeE-----------------------------------R  r0 = 794, jump 22578
```

Gas simulation at offset 26238 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r8 = u8 [r6 + 0x26e]
    DeE------------------------R..........................  r7 = r7 | 0x20
    D=========================eER.........................  r8 = r8 + 0x1
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x26e] = a1
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  u8 [r6 + 0x26f] = a0
    .D=========================eE------------------------R  r7 = r8 & 0xff
    ..D=========================eE-----------------------R  r8 = r7 | 0x100
    ..D...................................................  r7 = r5
    ..DeeeeeeeeeeeeeeeE----------------------------------R  r0 = 796, jump 22578
```

Gas simulation at offset 26272 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r8 = u8 [r6 + 0x26e]
    D=========================eER.........................  r8 = r8 + 0x1
    DeeeeeeeeeeeeeeeeeeeeeeeeeE-R.........................  u8 [r6 + 0x269] = a0
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x26e] = a1
    .D=========================eE------------------------R  r7 = r8 & 0xff
    .D==========================eE-----------------------R  r8 = r7 | 0x100
    ..D...................................................  r7 = r5
    ..DeeeeeeeeeeeeeeeE----------------------------------R  r0 = 798, jump 22578
```

Gas simulation at offset 26303 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  u8 [r6 + 0x26a] = a0
    DeE------------------------R......................  r7 = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r0 = u64 [r1 + 0x10]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r5 = u64 [r1 + 0x8]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER.....................  r6 = u64 [r1 + 0]
    .D========================eER.....................  r1 = r1 + 0x18
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 26322 with total cost of 28:

```
    DeER...........................  r1 = r1 + 0xffffffffffffffe8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0x10] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0x8] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0] = r6
    .D.............................  r5 = r7
    .DeE------------------------R..  r6 = r7 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER.  r7 = u8 [r6 + 0x26e]
    ..D=========================eER  r8 = r7 | 0x100
    ..D............................  r7 = r5
    ..DeeeeeeeeeeeeeeeE-----------R  r0 = 802, jump 22578
```

Gas simulation at offset 26355 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r7 = u8 [r6 + 0x26e]
    D=========================eER.........................  r7 = r7 + 0x1
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x26e] = a0
    D==========================eE------------------------R  r7 = r7 & 0xff
    .D==========================eE-----------------------R  r8 = r7 | 0x100
    .D....................................................  r7 = r5
    .DeeeeeeeeeeeeeeeE-----------------------------------R  r0 = 804, jump 22578
```

Gas simulation at offset 26382 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r8 = u8 [r6 + 0x26e]
    D=========================eER.........................  r8 = r8 + 0x1
    DeeeeeeeeeeeeeeeeeeeeeeeeeE-R.........................  u8 [r6 + 0x269] = a0
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x26e] = a1
    .D=========================eE------------------------R  r7 = r8 & 0xff
    .D==========================eE-----------------------R  r8 = r7 | 0x100
    ..D...................................................  r7 = r5
    ..DeeeeeeeeeeeeeeeE----------------------------------R  r0 = 806, jump 22578
```

Gas simulation at offset 26413 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x26a] = a0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = u16 [r6 + 0x269]
    D...........................  r7 = r5
    DeeeeeeeeeeeeeeeE----------R  r0 = 808, jump 22578
```

Gas simulation at offset 26429 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r7 = i16 [r6 + 0x269]
    D=========================eER.........................  r7 = r7 + 0x1
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r6 + 0x269] = r7
    DeE--------------------------------------------------R  r7 = 0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r0 = u64 [r1 + 0x10]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r5 = u64 [r1 + 0x8]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r6 = u64 [r1 + 0]
    .D=========================eE------------------------R  r1 = r1 + 0x18
    ..D========================eeeeeeeeeeeeeeeeeeeeeeE---R  jump [r0 + 0]
```

Gas simulation at offset 26455 with total cost of 61:

```
    DeER............................................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...................................  r8 = u8 [r7 + 0x26b]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...................................  r9 = u8 [r7 + 0x26f]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...................................  r10 = u8 [r7 + 0x265]
    .D=========================eER..................................  r11 = r9 & 0x1
    .D=========================eER..................................  r12 = r8 - r10
    ..D========================eER..................................  r9 = r9 & 0x3c
    ..D========================eER..................................  r10 = r10 ^ r8
    ..D=========================eER.................................  r11 = r11 + r12
    ...D========================eeeER...............................  r2 = r10 <u 0x80
    ...D=========================eE-R...............................  r11 = r11 + 0xffffffffffffffff
    ....D=========================eER...............................  r12 = r11 & 0xff
    ....D=========================eER...............................  r10 = r11 & 0x80
    .....D========================eER...............................  r8 = r8 ^ r11
    .....D=========================eER..............................  r9 = r9 | r10
    ......D========================eeeER............................  r10 = r11 <u 0x100
    .......D=======================eeeER............................  r12 = r12 <u 0x1
    .......D=======================eE--R............................  r8 = r8 << 0x38
    ........D=========================eER...........................  r12 = r12 << 0x1
    ........D=======================eE--R...........................  r8 = r8 >> 0x3f
    ........D=========================eER...........................  r9 = r9 | r10
    .........D=======================eeER...........................  r8 = r8 & ~r2
    .........D=========================eER..........................  r9 = r9 | r12
    ..........D========================eER..........................  r8 = r8 << 0x6
    ..........D=========================eER.........................  r8 = r8 | r9
    ..........D=====================eeeeeeeeeeeeeeeeeeeeeeeeeER.....  u8 [r7 + 0x26b] = a4
    ..........D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x26f] = a1
    ...........DeE-------------------------------------------------R  r7 = 0
    ...........DeeeeeeeeeeeeeeeeeeeeeeE----------------------------R  jump [r0 + 0]
```

Gas simulation at offset 26550 with total cost of 51:

```
    DeER..................................................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r8 = u8 [r7 + 0x26c]
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0x26e] = a1
    DeE--------------------------------------------------R  r7 = 0
    .DeeeeeeeeeeeeeeeeeeeeeeE----------------------------R  jump [r0 + 0]
```

Gas simulation at offset 26566 with total cost of 29:

```
    DeER............................  r7 = r7 + 0x7ff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  r8 = u8 [r7 + 0x266]
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...  r7 = u16 [r7 + 0x269]
    D==========================eER..  r8 = r8 << 0x20
    .D=========================eER..  r7 = r7 << 0x10
    .D==========================eER.  r7 = r7 | r8
    .D===========================eER  r7 = r7 + 0x1
    .DeeeeeeeeeeeeeeeeeeeeeeE------R  jump [r0 + 0]
```

Gas simulation at offset 26592 with total cost of 72:

```
    DeER.......................................................................  r1 = r1 + 0xffffffffffffffb8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..............................................  u64 [r1 + 0x40] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..............................................  u64 [r1 + 0x38] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..............................................  u64 [r1 + 0x30] = r6
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER..............................................  u64 [r1 + 0x28] = r8
    .DeE------------------------R..............................................  r6 = 0x30a98
    .D=========================eER.............................................  r8 = r6 + 0x2000
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER....................  r8 = u64 [r8 + 0x600]
    ..D==================================================eeeeeeeeeeeeeeeeeeeeER  jump 27287 if r8 == 0
```

Gas simulation at offset 26624 with total cost of 22:

```
    DeeER....................  i32 r8 = r7 >> 0x19
    D==eeeeeeeeeeeeeeeeeeeeER  jump 26967 if r8 != 0
```

Gas simulation at offset 26631 with total cost of 2:

```
    DeeER  i32 r3 = r7 + 0x1
    D....  r8 = r7
    .D...  r10 = r7
    .DeER  jump 26679 if r7 <=u 126
```

Gas simulation at offset 26642 with total cost of 12:

```
    DeER...........  i32 r8 = clz r3
    .DeeeER........  i32 r9 = 0x18 - r8
    ..DeE-R........  r8 = r8 << 0x7
    ...D=eeER......  i32 r11 = r3 >> r9
    ....DeeER......  i32 r9 = 0xffffffffffffffff << r9
    .....D=eER.....  r10 = r11 & 0x7f
    ......DeeER....  r9 = r3 & ~r9
    .......D=eeeER.  r9 = r9 >u 0
    .......DeE---R.  r10 = r10 - r8
    ........DeE--R.  r8 = r10 + 0x7ff
    ........D=eE-R.  r10 = r8 + 0x480
    .........D==eER  r8 = r10 + r9
    .........DeeE-R  fallthrough
```

Gas simulation at offset 26679 with total cost of 49:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.........  unlikely
    DeE---------------------------------------R.........  r12 = 0x2000
    D=eE--------------------------------------R.........  r9 = r6 + r12
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeE-------------R.........  r11 = u64 [r9 + 0x738]
    .DeeE-------------------------------------R.........  i32 r2 = r8 >> 0x6
    ..D=========================eE------------R.........  r5 = r11 >> r2
    ..D==========================eE-----------R.........  r5 = r5 & 0x1
    ...D==========================eeeeeeeeeeeeeeeeeeeeER  jump 26736 if r5 == 0
```

Gas simulation at offset 26703 with total cost of 48:

```
    DeER...............................................  r9 = r2 << 0x3
    DeER...............................................  r12 = r6 + 0x2000
    .DeER..............................................  r9 = r9 + r12
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER.....................  r9 = u64 [r9 + 0x608]
    .DeE-------------------------R.....................  r12 = 0xffffffffffffffff
    ..DeE------------------------R.....................  r8 = r12 << r8
    ..D=========================eER....................  r8 = r8 & r9
    ...D=========================eeeeeeeeeeeeeeeeeeeeER  jump 26736 if r8 == 0
```

Gas simulation at offset 26729 with total cost of 15:

```
    DeeER.............  r9 = ctz r8
    D==eeER...........  r12 = r9 if r8 != 0
    DeeeeeeeeeeeeeeeER  jump 26774
```

Gas simulation at offset 26736 with total cost of 23:

```
    DeER......................  r8 = r2 + 0x1
    DeER......................  r2 = 0xffffffffffffffff
    .DeER.....................  r8 = r2 << r8
    .D=eER....................  r8 = r8 & r11
    ..D=eeeeeeeeeeeeeeeeeeeeER  jump 26909 if r8 == 0
```

Gas simulation at offset 26752 with total cost of 33:

```
    DeeER...............................  r9 = ctz r8
    D==eeER.............................  r2 = r9 if r8 != 0
    .D===eER............................  r8 = r2 << 0x3
    .DeE---R............................  r9 = r6 + 0x2000
    ..D===eER...........................  r8 = r8 + r9
    ..D====eeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u64 [r8 + 0x608]
    ..D=============================eeER  r12 = ctz r8
    ..DeeE-----------------------------R  fallthrough
```

Gas simulation at offset 26774 with total cost of 57:

```
    DeER........................................................  r8 = r2 << 0x6
    D=eER.......................................................  r8 = r8 | r12
    D==eER......................................................  r8 = r8 << 0x20
    .D==eER.....................................................  r8 = r8 >> 0x1e
    .D===eER....................................................  r9 = r6 + r8
    .D====eeeeeeeeeeeeeeeeeeeeeeeeeER...........................  r10 = u32 [r9 + 0]
    ..D============================eeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u32 [r10 + 0x4]
    ..D=====================================================eER.  r8 = r8 >> 0x1
    ..D======================================================eER  jump 26967 if r7 >=u r8
```

Gas simulation at offset 26801 with total cost of 75:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...................................  u64 [r1 + 0] = r9
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...................................  u64 [r1 + 0x10] = r3
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...................................  u64 [r1 + 0x18] = r6
    .DeE--------------------------------------R...................................  r9 = r6 + 0x2000
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeE-------------R...................................  r6 = i32 [r9 + 0x600]
    ..D=======================eE--------------R...................................  r11 = r7 ^ 0xffffffffffffffff
    ..D========================eeE------------R...................................  i32 r8 = r8 + r11
    ...D======================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r0 = i32 [r9 + 0x748]
    ...D========================eeE---------------------R.........................  i32 r5 = r10 - r6
    ....D=========================eeE-------------------R.........................  i32 r4 = r5 >> 0x5
    ....D===========================eE------------------R.........................  r4 = r4 + 0x1
    .....D===========================eE-----------------R.........................  r11 = r7 + r4
    .....D=======================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  u64 [r1 + 0x20] = r8
    ......D======================eeeE----------------------R......................  r9 = r8 >u 0
    .......D==========================eeE------------------R......................  i32 r3 = r11 + r9
    .......D===========================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x8] = r0
    ........D==========================================eeeeeeeeeeeeeeeeeeeeE-----R  jump 26874 if r0 >=u r3
```

Gas simulation at offset 26854 with total cost of 2:

```
    DeER.  r9 = 0x4001
    D=eER  jump 26967 if r3 >=u r9
```

Gas simulation at offset 26861 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r8 = u64 [r1 + 0x18]
    D=========================eE--------------R...........  r9 = r8 + 0x2000
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r9 + 0x748] = r3
    .DeeE------------------------------------------------R  fallthrough
```

Gas simulation at offset 26874 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r11 = u32 [r10 + 0x8]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r9 = i32 [r10 + 0]
    DeE------------------------R..........................  r8 = r5 & 0xffffffffffffffe0
    .DeE-----------------------R..........................  r10 = r8 + r6
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r8 = u64 [r1 + 0]
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r8 + 0] = r11
    ..D...................................................  r5 = r9
    ..D=======================eE-------------------------R  jump 26985 if r11 == 0
```

Gas simulation at offset 26894 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r11 + 12] = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r0 = u64 [r1 + 0x10]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r12 = u64 [r1 + 0x8]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0x18]
    .DeeeeeeeeeeeeeeeE---------R  jump 27045
```

Gas simulation at offset 26909 with total cost of 24:

```
    DeeER......................  i32 r2 = r10 >> 0x6
    .D=eER.....................  r8 = r11 >> r2
    .D==eER....................  r8 = r8 & 0x1
    ..D==eeeeeeeeeeeeeeeeeeeeER  jump 26951 if r8 == 0
```

Gas simulation at offset 26921 with total cost of 48:

```
    DeER...............................................  r8 = r2 << 0x3
    DeER...............................................  r9 = r6 + 0x2000
    .DeER..............................................  r8 = r8 + r9
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER.....................  r8 = u64 [r8 + 0x608]
    .DeE-------------------------R.....................  r9 = r10 & 0x3f
    ..DeE------------------------R.....................  r12 = 0xffffffffffffffff
    ..D=eE-----------------------R.....................  r9 = r12 << r9
    ...D========================eER....................  r8 = r8 & r9
    ...D=========================eeeeeeeeeeeeeeeeeeeeER  jump 26729 if r8 != 0
```

Gas simulation at offset 26951 with total cost of 23:

```
    DeER......................  r8 = r2 + 0x1
    DeER......................  r2 = 0xffffffffffffffff
    .DeER.....................  r8 = r2 << r8
    .D=eER....................  r8 = r8 & r11
    ..D=eeeeeeeeeeeeeeeeeeeeER  jump 26752 if r8 != 0
```

Gas simulation at offset 26967 with total cost of 2:

```
    DeER.  r7 = 0
    DeeER  fallthrough
```

Gas simulation at offset 26970 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.......  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r0 = u64 [r1 + 0x40]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r5 = u64 [r1 + 0x38]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r6 = u64 [r1 + 0x30]
    .DeE--------------------------------------R.......  r1 = r1 + 0x48
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 26985 with total cost of 78:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER......................................  unlikely
    DeE---------------------------------------R......................................  r9 = r2 << 0x3
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R......................................  r6 = u64 [r1 + 0x18]
    .D========================eE--------------R......................................  r11 = r6 + 0x2000
    .D=========================eE-------------R......................................  r9 = r9 + r11
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r11 = u64 [r9 + 0x608]
    ..DeE-------------------------------------------------R..........................  r3 = 0xfffffffffffffffe
    ..D=eE------------------------------------------------R..........................  r12 = r3 <<r r12
    ...D=================================================eER.........................  r11 = r11 & r12
    ...D==================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r9 + 0x608] = r11
    ...DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------------------------------R  r0 = u64 [r1 + 0x10]
    ...DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------------------------------R  r12 = u64 [r1 + 0x8]
    ....D=================================================eE------------------------R  jump 27045 if r11 != 0
```

Gas simulation at offset 27025 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeE---------------------------------------R............  r8 = r6 + 0x2000
    D=eeeeeeeeeeeeeeeeeeeeeeeeeE--------------R............  r9 = u64 [r8 + 0x738]
    .DeE--------------------------------------R............  r11 = r3 <<r r2
    .D=========================eE-------------R............  r9 = r9 & r11
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r8 + 0x738] = r9
    ..DeeE------------------------------------------------R  fallthrough
```

Gas simulation at offset 27045 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeE-------------------------------------R  r2 = r4 <u r12
    .DeE--------------------------------------R  r8 = r0 << 0x1
    .DeE--------------------------------------R  r11 = r10 << 0x20
    ..DeE-------------------------------------R  r3 = r10 + 0x20
    ...DeeE-----------------------------------R  i32 r9 = r7 << 0x5
    ...DeE------------------------------------R  r8 = r8 + 0x1
    ....DeE-----------------------------------R  r11 = r11 >> 0x20
    ....D=eeeeeeeeeeeeeeeeeeeeeeeeeE----------R  u32 [r11 + 0] = r5
    ....D=eeeeeeeeeeeeeeeeeeeeeeeeeE----------R  u32 [r11 + 0x4] = r8
    .....DeE----------------------------------R  r12 = r3 + r9
    .....DeeeeeeeeeeeeeeeeeeeeeeeeeE----------R  r5 = u64 [r1 + 0x20]
    .....D=========================eE---------R  jump 27222 if r5 == 0
```

Gas simulation at offset 27082 with total cost of 1:

```
    D...  r8 = r5
    DeER  jump 27126 if r5 <=u 127
```

Gas simulation at offset 27088 with total cost of 15:

```
    DeER..............  r7 = 0x2000000
    D=eeeER...........  r7 = minu(r5, r7)
    D====eER..........  i32 r10 = clz r7
    .D====eeeER.......  i32 r8 = 0x18 - r10
    ..D======eeER.....  i32 r7 = r7 >> r8
    ..D========eER....  r7 = r7 & 0x7f
    ...D==eE-----R....  r10 = r10 << 0x7
    ...D========eER...  r7 = r7 - r10
    ...D=========eER..  r7 = r7 + 0x7ff
    ....D=========eER.  r8 = r7 + 0x480
    ....D==========eER  r8 = r8 + 0x1
    ....DeeE---------R  fallthrough
```

Gas simulation at offset 27126 with total cost of 54:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..............  unlikely
    DeeE--------------------------------------R..............  i32 r10 = r8 + 0xffffffffffffffff
    .DeE--------------------------------------R..............  r5 = r5 << 0x1
    .DeE--------------------------------------R..............  r7 = r12 << 0x20
    ..DeE-------------------------------------R..............  r8 = r10 << 0x2
    ..D=eE------------------------------------R..............  r8 = r8 + r6
    ..D==eeeeeeeeeeeeeeeeeeeeeeeeeE-----------R..............  r11 = u32 [r8 + 0]
    ...D=eeeeeeeeeeeeeeeeeeeeeeeeeE-----------R..............  u32 [r8 + 0] = r12
    ...DeeE-----------------------------------R..............  i32 r8 = r10 >> 0x6
    ....DeE-----------------------------------R..............  r4 = r10 & 0x3f
    ....D=eE----------------------------------R..............  r7 = r7 >> 0x20
    ....D==eeeeeeeeeeeeeeeeeeeeeeeeeE---------R..............  u32 [r7 + 0] = r0
    .....D=eeeeeeeeeeeeeeeeeeeeeeeeeE---------R..............  u32 [r7 + 0x4] = r5
    .....D========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r7 + 0x8] = r11
    .....D========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r7 + 12] = 0
    .....D==========================eE----------------------R  jump 27173 if r11 == 0
```

Gas simulation at offset 27169 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r11 + 0xc] = r12
    DeeE-----------------------R  fallthrough
```

Gas simulation at offset 27173 with total cost of 55:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...............  unlikely
    DeE---------------------------------------R...............  r7 = r8 << 0x3
    .DeE--------------------------------------R...............  r11 = r6 + 0x2000
    .D=eE-------------------------------------R...............  r7 = r7 + r11
    .D==eeeeeeeeeeeeeeeeeeeeeeeeeE------------R...............  r11 = u64 [r7 + 0x608]
    ..DeE-------------------------------------R...............  r5 = 0x1 << r4
    ..D==========================eE-----------R...............  r11 = r11 | r5
    ...D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u64 [r7 + 0x608] = r11
    ...DeE--------------------------------------------------R.  r0 = r6 + 0x2000
    ...D=eeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R.  r7 = u64 [r0 + 0x738]
    ....DeE-------------------------------------------------R.  r8 = 0x1 << r8
    ....D=========================eE------------------------R.  r7 = r7 | r8
    .....D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r0 + 0x738] = r7
    .....DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r5 = u64 [r1 + 0x20]
    .....D....................................................  r0 = r5
    .....DeeE------------------------------------------------R  fallthrough
```

Gas simulation at offset 27222 with total cost of 48:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER........  unlikely
    DeE---------------------------------------R........  r7 = r6 + 0x2000
    D=eeeeeeeeeeeeeeeeeeeeeeeeeE--------------R........  r8 = i32 [r7 + 0x600]
    .DeE--------------------------------------R........  r7 = r5 << 0x5
    .D=eeE------------------------------------R........  i32 r7 = r7 + r12
    ..D========================eeE------------R........  i32 r10 = r8 + 0x80000
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------R........  r8 = u64 [r1 + 0x28]
    ...D========================eE------------R........  r8 = r8 & r2
    ...D=========================eeeeeeeeeeeeeeeeeeeeER  jump 27260 if r7 >=u r10
```

Gas simulation at offset 27251 with total cost of 27:

```
    DeER..........................  r7 = r7 << 0x20
    D=eER.........................  r7 = r7 >> 0x20
    D==eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r7 + 0] = r0
    DeeE-------------------------R  fallthrough
```

Gas simulation at offset 27260 with total cost of 2:

```
    DeER.  r7 = r3 << 0x20
    D=eER  r7 = r7 >> 0x20
    DeE-R  jump 26970 if r8 == 0
```

Gas simulation at offset 27270 with total cost of 25:

```
    DeER........................  r8 = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r0 = u64 [r1 + 0x40]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r5 = u64 [r1 + 0x38]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0x30]
    .DeE-----------------------R  r1 = r1 + 0x48
    .DeeeeeeeeeeeeeeeE---------R  jump 28080
```

Gas simulation at offset 27287 with total cost of 15:

```
    D.................  r5 = r7
    DeeeeeeeeeeeeeeeER  r0 = 816, jump 27306
```

Gas simulation at offset 27294 with total cost of 1:

```
    D...  r9 = r7
    D...  r7 = r5
    DeER  jump 26624 if r9 != 0
```

Gas simulation at offset 27302 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeE-------------------------R  jump 26967
```

Gas simulation at offset 27306 with total cost of 28:

```
    DeER...........................  r8 = 0x30a98
    D=eER..........................  r9 = r8 + 0x2000
    D==eeeeeeeeeeeeeeeeeeeeeeeeeER.  r7 = u64 [r9 + 0x740]
    .D==========================eER  jump 27394 if r7 == 0
```

Gas simulation at offset 27322 with total cost of 77:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.....................................  unlikely
    DeE---------------------------------------R.....................................  r2 = 0x1
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.....................................  r11 = u64 [r9 + 0x680]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.....................................  r10 = u64 [r9 + 0x738]
    .DeE--------------------------------------R.....................................  r12 = 0x8000000000000000
    .D========================eE--------------R.....................................  r11 = r11 | r12
    .DeE--------------------------------------R.....................................  r12 = 0x8000
    ..D=======================eE--------------R.....................................  r10 = r10 | r12
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u64 [r9 + 0x738] = r10
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE------------------------R..........................  u32 [r9 + 0x748] = r2
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE------------------------R..........................  u64 [r9 + 0x600] = r7
    ...D=======================eE------------------------R..........................  r8 = r8 + 0x7ff
    ...D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u64 [r9 + 0x680] = r11
    ...D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u32 [r7 + 0] = 0
    ...D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u32 [r7 + 0x4] = r12
    ....D===============================================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u32 [r7 + 8] = 0
    ....D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r7 + 12] = 0
    ....D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r8 + 0x7fd] = r7
    .....D===============================================eeeE----------------------R  r7 = r7 >u 0
    .....DeeeeeeeeeeeeeeeE---------------------------------------------------------R  jump 27294
```

Gas simulation at offset 27394 with total cost of 15:

```
    DeeeER............  r7 = r7 >u 0
    DeeeeeeeeeeeeeeeER  jump 27294
```

Gas simulation at offset 27398 with total cost of 53:

```
    DeER....................................................  r1 = r1 + 0xffffffffffffffe8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...........................  u64 [r1 + 0x10] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...........................  u64 [r1 + 0x8] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER...........................  u64 [r1 + 0] = r6
    .DeE------------------------R...........................  r7 = r7 + 0xffffffffffffffe0
    .DeE------------------------R...........................  r4 = 0x30a98
    .D=eE-----------------------R...........................  r10 = r7 << 0x20
    ..D=eE----------------------R...........................  r8 = r4 + 0x2000
    ..D==eeeeeeeeeeeeeeeeeeeeeeeeeER........................  r9 = u64 [r8 + 0x600]
    ..D========================eE--R........................  r10 = r10 >> 0x20
    ...D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  r8 = u32 [r10 + 0x4]
    ...D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  r3 = i32 [r10 + 0]
    ....D=========================eeE---------------------R.  i32 r10 = r7 - r9
    .....D===============================================eER  r2 = r8 >> 0x1
    .....D==========================eE---------------------R  jump 27647 if r10 <u 32
```

Gas simulation at offset 27447 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeE---------------------------------------R...........  r10 = r3 << 0x5
    .DeeE-------------------------------------R...........  i32 r10 = r7 - r10
    .D==eE------------------------------------R...........  r12 = r10 << 0x20
    ..D==eE-----------------------------------R...........  r12 = r12 >> 0x20
    ..D===eeeeeeeeeeeeeeeeeeeeeeeeeE----------R...........  r0 = u32 [r12 + 0x4]
    ..D============================eE---------R...........  r11 = r0 & 0x1
    ...D============================eeeeeeeeeeeeeeeeeeeeER  jump 27647 if r11 != 0
```

Gas simulation at offset 27470 with total cost of 20:

```
    DeER...................  r8 = r0 >> 0x1
    DeeeeeeeeeeeeeeeeeeeeER  jump 27495 if r0 == 0
```

Gas simulation at offset 27476 with total cost of 20:

```
    DeER...................  r9 = 0x2000000
    D=eeeER................  r9 = minu(r8, r9)
    DeeeeeeeeeeeeeeeeeeeeER  jump 27499 if r0 >=u 256
```

Gas simulation at offset 27490 with total cost of 15:

```
    DeER..............  r9 = r9 + 0xffffffffffffffff
    DeeeeeeeeeeeeeeeER  jump 27525
```

Gas simulation at offset 27495 with total cost of 15:

```
    DeER..............  r9 = 0
    DeeeeeeeeeeeeeeeER  jump 27525
```

Gas simulation at offset 27499 with total cost of 10:

```
    DeER.........  i32 r11 = clz r9
    .DeeeER......  i32 r6 = 0x18 - r11
    ..D==eeER....  i32 r9 = r9 >> r6
    ..D====eER...  r9 = r9 & 0x7f
    ...DeE---R...  r11 = r11 << 0x7
    ...D====eER..  r9 = r9 - r11
    ...D=====eER.  r9 = r9 + 0x7ff
    ...D======eER  r9 = r9 + 0x480
    ....DeeE----R  fallthrough
```

Gas simulation at offset 27525 with total cost of 29:

```
    DeER............................  r11 = r9 << 0x20
    D=eER...........................  r11 = r11 >> 0x1e
    .D=eER..........................  r6 = r4 + r11
    .D==eeeeeeeeeeeeeeeeeeeeeeeeeER.  r11 = i32 [r6 + 0]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--R.  r3 = i32 [r12 + 0]
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-R.  r5 = u32 [r12 + 0x8]
    ..D==========================eER  jump 27554 if r11 != r10
```

Gas simulation at offset 27544 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r6 + 0] = r5
    DeE------------------------R  jump 27569 if r5 == 0
```

Gas simulation at offset 27549 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r5 + 12] = 0
    DeeeeeeeeeeeeeeeE----------R  jump 27629
```

Gas simulation at offset 27554 with total cost of 50:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........  r9 = u32 [r12 + 0xc]
    D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r9 + 0x8] = r5
    DeeeeeeeeeeeeeeeeeeeeE------------------------------R  jump 27629 if r5 == 0
```

Gas simulation at offset 27564 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r5 + 0xc] = r9
    DeeeeeeeeeeeeeeeE----------R  jump 27629
```

Gas simulation at offset 27569 with total cost of 55:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...............  unlikely
    DeeE--------------------------------------R...............  i32 r10 = r9 >> 0x6
    .DeE--------------------------------------R...............  r12 = 0x2000
    .D=eE-------------------------------------R...............  r11 = r10 << 0x3
    ..DeE-------------------------------------R...............  r5 = r4 + r12
    ..D=eE------------------------------------R...............  r11 = r11 + r5
    ..D==eeeeeeeeeeeeeeeeeeeeeeeeeE-----------R...............  r5 = u64 [r11 + 0x608]
    ...DeE------------------------------------R...............  r6 = r9 & 0x3f
    ...DeE------------------------------------R...............  r9 = 0xfffffffffffffffe
    ....DeE-----------------------------------R...............  r6 = r9 <<r r6
    ....D=========================eE----------R...............  r5 = r5 & r6
    .....D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r11 + 0x608] = r5
    .....D=========================eE------------------------R  jump 27629 if r5 != 0
```

Gas simulation at offset 27609 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeE---------------------------------------R............  r12 = r4 + 0x2000
    D=eeeeeeeeeeeeeeeeeeeeeeeeeE--------------R............  r11 = u64 [r12 + 0x738]
    .DeE--------------------------------------R............  r9 = r9 <<r r10
    .D=========================eE-------------R............  r9 = r9 & r11
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r12 + 0x738] = r9
    ..DeeE------------------------------------------------R  fallthrough
```

Gas simulation at offset 27629 with total cost of 26:

```
    DeER.........................  r9 = r4 + 0x2000
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  r9 = u64 [r9 + 0x600]
    .DeeE-----------------------R  i32 r2 = r8 + r2
    .DeE------------------------R  r0 = r0 << 0x4
    ..DeeE----------------------R  i32 r7 = r7 - r0
    ..DeeE----------------------R  fallthrough
```

Gas simulation at offset 27647 with total cost of 5:

```
    DeeER...  i32 r11 = r9 + 0x80000
    .DeER...  r10 = r2 << 0x5
    .D=eeER.  i32 r10 = r10 + r7
    ..D==eER  jump 27884 if r10 >=u r11
```

Gas simulation at offset 27662 with total cost of 48:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER........  unlikely
    DeE---------------------------------------R........  r12 = r10 << 0x20
    D=eE--------------------------------------R........  r12 = r12 >> 0x20
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeE-------------R........  r6 = u32 [r12 + 0x4]
    .D==========================eE------------R........  r9 = r6 & 0x1
    .D===========================eeeeeeeeeeeeeeeeeeeeER  jump 27884 if r9 != 0
```

Gas simulation at offset 27679 with total cost of 1:

```
    DeER  r0 = r6 >> 0x1
    DeER  jump 27722 if r6 == 0
```

Gas simulation at offset 27685 with total cost of 4:

```
    DeER...  r5 = 0x2000000
    D=eeeER  r5 = minu(r0, r5)
    DeE---R  jump 27755 if r6 >=u 256
```

Gas simulation at offset 27699 with total cost of 49:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.........  unlikely
    DeE---------------------------------------R.........  r9 = r5 + 0xffffffffffffffff
    .DeE--------------------------------------R.........  r5 = r9 << 0x20
    .D=eE-------------------------------------R.........  r5 = r5 >> 0x1e
    ..D=eE------------------------------------R.........  r6 = r4 + r5
    ..D==eeeeeeeeeeeeeeeeeeeeeeeeeE-----------R.........  r8 = i32 [r6 + 0]
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------R.........  r5 = u32 [r12 + 0x8]
    ...D==========================eeeeeeeeeeeeeeeeeeeeER  jump 27741 if r8 == r10
```

Gas simulation at offset 27720 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 27798
```

Gas simulation at offset 27722 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeE---------------------------------------R  r9 = 0
    DeE---------------------------------------R  r6 = 0x30a98
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r8 = i32 [0x30a98]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R  r5 = u32 [r12 + 0x8]
    .D========================eE--------------R  jump 27798 if r8 != r10
```

Gas simulation at offset 27741 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r6 + 0] = r5
    DeE------------------------R  jump 27816 if r5 == 0
```

Gas simulation at offset 27746 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r5 + 12] = 0
    DeeE-----------------------R  i32 r2 = r0 + r2
    DeeeeeeeeeeeeeeeE----------R  jump 27884
```

Gas simulation at offset 27755 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeE---------------------------------------R  i32 r8 = clz r5
    .DeeeE------------------------------------R  i32 r9 = 0x18 - r8
    ..D==eeE----------------------------------R  i32 r9 = r5 >> r9
    ...D===eE---------------------------------R  r9 = r9 & 0x7f
    ...DeE------------------------------------R  r8 = r8 << 0x7
    ...D====eE--------------------------------R  r9 = r9 - r8
    ....D====eE-------------------------------R  r8 = r9 + 0x7ff
    ....D=====eE------------------------------R  r9 = r8 + 0x480
    .....D=====eE-----------------------------R  r5 = r9 << 0x20
    .....D======eE----------------------------R  r5 = r5 >> 0x1e
    ......D======eE---------------------------R  r6 = r4 + r5
    ......D=======eeeeeeeeeeeeeeeeeeeeeeeeeE--R  r8 = i32 [r6 + 0]
    ......DeeeeeeeeeeeeeeeeeeeeeeeeeE---------R  r5 = u32 [r12 + 0x8]
    .......D===============================eE-R  jump 27741 if r8 == r10
```

Gas simulation at offset 27798 with total cost of 50:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........  r9 = u32 [r12 + 0xc]
    D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r9 + 0x8] = r5
    DeeeeeeeeeeeeeeeeeeeeE------------------------------R  jump 27880 if r5 == 0
```

Gas simulation at offset 27808 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r5 + 0xc] = r9
    DeeE-----------------------R  i32 r2 = r0 + r2
    DeeeeeeeeeeeeeeeE----------R  jump 27884
```

Gas simulation at offset 27816 with total cost of 55:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...............  unlikely
    DeeE--------------------------------------R...............  i32 r10 = r9 >> 0x6
    .DeE--------------------------------------R...............  r12 = 0x2000
    .D=eE-------------------------------------R...............  r8 = r10 << 0x3
    ..DeE-------------------------------------R...............  r5 = r4 + r12
    ..D=eE------------------------------------R...............  r8 = r8 + r5
    ..D==eeeeeeeeeeeeeeeeeeeeeeeeeE-----------R...............  r5 = u64 [r8 + 0x608]
    ...DeE------------------------------------R...............  r6 = r9 & 0x3f
    ...DeE------------------------------------R...............  r9 = 0xfffffffffffffffe
    ....DeE-----------------------------------R...............  r6 = r9 <<r r6
    ....D=========================eE----------R...............  r5 = r5 & r6
    .....D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r8 + 0x608] = r5
    .....D=========================eE------------------------R  jump 27880 if r5 != 0
```

Gas simulation at offset 27856 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeE---------------------------------------R............  r12 = r4 + 0x2000
    D=eeeeeeeeeeeeeeeeeeeeeeeeeE--------------R............  r8 = u64 [r12 + 0x738]
    .DeE--------------------------------------R............  r9 = r9 <<r r10
    .D=========================eE-------------R............  r8 = r8 & r9
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r12 + 0x738] = r8
    ..DeeE------------------------------------------------R  i32 r2 = r0 + r2
    ..DeeeeeeeeeeeeeeeE-----------------------------------R  jump 27884
```

Gas simulation at offset 27880 with total cost of 2:

```
    DeeER  i32 r2 = r0 + r2
    DeeER  fallthrough
```

Gas simulation at offset 27884 with total cost of 20:

```
    DeeeeeeeeeeeeeeeeeeeeER  jump 28023 if r2 == 0
```

Gas simulation at offset 27888 with total cost of 1:

```
    D...  r9 = r2
    DeER  jump 27932 if r2 <=u 127
```

Gas simulation at offset 27894 with total cost of 15:

```
    DeER..............  r8 = 0x2000000
    D=eeeER...........  r8 = minu(r2, r8)
    D====eER..........  i32 r10 = clz r8
    .D====eeeER.......  i32 r9 = 0x18 - r10
    ..D======eeER.....  i32 r8 = r8 >> r9
    ..D========eER....  r8 = r8 & 0x7f
    ...D==eE-----R....  r10 = r10 << 0x7
    ...D========eER...  r8 = r8 - r10
    ...D=========eER..  r8 = r8 + 0x7ff
    ....D=========eER.  r9 = r8 + 0x480
    ....D==========eER  r9 = r9 + 0x1
    ....DeeE---------R  fallthrough
```

Gas simulation at offset 27932 with total cost of 54:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..............  unlikely
    DeeE--------------------------------------R..............  i32 r10 = r9 + 0xffffffffffffffff
    .DeE--------------------------------------R..............  r8 = r2 << 0x1
    .DeE--------------------------------------R..............  r5 = r7 << 0x20
    ..DeE-------------------------------------R..............  r9 = r10 << 0x2
    ..D=eE------------------------------------R..............  r9 = r9 + r4
    ..D==eeeeeeeeeeeeeeeeeeeeeeeeeE-----------R..............  r12 = u32 [r9 + 0]
    ...D=eeeeeeeeeeeeeeeeeeeeeeeeeE-----------R..............  u32 [r9 + 0] = r7
    ...DeeE-----------------------------------R..............  i32 r9 = r10 >> 0x6
    ....DeE-----------------------------------R..............  r10 = r10 & 0x3f
    ....D=eE----------------------------------R..............  r5 = r5 >> 0x20
    ....D==eeeeeeeeeeeeeeeeeeeeeeeeeE---------R..............  u32 [r5 + 0] = r3
    ....D==eeeeeeeeeeeeeeeeeeeeeeeeeE---------R..............  u32 [r5 + 0x4] = r8
    .....D========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r5 + 0x8] = r12
    .....D========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r5 + 12] = 0
    .....D==========================eE----------------------R  jump 27979 if r12 == 0
```

Gas simulation at offset 27975 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r12 + 0xc] = r7
    DeeE-----------------------R  fallthrough
```

Gas simulation at offset 27979 with total cost of 55:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...............  unlikely
    DeE---------------------------------------R...............  r8 = r9 << 0x3
    .DeE--------------------------------------R...............  r12 = r4 + 0x2000
    .D=eE-------------------------------------R...............  r8 = r8 + r12
    .D==eeeeeeeeeeeeeeeeeeeeeeeeeE------------R...............  r12 = u64 [r8 + 0x608]
    ..DeE-------------------------------------R...............  r10 = 0x1 << r10
    ..D==========================eE-----------R...............  r10 = r10 | r12
    ...D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u64 [r8 + 0x608] = r10
    ...DeE--------------------------------------------------R.  r4 = r4 + 0x2000
    ...D=eeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R.  r8 = u64 [r4 + 0x738]
    ....DeE-------------------------------------------------R.  r9 = 0x1 << r9
    ....D=========================eE------------------------R.  r8 = r8 | r9
    .....D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r4 + 0x738] = r8
    .....DeeE------------------------------------------------R  fallthrough
```

Gas simulation at offset 28023 with total cost of 4:

```
    DeER...  r8 = r2 << 0x5
    D=eeER.  i32 r7 = r7 + r8
    .D==eER  jump 28041 if r7 >=u r11
```

Gas simulation at offset 28032 with total cost of 27:

```
    DeER..........................  r7 = r7 << 0x20
    D=eER.........................  r7 = r7 >> 0x20
    D==eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r7 + 0] = r2
    DeeE-------------------------R  fallthrough
```

Gas simulation at offset 28041 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.......  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r0 = u64 [r1 + 0x10]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r5 = u64 [r1 + 0x8]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r6 = u64 [r1 + 0]
    .DeE--------------------------------------R.......  r1 = r1 + 0x18
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 28055 with total cost of 20:

```
    DeeeeeeeeeeeeeeeeeeeeER  jump 28078 if r9 == 0
```

Gas simulation at offset 28058 with total cost of 2:

```
    DeER.  r9 = r9 + r7
    D....  r10 = r7
    DeeER  fallthrough
```

Gas simulation at offset 28064 with total cost of 50:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........  r11 = u8 [r8 + 0]
    D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r10 + 0] = a4
    DeE-------------------------------------------------R  r10 = r10 + 0x1
    .DeE------------------------------------------------R  r8 = r8 + 0x1
    .DeE------------------------------------------------R  jump 28064 if r10 != r9
```

Gas simulation at offset 28078 with total cost of 22:

```
    DeeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 28080 with total cost of 20:

```
    DeeeeeeeeeeeeeeeeeeeeER  jump 28097 if r9 == 0
```

Gas simulation at offset 28083 with total cost of 2:

```
    DeER.  r9 = r9 + r7
    D....  r10 = r7
    DeeER  fallthrough
```

Gas simulation at offset 28089 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r10 + 0] = a1
    DeE------------------------R  r10 = r10 + 0x1
    D=eeeeeeeeeeeeeeeeeeeeE----R  jump 28089 if r10 != r9
```

Gas simulation at offset 28097 with total cost of 22:

```
    DeeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 28099 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  u64 [0x30000] = r4
    DeE---------------------------------------R............  r4 = r8 << 0x20
    .DeE--------------------------------------R............  r4 = r4 >>a 0x20
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R............  r9 = i32 [r7 + 0]
    .D=========================eE-------------R............  r4 = r9 | r4
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r7 + 0] = r4
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r4 = u64 [0x30000]
    ..D========================eE-------------------------R  r9 = r9 & 0xff
    ..D=========================eE------------------------R  jump 28099 if r9 != 0
```

Gas simulation at offset 28130 with total cost of 15:

```
    DeER..............  r7 = 0x1e00
    DeER..............  r8 = 0x1
    DeER..............  r6 = 0x1
    DeeeeeeeeeeeeeeeER  r0 = 818, jump 26592
```

Gas simulation at offset 28146 with total cost of 27:

```
    DeER..........................  r10 = 0x2000
    D=eER.........................  r8 = r5 + r10
    D==eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r8 + 1872] = 0
    .DeE-------------------------R  r8 = 0x30008
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x30] = r8
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-R  r8 = u64 [0x30008]
    .D............................  r9 = r5
    ..D...........................  r5 = r7
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x40] = r9
    ..D========================eER  jump 28243 if r8 == 0
```

Gas simulation at offset 28180 with total cost of 2:

```
    DeER.  r7 = r9 + 0x2750
    D=eER  r7 = r7 & 0xfffffffffffffffc
    DeeER  fallthrough
```

Gas simulation at offset 28188 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  u64 [0x30000] = r4
    DeE---------------------------------------R............  r4 = r6 << 0x20
    .DeE--------------------------------------R............  r4 = r4 >>a 0x20
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R............  r9 = i32 [r7 + 0]
    .D=========================eE-------------R............  r4 = r9 | r4
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r7 + 0] = r4
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r4 = u64 [0x30000]
    ..D========================eE-------------------------R  r9 = r9 & 0xff
    ..D=========================eE------------------------R  jump 28188 if r9 != 0
```

Gas simulation at offset 28219 with total cost of 15:

```
    D.................  r7 = r8
    DeeeeeeeeeeeeeeeER  r0 = 820, jump 27398
```

Gas simulation at offset 28227 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r9 = u64 [r1 + 0x40]
    D=========================eER.........................  r7 = r9 + 0x2000
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 1872] = 0
    .DeE-------------------------------------------------R  r10 = 0x2000
    .DeeE------------------------------------------------R  fallthrough
```

Gas simulation at offset 28243 with total cost of 50:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........  r7 = u64 [r1 + 0x30]
    D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r7 + 0] = r5
    .DeE------------------------------------------------R  r7 = r9 + 0x2750
    .D=eE-----------------------------------------------R  r7 = r7 & 0xfffffffffffffffc
    .DeeE-----------------------------------------------R  fallthrough
```

Gas simulation at offset 28257 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  u64 [0x30000] = r4
    DeE---------------------------------------R............  r4 = r6 << 0x20
    .DeE--------------------------------------R............  r4 = r4 >>a 0x20
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R............  r8 = i32 [r7 + 0]
    .D=========================eE-------------R............  r4 = r8 | r4
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r7 + 0] = r4
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r4 = u64 [0x30000]
    ..D========================eE-------------------------R  r8 = r8 & 0xff
    ..D=========================eE------------------------R  jump 28257 if r8 != 0
```

Gas simulation at offset 28288 with total cost of 15:

```
    DeER..............  r7 = 0x200
    DeeeeeeeeeeeeeeeER  r0 = 822, jump 26592
```

Gas simulation at offset 28298 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r5 = u64 [r1 + 0x40]
    D=========================eER.........................  r8 = r5 + 0x2000
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r8 + 1872] = 0
    .DeE-------------------------------------------------R  jump 32329 if r7 == 0
```

Gas simulation at offset 28313 with total cost of 26:

```
    DeER.........................  r6 = 0x10240
    D=eER........................  r8 = r6 + 0x10
    DeE-R........................  r9 = 0x4000
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x28] = r7
    .DeeeeeeeeeeeeeeeE----------R  r0 = 824, jump 28055
```

Gas simulation at offset 28334 with total cost of 3:

```
    DeER..  r7 = r5 + 0x2750
    D=eER.  r7 = r7 & 0xfffffffffffffffc
    DeE-R.  r8 = 0x1
    .DeeER  fallthrough
```

Gas simulation at offset 28345 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  u64 [0x30000] = r4
    DeE---------------------------------------R............  r4 = r8 << 0x20
    .DeE--------------------------------------R............  r4 = r4 >>a 0x20
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R............  r9 = i32 [r7 + 0]
    .D=========================eE-------------R............  r4 = r9 | r4
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r7 + 0] = r4
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r4 = u64 [0x30000]
    ..D========================eE-------------------------R  r9 = r9 & 0xff
    ..D=========================eE------------------------R  jump 28345 if r9 != 0
```

Gas simulation at offset 28376 with total cost of 15:

```
    DeER..............  r7 = 0x100
    DeER..............  r8 = 0
    DeeeeeeeeeeeeeeeER  r0 = 826, jump 26592
```

Gas simulation at offset 28388 with total cost of 51:

```
    D.....................................................  r10 = r7
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r7 = u64 [r1 + 0x40]
    D=========================eER.........................  r7 = r7 + 0x2000
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 1872] = 0
    .DeE-------------------------------------------------R  jump 32329 if r10 == 0
```

Gas simulation at offset 28405 with total cost of 26:

```
    DeER.........................  r5 = 0x4000
    DeER.........................  r8 = r6 + 0x4010
    DeER.........................  r9 = 0x2000
    .D...........................  r7 = r10
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x20] = r10
    .DeeeeeeeeeeeeeeeE----------R  r0 = 828, jump 28055
```

Gas simulation at offset 28428 with total cost of 176:

```
    DeER...............................................................................................................................................................................  r6 = 0x1
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.......................................................................................................................................................  r7 = i16 [r1 + 0x2a8]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.......................................................................................................................................................  u64 [r1 + 0x48] = r5
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.......................................................................................................................................................  r8 = u64 [r1 + 0x28]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..............................................................................................................................  u64 [r1 + 0x50] = r8
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE------------------------R..............................................................................................................................  u64 [r1 + 0x58] = r5
    .DeE------------------------------------------------R..............................................................................................................................  r5 = 0x2000
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..............................................................................................................................  u64 [r1 + 0x60] = r5
    ..D=======================eeeeeeeeeeeeeeeeeeeeeeeeeER..............................................................................................................................  u32 [r1 + 776] = 0
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.............................................................................................................................  u32 [r1 + 780] = 0
    ..D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.....................................................................................................  u32 [r1 + 784] = 0
    ..D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.....................................................................................................  u8 [r1 + 788] = 0
    ...DeE-----------------------------------------------------------------------R.....................................................................................................  r8 = 0xfffffc0000000000
    ...D===============================================eeeeeeeeeeeeeeeeeeeeeeeeeER.....................................................................................................  u64 [r1 + 680] = 0
    ...D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER....................................................................................................  u64 [r1 + 0x2b0] = r6
    ....D=======================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER............................................................................  u64 [r1 + 696] = 0
    ....D=======================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER............................................................................  u64 [r1 + 0x2c0] = r8
    ....D=======================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER............................................................................  u16 [r1 + 0x7e] = r7
    .....DeE----------------------------------------------------------------------------------------------R............................................................................  r9 = 0xffff2000
    .....DeE----------------------------------------------------------------------------------------------R............................................................................  r11 = 0xffff8000ffffa000
    ......DeE---------------------------------------------------------------------------------------------R............................................................................  r12 = 0xffff4000ffff6000
    ......DeE---------------------------------------------------------------------------------------------R............................................................................  r7 = 0xffffd400ffffd800
    .......D=====================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  u64 [r1 + 0x2e8] = r7
    .......D=============================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER...................................................  u64 [r1 + 0x2f0] = r11
    .......D=============================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER...................................................  u64 [r1 + 0x2f8] = r12
    .......D=============================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER...................................................  u64 [r1 + 0x300] = r9
    ........D=============================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  r9 = u64 [r1 + 0x20]
    ........D======================================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u64 [r1 + 0x68] = r9
    ........D=====================================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-R.........................  u64 [r1 + 0x70] = r5
    ........D=====================================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-R.........................  u32 [r1 + 0x78] = r5
    .........D====================================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-R.........................  u16 [r1 + 0x7c] = r6
    .........DeE---------------------------------------------------------------------------------------------------------------------------------------------R.........................  r2 = 0xfffff40100000000
    ..........DeE--------------------------------------------------------------------------------------------------------------------------------------------R.........................  r9 = 0xfffff400fffff800
    ............................DeE--------------------------------------------------------------------------------------------------------------------------R.........................  r10 = 0xffffec00fffff000
    ............................DeE--------------------------------------------------------------------------------------------------------------------------R.........................  r8 = 0xffffe400ffffe800
    .............................DeE-------------------------------------------------------------------------------------------------------------------------R.........................  r7 = 0xffffdc00ffffe000
    .....................................................D=================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u64 [r1 + 0x2c8] = r9
    .....................................................D=================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u64 [r1 + 0x2d0] = r10
    .....................................................D=================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u64 [r1 + 0x2d8] = r8
    .....................................................D==================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x2e0] = r7
    ......................................................D=========================================================================================================================eER  r7 = r1 + 0x2a8
    ......................................................DeE-------------------------------------------------------------------------------------------------------------------------R  r9 = 0x2000
    ..............................................................................DeE-------------------------------------------------------------------------------------------------R  r8 = 0
    ..............................................................................DeeeeeeeeeeeeeeeE-----------------------------------------------------------------------------------R  r0 = 830, jump 32330
```

Gas simulation at offset 28652 with total cost of 50:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r7 = u64 [r1 + 0x2b0]
    D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x10] = r7
    DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r8 = u64 [r1 + 0x2b8]
    D=========================eE------------------------R  r7 = r7 + r8
    .D========================eE------------------------R  r5 = r5 + r8
    .DeE------------------------------------------------R  r9 = 0x2000
    .DeE------------------------------------------------R  r8 = 0
    .DeeeeeeeeeeeeeeeE----------------------------------R  r0 = 832, jump 28080
```

Gas simulation at offset 28681 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r7 = u8 [r1 + 0x310]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r8 = u64 [r1 + 0x2a8]
    D=========================eER.........................  r7 = r7 | 0x3
    D=========================eER.........................  r8 = r8 - r5
    .D=========================eER........................  r8 = r8 >> 0xe
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-R........................  u64 [r1 + 0x2b8] = r5
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-R........................  u32 [r1 + 752] = 0xffffffffffffa000
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r1 + 0x310] = a0
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u64 [r1 + 0x10]
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x18] = r5
    ..D=========================eeeeeeeeeeeeeeeeeeeeE----R  jump 30804 if r8 == 0
```

Gas simulation at offset 28722 with total cost of 25:

```
    DeER........................  r7 = r7 + r5
    DeER........................  r9 = 0x4000
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = u64 [r1 + 0x28]
    DeeeeeeeeeeeeeeeE----------R  r0 = 834, jump 28055
```

Gas simulation at offset 28738 with total cost of 128:

```
    DeER...............................................................................................................................  r5 = r5 + 0x4000
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.......................................................................................................  r9 = u64 [r1 + 0x18]
    D=========================eER......................................................................................................  r7 = r9 + 0xffffffffffff8000
    .D=========================eER.....................................................................................................  r8 = r9 + 0xffffffffffff4000
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-R.....................................................................................................  r9 = u8 [r1 + 0x311]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-R.....................................................................................................  r10 = u8 [r1 + 0x312]
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeER.....................................................................................................  r11 = u8 [r1 + 0x313]
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.............................................................................  r12 = u8 [r1 + 0x314]
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.............................................................................  u64 [r1 + 0x2b8] = r5
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER............................................................................  u32 [r1 + 0x2f4] = r7
    ...D========================eeeeeeeeeeeeeeeeeeeeeeeeeER............................................................................  u32 [r1 + 0x2f8] = r7
    ...D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER....................................................  u32 [r1 + 0x2fc] = r8
    ...D================================================eE------------------------R....................................................  r7 = r9 | 0x1
    ....D================================================eE-----------------------R....................................................  r9 = r10 | 0x1
    ....D================================================eE-----------------------R....................................................  r10 = r11 | 0x1
    .....D===============================================eE-----------------------R....................................................  r11 = r12 | 0x1
    .....D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  u32 [r1 + 0x300] = r8
    .....D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  u8 [r1 + 0x311] = a0
    ......D===============================================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  u8 [r1 + 0x312] = a2
    ......D======================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER...........................  u8 [r1 + 0x313] = a3
    ......D========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u8 [r1 + 0x314] = a4
    .......D=======================================================================eE------------------------R.........................  r7 = r1 + 0x2a8
    .......DeE-----------------------------------------------------------------------------------------------R.........................  r9 = 0x2000
    .......D=======================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r8 = u64 [r1 + 0x20]
    ........DeE----------------------------------------------------------------------------------------------R.........................  r0 = 0x344
    ........D=======================================================================eE-----------------------R.........................  r1 = r1 + 0xffffffffffffffd0
    ........D========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.......................  u64 [r1 + 0x28] = r0
    ........D=============================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER..  u64 [r1 + 0x20] = r9
    .........D==============================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x18] = r6
    .........D.........................................................................................................................  r6 = r7
    .........D==============================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  r5 = u64 [r7 + 0x10]
    .........DeeeeeeeeeeeeeeeE--------------------------------------------------------------------------------------------------------R  jump 32669
```

Gas simulation at offset 28853 with total cost of 76:

```
    DeER...........................................................................  r7 = r1 + 0x2a8
    DeER...........................................................................  r0 = 0x346
    DeER...........................................................................  r1 = r1 + 0xffffffffffffffc8
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  u64 [r1 + 0x30] = r0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  u64 [r1 + 0x28] = r5
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  u64 [r1 + 0x20] = r6
    .DeE------------------------R..................................................  r6 = 0x1
    ..D............................................................................  r5 = r7
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeER.................................................  r7 = u64 [r7 + 0]
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r10 = u64 [r5 + 0x10]
    ..D=================================================eER........................  r7 = r7 - r10
    ...D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x18] = r10
    ...DeeeeeeeeeeeeeeeE----------------------------------------------------------R  jump 32862
```

Gas simulation at offset 28892 with total cost of 27:

```
    DeeER.........................  i32 r7 = r5 + 0x750
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u64 [r1 + 0x40]
    .D========================eER.  r7 = r7 + r8
    .D=========================eER  r7 = r7 & 0xfffffffffffffffc
    .DeeE------------------------R  fallthrough
```

Gas simulation at offset 28906 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  u64 [0x30000] = r4
    DeE---------------------------------------R............  r4 = r6 << 0x20
    .DeE--------------------------------------R............  r4 = r4 >>a 0x20
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R............  r8 = i32 [r7 + 0]
    .D=========================eE-------------R............  r4 = r8 | r4
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r7 + 0] = r4
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r4 = u64 [0x30000]
    ..D========================eE-------------------------R  r8 = r8 & 0xff
    ..D=========================eE------------------------R  jump 28906 if r8 != 0
```

Gas simulation at offset 28937 with total cost of 15:

```
    DeER..............  r7 = 0x4
    DeeeeeeeeeeeeeeeER  r0 = 840, jump 26592
```

Gas simulation at offset 28946 with total cost of 51:

```
    D.....................................................  r5 = r7
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r8 = u64 [r1 + 0x40]
    D=========================eER.........................  r7 = r8 + 0x2000
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 1872] = 0
    .DeE-------------------------------------------------R  jump 32329 if r5 == 0
```

Gas simulation at offset 28963 with total cost of 16:

```
    DeER...............  r8 = r1 + 0x2a8
    DeER...............  r9 = 0x70
    D..................  r7 = r5
    .DeeeeeeeeeeeeeeeER  r0 = 842, jump 28055
```

Gas simulation at offset 28978 with total cost of 50:

```
    DeER.................................................  r7 = 0x18d48
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r9 = u64 [r1 + 0x48]
    DeE------------------------R.........................  r8 = 0x8000000000000000
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER........................  u64 [r1 + 0xe8] = r8
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER........................  u64 [r1 + 0xf0] = r5
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER........................  u64 [r1 + 0xf8] = r7
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER  r5 = u64 [r1 + 0x40]
    ..D========================eE-----------------------R  jump 29074 if r9 == 0
```

Gas simulation at offset 29014 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u64 [r1 + 0x50]
    DeE------------------------R  r8 = r5 + 0x2750
    D=eE-----------------------R  r8 = r8 & 0xfffffffffffffffc
    .DeE-----------------------R  r9 = 0x1
    .DeeE----------------------R  fallthrough
```

Gas simulation at offset 29028 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  u64 [0x30000] = r4
    DeE---------------------------------------R............  r4 = r9 << 0x20
    .DeE--------------------------------------R............  r4 = r4 >>a 0x20
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R............  r10 = i32 [r8 + 0]
    .D=========================eE-------------R............  r4 = r10 | r4
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r8 + 0] = r4
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r4 = u64 [0x30000]
    ..D========================eE-------------------------R  r10 = r10 & 0xff
    ..D=========================eE------------------------R  jump 29028 if r10 != 0
```

Gas simulation at offset 29059 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  r0 = 844, jump 27398
```

Gas simulation at offset 29065 with total cost of 26:

```
    DeER.........................  r7 = r5 + 0x2000
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 1872] = 0
    DeeE------------------------R  fallthrough
```

Gas simulation at offset 29074 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u64 [r1 + 0x60]
    D=========================eE--------------R  jump 29141 if r7 == 0
```

Gas simulation at offset 29081 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u64 [r1 + 0x68]
    DeE------------------------R  r8 = r5 + 0x2750
    D=eE-----------------------R  r8 = r8 & 0xfffffffffffffffc
    .DeE-----------------------R  r9 = 0x1
    .DeeE----------------------R  fallthrough
```

Gas simulation at offset 29095 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  u64 [0x30000] = r4
    DeE---------------------------------------R............  r4 = r9 << 0x20
    .DeE--------------------------------------R............  r4 = r4 >>a 0x20
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R............  r10 = i32 [r8 + 0]
    .D=========================eE-------------R............  r4 = r10 | r4
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r8 + 0] = r4
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r4 = u64 [0x30000]
    ..D========================eE-------------------------R  r10 = r10 & 0xff
    ..D=========================eE------------------------R  jump 29095 if r10 != 0
```

Gas simulation at offset 29126 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  r0 = 846, jump 27398
```

Gas simulation at offset 29132 with total cost of 26:

```
    DeER.........................  r7 = r5 + 0x2000
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 1872] = 0
    DeeE------------------------R  fallthrough
```

Gas simulation at offset 29141 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u64 [r1 + 0xe8]
    DeE---------------------------------------R  r8 = 0x8000000000000000
    .D========================eE--------------R  jump 30803 if r7 != r8
```

Gas simulation at offset 29160 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  r7 = u64 [r1 + 0x30]
    D=========================eE--------------R............  r6 = r7 + 0x7ff
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  r10 = u64 [r6 + 0x249]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R.  r7 = u64 [r1 + 0xf0]
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u64 [r1 + 0x28] = r7
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R.  r7 = u64 [r1 + 0xf8]
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u64 [r1 + 0x38] = r7
    ..D=================================================eER  jump 29282 if r10 == 0
```

Gas simulation at offset 29189 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r5 = u64 [r6 + 0x251]
    D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  r8 = u64 [r5 + 0]
    D==================================================eER  jump 29213 if r8 == 0
```

Gas simulation at offset 29199 with total cost of 25:

```
    D...........................  r7 = r10
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x20] = r10
    DeeeeeeeeeeeeeeeeeeeeeeE---R  r0 = 848, jump [r8 + 0]
```

Gas simulation at offset 29209 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r10 = u64 [r1 + 0x20]
    DeeE-----------------------R  fallthrough
```

Gas simulation at offset 29213 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u64 [r5 + 0x8]
    D=========================eE--------------R  jump 29282 if r7 == 0
```

Gas simulation at offset 29220 with total cost of 27:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..  r5 = u64 [r1 + 0x40]
    D=========================eER.  r7 = r5 + 0x2750
    D==========================eER  r7 = r7 & 0xfffffffffffffffc
    .DeE-------------------------R  r8 = 0x1
    .DeeE------------------------R  fallthrough
```

Gas simulation at offset 29234 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  u64 [0x30000] = r4
    DeE---------------------------------------R............  r4 = r8 << 0x20
    .DeE--------------------------------------R............  r4 = r4 >>a 0x20
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R............  r9 = i32 [r7 + 0]
    .D=========================eE-------------R............  r4 = r9 | r4
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r7 + 0] = r4
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r4 = u64 [0x30000]
    ..D========================eE-------------------------R  r9 = r9 & 0xff
    ..D=========================eE------------------------R  jump 29234 if r9 != 0
```

Gas simulation at offset 29265 with total cost of 15:

```
    D.................  r7 = r10
    DeeeeeeeeeeeeeeeER  r0 = 850, jump 27398
```

Gas simulation at offset 29273 with total cost of 26:

```
    DeER.........................  r7 = r5 + 0x2000
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 1872] = 0
    DeeE------------------------R  fallthrough
```

Gas simulation at offset 29282 with total cost of 50:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........  u64 [r6 + 585] = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........  r7 = u64 [r1 + 0x38]
    D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r6 + 0x251] = r7
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE------------------------R  u8 [r6 + 651] = 0x1
    .DeE------------------------------------------------R  r5 = 0x800
    .DeE------------------------------------------------R  r7 = r1 + 0x2a8
    ..DeE-----------------------------------------------R  r8 = 0
    ..DeE-----------------------------------------------R  r9 = 0x800
    ..DeeeeeeeeeeeeeeeE---------------------------------R  r0 = 852, jump 28080
```

Gas simulation at offset 29319 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u64 [r1 + 216] = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u32 [r1 + 224] = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u16 [r1 + 228] = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u64 [r1 + 200] = 0
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u16 [r1 + 208] = 0
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u64 [r1 + 144] = 0
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u32 [r1 + 152] = 0
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u8 [r1 + 156] = 0
    ..D================================================eER  r7 = r1 + 0xed
    ..DeE------------------------------------------------R  r9 = 0x16e
    ..DeE------------------------------------------------R  r8 = 0
    ...DeeeeeeeeeeeeeeeE---------------------------------R  r0 = 854, jump 28080
```

Gas simulation at offset 29367 with total cost of 77:

```
    DeER............................................................................  r7 = r1 + 0x2a8
    D=eER...........................................................................  r5 = r5 + r7
    D=eER...........................................................................  r7 = r7 + 0x7ff
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER...................................................  u64 [r1 + 184] = 0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER...................................................  u64 [r1 + 192] = 0
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  u32 [r1 + 672] = 0
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  u16 [r1 + 676] = 0
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u64 [r5 + 8] = 0
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u32 [r5 + 16] = 0
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u16 [r5 + 20] = 0
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u8 [r5 + 22] = 0
    ...D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u64 [r7 + 1] = 0
    ...D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u64 [r7 + 25] = 0
    ...D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r7 + 33] = 0
    ....D================================================eE------------------------R  r7 = r1 + 0x296
    ....DeE------------------------------------------------------------------------R  r9 = 0xa
    ....DeE------------------------------------------------------------------------R  r8 = 0
    .....DeeeeeeeeeeeeeeeE---------------------------------------------------------R  r0 = 856, jump 28080
```

Gas simulation at offset 29430 with total cost of 100:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  u64 [r1 + 616] = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  u64 [r1 + 624] = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  u64 [r1 + 632] = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  u64 [r1 + 640] = 0
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  u64 [r1 + 648] = 0
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  u16 [r1 + 656] = 0
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  u8 [r1 + 658] = 0
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  u32 [r1 + 608] = 0
    ..D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u8 [r1 + 612] = 0
    ..D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r7 = u64 [r6 + 0x209]
    ..D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u64 [r1 + 168] = 0
    ..D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u64 [r1 + 176] = 0
    ...D========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r1 + 138] = 0
    ...D========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r1 + 140] = 0
    ...D========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r1 + 142] = 0
    ...D========================================================================eE------------------------R  jump 29649 if r7 == 0
```

Gas simulation at offset 29494 with total cost of 27:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..  r5 = u64 [r1 + 0x40]
    D=========================eER.  r8 = r5 + 0x2750
    D==========================eER  r8 = r8 & 0xfffffffffffffffc
    .DeE-------------------------R  r10 = 0x1
    .DeeE------------------------R  fallthrough
```

Gas simulation at offset 29508 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  u64 [0x30000] = r4
    DeE---------------------------------------R............  r4 = r10 << 0x20
    .DeE--------------------------------------R............  r4 = r4 >>a 0x20
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R............  r9 = i32 [r8 + 0]
    .D=========================eE-------------R............  r4 = r9 | r4
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r8 + 0] = r4
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r4 = u64 [0x30000]
    ..D========================eE-------------------------R  r9 = r9 & 0xff
    ..D=========================eE------------------------R  jump 29508 if r9 != 0
```

Gas simulation at offset 29539 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  r0 = 858, jump 27398
```

Gas simulation at offset 29545 with total cost of 26:

```
    DeER.........................  r7 = r5 + 0x2000
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 1872] = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeE-R  r7 = u64 [r6 + 0x249]
    .D========================eER  jump 29649 if r7 == 0
```

Gas simulation at offset 29560 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r5 = u64 [r6 + 0x251]
    D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  r8 = u64 [r5 + 0]
    D==================================================eER  jump 29582 if r8 == 0
```

Gas simulation at offset 29570 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x20] = r7
    DeeeeeeeeeeeeeeeeeeeeeeE---R  r0 = 860, jump [r8 + 0]
```

Gas simulation at offset 29578 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u64 [r1 + 0x20]
    DeeE-----------------------R  fallthrough
```

Gas simulation at offset 29582 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r8 = u64 [r5 + 0x8]
    D=========================eE--------------R  jump 29649 if r8 == 0
```

Gas simulation at offset 29589 with total cost of 27:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..  r5 = u64 [r1 + 0x40]
    D=========================eER.  r8 = r5 + 0x2750
    .D=========================eER  r10 = r8 & 0xfffffffffffffffc
    .DeE-------------------------R  r8 = 0x1
    .DeeE------------------------R  fallthrough
```

Gas simulation at offset 29603 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  u64 [0x30000] = r4
    DeE---------------------------------------R............  r4 = r8 << 0x20
    .DeE--------------------------------------R............  r4 = r4 >>a 0x20
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R............  r9 = i32 [r10 + 0]
    .D=========================eE-------------R............  r4 = r9 | r4
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r10 + 0] = r4
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r4 = u64 [0x30000]
    ..D========================eE-------------------------R  r9 = r9 & 0xff
    ..D=========================eE------------------------R  jump 29603 if r9 != 0
```

Gas simulation at offset 29634 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  r0 = 862, jump 27398
```

Gas simulation at offset 29640 with total cost of 26:

```
    DeER.........................  r7 = r5 + 0x2000
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 1872] = 0
    DeeE------------------------R  fallthrough
```

Gas simulation at offset 29649 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r7 = u64 [r1 + 0x30]
    D=========================eE--------------R...........  r7 = r7 + 0x8
    DeE---------------------------------------R...........  r9 = 0x828
    .DeE--------------------------------------R...........  r8 = r1 + 0x2a8
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x30] = r7
    .DeeeeeeeeeeeeeeeE-----------------------------------R  r0 = 864, jump 28055
```

Gas simulation at offset 29673 with total cost of 100:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r7 = u8 [r1 + 0x2a0]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r8 = u8 [r1 + 0x2a1]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r9 = u8 [r1 + 0x2a2]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r10 = u8 [r1 + 0x2a3]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  r11 = u8 [r1 + 0x2a4]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  r12 = u8 [r1 + 0x2a5]
    .DeE------------------------------------------------R..................................................  r5 = 0x1
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  u8 [r6 + 0x31] = s0
    ..D=======================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  u8 [r6 + 0x32] = a0
    ..D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u8 [r6 + 0x33] = a1
    ..D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u8 [r6 + 0x34] = a2
    ..D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u8 [r6 + 0x35] = a3
    ...D===============================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u8 [r6 + 0x36] = a4
    ...D========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x37] = a5
    ...D========================================================================eE------------------------R  r7 = r6 + 0x38
    ....D=======================================================================eE------------------------R  r8 = r1 + 0x295
    ....DeE-----------------------------------------------------------------------------------------------R  r9 = 0xb
    ....DeeeeeeeeeeeeeeeE---------------------------------------------------------------------------------R  r0 = 866, jump 28055
```

Gas simulation at offset 29737 with total cost of 225:

```
    DeER................................................................................................................................................................................................................................  r10 = 0x17bf4
    DeeeeeeeeeeeeeeeeeeeeeeeeeER........................................................................................................................................................................................................  r12 = u64 [r1 + 0x268]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER........................................................................................................................................................................................................  r2 = u64 [r1 + 0x270]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER........................................................................................................................................................................................................  r11 = u64 [r1 + 0x278]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER.......................................................................................................................................................................................................  r5 = u64 [r1 + 0x280]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER...............................................................................................................................................................................  r0 = u64 [r1 + 0x288]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER...............................................................................................................................................................................  r3 = i16 [r1 + 0x290]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER...............................................................................................................................................................................  r4 = u8 [r1 + 0x292]
    ..DeE-----------------------------------------------R...............................................................................................................................................................................  r7 = 0xc00000000001c000
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..............................................................................................................................................................................  r9 = i32 [r1 + 0x260]
    ..D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER......................................................................................................................................................  r8 = u8 [r1 + 0x264]
    ...D===============================================eeeeeeeeeeeeeeeeeeeeeeeeeER......................................................................................................................................................  u64 [r6 + 0x59] = r12
    ...DeE-----------------------------------------------------------------------R......................................................................................................................................................  r12 = 0x8
    ...D===============================================eeeeeeeeeeeeeeeeeeeeeeeeeER......................................................................................................................................................  u64 [r6 + 0x61] = r2
    ...D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.....................................................................................................................................................  u64 [r6 + 0x69] = r11
    ....D=======================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.............................................................................................................................  u64 [r6 + 0x71] = r5
    ....DeE-----------------------------------------------------------------------------------------------R.............................................................................................................................  r11 = 0x2
    ....D=======================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.............................................................................................................................  u16 [r6 + 135] = 0
    ....D=======================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.............................................................................................................................  u64 [r1 + 0x18] = r7
    .....D=======================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER............................................................................................................................  u64 [r6 + 0x89] = r7
    .....D===============================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER....................................................................................................  u32 [r6 + 0x91] = r9
    .....D===============================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER....................................................................................................  u8 [r6 + 0x95] = a1
    .....D===============================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER....................................................................................................  u16 [r6 + 67] = 0x1
    ......D===============================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER...................................................................................................  u32 [r6 + 69] = 0
    ......D=======================================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  u64 [r1 + 0x20] = r10
    ......D=======================================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  u64 [r6 + 0x49] = r10
    ......D=======================================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  u64 [r6 + 81] = 0x9
    .......D=======================================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER..........................................................................  u8 [r6 + 150] = 0x1
    .......D===============================================================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  u16 [r6 + 151] = 0
    .......D===============================================================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  u16 [r6 + 0x99] = r12
    .......D===============================================================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  u8 [r6 + 0x9b] = a4
    ........D===============================================================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.................................................  u64 [r6 + 0x79] = r0
    ........D=======================================================================================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u16 [r6 + 0x81] = r3
    ............................D===================================================================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u8 [r6 + 0x83] = t2
    ............................D===================================================================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u8 [r6 + 133] = 0
    ............................D====================================================================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER........................  u32 [r6 + 157] = 0x1
    .............................D===========================================================================================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r6 + 161] = 0x200
    .....................................................D===================================================================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 163] = 0
    .....................................................D===================================================================================================================================================eE------------------------R  r7 = r6 + 0xa4
    ......................................................D===================================================================================================================================================eE-----------------------R  r8 = r1 + 0xe8
    ......................................................DeE--------------------------------------------------------------------------------------------------------------------------------------------------------------------------R  r9 = 0x173
    ......................................................DeeeeeeeeeeeeeeeE------------------------------------------------------------------------------------------------------------------------------------------------------------R  r0 = 868, jump 28055
```

Gas simulation at offset 29907 with total cost of 76:

```
    DeER...........................................................................  r10 = 0x105
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...................................................  r7 = u64 [r1 + 0xd8]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...................................................  r8 = i32 [r1 + 0xe0]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...................................................  r9 = i16 [r1 + 0xe4]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  u16 [r6 + 0x217] = r10
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u64 [r6 + 0x219] = r7
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u32 [r6 + 0x221] = r8
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u16 [r6 + 0x225] = r9
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u16 [r6 + 551] = 0
    ..D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u16 [r6 + 553] = 0xc1
    ..D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u8 [r6 + 555] = 0
    ...D===============================================eE------------------------R.  r7 = r6 + 0x22c
    ...D================================================eE-----------------------R.  r8 = r1 + 0xc8
    ....DeE----------------------------------------------------------------------R.  r9 = 0xa
    ....D===============================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x10] = r7
    ....DeeeeeeeeeeeeeeeE---------------------------------------------------------R  r0 = 870, jump 28055
```

Gas simulation at offset 29973 with total cost of 26:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  u8 [r6 + 566] = 0x7
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  u8 [r6 + 567] = 0x21
    DeE------------------------R.  r7 = r6 + 0x238
    .DeE-----------------------R.  r8 = r1 + 0xb8
    .DeE-----------------------R.  r9 = 0x10
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x8] = r7
    ..DeeeeeeeeeeeeeeeE---------R  r0 = 872, jump 28055
```

Gas simulation at offset 30003 with total cost of 100:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r7 = u64 [r1 + 0xa0]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r8 = u64 [r1 + 0xa8]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r9 = u64 [r1 + 0xb0]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r10 = u64 [r1 + 0x90]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  r11 = i32 [r1 + 0x98]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  r12 = u8 [r1 + 0x9c]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  u64 [r6 + 585] = 0
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  u64 [r6 + 0x251] = r7
    ..D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u64 [r6 + 0x259] = r8
    ..D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u64 [r6 + 0x261] = r9
    ..D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u64 [r6 + 0x269] = r10
    ..D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u32 [r6 + 0x271] = r11
    ...D========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x275] = a5
    ...D========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 630] = 0xfffffffffffffffd
    ...DeE------------------------------------------------------------------------------------------------R  r5 = 0x2
    ...D========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 631] = 0x24
    ....D=======================================================================eE------------------------R  r7 = r6 + 0x278
    ....DeE-----------------------------------------------------------------------------------------------R  r9 = 0xb
    ....DeE-----------------------------------------------------------------------------------------------R  r8 = 0
    .....DeeeeeeeeeeeeeeeE--------------------------------------------------------------------------------R  r0 = 874, jump 28080
```

Gas simulation at offset 30083 with total cost of 100:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r7 = i16 [r1 + 0x86]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r8 = i16 [r1 + 0x88]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r9 = i16 [r1 + 0x8a]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  r10 = i16 [r1 + 0x8c]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  r11 = i16 [r1 + 0x8e]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  r12 = u64 [r1 + 0x28]
    .D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u64 [r6 + 0x249] = r12
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R.........................  r12 = u64 [r1 + 0x38]
    ..D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u64 [r6 + 0x251] = r12
    ..D=======================eeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R.........................  u16 [r6 + 0x283] = r7
    ..D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u16 [r6 + 0x285] = r8
    ..D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u16 [r6 + 0x287] = r9
    ...D========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r6 + 0x289] = r10
    ...D========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r6 + 0x28b] = r11
    ...D========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 651] = 0x1
    ....D=======================================================================eE------------------------R  r7 = r1 + 0x2a8
    ....DeE-----------------------------------------------------------------------------------------------R  r9 = 0x16e
    ....DeE-----------------------------------------------------------------------------------------------R  r8 = 0
    .....DeeeeeeeeeeeeeeeE--------------------------------------------------------------------------------R  r0 = 876, jump 28080
```

Gas simulation at offset 30158 with total cost of 50:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r7 = u64 [r6 + 0x209]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u64 [r1 + 232] = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u32 [r1 + 240] = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u16 [r1 + 244] = 0
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 616] = 0
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r1 + 624] = 0
    .D========================eeeeeeeeeeeeeeeeeeeeE-----R  jump 30248 if r7 == 0
```

Gas simulation at offset 30185 with total cost of 27:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..  r5 = u64 [r1 + 0x40]
    D=========================eER.  r8 = r5 + 0x2750
    D==========================eER  r8 = r8 & 0xfffffffffffffffc
    .DeE-------------------------R  r9 = 0x1
    .DeeE------------------------R  fallthrough
```

Gas simulation at offset 30199 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  u64 [0x30000] = r4
    DeE---------------------------------------R............  r4 = r9 << 0x20
    .DeE--------------------------------------R............  r4 = r4 >>a 0x20
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R............  r10 = i32 [r8 + 0]
    .D=========================eE-------------R............  r4 = r10 | r4
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r8 + 0] = r4
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r4 = u64 [0x30000]
    ..D========================eE-------------------------R  r10 = r10 & 0xff
    ..D=========================eE------------------------R  jump 30199 if r10 != 0
```

Gas simulation at offset 30230 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  r0 = 878, jump 27398
```

Gas simulation at offset 30236 with total cost of 26:

```
    DeER.........................  r7 = r5 + 0x2000
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 1872] = 0
    DeE-------------------------R  r5 = 0x2
    .DeeE-----------------------R  fallthrough
```

Gas simulation at offset 30248 with total cost of 16:

```
    DeER...............  r7 = r6 + 0xa9
    DeER...............  r8 = r1 + 0x2a8
    .DeER..............  r9 = 0x16e
    .DeeeeeeeeeeeeeeeER  r0 = 880, jump 28055
```

Gas simulation at offset 30266 with total cost of 76:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...................................................  r7 = u64 [r1 + 0xe8]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...................................................  r8 = i32 [r1 + 0xf0]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...................................................  r9 = i16 [r1 + 0xf4]
    DeE------------------------R...................................................  r10 = 0x105
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  u16 [r6 + 0x217] = r10
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u64 [r6 + 0x219] = r7
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u32 [r6 + 0x221] = r8
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u16 [r6 + 0x225] = r9
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u16 [r6 + 551] = 0
    ..D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u16 [r6 + 553] = 0xc1
    ..D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u8 [r6 + 555] = 0
    ...D===============================================eE------------------------R.  r8 = r1 + 0x268
    ...DeE-----------------------------------------------------------------------R.  r9 = 0xa
    ...D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u64 [r1 + 0x10]
    ....DeeeeeeeeeeeeeeeE---------------------------------------------------------R  r0 = 882, jump 28055
```

Gas simulation at offset 30328 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 566] = 0x7
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 567] = 0x21
    DeE------------------------R  r9 = 0x10
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u64 [r1 + 0x8]
    .DeE-----------------------R  r8 = 0
    .DeeeeeeeeeeeeeeeE---------R  r0 = 884, jump 28080
```

Gas simulation at offset 30352 with total cost of 250:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.................................................................................................................................................................................................................................  u64 [r6 + 9] = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.................................................................................................................................................................................................................................  u64 [r6 + 17] = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.................................................................................................................................................................................................................................  u32 [r6 + 25] = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.................................................................................................................................................................................................................................  u16 [r6 + 29] = 0
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER........................................................................................................................................................................................................  u8 [r6 + 53] = 0
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER........................................................................................................................................................................................................  u8 [r6 + 54] = 0
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER........................................................................................................................................................................................................  u8 [r6 + 55] = 0
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER........................................................................................................................................................................................................  u64 [r6 + 57] = 0
    ..D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER...............................................................................................................................................................................  u16 [r6 + 129] = 0
    ..D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER...............................................................................................................................................................................  u8 [r6 + 131] = 0
    ..D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER...............................................................................................................................................................................  u8 [r6 + 133] = 0
    ..D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER...............................................................................................................................................................................  u16 [r6 + 135] = 0
    ...D========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER......................................................................................................................................................  u64 [r6 + 97] = 0
    ...D========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER......................................................................................................................................................  u64 [r6 + 105] = 0
    ...D========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER......................................................................................................................................................  u64 [r6 + 113] = 0
    ...D========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER......................................................................................................................................................  u64 [r6 + 121] = 0
    ....D================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.............................................................................................................................  u8 [r6 + 31] = 0
    ....D================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.............................................................................................................................  u64 [r6 + 33] = 0
    ....D================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.............................................................................................................................  u64 [r6 + 41] = 0
    ....D================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.............................................................................................................................  u32 [r6 + 49] = 0x1
    .....D========================================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER....................................................................................................  u64 [r6 + 65] = 0x10000
    .....D========================================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER....................................................................................................  r8 = u64 [r1 + 0x20]
    .....D=================================================================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  u64 [r6 + 0x49] = r8
    .....D========================================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R...........................................................................  u64 [r6 + 81] = 0x9
    ......D=======================================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R...........................................................................  u64 [r6 + 89] = 0
    ......DeE------------------------------------------------------------------------------------------------------------------------------------------------------------------------R...........................................................................  r8 = 0x10000000000
    ......D================================================================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  u32 [r6 + 157] = 0x1
    .......D===============================================================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  u16 [r6 + 161] = 0x200
    .......D===============================================================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................  u8 [r6 + 163] = 0
    .......D========================================================================================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  r7 = u64 [r1 + 0x18]
    .......D=================================================================================================================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u64 [r6 + 0x89] = r7
    ........D=======================================================================================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R.........................  u64 [r6 + 0x91] = r8
    ............................D===================================================================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R.........................  u16 [r6 + 153] = 0x8
    ............................D===================================================================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R.........................  u8 [r6 + 0x9b] = s0
    ............................D============================================================================================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u16 [r6 + 635] = 0
    ............................D============================================================================================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u16 [r6 + 637] = 0
    .....................................................D===================================================================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u16 [r6 + 639] = 0
    .....................................................DeE---------------------------------------------------------------------------------------------------------------------------------------------------------------------------R.........................  r8 = 0xff
    .....................................................D============================================================================================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  r5 = u64 [r1 + 0x30]
    .....................................................D.......................................................................................................................................................................................................  r7 = r5
    ......................................................DeeeeeeeeeeeeeeeE-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------R  r0 = 886, jump 22578
```

Gas simulation at offset 30508 with total cost of 15:

```
    DeER..............  r8 = 0xff
    D.................  r7 = r5
    DeeeeeeeeeeeeeeeER  r0 = 888, jump 22578
```

Gas simulation at offset 30520 with total cost of 15:

```
    DeER..............  r8 = 0xff
    D.................  r7 = r5
    DeeeeeeeeeeeeeeeER  r0 = 890, jump 22578
```

Gas simulation at offset 30532 with total cost of 15:

```
    DeER..............  r8 = 0x100
    D.................  r7 = r5
    DeeeeeeeeeeeeeeeER  r0 = 892, jump 22578
```

Gas simulation at offset 30544 with total cost of 15:

```
    DeER..............  r8 = 0x1ff
    D.................  r7 = r5
    DeeeeeeeeeeeeeeeER  r0 = 894, jump 22578
```

Gas simulation at offset 30556 with total cost of 15:

```
    DeER..............  r8 = 0x1fe
    D.................  r7 = r5
    DeeeeeeeeeeeeeeeER  r0 = 896, jump 22578
```

Gas simulation at offset 30568 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 630] = 0xfffffffffffffffd
    DeE------------------------R  r8 = 0xfffc
    D...........................  r7 = r5
    DeeeeeeeeeeeeeeeE----------R  r0 = 898, jump 22578
```

Gas simulation at offset 30586 with total cost of 26:

```
    DeER.........................  r7 = r7 & 0xff
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x40] = r7
    DeE-------------------------R  r8 = 0xfffd
    D............................  r7 = r5
    .DeeeeeeeeeeeeeeeE----------R  r0 = 900, jump 22578
```

Gas simulation at offset 30606 with total cost of 51:

```
    DeER..................................................  r7 = r7 << 0x8
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r8 = u64 [r1 + 0x40]
    D=========================eER.........................  r7 = r7 | r8
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u16 [r6 + 0x271] = r7
    .DeeeeeeeeeeeeeeeE-----------------------------------R  r0 = 902, jump 5507
```

Gas simulation at offset 30625 with total cost of 2:

```
    DeER.  r7 = r7 & 0x1
    D=eER  jump 30803 if r7 != 0
```

Gas simulation at offset 30632 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  r0 = 904, jump 5507
```

Gas simulation at offset 30638 with total cost of 2:

```
    DeER.  r7 = r7 & 0x1
    D=eER  jump 30803 if r7 != 0
```

Gas simulation at offset 30645 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  r0 = 906, jump 5507
```

Gas simulation at offset 30651 with total cost of 2:

```
    DeER.  r7 = r7 & 0x1
    D=eER  jump 30803 if r7 != 0
```

Gas simulation at offset 30658 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  r0 = 908, jump 5507
```

Gas simulation at offset 30664 with total cost of 2:

```
    DeER.  r7 = r7 & 0x1
    D=eER  jump 30803 if r7 != 0
```

Gas simulation at offset 30671 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r7 = u8 [r6 + 0x287]
    D=========================eE--------------R...........  r7 = r7 | 0x4
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x287] = a0
    .DeeeeeeeeeeeeeeeE-----------------------------------R  r0 = 910, jump 5507
```

Gas simulation at offset 30689 with total cost of 2:

```
    DeER.  r7 = r7 & 0x1
    D=eER  jump 30803 if r7 != 0
```

Gas simulation at offset 30695 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r7 = u8 [r6 + 0x287]
    D=========================eE--------------R...........  r7 = r7 & 0xfb
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x287] = a0
    .DeeeeeeeeeeeeeeeE-----------------------------------R  r0 = 912, jump 5507
```

Gas simulation at offset 30714 with total cost of 2:

```
    DeER.  r7 = r7 & 0x1
    D=eER  jump 30803 if r7 != 0
```

Gas simulation at offset 30720 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  r0 = 914, jump 5507
```

Gas simulation at offset 30726 with total cost of 2:

```
    DeER.  r7 = r7 & 0x1
    D=eER  jump 30803 if r7 != 0
```

Gas simulation at offset 30732 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  r0 = 916, jump 5507
```

Gas simulation at offset 30738 with total cost of 2:

```
    DeER.  r7 = r7 & 0x1
    D=eER  jump 30803 if r7 != 0
```

Gas simulation at offset 30744 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r7 = u8 [r6 + 0x287]
    D=========================eE--------------R...........  r7 = r7 | 0x4
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x287] = a0
    .DeeeeeeeeeeeeeeeE-----------------------------------R  r0 = 918, jump 5507
```

Gas simulation at offset 30762 with total cost of 2:

```
    DeER.  r7 = r7 & 0x1
    D=eER  jump 30803 if r7 != 0
```

Gas simulation at offset 30768 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r7 = u8 [r6 + 0x287]
    D=========================eE--------------R...........  r7 = r7 & 0xfb
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r6 + 0x287] = a0
    .DeE-------------------------------------------------R  r1 = r1 + 0x2f0
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeE------------------------R  r0 = u64 [r1 + 0x7f0]
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeE------------------------R  r5 = u64 [r1 + 0x7e8]
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeE------------------------R  r6 = u64 [r1 + 0x7e0]
    ..D=========================eE-----------------------R  r1 = r1 + 0x7f8
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeE--R  jump [r0 + 0]
```

Gas simulation at offset 30803 with total cost of 2:

```
    DeeER  trap
```

Gas simulation at offset 30804 with total cost of 25:

```
    DeER........................  r7 = r1 + 0x2a8
    DeER........................  r9 = 0x4000
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = u64 [r1 + 0x18]
    .DeeeeeeeeeeeeeeeE---------R  r0 = 920, jump 32330
```

Gas simulation at offset 30821 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u64 [r1 + 0x2b0]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r5 = u64 [r1 + 0x2b8]
    DeeeeeeeeeeeeeeeE----------R  jump 28722
```

Gas simulation at offset 30832 with total cost of 52:

```
    DeER...................................................  r1 = r1 + 0xfffffffffffffff8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  u64 [r1 + 0] = r0
    DeE-------------------------R..........................  r0 = 0x39a
    D=eE------------------------R..........................  r1 = r1 + 0xfffffffffffff808
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u64 [r1 + 0x7f0] = r0
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u64 [r1 + 0x7e8] = r5
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u64 [r1 + 0x7e0] = r6
    .D=========================eER.........................  r1 = r1 + 0xfffffffffffffd10
    ..DeE------------------------R.........................  r8 = 0xb3200
    ..DeE------------------------R.........................  r5 = 0x30a98
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x38] = r8
    ...D========================eE------------------------R  r7 = r5 + 0x2750
    ...D=========================eE-----------------------R  r7 = r7 & 0xfffffffffffffffc
    ...DeE------------------------------------------------R  r8 = 0x1
    ....DeeeeeeeeeeeeeeeE---------------------------------R  jump 28099
```

Gas simulation at offset 30887 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r0 = u64 [r1 + 0]
    DeE------------------------R......................  r1 = r1 + 0x8
    D=========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 30894 with total cost of 2:

```
    DeER.  r7 = r7 & 0x1
    D=eER  jump 31088 if r7 != 0
```

Gas simulation at offset 30901 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeE---------------------------------------R  r6 = 0x30008
    D=eE--------------------------------------R  r7 = r6 + 0x7ff
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeE-------------R  r5 = u64 [r7 + 0x209]
    .D==========================eE------------R  jump 31021 if r5 != 0
```

Gas simulation at offset 30918 with total cost of 26:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  u64 [r1 + 0] = r7
    DeE------------------------R.  r8 = 0x30a98
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x8] = r8
    .DeE------------------------R  r7 = r8 + 0x2750
    .D=eE-----------------------R  r7 = r7 & 0xfffffffffffffffc
    .DeE------------------------R  r8 = 0x1
    ..DeeE----------------------R  fallthrough
```

Gas simulation at offset 30939 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  u64 [0x30000] = r4
    DeE---------------------------------------R............  r4 = r8 << 0x20
    .DeE--------------------------------------R............  r4 = r4 >>a 0x20
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R............  r9 = i32 [r7 + 0]
    .D=========================eE-------------R............  r4 = r9 | r4
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r7 + 0] = r4
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r4 = u64 [0x30000]
    ..D========================eE-------------------------R  r9 = r9 & 0xff
    ..D=========================eE------------------------R  jump 30939 if r9 != 0
```

Gas simulation at offset 30970 with total cost of 15:

```
    DeER..............  r7 = 0xf00
    DeER..............  r8 = 0
    DeeeeeeeeeeeeeeeER  r0 = 926, jump 26592
```

Gas simulation at offset 30982 with total cost of 51:

```
    D.....................................................  r5 = r7
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r8 = u64 [r1 + 0x8]
    D=========================eER.........................  r7 = r8 + 0x2000
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 1872] = 0
    .DeE-------------------------------------------------R  jump 32329 if r5 == 0
```

Gas simulation at offset 30999 with total cost of 15:

```
    DeER..............  r9 = 0x1e000
    D.................  r7 = r5
    DeER..............  r8 = 0
    DeeeeeeeeeeeeeeeER  r0 = 928, jump 28080
```

Gas simulation at offset 31014 with total cost of 50:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r7 = u64 [r1 + 0]
    D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r7 + 0x209] = r5
    DeeE------------------------------------------------R  fallthrough
```

Gas simulation at offset 31021 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r8 = u64 [r6 + 0]
    D=========================eE--------------R  jump 31089 if r8 == 0
```

Gas simulation at offset 31027 with total cost of 2:

```
    DeER.  r11 = 0x3bffc
    DeER.  r9 = 0x200
    DeER.  r10 = 0x173f4
    DeeER  fallthrough
```

Gas simulation at offset 31042 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u16 [r5 + 0]
    D=========================eE--------------R  jump 31090 if r7 >=u r9
```

Gas simulation at offset 31048 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    D......................................................  r12 = r11
    DeE---------------------------------------R............  r7 = r7 << 0x2
    D=eE--------------------------------------R............  r7 = r7 + r10
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeE-------------R............  r7 = i32 [r7 + 0]
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r8 + 0] = r7
    .DeE--------------------------------------------------R  r11 = r11 + 0xfffffffffffffffc
    .DeE--------------------------------------------------R  r8 = r8 + 0x4
    ..DeE-------------------------------------------------R  r5 = r5 + 0x2
    ..DeE-------------------------------------------------R  jump 31042 if r12 != 0
```

Gas simulation at offset 31073 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.......  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r0 = u64 [r1 + 0x20]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r5 = u64 [r1 + 0x18]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r6 = u64 [r1 + 0x10]
    .DeE--------------------------------------R.......  r1 = r1 + 0x28
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 31088 with total cost of 2:

```
    DeeER  trap
```

Gas simulation at offset 31089 with total cost of 2:

```
    DeeER  trap
```

Gas simulation at offset 31090 with total cost of 2:

```
    DeeER  trap
```

Gas simulation at offset 31091 with total cost of 27:

```
    DeER..........................  r1 = r1 + 0xfffffffffffffff8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.  u64 [r1 + 0] = r0
    DeE-------------------------R.  r0 = 0x3a2
    D=eE------------------------R.  r1 = r1 + 0xffffffffffffffd8
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x20] = r0
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x18] = r5
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x10] = r6
    .DeE-------------------------R  r0 = 0x39c
    ..DeeeeeeeeeeeeeeeE----------R  jump 5507
```

Gas simulation at offset 31119 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r0 = u64 [r1 + 0]
    DeE------------------------R......................  r1 = r1 + 0x8
    D=========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 31126 with total cost of 21:

```
    DeER....................  r9 = 0x1
    DeER....................  r10 = 0x1fffffffe0
    D=eeeeeeeeeeeeeeeeeeeeER  jump 31147 if r10 >=u r8
```

Gas simulation at offset 31142 with total cost of 15:

```
    DeER..............  r7 = 0
    DeeeeeeeeeeeeeeeER  jump 32638
```

Gas simulation at offset 31147 with total cost of 26:

```
    DeER.........................  r1 = r1 + 0xffffffffffffffa8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x50] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x48] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x40] = r6
    .DeE------------------------R  r5 = 0x30a98
    .D=eE-----------------------R  r10 = r5 + 0x2750
    .D==eE----------------------R  r10 = r10 & 0xfffffffffffffffc
    ..DeeE----------------------R  fallthrough
```

Gas simulation at offset 31172 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  u64 [0x30000] = r4
    DeE---------------------------------------R............  r4 = r9 << 0x20
    .DeE--------------------------------------R............  r4 = r4 >>a 0x20
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R............  r11 = i32 [r10 + 0]
    .D=========================eE-------------R............  r4 = r11 | r4
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r10 + 0] = r4
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r4 = u64 [0x30000]
    ..D========================eE-------------------------R  r11 = r11 & 0xff
    ..D=========================eE------------------------R  jump 31172 if r11 != 0
```

Gas simulation at offset 31203 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.......  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r9 = u32 [r7 + 0xffffffffffffffe4]
    DeE---------------------------------------R.......  r8 = r8 + 0x1f
    .DeE--------------------------------------R.......  r3 = r8 >> 0x5
    ..DeeE------------------------------------R.......  i32 r8 = r3 + 0
    ..D=======================eE--------------R.......  r9 = r9 >> 0x1
    ...D=======================eE-------------R.......  r6 = r9 + 0xffffffffffffffff
    ...D========================eeeeeeeeeeeeeeeeeeeeER  jump 31429 if r6 == r8
```

Gas simulation at offset 31225 with total cost of 1:

```
    DeER  jump 31340 if r8 >=u r6
```

Gas simulation at offset 31228 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeE---------------------------------------R  r2 = r7 + 0xffffffffffffffe0
    .DeE--------------------------------------R  r11 = r2 << 0x20
    .D=eE-------------------------------------R  r11 = r11 >> 0x20
    .D==eeeeeeeeeeeeeeeeeeeeeeeeeE------------R  r10 = u32 [r11 + 0x4]
    ..DeeE------------------------------------R  i32 r9 = r3 + 0x1
    ..D==========================eE-----------R  r10 = r10 >> 0x1
    ...D==========================eE----------R  jump 31429 if r9 >=u r10
```

Gas simulation at offset 31251 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeE---------------------------------------R  r12 = r9 << 0x1
    D=eE--------------------------------------R  r12 = r12 + 0x1
    .DeE--------------------------------------R  r6 = r5 + 0x2000
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeE-------------R  u32 [r11 + 0x4] = r12
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeE-------------R  r11 = i32 [r6 + 0x600]
    ..DeE-------------------------------------R  r12 = 0x80000
    ..DeE-------------------------------------R  r6 = r10 << 0x5
    ...D========================eeE-----------R  i32 r4 = r11 + r12
    ....DeeE----------------------------------R  i32 r6 = r6 + r2
    .....DeeE---------------------------------R  i32 r0 = r10 - r9
    .....D========================eE----------R  jump 31792 if r6 >=u r4
```

Gas simulation at offset 31290 with total cost of 48:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER........  unlikely
    D..................................................  r8 = r5
    DeE---------------------------------------R........  r5 = r6 << 0x20
    .DeE--------------------------------------R........  r5 = r5 >> 0x20
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeE-------------R........  r11 = u32 [r5 + 0x4]
    .D==========================eE------------R........  r12 = r11 & 0x1
    ..D==========================eeeeeeeeeeeeeeeeeeeeER  jump 31626 if r12 != 0
```

Gas simulation at offset 31309 with total cost of 26:

```
    DeER.........................  r10 = r11 >> 0x1
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x38] = r10
    DeeeeeeeeeeeeeeeeeeeeE------R  jump 31631 if r11 == 0
```

Gas simulation at offset 31319 with total cost of 20:

```
    DeER...................  r3 = 0x2000000
    D=eeeER................  r3 = minu(r10, r3)
    DeeeeeeeeeeeeeeeeeeeeER  jump 31635 if r11 >=u 256
```

Gas simulation at offset 31334 with total cost of 15:

```
    DeER..............  r3 = r3 + 0xffffffffffffffff
    DeeeeeeeeeeeeeeeER  jump 31661
```

Gas simulation at offset 31340 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x38] = r5
    DeE------------------------R  r9 = 0xffffffff
    D=eE-----------------------R  jump 31406 if r3 != r9
```

Gas simulation at offset 31356 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x30] = r7
    D...........................  r7 = r8
    DeE------------------------R  r8 = 0
    DeeeeeeeeeeeeeeeE----------R  r0 = 932, jump 26592
```

Gas simulation at offset 31369 with total cost of 20:

```
    DeeeeeeeeeeeeeeeeeeeeER  jump 31425 if r7 == 0
```

Gas simulation at offset 31372 with total cost of 26:

```
    DeER.........................  r9 = r6 << 0x25
    D=eER........................  r9 = r9 >> 0x20
    D............................  r5 = r7
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0x30]
    .D...........................  r8 = r6
    .DeeeeeeeeeeeeeeeE----------R  r0 = 934, jump 28055
```

Gas simulation at offset 31391 with total cost of 15:

```
    D.................  r7 = r6
    DeeeeeeeeeeeeeeeER  r0 = 936, jump 27398
```

Gas simulation at offset 31399 with total cost of 25:

```
    D...........................  r7 = r5
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r5 = u64 [r1 + 0x38]
    DeeeeeeeeeeeeeeeE----------R  jump 31429
```

Gas simulation at offset 31406 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeE---------------------------------------R  r9 = r7 + 0xffffffffffffffe0
    .DeE--------------------------------------R  r5 = r9 << 0x20
    .D=eE-------------------------------------R  r5 = r5 >> 0x20
    .D==eeeeeeeeeeeeeeeeeeeeeeeeeE------------R  r10 = u32 [r5 + 0x4]
    ..D==========================eE-----------R  r2 = r10 >> 0x1
    ..D===========================eE----------R  jump 31451 if r8 >=u r2
```

Gas simulation at offset 31425 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r5 = u64 [r1 + 0x38]
    DeeE-----------------------R  fallthrough
```

Gas simulation at offset 31429 with total cost of 47:

```
    DeER..............................................  r8 = r5 + 0x2000
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.....................  u8 [r8 + 1872] = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeE-R.....................  r0 = u64 [r1 + 0x50]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER.....................  r5 = u64 [r1 + 0x48]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER.....................  r6 = u64 [r1 + 0x40]
    .D========================eER.....................  r1 = r1 + 0x58
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 31451 with total cost of 78:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER......................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R......................................  r11 = u64 [r1 + 0x38]
    D=========================eE--------------R......................................  r10 = r11 + 0x2000
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER...........................  r4 = u64 [r10 + 0x600]
    .DeE-------------------------------------------------R...........................  r11 = r2 << 0x5
    ..D=================================================eeER.........................  i32 r10 = r4 + 0x80000
    ...DeeE------------------------------------------------R.........................  i32 r11 = r11 + r9
    ...D==================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x30] = r10
    ...D==================================================eE------------------------R  jump 31356 if r11 >=u r10
```

Gas simulation at offset 31480 with total cost of 48:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER........  unlikely
    DeE---------------------------------------R........  r12 = r11 << 0x20
    D=eE--------------------------------------R........  r12 = r12 >> 0x20
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeE-------------R........  r0 = u32 [r12 + 0x4]
    .D==========================eE------------R........  r10 = r0 & 0x1
    .D===========================eeeeeeeeeeeeeeeeeeeeER  jump 31356 if r10 != 0
```

Gas simulation at offset 31497 with total cost of 26:

```
    DeER.........................  r10 = r0 >> 0x1
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x20] = r10
    .DeeE-----------------------R  i32 r10 = r10 + r2
    .D==eeeeeeeeeeeeeeeeeeeeE---R  jump 31356 if r8 >=u r10
```

Gas simulation at offset 31510 with total cost of 97:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER........................................................................  u64 [r1 + 0] = r12
    DeeE-----------------------R........................................................................  i32 r12 = r3 + 0x1
    .D=eE----------------------R........................................................................  r3 = r12 << 0x5
    .D==eeeeeeeeeeeeeeeeeeeeeeeeeER.....................................................................  u64 [r1 + 0x10] = r3
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--R.....................................................................  u64 [r1 + 0x8] = r10
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-R.....................................................................  u64 [r1 + 0x28] = r12
    ..D=======================eE--R.....................................................................  r10 = r10 ^ r12
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..............................................  u64 [r1 + 0x18] = r10
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..............................................  r10 = u64 [r1 + 0x38]
    ...DeE-----------------------------------------------R..............................................  r12 = 0x2000
    ...D================================================eER.............................................  r10 = r10 + r12
    ...D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.............................................  r2 = u64 [r1 + 0x10]
    ...D=================================================eER............................................  r2 = r2 + r9
    ....D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER....................  r3 = i32 [r10 + 0x748]
    ....D=================================================eeE----------------------R....................  i32 r10 = r2 - r4
    .....D..............................................................................................  r4 = r2
    .....D==================================================eeE--------------------R....................  i32 r2 = r10 >> 0x5
    ......D======================eeeeeeeeeeeeeeeeeeeeeeeeeE------------------------R....................  r10 = u64 [r1 + 0x18]
    ......D===============================================eeeE---------------------R....................  r10 = r10 >u 0
    .......D==================================================eE-------------------R....................  r2 = r2 + r10
    .......D======================================================================eeeeeeeeeeeeeeeeeeeeER  jump 31593 if r3 >=u r2
```

Gas simulation at offset 31572 with total cost of 2:

```
    DeER.  r10 = 0x4001
    D=eER  jump 31356 if r2 >=u r10
```

Gas simulation at offset 31580 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r10 = u64 [r1 + 0x38]
    D=========================eE--------------R...........  r8 = r10 + 0x2000
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r8 + 0x748] = r2
    .DeeE------------------------------------------------R  fallthrough
```

Gas simulation at offset 31593 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x10] = r4
    DeeeeeeeeeeeeeeeeeeeeE-----R  jump 31971 if r0 == 0
```

Gas simulation at offset 31600 with total cost of 28:

```
    DeER...........................  r8 = 0x2000000
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...  r6 = u64 [r1 + 0x20]
    D=========================eeeER  r8 = minu(r6, r8)
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--R  r12 = u64 [r1 + 0]
    .DeeeeeeeeeeeeeeeeeeeeE-------R  jump 31977 if r0 >=u 256
```

Gas simulation at offset 31620 with total cost of 15:

```
    DeER..............  r3 = r8 + 0xffffffffffffffff
    DeeeeeeeeeeeeeeeER  jump 32003
```

Gas simulation at offset 31626 with total cost of 15:

```
    D.................  r5 = r8
    DeeeeeeeeeeeeeeeER  jump 31792
```

Gas simulation at offset 31631 with total cost of 15:

```
    DeER..............  r3 = 0
    DeeeeeeeeeeeeeeeER  jump 31661
```

Gas simulation at offset 31635 with total cost of 10:

```
    DeER.........  i32 r10 = clz r3
    .DeeeER......  i32 r11 = 0x18 - r10
    ..D==eeER....  i32 r11 = r3 >> r11
    ...D===eER...  r11 = r11 & 0x7f
    ...DeE---R...  r10 = r10 << 0x7
    ...D====eER..  r11 = r11 - r10
    ....D====eER.  r10 = r11 + 0x7ff
    ....D=====eER  r3 = r10 + 0x480
    .....DeeE---R  fallthrough
```

Gas simulation at offset 31661 with total cost of 29:

```
    DeER............................  r10 = r3 << 0x20
    D=eER...........................  r10 = r10 >> 0x1e
    .D=eER..........................  r11 = r8 + r10
    .D==eeeeeeeeeeeeeeeeeeeeeeeeeER.  r10 = i32 [r11 + 0]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--R.  r12 = u32 [r5 + 0x8]
    ..D==========================eER  jump 31696 if r10 != r6
```

Gas simulation at offset 31678 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r11 + 0] = r12
    DeE------------------------R  jump 31719 if r12 == 0
```

Gas simulation at offset 31683 with total cost of 27:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..  u32 [r12 + 12] = 0
    D.............................  r5 = r8
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u64 [r1 + 0x38]
    .D========================eeER  i32 r0 = r8 + r0
    .DeeeeeeeeeeeeeeeE-----------R  jump 31792
```

Gas simulation at offset 31696 with total cost of 50:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........  r11 = u32 [r5 + 0xc]
    D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r11 + 0x8] = r12
    D....................................................  r5 = r8
    .DeeeeeeeeeeeeeeeeeeeeE-----------------------------R  jump 31785 if r12 == 0
```

Gas simulation at offset 31708 with total cost of 27:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..  u32 [r12 + 0xc] = r11
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u64 [r1 + 0x38]
    D=========================eeER  i32 r0 = r8 + r0
    .DeeeeeeeeeeeeeeeE-----------R  jump 31792
```

Gas simulation at offset 31719 with total cost of 55:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...............  unlikely
    DeeE--------------------------------------R...............  i32 r6 = r3 >> 0x6
    .D=eE-------------------------------------R...............  r10 = r6 << 0x3
    .DeE--------------------------------------R...............  r11 = r8 + 0x2000
    ..D=eE------------------------------------R...............  r10 = r10 + r11
    ..D==eeeeeeeeeeeeeeeeeeeeeeeeeE-----------R...............  r5 = u64 [r10 + 0x608]
    ..DeE-------------------------------------R...............  r12 = r3 & 0x3f
    ...DeE------------------------------------R...............  r11 = 0xfffffffffffffffe
    ...D=eE-----------------------------------R...............  r12 = r11 <<r r12
    ....D=========================eE----------R...............  r12 = r12 & r5
    ....D.....................................................  r5 = r8
    ....D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r10 + 0x608] = r12
    ....D==========================eE------------------------R  jump 31785 if r12 != 0
```

Gas simulation at offset 31758 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeE---------------------------------------R............  r10 = r5 + 0x2000
    D=eeeeeeeeeeeeeeeeeeeeeeeeeE--------------R............  r12 = u64 [r10 + 0x738]
    .DeE--------------------------------------R............  r11 = r11 <<r r6
    .D=========================eE-------------R............  r11 = r11 & r12
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r10 + 0x738] = r11
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r8 = u64 [r1 + 0x38]
    ..D=========================eeE-----------------------R  i32 r0 = r8 + r0
    ..DeeeeeeeeeeeeeeeE-----------------------------------R  jump 31792
```

Gas simulation at offset 31785 with total cost of 27:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..  r8 = u64 [r1 + 0x38]
    D=========================eeER  i32 r0 = r8 + r0
    DeeE-------------------------R  fallthrough
```

Gas simulation at offset 31792 with total cost of 20:

```
    DeeeeeeeeeeeeeeeeeeeeER  jump 31947 if r0 == 0
```

Gas simulation at offset 31796 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x38] = r4
    DeE------------------------R  r12 = r9 << 0x5
    .DeE-----------------------R  r3 = r12 + r2
    .D..........................  r11 = r0
    .DeE-----------------------R  jump 31849 if r0 <=u 127
```

Gas simulation at offset 31811 with total cost of 15:

```
    DeER..............  r8 = 0x2000000
    D=eeeER...........  r8 = minu(r0, r8)
    D====eER..........  i32 r11 = clz r8
    .D====eeeER.......  i32 r10 = 0x18 - r11
    ..D======eeER.....  i32 r8 = r8 >> r10
    ..D========eER....  r8 = r8 & 0x7f
    ...D==eE-----R....  r11 = r11 << 0x7
    ...D========eER...  r8 = r8 - r11
    ...D=========eER..  r8 = r8 + 0x7ff
    ....D=========eER.  r11 = r8 + 0x480
    ....D==========eER  r11 = r11 + 0x1
    ....DeeE---------R  fallthrough
```

Gas simulation at offset 31849 with total cost of 54:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..............  unlikely
    DeeE--------------------------------------R..............  i32 r8 = r11 + 0xffffffffffffffff
    .DeE--------------------------------------R..............  r10 = r0 << 0x1
    .DeE--------------------------------------R..............  r12 = r3 << 0x20
    ..DeE-------------------------------------R..............  r11 = r8 << 0x2
    ..D......................................................  r4 = r5
    ..D=eE------------------------------------R..............  r11 = r11 + r5
    ...D=eeeeeeeeeeeeeeeeeeeeeeeeeE-----------R..............  r5 = u32 [r11 + 0]
    ...D=eeeeeeeeeeeeeeeeeeeeeeeeeE-----------R..............  u32 [r11 + 0] = r3
    ....DeeE----------------------------------R..............  i32 r6 = r8 >> 0x6
    .....DeE----------------------------------R..............  r11 = r8 & 0x3f
    .....D=eE---------------------------------R..............  r12 = r12 >> 0x20
    .....D==eeeeeeeeeeeeeeeeeeeeeeeeeE--------R..............  u32 [r12 + 0] = r9
    ......D=eeeeeeeeeeeeeeeeeeeeeeeeeE--------R..............  u32 [r12 + 0x4] = r10
    ......D=======================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r12 + 0x8] = r5
    ......D=======================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r12 + 12] = 0
    ......D==========================eE---------------------R  jump 31898 if r5 == 0
```

Gas simulation at offset 31894 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r5 + 0xc] = r3
    DeeE-----------------------R  fallthrough
```

Gas simulation at offset 31898 with total cost of 55:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...............  unlikely
    DeE---------------------------------------R...............  r8 = r6 << 0x3
    .DeE--------------------------------------R...............  r12 = r4 + 0x2000
    .D=eE-------------------------------------R...............  r8 = r8 + r12
    .D==eeeeeeeeeeeeeeeeeeeeeeeeeE------------R...............  r12 = u64 [r8 + 0x608]
    ..DeE-------------------------------------R...............  r11 = 0x1 << r11
    ..D==========================eE-----------R...............  r11 = r11 | r12
    ...D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u64 [r8 + 0x608] = r11
    ...DeE--------------------------------------------------R.  r10 = r4 + 0x2000
    ...D=eeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R.  r8 = u64 [r10 + 0x738]
    ....DeE-------------------------------------------------R.  r11 = 0x1 << r6
    ....D.....................................................  r5 = r4
    .....D========================eE------------------------R.  r8 = r8 | r11
    .....D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r10 + 0x738] = r8
    .....DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r4 = u64 [r1 + 0x38]
    .....DeeE------------------------------------------------R  fallthrough
```

Gas simulation at offset 31947 with total cost of 24:

```
    DeER.......................  r9 = r9 + r0
    D=eER......................  r9 = r9 << 0x5
    .D=eeER....................  i32 r8 = r9 + r2
    .D===eeeeeeeeeeeeeeeeeeeeER  jump 31429 if r8 >=u r4
```

Gas simulation at offset 31960 with total cost of 27:

```
    DeER..........................  r8 = r8 << 0x20
    D=eER.........................  r8 = r8 >> 0x20
    D==eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r8 + 0] = r0
    DeeeeeeeeeeeeeeeE------------R  jump 31429
```

Gas simulation at offset 31971 with total cost of 25:

```
    DeER........................  r3 = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r12 = u64 [r1 + 0]
    DeeeeeeeeeeeeeeeE----------R  jump 32003
```

Gas simulation at offset 31977 with total cost of 10:

```
    DeER.........  i32 r10 = clz r8
    .DeeeER......  i32 r6 = 0x18 - r10
    ..D==eeER....  i32 r8 = r8 >> r6
    ..D====eER...  r8 = r8 & 0x7f
    ...DeE---R...  r10 = r10 << 0x7
    ...D====eER..  r8 = r8 - r10
    ...D=====eER.  r8 = r8 + 0x7ff
    ....D=====eER  r3 = r8 + 0x480
    ....DeeE----R  fallthrough
```

Gas simulation at offset 32003 with total cost of 52:

```
    DeER...................................................  r8 = r3 << 0x20
    D=eER..................................................  r8 = r8 >> 0x1e
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...........................  r10 = u64 [r1 + 0x38]
    .D========================eER..........................  r8 = r8 + r10
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER.  r4 = i32 [r8 + 0]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R.  r6 = u32 [r12 + 0x8]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R.  r0 = u64 [r1 + 0x8]
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE------------------------R.  r10 = u64 [r1 + 0x28]
    ..D=========================eeE----------------------R.  i32 r2 = r0 - r10
    ...D================================================eER  jump 32042 if r4 != r11
```

Gas simulation at offset 32032 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r8 + 0] = r6
    DeE------------------------R  jump 32057 if r6 == 0
```

Gas simulation at offset 32037 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r6 + 12] = 0
    DeeeeeeeeeeeeeeeE----------R  jump 32120
```

Gas simulation at offset 32042 with total cost of 50:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........  r8 = u32 [r12 + 0xc]
    D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r8 + 0x8] = r6
    DeE-------------------------------------------------R  jump 32120 if r6 == 0
```

Gas simulation at offset 32052 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r6 + 0xc] = r8
    DeeeeeeeeeeeeeeeE----------R  jump 32120
```

Gas simulation at offset 32057 with total cost of 79:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.......................................  unlikely
    DeeE--------------------------------------R.......................................  i32 r11 = r3 >> 0x6
    .D=eE-------------------------------------R.......................................  r8 = r11 << 0x3
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......................................  r10 = u64 [r1 + 0x38]
    .D=========================eE-------------R.......................................  r10 = r10 + 0x2000
    ..D=========================eE------------R.......................................  r8 = r8 + r10
    ..D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r6 = u64 [r8 + 0x608]
    ..DeE--------------------------------------------------R..........................  r12 = r3 & 0x3f
    ...DeE-------------------------------------------------R..........................  r10 = 0xfffffffffffffffe
    ...D=eE------------------------------------------------R..........................  r12 = r10 <<r r12
    ....D=================================================eER.........................  r12 = r12 & r6
    ....D==================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r8 + 0x608] = r12
    ....D==================================================eE------------------------R  jump 32120 if r12 != 0
```

Gas simulation at offset 32097 with total cost of 77:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.....................................  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.....................................  r8 = u64 [r1 + 0x38]
    D=========================eE--------------R.....................................  r4 = r8 + 0x2000
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r8 = u64 [r4 + 0x738]
    .DeE-------------------------------------------------R..........................  r10 = r10 <<r r11
    .D==================================================eER.........................  r8 = r8 & r10
    ..D==================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r4 + 0x738] = r8
    ..DeeE-------------------------------------------------------------------------R  fallthrough
```

Gas simulation at offset 32120 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  r4 = u64 [r1 + 0x28]
    D=========================eE--------------R............  r8 = r4 << 0x1
    .D=========================eE-------------R............  r8 = r8 + 0x1
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r5 + 0x4] = r8
    .DeeeeeeeeeeeeeeeeeeeeE-------------------------------R  jump 32283 if r2 == 0
```

Gas simulation at offset 32137 with total cost of 1:

```
    D...  r10 = r2
    DeER  jump 32181 if r2 <=u 127
```

Gas simulation at offset 32143 with total cost of 15:

```
    DeER..............  r8 = 0x2000000
    D=eeeER...........  r8 = minu(r2, r8)
    D====eER..........  i32 r11 = clz r8
    .D====eeeER.......  i32 r10 = 0x18 - r11
    ..D======eeER.....  i32 r8 = r8 >> r10
    ..D========eER....  r8 = r8 & 0x7f
    ...D==eE-----R....  r11 = r11 << 0x7
    ...D========eER...  r8 = r8 - r11
    ...D=========eER..  r8 = r8 + 0x7ff
    ....D=========eER.  r10 = r8 + 0x480
    ....D==========eER  r10 = r10 + 0x1
    ....DeeE---------R  fallthrough
```

Gas simulation at offset 32181 with total cost of 79:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.......................................  unlikely
    DeeE--------------------------------------R.......................................  i32 r8 = r10 + 0xffffffffffffffff
    .DeE--------------------------------------R.......................................  r3 = r2 << 0x1
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......................................  r6 = u64 [r1 + 0x10]
    ..D========================eE-------------R.......................................  r5 = r6 << 0x20
    ..DeE-------------------------------------R.......................................  r10 = r8 << 0x2
    ...DeeeeeeeeeeeeeeeeeeeeeeeeeE------------R.......................................  r11 = u64 [r1 + 0x38]
    ...D=========================eE-----------R.......................................  r10 = r10 + r11
    ...D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r12 = u32 [r10 + 0]
    ...D==================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.  u32 [r10 + 0] = r6
    ....DeeE------------------------------------------------------------------------R.  i32 r10 = r8 >> 0x6
    .....DeE------------------------------------------------------------------------R.  r11 = r8 & 0x3f
    .....D======================eE--------------------------------------------------R.  r5 = r5 >> 0x20
    .....D=======================eeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R.  u32 [r5 + 0] = r4
    ......D======================eeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R.  u32 [r5 + 0x4] = r3
    ......D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r5 + 0x8] = r12
    ......D======================eeeeeeeeeeeeeeeeeeeeeeeeeE--------------------------R  u32 [r5 + 12] = 0
    ......D================================================eeeeeeeeeeeeeeeeeeeeE-----R  jump 32234 if r12 == 0
```

Gas simulation at offset 32230 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r12 + 0xc] = r6
    DeeE-----------------------R  fallthrough
```

Gas simulation at offset 32234 with total cost of 78:

```
    DeER.............................................................................  r8 = r10 << 0x3
    DeER.............................................................................  r3 = 0x2000
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.....................................................  r6 = u64 [r1 + 0x38]
    .D========================eER....................................................  r12 = r6 + r3
    .D=========================eER...................................................  r8 = r8 + r12
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r12 = u64 [r8 + 0x608]
    ..DeE-------------------------------------------------R..........................  r11 = 0x1 << r11
    ..D==================================================eER.........................  r11 = r11 | r12
    ...D==================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r8 + 0x608] = r11
    ...D======================eE----------------------------------------------------R  r6 = r6 + r3
    ...D=======================eeeeeeeeeeeeeeeeeeeeeeeeeE---------------------------R  r8 = u64 [r6 + 0x738]
    ....DeE-------------------------------------------------------------------------R  r10 = 0x1 << r10
    ....D===============================================eE--------------------------R  r8 = r8 | r10
    .....D===============================================eeeeeeeeeeeeeeeeeeeeeeeeeE-R  u64 [r6 + 0x738] = r8
    .....DeeeeeeeeeeeeeeeE----------------------------------------------------------R  jump 32286
```

Gas simulation at offset 32283 with total cost of 2:

```
    D....  r2 = r4
    DeeER  fallthrough
```

Gas simulation at offset 32286 with total cost of 46:

```
    DeER.............................................  r8 = r0 << 0x5
    D=eeER...........................................  i32 r8 = r8 + r9
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER....................  r9 = u64 [r1 + 0x30]
    .D=========================eeeeeeeeeeeeeeeeeeeeER  jump 31425 if r8 >=u r9
```

Gas simulation at offset 32299 with total cost of 27:

```
    DeER..........................  r8 = r8 << 0x20
    D=eER.........................  r8 = r8 >> 0x20
    D==eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r8 + 0] = r2
    DeeeeeeeeeeeeeeeeeeeeeeeeeE--R  r5 = u64 [r1 + 0x38]
    .DeeeeeeeeeeeeeeeE-----------R  jump 31429
```

Gas simulation at offset 32313 with total cost of 26:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r7 = u64 [0x30008]
    D=========================eER  jump 32323 if r7 == 0
```

Gas simulation at offset 32321 with total cost of 22:

```
    DeeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 32323 with total cost of 2:

```
    DeeER  trap
```

Gas simulation at offset 32324 with total cost of 1:

```
    DeER  jump 32328 if r7 != 0
```

Gas simulation at offset 32327 with total cost of 2:

```
    DeeER  trap
```

Gas simulation at offset 32328 with total cost of 2:

```
    DeeER  trap
```

Gas simulation at offset 32329 with total cost of 2:

```
    DeeER  trap
```

Gas simulation at offset 32330 with total cost of 26:

```
    DeER.........................  r1 = r1 + 0xffffffffffffffb8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x40] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x38] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x30] = r6
    .DeE------------------------R  r9 = r9 + r8
    .D=eE-----------------------R  jump 32428 if r9 <u r8
```

Gas simulation at offset 32348 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    D..........................................  r5 = r7
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u64 [r7 + 0]
    DeE---------------------------------------R  r8 = 0x8
    .D========================eE--------------R  r10 = r7 << 0x1
    .DeeeE------------------------------------R  r8 = maxu(r9, r8)
    ..D========================eeeE-----------R  r6 = maxu(r8, r10)
    ..D===========================eE----------R  jump 32428 if r6 <s 0
```

Gas simulation at offset 32368 with total cost of 1:

```
    DeER  jump 32385 if r7 == 0
```

Gas simulation at offset 32371 with total cost of 50:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........  r8 = u64 [r5 + 0x8]
    D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x18] = r8
    DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  u64 [r1 + 0x28] = r7
    .DeE------------------------------------------------R  r7 = 0x1
    .DeeE-----------------------------------------------R  fallthrough
```

Gas simulation at offset 32385 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x20] = r7
    D...........................  r7 = r1
    DeE------------------------R  r9 = r1 + 0x18
    .D..........................  r8 = r6
    .DeeeeeeeeeeeeeeeE---------R  r0 = 938, jump 32439
```

Gas simulation at offset 32400 with total cost of 26:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r7 = u64 [r1 + 0]
    D=========================eER  jump 32433 if r7 != 0
```

Gas simulation at offset 32405 with total cost of 50:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER..........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........  r7 = u64 [r1 + 0x8]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R..........  u64 [r5 + 0] = r6
    D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r5 + 0x8] = r7
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE------------------------R  r0 = u64 [r1 + 0x40]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE------------------------R  r5 = u64 [r1 + 0x38]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0x30]
    .D=========================eE-----------------------R  r1 = r1 + 0x48
    ..D========================eeeeeeeeeeeeeeeeeeeeeeE--R  jump [r0 + 0]
```

Gas simulation at offset 32428 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeE---------------------------------------R  r7 = 0
    DeeeeeeeeeeeeeeeE-------------------------R  jump 32324
```

Gas simulation at offset 32433 with total cost of 40:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R  r7 = u64 [r1 + 0x8]
    DeeeeeeeeeeeeeeeE-------------------------R  jump 32324
```

Gas simulation at offset 32439 with total cost of 27:

```
    DeER..........................  r1 = r1 + 0xffffffffffffffe0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.  u64 [r1 + 0x18] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.  u64 [r1 + 0x10] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.  u64 [r1 + 0x8] = r6
    .D............................  r5 = r8
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r8 = u64 [r9 + 0x8]
    .D............................  r6 = r7
    .D=========================eER  jump 32481 if r8 == 0
```

Gas simulation at offset 32461 with total cost of 45:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.....  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.....  r7 = u64 [r9 + 0x10]
    D=========================eeeeeeeeeeeeeeeeeeeeER  jump 32545 if r7 == 0
```

Gas simulation at offset 32468 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u64 [r9 + 0]
    D...........................  r8 = r5
    DeeeeeeeeeeeeeeeE----------R  r0 = 940, jump 31126
```

Gas simulation at offset 32478 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 32638
```

Gas simulation at offset 32481 with total cost of 21:

```
    DeER....................  r7 = 0x1
    DeER....................  r8 = 0x1fffffffe0
    D=eeeeeeeeeeeeeeeeeeeeER  jump 32561 if r8 <u r5
```

Gas simulation at offset 32497 with total cost of 26:

```
    DeER.........................  r9 = 0x30a98
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0] = r9
    D=eE------------------------R  r8 = r9 + 0x2750
    .D=eE-----------------------R  r8 = r8 & 0xfffffffffffffffc
    .DeeE-----------------------R  fallthrough
```

Gas simulation at offset 32512 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  u64 [0x30000] = r4
    DeE---------------------------------------R............  r4 = r7 << 0x20
    .DeE--------------------------------------R............  r4 = r4 >>a 0x20
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R............  r9 = i32 [r8 + 0]
    .D=========================eE-------------R............  r4 = r9 | r4
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r8 + 0] = r4
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r4 = u64 [0x30000]
    ..D========================eE-------------------------R  r9 = r9 & 0xff
    ..D=========================eE------------------------R  jump 32512 if r9 != 0
```

Gas simulation at offset 32543 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  jump 32611
```

Gas simulation at offset 32545 with total cost of 21:

```
    DeER....................  r7 = 0x1
    DeER....................  r8 = 0x1fffffffe0
    D=eeeeeeeeeeeeeeeeeeeeER  jump 32565 if r8 >=u r5
```

Gas simulation at offset 32561 with total cost of 15:

```
    DeER..............  r7 = 0
    DeeeeeeeeeeeeeeeER  jump 32638
```

Gas simulation at offset 32565 with total cost of 26:

```
    DeER.........................  r9 = 0x30a98
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0] = r9
    D=eE------------------------R  r8 = r9 + 0x2750
    .D=eE-----------------------R  r8 = r8 & 0xfffffffffffffffc
    .DeeE-----------------------R  fallthrough
```

Gas simulation at offset 32580 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  u64 [0x30000] = r4
    DeE---------------------------------------R............  r4 = r7 << 0x20
    .DeE--------------------------------------R............  r4 = r4 >>a 0x20
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R............  r9 = i32 [r8 + 0]
    .D=========================eE-------------R............  r4 = r9 | r4
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r8 + 0] = r4
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r4 = u64 [0x30000]
    ..D========================eE-------------------------R  r9 = r9 & 0xff
    ..D=========================eE------------------------R  jump 32580 if r9 != 0
```

Gas simulation at offset 32611 with total cost of 16:

```
    DeER...............  r7 = r5 + 0x1f
    D=eER..............  r7 = r7 >> 0x5
    .D=eeER............  i32 r7 = r7 + 0
    .DeE--R............  r8 = 0
    .DeeeeeeeeeeeeeeeER  r0 = 942, jump 26592
```

Gas simulation at offset 32627 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r9 = u64 [r1 + 0]
    D=========================eER.........................  r8 = r9 + 0x2000
    D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r8 + 1872] = 0
    .DeeE------------------------------------------------R  fallthrough
```

Gas simulation at offset 32638 with total cost of 52:

```
    DeeeER.................................................  r8 = r7 <u 0x1
    DeE--R.................................................  r9 = 0x1
    .DeeER.................................................  r9 = r7 if r7 != 0
    .D==eeeeeeeeeeeeeeeeeeeeeeeeeER........................  u64 [r6 + 0] = r8
    .D==eeeeeeeeeeeeeeeeeeeeeeeeeER........................  u64 [r6 + 0x8] = r9
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-R........................  u64 [r6 + 0x10] = r5
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-R........................  r0 = u64 [r1 + 0x18]
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  r5 = u64 [r1 + 0x10]
    ..D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0x8]
    ...D=========================eE-----------------------R  r1 = r1 + 0x20
    ...D========================eeeeeeeeeeeeeeeeeeeeeeE---R  jump [r0 + 0]
```

Gas simulation at offset 32669 with total cost of 46:

```
    D................................................  r10 = r8
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.....................  r7 = u64 [r6 + 0]
    D=========================eER....................  r7 = r7 - r5
    D................................................  r8 = r5
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER....................  u64 [r1 + 8] = 0x2000
    .D=========================eeeeeeeeeeeeeeeeeeeeER  jump 32834 if r7 <u 8192
```

Gas simulation at offset 32689 with total cost of 26:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  u64 [r1 + 0] = r8
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r7 = u64 [r6 + 0x8]
    D=========================eER  r7 = r7 + r8
    D............................  r8 = r10
    .DeeeeeeeeeeeeeeeE----------R  r0 = 944, jump 28055
```

Gas simulation at offset 32705 with total cost of 224:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.......................................................................................................................................................................................................  r8 = u8 [r6 + 0x5c]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.......................................................................................................................................................................................................  r7 = u8 [r6 + 0x5d]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.......................................................................................................................................................................................................  r12 = u8 [r6 + 0x5e]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.......................................................................................................................................................................................................  r11 = u8 [r6 + 0x5f]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..............................................................................................................................................................................  r2 = u8 [r6 + 0x60]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..............................................................................................................................................................................  r0 = u8 [r6 + 0x61]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..............................................................................................................................................................................  r3 = u8 [r6 + 0x62]
    .D========================eeeeeeeeeeeeeeeeeeeeeeeeeER..............................................................................................................................................................................  r9 = u8 [r6 + 0x63]
    ..D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.....................................................................................................................................................  u64 [r1 + 0x10] = r9
    ..D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.....................................................................................................................................................  r9 = u64 [r1 + 0]
    ..D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.....................................................................................................................................................  r10 = u64 [r1 + 0x8]
    ..D=========================================================================eER....................................................................................................................................................  r9 = r9 + r10
    ...D=========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER...........................................................................................................................  u64 [r6 + 0x10] = r9
    ...D===============================================eE--------------------------------------------------R...........................................................................................................................  r4 = r8 | 0x1
    ...D================================================eE-------------------------------------------------R...........................................................................................................................  r7 = r7 | 0x1
    ....D================================================eE------------------------------------------------R...........................................................................................................................  r9 = r12 | 0x1
    ....D=================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-----------------------R...........................................................................................................................  u32 [r6 + 0x18] = r5
    ....D=======================================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-R...........................................................................................................................  u32 [r6 + 0x1c] = r5
    .....D======================================================================eeeeeeeeeeeeeeeeeeeeeeeeeE-R...........................................................................................................................  u32 [r6 + 0x20] = r5
    .....D=========================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................................................................................................................  u32 [r6 + 0x24] = r5
    .....D===============================================================================================eE--R.........................................................................................................................  r11 = r11 | 0x1
    ......D==============================================================================================eE--R.........................................................................................................................  r10 = r2 | 0x1
    ......D===============================================================================================eE-R.........................................................................................................................  r0 = r0 | 0x1
    .......D==============================================================================================eE-R.........................................................................................................................  r8 = r3 | 0x1
    .......D==============================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER..................................................................................................  u32 [r6 + 0x28] = r5
    .......D===============================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.................................................................................................  u32 [r6 + 0x2c] = r5
    ........D==============================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.................................................................................................  u32 [r6 + 0x30] = r5
    ........D===============================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER................................................................................................  u32 [r6 + 0x34] = r5
    ........D======================================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................................................................  r12 = u64 [r1 + 0x10]
    ........D===============================================================================================================================================eER........................................................................  r12 = r12 | 0x1
    .........D======================================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER........................................................................  u8 [r6 + 0x5c] = t2
    .........D======================================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER........................................................................  u8 [r6 + 0x5d] = a0
    ............................D====================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.......................................................................  u8 [r6 + 0x5e] = a2
    ............................D============================================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER...............................................  u8 [r6 + 0x5f] = a4
    ............................D============================================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER...............................................  u8 [r6 + 0x60] = a3
    ............................D============================================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER...............................................  u8 [r6 + 0x61] = ra
    .....................................................D====================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER..............................................  u8 [r6 + 0x62] = a1
    .....................................................D============================================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  u8 [r6 + 0x63] = a5
    .....................................................D.............................................................................................................................................................................  r7 = r5
    .....................................................D============================================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r0 = u64 [r1 + 0x28]
    ......................................................D===========================================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER......................  r5 = u64 [r1 + 0x20]
    ..............................................................................D====================================================================================================eeeeeeeeeeeeeeeeeeeeeeeeeER.....................  r6 = u64 [r1 + 0x18]
    ..............................................................................D============================================================================================================================eER.....................  r1 = r1 + 0x30
    ..............................................................................D============================================================================================================================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 32834 with total cost of 25:

```
    D...........................  r7 = r6
    D...........................  r8 = r5
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r9 = u64 [r1 + 0x8]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x10] = r10
    .DeeeeeeeeeeeeeeeE---------R  r0 = 946, jump 32330
```

Gas simulation at offset 32850 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r10 = u64 [r1 + 0x10]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r9 = u64 [r1 + 0x8]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = u64 [r6 + 0x10]
    DeeeeeeeeeeeeeeeE----------R  jump 32689
```

Gas simulation at offset 32862 with total cost of 20:

```
    D......................  r8 = r10
    DeeeeeeeeeeeeeeeeeeeeER  jump 33011 if r7 <=u 2047
```

Gas simulation at offset 32870 with total cost of 27:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..  r7 = u64 [r5 + 0x8]
    DeE------------------------R..  r9 = 0x800
    DeE------------------------R..  r10 = 0xffffffffffffd800
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.  u64 [r1 + 0x10] = r10
    .D========================eER.  r7 = r7 + r8
    .DeE------------------------R.  r8 = r8 + r9
    .D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x8] = r8
    .DeE-------------------------R  r8 = 0
    ..DeeeeeeeeeeeeeeeE----------R  r0 = 948, jump 28080
```

Gas simulation at offset 32901 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r7 = u8 [r5 + 0x64]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER..........................  r12 = u64 [r1 + 0x18]
    D=========================eER.........................  r10 = r12 + 0xffffffffffffe000
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r8 = u64 [r1 + 0x8]
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r5 + 0x10] = r8
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r5 + 0x38] = r10
    .DeE-------------------------------------------------R  jump 32989 if r6 == 0
```

Gas simulation at offset 32923 with total cost of 51:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...........  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r9 = u8 [r5 + 0x65]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R...........  r8 = u64 [r1 + 0x10]
    D=========================eE--------------R...........  r8 = r8 + r12
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R...........  u32 [r5 + 0x3c] = r10
    .D=========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r5 + 0x40] = r8
    .DeeE------------------------------------------------R  fallthrough
```

Gas simulation at offset 32940 with total cost of 76:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...................................................  r10 = u8 [r5 + 0x66]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER...................................................  r11 = u8 [r5 + 0x67]
    DeE------------------------R...................................................  r7 = r7 | 0x3
    DeE------------------------R...................................................  r9 = r9 | 0x3
    .D========================eER..................................................  r10 = r10 | 0x3
    .D========================eER..................................................  r11 = r11 | 0x3
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  u32 [r5 + 0x44] = r8
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER..................................................  u8 [r5 + 0x64] = a0
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u8 [r5 + 0x65] = a2
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u8 [r5 + 0x66] = a3
    ..D========================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  u8 [r5 + 0x67] = a4
    ..D............................................................................  r7 = r12
    ...D=======================eeeeeeeeeeeeeeeeeeeeeeeeeER.........................  r0 = u64 [r1 + 0x30]
    ...D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  r5 = u64 [r1 + 0x28]
    ...D================================================eeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0x20]
    ...D================================================eE------------------------R  r1 = r1 + 0x38
    ....D===============================================eeeeeeeeeeeeeeeeeeeeeeE---R  jump [r0 + 0]
```

Gas simulation at offset 32989 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  r8 = u64 [r1 + 0x10]
    D=========================eE--------------R............  r8 = r8 + r12
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  r9 = u8 [r5 + 0x65]
    .D=========================eE-------------R............  r10 = r8 + 0x400
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r5 + 0x3c] = r10
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r5 + 0x40] = r10
    ..DeeeeeeeeeeeeeeeE-----------------------------------R  jump 32940
```

Gas simulation at offset 33011 with total cost of 25:

```
    DeER........................  r9 = 0x800
    D...........................  r7 = r5
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = u64 [r1 + 0x18]
    DeeeeeeeeeeeeeeeE----------R  r0 = 950, jump 32330
```

Gas simulation at offset 33026 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r8 = u64 [r5 + 0x10]
    DeeeeeeeeeeeeeeeE----------R  jump 32870
```

Gas simulation at offset 33032 with total cost of 45:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER....................  r8 = u64 [r7 + 0]
    D=========================eeeeeeeeeeeeeeeeeeeeER  jump 33119 if r8 == 0
```

Gas simulation at offset 33037 with total cost of 26:

```
    DeER.........................  r1 = r1 + 0xfffffffffffffff0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x8] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0] = r5
    DeeeeeeeeeeeeeeeeeeeeeeeeeE-R  r7 = u64 [r7 + 0x8]
    .DeE------------------------R  r5 = 0x30a98
    .D=eE-----------------------R  r8 = r5 + 0x2750
    .D==eE----------------------R  r8 = r8 & 0xfffffffffffffffc
    ..DeE-----------------------R  r9 = 0x1
    ..DeeE----------------------R  fallthrough
```

Gas simulation at offset 33064 with total cost of 52:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER............  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R............  u64 [0x30000] = r4
    DeE---------------------------------------R............  r4 = r9 << 0x20
    .DeE--------------------------------------R............  r4 = r4 >>a 0x20
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R............  r10 = i32 [r8 + 0]
    .D=========================eE-------------R............  r4 = r10 | r4
    .D==========================eeeeeeeeeeeeeeeeeeeeeeeeeER  u32 [r8 + 0] = r4
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------------------R  r4 = u64 [0x30000]
    ..D========================eE-------------------------R  r10 = r10 & 0xff
    ..D=========================eE------------------------R  jump 33064 if r10 != 0
```

Gas simulation at offset 33095 with total cost of 15:

```
    DeeeeeeeeeeeeeeeER  r0 = 954, jump 27398
```

Gas simulation at offset 33101 with total cost of 47:

```
    DeER..............................................  r7 = r5 + 0x2000
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER.....................  u8 [r7 + 1872] = 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeE-R.....................  r0 = u64 [r1 + 0x8]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER.....................  r5 = u64 [r1 + 0]
    .DeE------------------------R.....................  r1 = r1 + 0x10
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 33119 with total cost of 22:

```
    DeeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 33121 with total cost of 57:

```
    DeER........................................................  r9 = r8 + 0xffffffffffffa000
    DeER........................................................  r10 = 0xe000
    D=eER.......................................................  r9 = r9 & r10
    .D=eER......................................................  r9 = r9 >> 0xb
    .D==eER.....................................................  r9 = r9 + r7
    .D===eeeeeeeeeeeeeeeeeeeeeeeeeER............................  r9 = i32 [r9 + 0x48]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE---R............................  r7 = u64 [r7 + 0x8]
    ..D===========================eeER..........................  i32 r8 = r8 + r9
    ..D=============================eER.........................  r7 = r7 + r8
    ..D==============================eeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u8 [r7 + 0]
    ...DeeeeeeeeeeeeeeeeeeeeeeE--------------------------------R  jump [r0 + 0]
```

Gas simulation at offset 33155 with total cost of 31:

```
    DeER..............................  r10 = r8 + 0xffffffffffffa000
    D=eER.............................  r10 = r10 << 0x30
    D==eER............................  r10 = r10 >> 0x3d
    .D==eER...........................  r11 = r7 + r10
    .D===eeeeeeeeeeeeeeeeeeeeeeeeeER..  r11 = u8 [r11 + 0x68]
    .D============================eER.  r11 = r11 & 0x2
    ..D============================eER  jump 33200 if r11 == 0
```

Gas simulation at offset 33177 with total cost of 55:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...............  unlikely
    DeE---------------------------------------R...............  r10 = r10 << 0x2
    D=eE--------------------------------------R...............  r10 = r10 + r7
    D==eeeeeeeeeeeeeeeeeeeeeeeeeE-------------R...............  r10 = i32 [r10 + 0x48]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R...............  r7 = u64 [r7 + 0x8]
    .D==========================eeE-----------R...............  i32 r8 = r8 + r10
    .D============================eE----------R...............  r7 = r7 + r8
    ..D============================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0] = a2
    ..DeeeeeeeeeeeeeeeeeeeeeeE-------------------------------R  jump [r0 + 0]
```

Gas simulation at offset 33200 with total cost of 22:

```
    DeeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 33202 with total cost of 22:

```
    DeER.....................  r7 = 0
    DeeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 33206 with total cost of 22:

```
    DeeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 33208 with total cost of 63:

```
    DeER..............................................................  r9 = r8 >> 0xc
    .DeeeER...........................................................  r9 = r9 <u 0x3
    .DeE--R...........................................................  r10 = 0xfffffffffffff000
    ..D==eeER.........................................................  r10 = 0 if r9 != 0
    ..D====eER........................................................  r8 = r8 + r10
    ...D====eER.......................................................  r9 = r8 >> 0x8
    ...D=====eER......................................................  r9 = r9 & 0xfc
    ...D======eER.....................................................  r9 = r9 + r7
    ....D======eeeeeeeeeeeeeeeeeeeeeeeeeER............................  r9 = i32 [r9 + 0x18]
    ....DeeeeeeeeeeeeeeeeeeeeeeeeeE------R............................  r7 = u64 [r7 + 0x8]
    ....D===eE---------------------------R............................  r8 = zext16 r8
    .....D==============================eeER..........................  i32 r8 = r8 + r9
    .....D================================eER.........................  r7 = r7 + r8
    .....D=================================eeeeeeeeeeeeeeeeeeeeeeeeeER  r7 = u8 [r7 + 0]
    ......DeeeeeeeeeeeeeeeeeeeeeeE-----------------------------------R  jump [r0 + 0]
```

Gas simulation at offset 33251 with total cost of 37:

```
    DeER....................................  r10 = r8 >> 0xc
    .DeeeER.................................  r10 = r10 <u 0x3
    .DeE--R.................................  r11 = 0xfffffffffffff000
    ..D==eeER...............................  r11 = 0 if r10 != 0
    ..D====eER..............................  r8 = r8 + r11
    ...D====eER.............................  r10 = r8 << 0x30
    ...D=====eER............................  r10 = r10 >> 0x3a
    ....D=====eER...........................  r11 = r7 + r10
    ....D======eeeeeeeeeeeeeeeeeeeeeeeeeER..  r11 = u8 [r11 + 0x5c]
    ....D===============================eER.  r11 = r11 & 0x2
    .....D===============================eER  jump 33309 if r11 == 0
```

Gas simulation at offset 33284 with total cost of 55:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER...............  unlikely
    DeE---------------------------------------R...............  r10 = r10 << 0x2
    D=eE--------------------------------------R...............  r10 = r10 + r7
    D==eeeeeeeeeeeeeeeeeeeeeeeeeE-------------R...............  r10 = i32 [r10 + 0x18]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R...............  r7 = u64 [r7 + 0x8]
    .DeE--------------------------------------R...............  r8 = zext16 r8
    .D==========================eeE-----------R...............  i32 r8 = r8 + r10
    ..D===========================eE----------R...............  r7 = r7 + r8
    ..D============================eeeeeeeeeeeeeeeeeeeeeeeeeER  u8 [r7 + 0] = a2
    ..DeeeeeeeeeeeeeeeeeeeeeeE-------------------------------R  jump [r0 + 0]
```

Gas simulation at offset 33309 with total cost of 22:

```
    DeeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 33311 with total cost of 26:

```
    DeER.........................  r1 = r1 + 0xfffffffffffffff0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x8] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0] = r6
    .DeE------------------------R  r5 = 0x7fffffffffffffff
    .DeE------------------------R  r12 = 0x8010000000000000
    ..DeE-----------------------R  r11 = r7 & r5
    ..D=eE----------------------R  r10 = r11 + r12
    ...DeE----------------------R  r6 = 0x8010000000000001
    ...DeE----------------------R  r9 = r8 & r5
    ....DeeeeeeeeeeeeeeeeeeeeE--R  jump 33458 if r10 <u r6
```

Gas simulation at offset 33361 with total cost of 21:

```
    DeER....................  r12 = r12 + r9
    D=eeeeeeeeeeeeeeeeeeeeER  jump 33458 if r12 <u r6
```

Gas simulation at offset 33367 with total cost of 27:

```
    DeeeER........................  r9 = r11 <u r9
    D.............................  r10 = r7
    .D............................  r12 = r8
    .DeE-R........................  r2 = 0xfffffffffffff
    ..D=eeER......................  r10 = r8 if r9 == 0
    ..D=eeER......................  r12 = r7 if r9 == 0
    ...D==eER.....................  r9 = r12 << 0x1
    ...D==eER.....................  r11 = r10 << 0x1
    ....D==eER....................  r3 = r9 >> 0x35
    ....D==eER....................  r9 = r11 >> 0x35
    .....DeE-R....................  r4 = r12 & r2
    .....D==eeeeeeeeeeeeeeeeeeeeER  jump 33577 if r3 == 0
```

Gas simulation at offset 33409 with total cost of 20:

```
    DeER...................  r6 = r10 & r2
    DeeeeeeeeeeeeeeeeeeeeER  jump 33595 if r9 == 0
```

Gas simulation at offset 33416 with total cost of 22:

```
    DeER.....................  r11 = 0x8000000000000000
    DeER.....................  r8 = r8 ^ r7
    DeER.....................  r4 = r4 << 0x3
    .DeER....................  r10 = 0x1
    .DeER....................  r5 = 0x80000000000000
    ..DeER...................  r7 = r6 << 0x3
    ..D=eER..................  r7 = r7 | r5
    ..DeeeeeeeeeeeeeeeeeeeeER  jump 33497 if r3 != r9
```

Gas simulation at offset 33454 with total cost of 15:

```
    D.................  r10 = r7
    DeeeeeeeeeeeeeeeER  jump 33518
```

Gas simulation at offset 33458 with total cost of 21:

```
    DeER....................  r12 = 0x7ff0000000000000
    D=eeeeeeeeeeeeeeeeeeeeER  jump 33550 if r12 >=u r11
```

Gas simulation at offset 33471 with total cost of 3:

```
    DeER..  r7 = 0x8000000000000
    D=eER.  r8 = r11 | r7
    .DeeER  fallthrough
```

Gas simulation at offset 33485 with total cost of 25:

```
    D...........................  r7 = r8
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r5 = u64 [r1 + 0x8]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0]
    DeE------------------------R  r1 = r1 + 0x10
    .DeeeeeeeeeeeeeeeeeeeeeeE--R  jump [r0 + 0]
```

Gas simulation at offset 33497 with total cost of 21:

```
    DeER....................  r9 = r3 - r9
    D=eeeeeeeeeeeeeeeeeeeeER  jump 33518 if r9 >u 63
```

Gas simulation at offset 33504 with total cost of 8:

```
    DeeeER.....  i32 r10 = 0 - r9
    .D==eER....  r10 = r7 << r10
    ..D==eeeER.  r10 = r10 >u 0
    ...DeE---R.  r7 = r7 >> r9
    ...D====eER  r10 = r10 | r7
    ...DeeE---R  fallthrough
```

Gas simulation at offset 33518 with total cost of 21:

```
    DeER....................  r7 = r12 & r11
    DeER....................  r9 = r4 | r5
    .DeeeeeeeeeeeeeeeeeeeeER  jump 33609 if r8 <s 0
```

Gas simulation at offset 33527 with total cost of 22:

```
    DeER.....................  r8 = r10 + r9
    D=eER....................  r9 = r8 << 0x7
    .D=eeeeeeeeeeeeeeeeeeeeER  jump 33634 if r9 >=s 0
```

Gas simulation at offset 33536 with total cost of 16:

```
    DeER...............  r10 = r10 & 0x1
    DeER...............  r8 = r8 >> 0x1
    D=eER..............  r8 = r8 | r10
    DeE-R..............  r3 = r3 + 0x1
    .DeeeeeeeeeeeeeeeER  jump 33634
```

Gas simulation at offset 33550 with total cost of 20:

```
    DeeeeeeeeeeeeeeeeeeeeER  jump 33735 if r12 >=u r9
```

Gas simulation at offset 33554 with total cost of 26:

```
    DeER.........................  r7 = 0x8000000000000
    D=eER........................  r7 = r7 | r9
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r5 = u64 [r1 + 0x8]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0]
    .DeE------------------------R  r1 = r1 + 0x10
    .DeeeeeeeeeeeeeeeeeeeeeeE---R  jump [r0 + 0]
```

Gas simulation at offset 33577 with total cost of 23:

```
    DeER......................  r11 = clz r4
    D=eER.....................  r6 = r11 + 0x35
    .DeeER....................  r3 = 0xc - r11
    ..DeER....................  r4 = r4 << r6
    ..DeER....................  r6 = r10 & r2
    ...DeeeeeeeeeeeeeeeeeeeeER  jump 33416 if r9 != 0
```

Gas simulation at offset 33595 with total cost of 17:

```
    DeER................  r9 = clz r6
    D=eER...............  r11 = r9 + 0x35
    .DeeER..............  r9 = 0xc - r9
    ..DeER..............  r6 = r6 << r11
    ..DeeeeeeeeeeeeeeeER  jump 33416
```

Gas simulation at offset 33609 with total cost of 21:

```
    DeER....................  r8 = r9 - r10
    D=eeeeeeeeeeeeeeeeeeeeER  jump 33485 if r8 == 0
```

Gas simulation at offset 33615 with total cost of 21:

```
    DeER....................  r9 = r8 >> 0x37
    D=eeeeeeeeeeeeeeeeeeeeER  jump 33634 if r9 != 0
```

Gas simulation at offset 33621 with total cost of 16:

```
    DeER...............  r9 = clz r8
    D=eER..............  r9 = r9 + 0xfffffffffffffff8
    D==eER.............  r8 = r8 << r9
    .D=eER.............  r3 = r3 - r9
    .DeeeeeeeeeeeeeeeER  jump 33664
```

Gas simulation at offset 33634 with total cost of 21:

```
    DeER....................  r9 = 0x7fe
    D=eeeeeeeeeeeeeeeeeeeeER  jump 33664 if r9 >=s r3
```

Gas simulation at offset 33641 with total cost of 26:

```
    DeER.........................  r8 = 0x7ff0000000000000
    D=eER........................  r7 = r7 | r8
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r5 = u64 [r1 + 0x8]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0]
    .DeE------------------------R  r1 = r1 + 0x10
    .DeeeeeeeeeeeeeeeeeeeeeeE---R  jump [r0 + 0]
```

Gas simulation at offset 33664 with total cost of 20:

```
    DeeeeeeeeeeeeeeeeeeeeER  jump 33686 if r3 >s 0
```

Gas simulation at offset 33667 with total cost of 11:

```
    DeeeER........  i32 r9 = 0x1 - r3
    .DeE-R........  r3 = 0
    ..D=eeeER.....  i32 r10 = 0 - r9
    ...D===eER....  r10 = r8 << r10
    ....DeE--R....  r8 = r8 >> r9
    .....D==eeeER.  r9 = r10 >u 0
    .....D=====eER  r8 = r8 | r9
    ......DeeE---R  fallthrough
```

Gas simulation at offset 33686 with total cost of 29:

```
    DeER............................  r9 = r8 & 0x7
    DeER............................  r8 = r8 >> 0x3
    DeER............................  r3 = r3 << 0x34
    .DeER...........................  r8 = r8 & r2
    .DeeeER.........................  r10 = r9 <u 0x5
    ..DeE-R.........................  r7 = r3 | r7
    ..DeE-R.........................  r9 = r9 + 0xfffffffffffffffc
    ..D==eER........................  r10 = r10 ^ 0x1
    ..D=eE-R........................  r7 = r7 | r8
    ...D==eER.......................  r7 = r7 + r10
    ...DeeeER.......................  r8 = r9 <u 0x1
    ....D==eER......................  r8 = r8 & r7
    ....D===eER.....................  r7 = r7 + r8
    ....DeeeeeeeeeeeeeeeeeeeeeeeeeER  r5 = u64 [r1 + 0x8]
    ....DeeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0]
    .....D=eE----------------------R  r1 = r1 + 0x10
    .....DeeeeeeeeeeeeeeeeeeeeeeE--R  jump [r0 + 0]
```

Gas simulation at offset 33735 with total cost of 21:

```
    DeER....................  r12 = 0x7ff0000000000000
    D=eeeeeeeeeeeeeeeeeeeeER  jump 33789 if r11 != r12
```

Gas simulation at offset 33748 with total cost of 27:

```
    DeER..........................  r8 = r8 ^ r7
    DeER..........................  r9 = 0x8000000000000000
    D=eER.........................  r9 = r9 ^ r8
    .DeER.........................  r8 = 0x7ff8000000000000
    .D=eeER.......................  r8 = r7 if r9 != 0
    ..D...........................  r7 = r8
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeER  r5 = u64 [r1 + 0x8]
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0]
    ..DeE------------------------R  r1 = r1 + 0x10
    ...DeeeeeeeeeeeeeeeeeeeeeeE--R  jump [r0 + 0]
```

Gas simulation at offset 33789 with total cost of 20:

```
    DeeeeeeeeeeeeeeeeeeeeER  jump 33485 if r9 == r12
```

Gas simulation at offset 33793 with total cost of 20:

```
    DeeeeeeeeeeeeeeeeeeeeER  jump 33810 if r11 == 0
```

Gas simulation at offset 33796 with total cost of 20:

```
    DeeeeeeeeeeeeeeeeeeeeER  jump 33367 if r9 != 0
```

Gas simulation at offset 33800 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r5 = u64 [r1 + 0x8]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0]
    DeE------------------------R  r1 = r1 + 0x10
    DeeeeeeeeeeeeeeeeeeeeeeE---R  jump [r0 + 0]
```

Gas simulation at offset 33810 with total cost of 26:

```
    DeER.........................  r10 = 0xffffffffffffffff
    D=eeER.......................  r7 = r10 if r9 != 0
    D===eER......................  r7 = r7 & r8
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER  r5 = u64 [r1 + 0x8]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0]
    .DeE------------------------R  r1 = r1 + 0x10
    .DeeeeeeeeeeeeeeeeeeeeeeE---R  jump [r0 + 0]
```

Gas simulation at offset 33829 with total cost of 26:

```
    DeER.........................  r1 = r1 + 0xfffffffffffffff8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0] = r5
    DeE-------------------------R  r10 = r7 << 0x21
    .DeE------------------------R  r9 = 0xffffffff80000000
    .DeE------------------------R  r5 = r10 >> 0x21
    ..DeeE----------------------R  i32 r10 = r5 + 0xffffffff80800000
    ..DeE-----------------------R  r12 = 0xffffffff80800001
    ...DeeE---------------------R  r9 = r8 & ~r9
    ...D=eeeeeeeeeeeeeeeeeeeeE--R  jump 34013 if r10 <u r12
```

Gas simulation at offset 33865 with total cost of 22:

```
    DeeER....................  i32 r11 = r9 + 0xffffffff80800000
    D==eeeeeeeeeeeeeeeeeeeeER  jump 34013 if r11 <u 2155872257
```

Gas simulation at offset 33879 with total cost of 27:

```
    DeER..........................  r2 = 0x7fffff
    DeeeER........................  r9 = r5 <u r9
    .D............................  r10 = r7
    .D............................  r11 = r8
    .D==eeER......................  r10 = r8 if r9 == 0
    ..D=eeER......................  r11 = r7 if r9 == 0
    ..D===eER.....................  r9 = r11 << 0x21
    ...D==eER.....................  r12 = r10 << 0x21
    ...D===eER....................  r3 = r9 >> 0x38
    ....D==eER....................  r12 = r12 >> 0x38
    ....D=eE-R....................  r9 = r11 & r2
    ....D===eeeeeeeeeeeeeeeeeeeeER  jump 34060 if r3 == 0
```

Gas simulation at offset 33916 with total cost of 20:

```
    DeER...................  r5 = r10 & 0x7fffff
    DeeeeeeeeeeeeeeeeeeeeER  jump 34080 if r12 == 0
```

Gas simulation at offset 33925 with total cost of 22:

```
    DeER.....................  r4 = 0xffffffff80000000
    DeER.....................  r8 = r8 ^ r7
    DeER.....................  r7 = r9 << 0x3
    .DeER....................  r10 = 0x4000000
    .DeER....................  r9 = r5 << 0x3
    .D=eER...................  r9 = r9 | r10
    ..DeeeeeeeeeeeeeeeeeeeeER  jump 33974 if r3 == r12
```

Gas simulation at offset 33952 with total cost of 21:

```
    DeER....................  r12 = r3 - r12
    D=eeeeeeeeeeeeeeeeeeeeER  jump 34094 if r12 >u 31
```

Gas simulation at offset 33960 with total cost of 9:

```
    DeeeER......  i32 r5 = 0 - r12
    .D==eeER....  i32 r5 = r9 << r5
    ..D===eeeER.  r5 = r5 >u 0
    ...DeeE---R.  i32 r9 = r9 >> r12
    ...D=====eER  r9 = r9 | r5
    ....DeeE---R  fallthrough
```

Gas simulation at offset 33974 with total cost of 20:

```
    DeER...................  r11 = r11 & 0xffffffff80000000
    DeER...................  r7 = r7 | 0x4000000
    DeeeeeeeeeeeeeeeeeeeeER  jump 34112 if r8 <s 0
```

Gas simulation at offset 33989 with total cost of 23:

```
    DeeER.....................  i32 r8 = r9 + r7
    .D=eER....................  r7 = r8 << 0x24
    .D==eeeeeeeeeeeeeeeeeeeeER  jump 34137 if r7 >=s 0
```

Gas simulation at offset 33999 with total cost of 16:

```
    DeER...............  r9 = r9 & 0x1
    DeeER..............  i32 r8 = r8 >> 0x1
    D==eER.............  r8 = r8 | r9
    .DeE-R.............  r3 = r3 + 0x1
    .DeeeeeeeeeeeeeeeER  jump 34137
```

Gas simulation at offset 34013 with total cost of 21:

```
    DeER....................  r11 = 0x7f800000
    D=eeeeeeeeeeeeeeeeeeeeER  jump 34037 if r11 >=u r5
```

Gas simulation at offset 34022 with total cost of 2:

```
    DeER.  r8 = r5 | 0x400000
    DeeER  fallthrough
```

Gas simulation at offset 34028 with total cost of 25:

```
    D...........................  r7 = r8
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r5 = u64 [r1 + 0]
    DeE------------------------R  r1 = r1 + 0x8
    DeeeeeeeeeeeeeeeeeeeeeeE---R  jump [r0 + 0]
```

Gas simulation at offset 34037 with total cost of 20:

```
    DeeeeeeeeeeeeeeeeeeeeER  jump 34229 if r9 <=u 2139095040
```

Gas simulation at offset 34045 with total cost of 25:

```
    DeER........................  r8 = 0x400000
    D=eER.......................  r7 = r9 | r8
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r5 = u64 [r1 + 0]
    .DeE-----------------------R  r1 = r1 + 0x8
    .DeeeeeeeeeeeeeeeeeeeeeeE--R  jump [r0 + 0]
```

Gas simulation at offset 34060 with total cost of 23:

```
    DeER......................  i32 r5 = clz r9
    D=eER.....................  r4 = r5 + 0x18
    .DeeER....................  r3 = 0x9 - r5
    ..DeeER...................  i32 r9 = r9 << r4
    ...DeER...................  r5 = r10 & 0x7fffff
    ...DeeeeeeeeeeeeeeeeeeeeER  jump 33925 if r12 != 0
```

Gas simulation at offset 34080 with total cost of 17:

```
    DeER................  i32 r10 = clz r5
    D=eER...............  r4 = r10 + 0x18
    .DeeER..............  r12 = 0x9 - r10
    ..DeeER.............  i32 r5 = r5 << r4
    ..DeeeeeeeeeeeeeeeER  jump 33925
```

Gas simulation at offset 34094 with total cost of 20:

```
    DeER...................  r9 = 0x1
    DeER...................  r11 = r11 & 0xffffffff80000000
    DeER...................  r7 = r7 | 0x4000000
    DeeeeeeeeeeeeeeeeeeeeER  jump 33989 if r8 >=s 0
```

Gas simulation at offset 34112 with total cost of 22:

```
    DeeER....................  i32 r8 = r7 - r9
    D==eeeeeeeeeeeeeeeeeeeeER  jump 34028 if r8 == 0
```

Gas simulation at offset 34118 with total cost of 22:

```
    DeeER....................  i32 r7 = r8 >> 0x1a
    D==eeeeeeeeeeeeeeeeeeeeER  jump 34137 if r7 != 0
```

Gas simulation at offset 34124 with total cost of 17:

```
    DeER................  i32 r7 = clz r8
    D=eER...............  r7 = r7 + 0xfffffffffffffffb
    .D=eeER.............  i32 r8 = r8 << r7
    .D=eE-R.............  r3 = r3 - r7
    ..DeeeeeeeeeeeeeeeER  jump 34158
```

Gas simulation at offset 34137 with total cost of 20:

```
    DeeeeeeeeeeeeeeeeeeeeER  jump 34158 if r3 <=s 254
```

Gas simulation at offset 34142 with total cost of 25:

```
    DeER........................  r8 = 0x7f800000
    D=eER.......................  r7 = r11 | r8
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r5 = u64 [r1 + 0]
    .DeE-----------------------R  r1 = r1 + 0x8
    .DeeeeeeeeeeeeeeeeeeeeeeE--R  jump [r0 + 0]
```

Gas simulation at offset 34158 with total cost of 20:

```
    DeeeeeeeeeeeeeeeeeeeeER  jump 34181 if r3 >s 0
```

Gas simulation at offset 34161 with total cost of 8:

```
    DeeeER.....  i32 r7 = 0x1 - r3
    .DeE-R.....  r3 = r3 + 0xffffffffffffffff
    ..DeeER....  i32 r9 = r8 << r3
    ...D=eeeER.  r9 = r9 >u 0
    ....DeeE-R.  i32 r8 = r8 >> r7
    ....D===eER  r8 = r8 | r9
    .....DeE--R  r3 = 0
    .....DeeE-R  fallthrough
```

Gas simulation at offset 34181 with total cost of 30:

```
    DeER.............................  r7 = r8 & 0x7
    DeER.............................  r8 = r8 >> 0x3
    DeER.............................  r3 = r3 << 0x17
    .DeER............................  r8 = r8 & 0x7fffff
    .DeeeER..........................  r9 = r7 <u 0x5
    ..DeE-R..........................  r10 = r3 | r11
    ..DeE-R..........................  r7 = r7 + 0xfffffffffffffffc
    ..D==eER.........................  r9 = r9 ^ 0x1
    ...DeE-R.........................  r8 = r8 | r10
    ...D==eER........................  r8 = r8 + r9
    ....DeeeER.......................  r7 = r7 <u 0x1
    ....D===eER......................  r7 = r7 & r8
    .....D===eeER....................  i32 r7 = r7 + r8
    .....DeeeeeeeeeeeeeeeeeeeeeeeeeER  r5 = u64 [r1 + 0]
    .....DeE------------------------R  r1 = r1 + 0x8
    ......DeeeeeeeeeeeeeeeeeeeeeeE--R  jump [r0 + 0]
```

Gas simulation at offset 34229 with total cost of 20:

```
    DeeeeeeeeeeeeeeeeeeeeER  jump 34263 if r5 != 2139095040
```

Gas simulation at offset 34236 with total cost of 26:

```
    DeER.........................  r8 = r8 ^ r7
    D=eER........................  r9 = r8 ^ 0xffffffff80000000
    DeE-R........................  r8 = 0x7fc00000
    .D=eeER......................  r8 = r7 if r9 != 0
    .D...........................  r7 = r8
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER  r5 = u64 [r1 + 0]
    ..DeE-----------------------R  r1 = r1 + 0x8
    ..DeeeeeeeeeeeeeeeeeeeeeeE--R  jump [r0 + 0]
```

Gas simulation at offset 34263 with total cost of 20:

```
    DeeeeeeeeeeeeeeeeeeeeER  jump 34028 if r9 == 2139095040
```

Gas simulation at offset 34271 with total cost of 20:

```
    DeeeeeeeeeeeeeeeeeeeeER  jump 34285 if r5 == 0
```

Gas simulation at offset 34274 with total cost of 20:

```
    DeeeeeeeeeeeeeeeeeeeeER  jump 33879 if r9 != 0
```

Gas simulation at offset 34278 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r5 = u64 [r1 + 0]
    DeE------------------------R  r1 = r1 + 0x8
    DeeeeeeeeeeeeeeeeeeeeeeE---R  jump [r0 + 0]
```

Gas simulation at offset 34285 with total cost of 26:

```
    DeER.........................  r10 = 0xffffffffffffffff
    D=eeER.......................  r7 = r10 if r9 != 0
    D===eER......................  r7 = r7 & r8
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER  r5 = u64 [r1 + 0]
    .DeE------------------------R  r1 = r1 + 0x8
    .DeeeeeeeeeeeeeeeeeeeeeeE---R  jump [r0 + 0]
```

Gas simulation at offset 34301 with total cost of 30:

```
    DeER.............................  r1 = r1 + 0xffffffffffffffe8
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER....  u64 [r1 + 0x10] = r0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER....  u64 [r1 + 0x8] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER....  u64 [r1 + 0] = r6
    .D...............................  r9 = r7
    .DeE------------------------R....  r2 = 0x7fffff
    .DeE------------------------R....  r12 = r7 << 0x21
    ..DeE-----------------------R....  r6 = r8 << 0x21
    ..D=eE----------------------R....  r7 = r7 ^ r8
    ..DeE-----------------------R....  r5 = 0xffffffff80000000
    ...D=eE---------------------R....  r4 = r12 >> 0x38
    ...D==eE--------------------R....  r0 = r6 >> 0x38
    ....D==eE-------------------R....  r7 = r7 & r5
    ....D===eE------------------R....  r11 = r9 & r2
    .....D===eE-----------------R....  r10 = r4 + 0xffffffffffffff01
    .....D====eE----------------R....  r3 = r8 & r2
    ......D====eeeeeeeeeeeeeeeeeeeeER  jump 34451 if r10 <u 4294967042
```

Gas simulation at offset 34358 with total cost of 21:

```
    DeER....................  r10 = r0 + 0xffffffffffffff01
    D=eeeeeeeeeeeeeeeeeeeeER  jump 34451 if r10 <u 4294967042
```

Gas simulation at offset 34367 with total cost of 2:

```
    D....  r10 = r11
    DeER.  r5 = 0
    DeeER  fallthrough
```

Gas simulation at offset 34372 with total cost of 29:

```
    DeER............................  r3 = r3 << 0x8
    DeER............................  r8 = r10 | 0x800000
    .DeER...........................  r9 = r3 | 0xffffffff80000000
    .DeER...........................  r8 = r8 << 0x20
    .D=eER..........................  r9 = r9 << 0x20
    ..D=eeeeER......................  r8 = r8 mulhu r9
    ...D====eER.....................  r9 = r8 >> 0x20
    ...DeE----R.....................  r11 = r0 + r4
    ....D====eER....................  r10 = r9 << 0x28
    ....DeE----R....................  r4 = r11 + r5
    .....D====eeeeeeeeeeeeeeeeeeeeER  jump 34483 if r10 <s 0
```

Gas simulation at offset 34411 with total cost of 4:

```
    DeER...  r11 = r4 + 0xffffffffffffff81
    .DeeER.  i32 r10 = r8 >> 0x1f
    .DeE-R.  r9 = r9 << 0x1
    ..D=eER  r9 = r9 | r10
    ..DeE-R  r8 = r8 << 0x1
    ..DeE-R  r10 = 0xfe
    ..D=eER  jump 34493 if r10 <s r11
```

Gas simulation at offset 34433 with total cost of 20:

```
    DeeeeeeeeeeeeeeeeeeeeER  jump 34583 if r11 <=s 0
```

Gas simulation at offset 34437 with total cost of 15:

```
    DeER..............  r9 = r9 & 0x7fffff
    DeER..............  r11 = r11 << 0x17
    D=eER.............  r9 = r9 | r11
    DeeeeeeeeeeeeeeeER  jump 34611
```

Gas simulation at offset 34451 with total cost of 21:

```
    DeER....................  r12 = r12 >> 0x21
    DeER....................  r6 = 0x7f800000
    D=eeeeeeeeeeeeeeeeeeeeER  jump 34516 if r6 >=u r12
```

Gas simulation at offset 34463 with total cost of 2:

```
    DeER.  r7 = r9 | 0x400000
    DeeER  fallthrough
```

Gas simulation at offset 34469 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.......  unlikely
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r0 = u64 [r1 + 0x10]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r5 = u64 [r1 + 0x8]
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r6 = u64 [r1 + 0]
    .DeE--------------------------------------R.......  r1 = r1 + 0x18
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 34483 with total cost of 2:

```
    DeER.  r11 = r4 + 0xffffffffffffff82
    DeER.  r10 = 0xfe
    D=eER  jump 34433 if r10 >=s r11
```

Gas simulation at offset 34493 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.......  unlikely
    DeE---------------------------------------R.......  r8 = 0x7f800000
    D=eE--------------------------------------R.......  r7 = r7 | r8
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r0 = u64 [r1 + 0x10]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......  r5 = u64 [r1 + 0x8]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......  r6 = u64 [r1 + 0]
    .D=eE-------------------------------------R.......  r1 = r1 + 0x18
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 34516 with total cost of 3:

```
    DeeER.  r9 = r8 & ~r5
    D==eER  jump 34545 if r9 <=u 2139095040
```

Gas simulation at offset 34526 with total cost of 47:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER.......  unlikely
    DeE---------------------------------------R.......  r7 = r8 | 0x400000
    DeeeeeeeeeeeeeeeeeeeeeeeeeE---------------R.......  r0 = u64 [r1 + 0x10]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......  r5 = u64 [r1 + 0x8]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R.......  r6 = u64 [r1 + 0]
    .DeE--------------------------------------R.......  r1 = r1 + 0x18
    .D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 34545 with total cost of 2:

```
    DeER.  r8 = 0x7f800000
    D=eER  jump 34653 if r12 != r8
```

Gas simulation at offset 34554 with total cost of 48:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER........  unlikely
    DeE---------------------------------------R........  r8 = r7 | 0x7f800000
    DeE---------------------------------------R........  r7 = 0x7fc00000
    .DeeE-------------------------------------R........  r7 = r8 if r9 != 0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R........  r0 = u64 [r1 + 0x10]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R........  r5 = u64 [r1 + 0x8]
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------R........  r6 = u64 [r1 + 0]
    ..D=eE------------------------------------R........  r1 = r1 + 0x18
    ..D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 34583 with total cost of 3:

```
    DeeER.  r10 = 0x1 - r11
    DeE-R.  r12 = 0x1f
    .D=eER  jump 34469 if r12 <u r10
```

Gas simulation at offset 34592 with total cost of 6:

```
    DeER.....  r11 = r11 + 0xffffffffffffffff
    .DeeER...  i32 r12 = r8 >> r10
    ..DeER...  r8 = r8 | r9
    ..D=eeER.  i32 r8 = r8 << r11
    ...D==eER  r8 = r8 | r12
    ...DeeE-R  i32 r9 = r9 >> r10
    ....DeeER  fallthrough
```

Gas simulation at offset 34611 with total cost of 50:

```
    DeER.................................................  r7 = r7 | r9
    DeeER................................................  i32 r8 = r8 + 0
    DeE-R................................................  r9 = 0xffffffff80000000
    .D=eeeER.............................................  r10 = r9 <u r8
    .D=eE--R.............................................  r8 = r8 ^ r9
    ..D===eER............................................  r7 = r7 + r10
    ..D=eeeER............................................  r8 = r8 <u 0x1
    ...D===eER...........................................  r8 = r8 & r7
    ...D====eeER.........................................  i32 r7 = r7 + r8
    ...DeeeeeeeeeeeeeeeeeeeeeeeeeER......................  r0 = u64 [r1 + 0x10]
    ....DeeeeeeeeeeeeeeeeeeeeeeeeeER.....................  r5 = u64 [r1 + 0x8]
    ....D==eeeeeeeeeeeeeeeeeeeeeeeeeER...................  r6 = u64 [r1 + 0]
    ....D=====eE---------------------R...................  r1 = r1 + 0x18
    ....D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 34653 with total cost of 1:

```
    DeER  jump 34689 if r9 != 2139095040
```

Gas simulation at offset 34660 with total cost of 48:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER........  unlikely
    DeE---------------------------------------R........  r8 = r7 | 0x7f800000
    DeE---------------------------------------R........  r7 = 0x7fc00000
    .DeeE-------------------------------------R........  r7 = r8 if r12 != 0
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R........  r0 = u64 [r1 + 0x10]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeE--------------R........  r5 = u64 [r1 + 0x8]
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeE-------------R........  r6 = u64 [r1 + 0]
    ..D=eE------------------------------------R........  r1 = r1 + 0x18
    ..D========================eeeeeeeeeeeeeeeeeeeeeeER  jump [r0 + 0]
```

Gas simulation at offset 34689 with total cost of 1:

```
    DeER  jump 34469 if r12 == 0
```

Gas simulation at offset 34693 with total cost of 1:

```
    DeER  jump 34469 if r9 == 0
```

Gas simulation at offset 34697 with total cost of 21:

```
    DeER....................  r12 = r12 >> 0x17
    D=eeeeeeeeeeeeeeeeeeeeER  jump 34716 if r12 != 0
```

Gas simulation at offset 34703 with total cost of 18:

```
    DeER.................  i32 r8 = clz r11
    D=eER................  r12 = r8 + 0x18
    .DeeER...............  r5 = 0x9 - r8
    ..DeeER..............  i32 r10 = r11 << r12
    ...DeeeeeeeeeeeeeeeER  jump 34721
```

Gas simulation at offset 34716 with total cost of 2:

```
    D....  r10 = r11
    DeER.  r5 = 0
    DeeER  fallthrough
```

Gas simulation at offset 34721 with total cost of 21:

```
    DeER....................  r9 = r9 >> 0x17
    D=eeeeeeeeeeeeeeeeeeeeER  jump 34372 if r9 != 0
```

Gas simulation at offset 34728 with total cost of 17:

```
    DeER................  i32 r8 = clz r3
    D=eER...............  r9 = r8 + 0x18
    D=eER...............  r5 = r5 - r8
    .D=eeER.............  i32 r3 = r3 << r9
    .D=eE-R.............  r5 = r5 + 0x9
    ..DeeeeeeeeeeeeeeeER  jump 34372
```

Gas simulation at offset 34745 with total cost of 26:

```
    DeER.........................  r1 = r1 + 0xfffffffffffffff0
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0x8] = r5
    D=eeeeeeeeeeeeeeeeeeeeeeeeeER  u64 [r1 + 0] = r6
    D............................  r9 = r7
    .DeE------------------------R  r3 = 0x7fffff
    .DeeE-----------------------R  i32 r12 = r7 >> 0x17
    ..DeE-----------------------R  r10 = r8 << 0x21
    ..D=eE----------------------R  r11 = r10 >> 0x38
    ...DeE----------------------R  r7 = r8 & 0xffffffff80000000
    ...D=eE---------------------R  r2 = r9 & r3
    ....DeE---------------------R  r4 = r8 & r3
    ....D=eeeeeeeeeeeeeeeeeeeeE-R  jump 34959 if r12 == 0
```

Gas simulation at offset 34785 with total cost of 21:

```
    DeER....................  r5 = r11 + 0xffffffffffffff01
    DeER....................  r6 = 0xffffffffffffff02
    D=eeeeeeeeeeeeeeeeeeeeER  jump 34959 if r5 <u r6
```

Gas simulation at offset 34797 with total cost of 2:

```
    DeER.  r9 = 0
    DeeER  fallthrough
```

Gas simulation at offset 34800 with total cost of 76:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeER....................................  unlikely
    DeE---------------------------------------R....................................  r12 = r12 - r11
    DeE---------------------------------------R....................................  r4 = r4 | 0x800000
    D=eE--------------------------------------R....................................  r9 = r9 + r12
    .DeE--------------------------------------R....................................  r8 = r2 | 0x800000
    ..DeeE------------------------------------R....................................  i32 r10 = r4 << 0x8
    ...D=eeE----------------------------------R....................................  r11 = 0x7504f333 - r10
    ....DeE-----------------------------------R....................................  r12 = r10 << 0x20
    ....D=eE----------------------------------R....................................  r10 = r12 >> 0x20
    .....D=eeeE-------------------------------R....................................  r10 = r11 * r10
    .....D====eE------------------------------R....................................  r10 = r10 >> 0x20
    ......D====eeeE---------------------------R....................................  i32 r10 = 0 - r10
    .......D======eE--------------------------R....................................  r10 = r10 << 0x20
    .......D=======eE-------------------------R....................................  r10 = r10 >> 0x20
    .......D========eeeE----------------------R....................................  r10 = r10 * r11
    .......D===========eE---------------------R....................................  r10 = r10 >> 0x1f
    ........D===========eE--------------------R....................................  r10 = r10 << 0x20
    .........D===========eeeeE----------------R....................................  r11 = r10 mulhu r12
    ..........D==============eE---------------R....................................  r11 = r11 >> 0x20
    ...........D==============eeeE------------R....................................  i32 r11 = 0 - r11
    ............D================eE-----------R....................................  r11 = r11 << 0x20
    .............D================eeeeE-------R....................................  r11 = r11 mulhu r10
    ..............DeE-------------------------R....................................  r10 = r8 << 0x1
    ..............D===================eE------R....................................  r11 = r11 >> 0x1f
    ..............D====================eE-----R....................................  r11 = r11 << 0x20
    ...............D====================eeeeE-R....................................  r12 = r11 mulhu r12
    ................D=======================eER....................................  r12 = r12 >> 0x20
    .................D=======================eeeER.................................  i32 r12 = 0 - r12
    ..................D=========================eER................................  r12 = r12 << 0x20
    ...................D=========================eeeeER............................  r11 = r12 mulhu r11
    ....................D============================eER...........................  r11 = r11 >> 0x1f
    ....................D=============================eER..........................  r11 = r11 + 0xfffffffffffffff4
    ...........................................D=======eER.........................  r11 = r11 << 0x20
    ...........................................DeE-------R.........................  r12 = r10 << 0x20
    ............................................D=======eeeeER.....................  r11 = r11 mulhu r12
    .............................................D==========eER....................  r12 = r11 >> 0x38
    .............................................D==========eER....................  r11 = r11 >> 0x20
    .............................................D===========eeeeeeeeeeeeeeeeeeeeER  jump 34986 if r12 != 0
```

Gas simulation at offset 34918 with total cost of 23:

```
    DeER......................  r2 = r2 << 0x18
    DeeeER....................  r8 = r4 * r11
    .D==eeER..................  i32 r12 = r2 - r8
    .DeE---R..................  r9 = r9 + 0x7e
    ..D.......................  r8 = r10
    ..DeE--R..................  r10 = 0xfe
    ..D=eeeeeeeeeeeeeeeeeeeeER  jump 35008 if r10 <s r9
```

Gas simulation at offset 34939 with total cost of 20:

```
    DeeeeeeeeeeeeeeeeeeeeER  jump 35057 if r9 <=s 0
```

Gas simulation at offset 34942 with total cost of 16:

```
    DeER...............  r8 = r11 & 0x7fffff
    DeER...............  r9 = r9 << 0x17
    D=eER..............  r9 = r9 | r8
    .DeER..............  r12 = r12 << 0x1
    .DeeeeeeeeeeeeeeeER  jump 35085
```

Gas simulation at offset 34959 with total cost of 21:

```
    DeER....................  r10 = r10 >> 0x21
    DeER....................  r5 = 0x7f800000
    D=eeeeeeeeeeeeeeeeeeeeER  jump 35028 if r5 >=u r10
```

Gas simulation at offset 34971 with total cost of 25:

```
    DeER........................  r7 = r8 | 0x400000
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r5 = u64 [r1 + 0x8]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0]
    .DeE-----------------------R  r1 = r1 + 0x10
    .DeeeeeeeeeeeeeeeeeeeeeeE--R  jump [r0 + 0]
```

Gas simulation at offset 34986 with total cost of 23:

```
    DeER......................  r9 = r9 + 0x7f
    DeER......................  r11 = r11 >> 0x1
    DeER......................  r2 = r2 << 0x17
    .DeeeER...................  r10 = r11 * r4
    ..D==eeER.................  i32 r12 = r2 - r10
    ..DeE---R.................  r10 = 0xfe
    ...DeeeeeeeeeeeeeeeeeeeeER  jump 34939 if r10 >=s r9
```

Gas simulation at offset 35008 with total cost of 2:

```
    DeER.  r8 = 0x7f800000
    D=eER  r7 = r7 | r8
    DeeER  fallthrough
```

Gas simulation at offset 35018 with total cost of 25:

```
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r5 = u64 [r1 + 0x8]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0]
    DeE------------------------R  r1 = r1 + 0x10
    DeeeeeeeeeeeeeeeeeeeeeeE---R  jump [r0 + 0]
```

Gas simulation at offset 35028 with total cost of 20:

```
    DeeeeeeeeeeeeeeeeeeeeER  jump 35018 if r10 == 2139095040
```

Gas simulation at offset 35035 with total cost of 20:

```
    DeeeeeeeeeeeeeeeeeeeeER  jump 35110 if r9 == 0
```

Gas simulation at offset 35038 with total cost of 20:

```
    DeeeeeeeeeeeeeeeeeeeeER  jump 35129 if r10 == 0
```

Gas simulation at offset 35041 with total cost of 20:

```
    DeeeeeeeeeeeeeeeeeeeeER  jump 35145 if r12 != 0
```

Gas simulation at offset 35044 with total cost of 17:

```
    DeER................  i32 r8 = clz r2
    D=eER...............  r5 = r8 + 0x18
    .DeeER..............  r9 = 0x9 - r8
    ..DeeER.............  i32 r2 = r2 << r5
    ..DeeeeeeeeeeeeeeeER  jump 35148
```

Gas simulation at offset 35057 with total cost of 21:

```
    DeER....................  r10 = 0xffffffffffffffe9
    D=eeeeeeeeeeeeeeeeeeeeER  jump 35018 if r9 <s r10
```

Gas simulation at offset 35063 with total cost of 12:

```
    DeER...........  r10 = r9 + 0x17
    .DeeeER........  i32 r12 = 0x1 - r9
    ..D==eeER......  i32 r9 = r11 >> r12
    ...DeeE-R......  i32 r8 = r8 << r10
    ....D==eeeER...  r10 = r4 * r9
    ....D=====eER..  r10 = r10 << 0x1
    .....D=====eeER  i32 r12 = r8 - r10
    .....DeeE-----R  fallthrough
```

Gas simulation at offset 35085 with total cost of 28:

```
    DeER...........................  r8 = r9 & 0x1
    D=eeER.........................  i32 r8 = r8 + r12
    .D==eeeER......................  r8 = r4 <u r8
    ..D====eeER....................  i32 r8 = r8 + r9
    ..D======eER...................  r7 = r7 | r8
    ..DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r5 = u64 [r1 + 0x8]
    ...DeeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0]
    ...DeE------------------------R  r1 = r1 + 0x10
    ...DeeeeeeeeeeeeeeeeeeeeeeE---R  jump [r0 + 0]
```

Gas simulation at offset 35110 with total cost of 26:

```
    DeER.........................  r8 = 0x7fc00000
    D=eeER.......................  r7 = r8 if r10 == 0
    DeeeeeeeeeeeeeeeeeeeeeeeeeER.  r5 = u64 [r1 + 0x8]
    .DeeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0]
    .DeE------------------------R  r1 = r1 + 0x10
    .DeeeeeeeeeeeeeeeeeeeeeeE---R  jump [r0 + 0]
```

Gas simulation at offset 35129 with total cost of 25:

```
    DeER........................  r7 = r8 | 0x7f800000
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r5 = u64 [r1 + 0x8]
    DeeeeeeeeeeeeeeeeeeeeeeeeeER  r6 = u64 [r1 + 0]
    .DeE-----------------------R  r1 = r1 + 0x10
    .DeeeeeeeeeeeeeeeeeeeeeeE--R  jump [r0 + 0]
```

Gas simulation at offset 35145 with total cost of 2:

```
    DeER.  r9 = 0
    DeeER  fallthrough
```

Gas simulation at offset 35148 with total cost of 2:

```
    DeER.  r10 = r10 >> 0x17
    D=eER  jump 34800 if r10 != 0
```

Gas simulation at offset 35155 with total cost of 17:

```
    DeER................  i32 r8 = clz r4
    D=eER...............  r10 = r8 + 0x18
    D=eER...............  r8 = r8 + r9
    .D=eeER.............  i32 r4 = r4 << r10
    ..DeE-R.............  r9 = r8 + 0xfffffffffffffff7
    ..DeeeeeeeeeeeeeeeER  jump 34800
```

