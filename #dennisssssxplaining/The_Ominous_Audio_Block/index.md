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

## if you want to know more about DSP+music+programming:

---

### tutorials

- https://www.hackaudio.com/ 
- http://www.martin-finke.de/articles 
- http://basicsynth.com 
- http://www.musicdsp.org 
- [SynthSchool](https://www.youtube.com/@SynthSchool) ( "videos on basic synthesizer techniques" )
    - https://youtu.be/A6pp6OMU5r8
    - https://youtu.be/9niampRkFW0
    - https://youtu.be/YsZKvLnf7wU
    - https://youtu.be/ZQcEyXI1OGM
    - etcetera
- [Phil’s Lab: DSP](https://www.youtube.com/playlist?list=PLXSyc11qLa1ZCn0JCnaaXOWN6Z46rK9jd) ( "basic DSP techniques implemented in C … not limited to audio" )
- [Ableton: Get started making music](https://learningmusic.ableton.com)
- …

---

### further readings:

- [Curtis Roads: The Computer Music Tutorial](https://mitpress.mit.edu/9780262044912/the-computer-music-tutorial/)
- [Richard Boulanger + Victor Lazzarini: The Audio Programming Book](https://mitpress.mit.edu/9780262014465/the-audio-programming-book/)
- [Gareth Loy: Musimathics, Volume 1: The Mathematical Foundations of Music](https://mitpressbookstore.mit.edu/book/9780262516556) http://www.musimathics.com
- …

---

EOF
