---
size: 16:9
---

The Ominous Audio Block

---

this is how most Digital Signal Processing (DSP) interfaces with the world:

```cpp
void process(float[][] input, float[][] output) {
     // process input + output
}
```

---

# why should you know about this?

---

## 1. if you want to use or integrate or modify:

- libraries
- APIs
- snippets ( e.g from ChatGPT )

---

## 2. if you want to roll your own:

- libraries
- VSTs ( or Audio Units )
- write MCU code
- application
- transcend the confinements of *programming* languages e.g
    - processing/java
    - c/c++
    - rust

---

bottomline, you should know about `The Ominous Audio Block`

---

an extremely brief explanation of `The Ominous Audio Block`

---

> instead of just calculating a signal *sample by sample*, it is produced in a block aka an `Audio Block`.

---

```
  ×         ×             ×              
  |         | ×           | ×            
  | ×     × | | ×         | |         ×  
  | | ×   | | | |       × | |     × × | ×
  | | | × | | | | ×   × | | | × | | | | |
  | | | | | | | | | × | | | | | × | | | |
+----------------------------------------> TIME

  × × × × × × × × × × × × × × × × × × × ×  SAMPLES OVER TIME
 -|---------------|---------------|------  AUDIO BLOCKS OF 8 SAMPLES
```

---

BTW a `SAMPLE` is usually a float value between `‌[-1.0, 1.0]`.

---

some libraries and projects that use this concept:

- [Klangstrom](https://github.com/dennisppaul/klangstrom-arduino) #arduino ==TODO upload update==
- [Wellen](https://github.com/dennisppaul/wellen) #processing
- [Mozzi](https://sensorium.github.io/Mozzi/learn/) #arduino
- [Teensy Audio Library](https://www.pjrc.com/teensy/td_libs_Audio.html) with the help of [Klangstrom Teensy Audio Library](https://github.com/dennisppaul/klangstrom-teensy)
- [Mutable Instruments](https://github.com/pichenettes)
- [DaisySP](https://github.com/electro-smith/DaisySP)

and many, many more.

---

PS why should i learn DSP in the first place when there are all these nice visual environements and DAWs?

---

## reason#1

become literate in the basic building blocks.    
do not just *consume* but also become able to *produce*.

---

## reason#2 

translates well into other contexts e.g MCU

---

## reason#3

sonification ( data + parameters + interactions )

---

EOF