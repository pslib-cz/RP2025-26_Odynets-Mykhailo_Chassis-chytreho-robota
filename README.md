# Podvozek

## Před začatkem prace:
- nastudovat robotiku, elektroniku, 3D modelování
- udělat výzkum světu robotu
- promyslet potřebné cíle a způsoby jejich realizace

## Na podvozku se musí umístit:
- 2 motory
- ultrasonický senzor
- ir senzor
- baterie
- robot controller (Mictobit nebo Raspberry Pi)
- motor driver
- kabely

## Dodatečně
- Displej
- Kamera
- Lidar

## 3D model:
- 2 kola
- modularní
- - každý modul má svoje použití (Napřiklad modul pro motory, modul pro ultrasonický senzor atd)
  - Systém pro spojení modulu

## Vybrané součastky:
Raspberry Pi


# 🤖 Modulární 2WD Robotický Podvozek

Tento projekt definuje univerzální mechanickou platformu pro malá kolová vozidla. Konstrukce klade důraz na extrémní modularitu a snadnou vyrobitelnost na běžných FDM 3D tiskárnách.

---

## 🏗 Popis konstrukce

Podvozek je navržen jako otevřený systém, který není vázán na konkrétní rozměry elektroniky nebo typy motorů.

### 🔲 Univerzální Grid (Mřížka)
Celá základna je tvořena rastrem otvorů o průměru **3.5 mm** (pro šrouby M3) s roztečí **20 mm**.  
To umožňuje připevnit jakoukoli komponentu pomocí jednoduchých tištěných adaptérů.

### 🧱 Sandwich Concept (Dvoupatrové uspořádání)

- **Spodní patro**
  - Mechanický pohon (motory)
  - Zdroj energie (baterie)
  - Opěrné kolečko  
  👉 Zajišťuje nízké těžiště a stabilitu

- **Horní patro**
  - Řídicí elektronika
  - Senzory  
  👉 Odděleno pomocí distančních sloupků (čistá zóna)

### 🔌 Cable Management
- Podélný slot ve středu podvozku pro vertikální vedení kabelů  
- Integrovaná očka po obvodu pro fixaci kabeláže (stahovací pásky)

### 🖨 Design pro 3D tisk
- Všechny díly jsou navrženy jako **flat design**
- Není potřeba tiskových podpor
- Vyšší pevnost vrstev
- Minimalizace warping efektu

---

## 🛠 Seznam komponent

Podvozek je připraven pro osazení následující sestavou (nebo jejich ekvivalenty):

| Kategorie            | Komponenta              | Specifikace |
|---------------------|------------------------|------------|
| 🚗 Pohon            | 2x DC Motor            | Typicky žlutý "TT motor" (převodovka 1:48) |
| ⚖️ Stabilizace      | 1x Caster Wheel        | Otočné kuličkové kolečko (v ložisku) |
| 🧠 Řízení           | Micro:bit / Raspberry Pi | Hlavní procesorová jednotka |
| ⚡ Výkonová část     | Motor Driver           | L298N, L293D nebo DRV8833 |
| 📡 Senzorika (Dálka)| Ultrasonický senzor    | HC-SR04 pro detekci překážek |
| 🛣 Senzorika (Trasa)| IR Senzor              | Infračervený modul pro sledování čáry |
| 👁️ Senzorika (Obraz) | Kamera                 | Např. Raspberry Pi Camera Module |
| 🧭 Senzorika (Mapování) | LiDAR               | Např. VL53L0X / RPLIDAR |
| 🖥️ Výstup             | Displej                | Malý (např. SSD1306, I2C) |
| 🔋 Napájení         | Akumulátor             | Li-ion pack (7.4V) nebo powerbanka |
| 🔩 Spojovací materiál | Šrouby a matice      | Nerezové M3 (různé délky) |

---

## 📌 Vlastnosti

- ✅ Vysoce modulární konstrukce  
- ✅ Kompatibilní s běžnými komponentami  
- ✅ Optimalizováno pro FDM 3D tisk  
- ✅ Snadná rozšiřitelnost pomocí adaptérů  
- ✅ Vhodné pro edukaci i prototypování  

---

## 🚀 Možné využití

- Line follower robot  
- Autonomní robot s detekcí překážek  
- Edukační platforma pro programování a robotiku  
- IoT experimenty
