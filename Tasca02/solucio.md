# 💡 T02: Selecció d’un SAI per una empresa client  
**Autor:** Christian Bogdanas  
**Grup:** SMX2B  
**Assignatura:** Seguretat Informàtica  
**Data:** 30/09/2025  

🔗 [Document original (Google Docs)](https://docs.google.com/document/d/14Zz6phLE-ikib-ifr_s3p1atZdt6ppIlHDLgDQN1hdU/edit?usp=sharing)

![Imagen de chico tocando sai](img/manga2.png)

---

## 📑 Índex
- Descripció del cas  
- Equips i consum estimat  
- Models de referència  
- Càlculs  
  - Desglossament per equips  
  - Total sense reserva  
  - Reserva del 20%  
- Càlcul de l’autonomia del SAI  
  - Dades de partida  
  - Substitució de valors  
  - Desenvolupament de les operacions  
  - Resultat final  
  - Conclusió  
- Comparació de SAI  
  - Opció 1: SLC-4000-TWIN RT3  
  - Opció 2: SLC-7,5-CUBE4  
- Comparativa d’opcions de SAI  
- Conclusió  

---

## 🏢 Descripció del cas
L’empresa **TecnoGestió S.L.**, dedicada a la **gestió documental** i **assessorament informàtic**, té un petit despatx amb:
- 4 ordinadors de sobretaula  
- 1 impressora-fotocopiadora multifunció (similar a les que té l’escola)  
- 1 router d’accés a Internet  

Davant les constants incidències amb el **subministrament elèctric** a la zona, la direcció ha decidit adquirir un **SAI** per garantir la **continuïtat del servei** i **protegir els equips**.

S’han posat en contacte amb l’empresa on esteu fent l’estada i el vostre responsable us ha encarregat que en feu **l’estudi i tria del SAI.**

---

## ⚙️ Equips i consum estimat
- 4 ordinadors: 584 V × 4  
- Processadors: 65 V × 4  
- 4 monitors: 55 V × 4  
- Router: 39 V × 1  

### Models de referència
- **Ordinador:** [VolttierPC Oficina AMD Ryzen 5 5600G, 32 GB, 1 TB SSD](https://www.pccomponentes.com/ordenador-sobremesa-volttierpc-pc-oficina-amd-ryzen-5-5600g-32gb-1tb-ssd)  
- **Monitor:** [MSI PRO MP242A E2 23.8" LED IPS FullHD 120 Hz](https://www.pccomponentes.com/monitor-msi-pro-mp242a-e2-238-led-ips-fullhd-120hz)

---

## 🧮 Càlculs

### 🔹 Desglossament per equips
- 4 Ordinadors: 584 × 4 = 2.336 VA  
- 4 Processadors: 65 × 4 = 260 VA  
- 4 Monitors: 55 × 4 = 220 VA  
- 1 Router: 39 × 1 = 39 VA  

### 2️⃣ Total sense reserva
2.336 + 260 + 220 + 39 = 2.855 VA (≈ 2.855 W)

### 3️⃣ Reserva del 20%
2.855 × 0,20 = 571 VA (≈ 571 W)

### 4️⃣ Total amb reserva
2.855 + 571 = 3.426 VA (≈ 3.426 W)


---

## 🔋 Càlcul de l’autonomia del SAI

El SAI ha de garantir un **temps mínim d’uns 10 minuts**, prou per desar els treballs i apagar correctament els equips.

Per calcular l’autonomia necessària del SAI, s’utilitza la fórmula següent:

Capacitat de les bateries (Ah) = Temps (min) × Potència (VA) / (Eficiència × 60)


### 1️⃣ Dades de partida
- Potència total dels equips (amb reserva del 20%): **3.426 VA**  
- Temps d’autonomia desitjat: **10 minuts**  
- Eficiència del SAI: **0,7 (70%)**

### 2️⃣ Substitució de valors
Capacitat = (10 × 3.426) / (0,7 × 60)


### 3️⃣ Desenvolupament de les operacions
10 × 3.426 = 34.260

0,7 × 60 = 42

34.260 ÷ 42 = 815,7


### 4️⃣ Resultat final
Capacitat de les bateries = 815,7 Ah


### 5️⃣ Conclusió
Per mantenir els equips amb una potència total de **3.426 VA** durant **10 minuts**, i tenint en compte una eficiència del **70%**, el SAI hauria de disposar d’una **bateria amb una capacitat aproximada de 816 Ah**.  
Aquesta autonomia seria suficient per poder desar els treballs i apagar correctament tots els equips en cas de tall de subministrament elèctric.

---

## ⚖️ Comparació de SAI

### 🅰️ Opció 1: SLC-4000-TWIN RT3
- Potència: **4.000 VA (FP = 1 → 4.000 W reals)**  
- Tipus: **On-line doble conversió**  
- Format: **Torre / Rack 3U**  
- Fases: **Monofàsic**  
- Aplicació típica: petites i mitjanes instal·lacions (oficines, servidors mitjans, xarxes).  
- Avantatge clau: compacte, flexible i suficient per a la càrrega de **3.426 W**.

---

### 🅱️ Opció 2: SLC-7,5-CUBE4
- Potència: **7.500 VA (FP = 1 → 7.500 W reals)**  
- Tipus: **On-line doble conversió**  
- Format: **Torre (CUBE)**  
- Fases: **Trifàsic**  
- Aplicació típica: grans instal·lacions, CPDs, entorns crítics amb alta demanda.  
- Avantatge clau: major escalabilitat i redundància, però amb més cost i complexitat.

---

## 📊 Comparativa d’opcions de SAI

| **Característica** | **Opció 1: SLC-4000-TWIN RT3** | **Opció 2: SLC-7,5-CUBE4** |
|--------------------|----------------------------------|-----------------------------|
| **Potència nominal** | 4.000 VA (FP = 1 → 4.000 W) | 7.500 VA (FP = 1 → 7.500 W) |
| **Tipus de tecnologia** | On-line doble conversió | On-line doble conversió |
| **Format físic** | Torre / Rack 3U | Torre (CUBE) |
| **Fases** | Monofàsic | Trifàsic |
| **Aplicació típica** | Petites i mitjanes instal·lacions: oficines, servidors mitjans, xarxes locals. | Grans instal·lacions, CPDs i entorns crítics amb alta demanda energètica. |
| **Avantatge principal** | Compacte, flexible i suficient per cobrir la càrrega actual (3.426 W). | Major escalabilitat, redundància i capacitat per a futurs increments de càrrega. |
| **Inconvenient principal** | Menor marge de creixement si augmenta la càrrega. | Cost i complexitat més elevats per una càrrega moderada. |

---

## 🧩 Conclusió
Tenint en compte que la **càrrega total calculada és de 3.426 VA**, l’**Opció 1 (SLC-4000-TWIN RT3)** és la més adequada, ja que ofereix **capacitat suficient, eficiència i compacitat**, sense sobredimensionar el sistema.  

L’**Opció 2 (SLC-7,5-CUBE4)** seria recomanable només si es preveu un **increment significatiu de la demanda** o si és necessària una **infraestructura més robusta i escalable**.

---


