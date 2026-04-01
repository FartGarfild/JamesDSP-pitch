# JamesDSP Pitch Shifter (Liveprog)

**Real-time pitch shifting plugin for JamesDSP**

Працює на **Android (RootlessJamesDSP)** і **на ПК** (desktop версія JamesDSP / JDSP4Linux).

---

### 🇺🇦 Українська версія

#### Історія створення
Написано і повністю протестовано **на телефоні**.  
Тестував на **OPPO Enco Air 4 Pro** з кодеком **LHDC 5.0** — якість звуку висока, артефакти добре контролюються.

#### Особливості
- Гранулярний pitch shifter з **повним ручним налаштуванням** усіх параметрів
- Від легкої корекції тону до креативних ефектів (робот-голос, вінтажне радіо, granular destruction)
- Артефакти на високому/низькому пітчі добре контролюються вибором **window size** та **buffers**
- Параметр **smooth** можна технічно зменшити з 0.001 до 0.0001 для ще більш плавного звучання, але це значно підвищує навантаження на CPU. Тому за замовчуванням залишено 0.001 — його достатньо в більшості випадків і він добре помітний.

#### Рекомендовані пресети

**Robot Voice**  
Pitch: -3  
Window size: 30 ms  
Dry mix: -5 dB  
Buffers: 32  
Smooth: 0.001

**Vintage Radio**  
Pitch: -2 … -5  
Window size: 5 ms  
Dry mix: -120 dB (або додай echo)  
Buffers: 32  
Smooth: 0.001

**Clean Pitch (максимально прозорий)**  
Pitch: +1 … -1  
Window size: 200–300 ms  
Dry mix: -15 … -30 dB  
Buffers: 4–8  
Smooth: 0.001

**Granular Destruction ("metal destruction")**  
Pitch: -8 … -12  
Window size: 800–1000 ms  
Dry mix: -10 dB  
Buffers: 2–4  
Smooth: 0.001

**Порада щодо артефактів і плавності:**
- На високому пітчі зменшуй **window size** і **buffers** — ефект стає чистішим.
- Якщо в тебе потужний пристрій і хочеш максимальну плавність — спробуй зменшити **smooth** до 0.0001 (але стеж за навантаженням на процесор).
- Найкраще звучання виходить, коли ти сам підбираєш параметри під трек і навушники.

#### Встановлення
1. Завантаж файл `pitch_shifter.eel`
2. У JamesDSP → **Liveprog** → імпортуй або додай скрипт
3. Увімкни і налаштуй слайдери на свій смак

Скрипт дає **повну свободу** ручного керування — в цьому його головний прикол.

---

### 🇬🇧 English version

#### About
Written and fully tested **on a smartphone**.  
Tested on **OPPO Enco Air 4 Pro** with **LHDC 5.0** codec — high audio quality, artifacts are well controlled.

#### Features
- Granular pitch shifter with **full manual control** of all parameters
- From subtle pitch correction to creative effects (robot voice, vintage radio, granular destruction)
- Artifacts at high/low pitch are well controlled by **window size** and **buffers**
- The **smooth** parameter can technically be lowered from 0.001 to 0.0001 for even smoother sound, but it significantly increases CPU usage. Therefore, the default is left at 0.001 — it is sufficient in most cases and clearly audible.

#### Recommended Presets

**Robot Voice**  
Pitch: -3  
Window size: 30 ms  
Dry mix: -5 dB  
Buffers: 32  
Smooth: 0.001

**Vintage Radio**  
Pitch: -2 … -5  
Window size: 5 ms  
Dry mix: -120 dB (or add echo)  
Buffers: 32  
Smooth: 0.001

**Clean Pitch (maximum transparency)**  
Pitch: +1 … -1  
Window size: 200–300 ms  
Dry mix: -15 … -30 dB  
Buffers: 4–8  
Smooth: 0.001

**Granular Destruction ("metal destruction")**  
Pitch: -8 … -12  
Window size: 800–1000 ms  
Dry mix: -10 dB  
Buffers: 2–4  
Smooth: 0.001

**Tips:**
- For high pitch, reduce **window size** and **buffers** — the effect becomes much cleaner.
- If you have a powerful device and want maximum smoothness, try lowering **smooth** to 0.0001 (but monitor CPU load).
- Best results come when you tweak the parameters yourself for your track and headphones.

#### Installation
1. Download the file `pitch_shifter.eel`
2. In JamesDSP → **Liveprog** → import or add the script
3. Enable and adjust the sliders to your taste

The script gives **full manual control** — that's the main fun of Liveprog.

---

**Made on a phone in one evening** 😎  
Tested on OPPO Enco Air 4 Pro (LHDC 5.0)  
Works on both Android and Desktop JamesDSP
