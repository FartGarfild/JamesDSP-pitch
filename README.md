# JamesDSP Pitch Shifter (Liveprog)

**Real-time pitch shifting plugin for JamesDSP**

Працює на **Android (RootlessJamesDSP)** і **на ПК** (desktop версія JamesDSP / JDSP4Linux), оскільки EEL-скрипти універсальні.

---

### 🇺🇦 Українська версія

#### Історія створення
Написано і повністю протестовано **на телефоні**.  
Тестував на **OPPO Enco Air 4 Pro** з кодеком **LHDC 5.0** — якість звуку висока, артефакти добре контролюються.

#### Особливості
- Гранулярний pitch shifter з **повним ручним налаштуванням** усіх параметрів через інтерфейс JamesDSP
- Від легкої корекції тону до креативних ефектів: робот-голос, вінтажне радіо, granular destruction
- Артефакти на високому/низькому пітчі мінімізуються правильним вибором **window size** та **buffers**
- Ніяких прихованих обмежень — максимальна свобода для експериментів

#### Рекомендовані пресети

**Robot Voice**  
Pitch: -3  
Window size: 30 ms  
Dry mix: -5 dB  
Buffers: 32

**Vintage Radio**  
Pitch: -2 … -5  
Window size: 5 ms  
Dry mix: -120 dB (або додай echo)  
Buffers: 32

**Clean Pitch (максимально прозорий)**  
Pitch: +1 … -1  
Window size: 200–300 ms  
Dry mix: -15 … -30 dB  
Buffers: 4–8

**Granular Destruction ("metal destruction")**  
Pitch: -8 … -12  
Window size: 800–1000 ms  
Dry mix: -10 dB  
Buffers: 2–4

**Порада:**  
На високому пітчі зменшуй window size і buffers — ефект стає значно чистішим.  
Найкраще звучання виходить, коли сам підбираєш параметри під свій трек і навушники.

#### Встановлення
1. Завантаж файл `pitch_shifter.eel`
2. У JamesDSP → **Liveprog** → імпортуй або додай скрипт
3. Увімкни і налаштуй слайдери на свій смак

Скрипт повністю відкритий для ручного керування — в цьому його головний прикол.

---

### 🇬🇧 English version

#### About
Written and fully tested **on a smartphone**.  
Tested on **OPPO Enco Air 4 Pro** with **LHDC 5.0** codec — high sound quality, artifacts are well controlled.

#### Features
- Granular pitch shifter with **full manual control** of all parameters via JamesDSP interface
- From subtle pitch correction to creative effects: robot voice, vintage radio, granular destruction
- Artifacts at high/low pitch are minimized by proper **window size** and **buffers** settings
- No hidden limitations — maximum freedom for experiments

#### Recommended Presets

**Robot Voice**  
Pitch: -3  
Window size: 30 ms  
Dry mix: -5 dB  
Buffers: 32

**Vintage Radio**  
Pitch: -2 … -5  
Window size: 5 ms  
Dry mix: -120 dB (or add echo)  
Buffers: 32

**Clean Pitch (maximum transparency)**  
Pitch: +1 … -1  
Window size: 200–300 ms  
Dry mix: -15 … -30 dB  
Buffers: 4–8

**Granular Destruction ("metal destruction")**  
Pitch: -8 … -12  
Window size: 800–1000 ms  
Dry mix: -10 dB  
Buffers: 2–4

**Tip:**  
For high pitch, reduce window size and buffers — the effect becomes much cleaner.  
Best sound comes when you tweak the parameters yourself for your track and headphones.

#### Installation
1. Download the file `pitch_shifter.eel`
2. In JamesDSP → **Liveprog** → import or add the script
3. Enable and adjust the sliders to your taste

The script gives **full manual control** — that's the main fun of Liveprog.

---

**Made on a phone in one evening** 😎  
Tested on OPPO Enco Air 4 Pro (LHDC 5.0)  
Works on both Android and Desktop JamesDSP
