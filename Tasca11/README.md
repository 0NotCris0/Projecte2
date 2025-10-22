# 🧩 T11 - WordPress Local

## 🎯 Objectius de la tasca

- Aprendre a utilitzar **WP Local** per gestionar instal·lacions de WordPress en local.  
- Crear i configurar un lloc web de proves individual.  
- Practicar amb les funcionalitats bàsiques de WordPress (pàgines, entrades, ajustaments generals).  
- Mantenir una instal·lació activa al llarg del curs que servirà com a base de totes les pràctiques.

---

## 🪜 Passos a realitzar

### 1. Obrir WP Local
- Inicia el programari **WP Local** al PC de classe.  
- Comprova que el panell principal estigui buit o que només hi hagi les webs ja creades.

### 2. Crear un nou lloc de WordPress
- Afegeix una nova instal·lació des del botó **“Create a new site”**.  
- Escriu el nom de la teva web seguint aquest patró:  
  `web_proves_[Nom]`  
  *(Per exemple: web_proves_Cristian — però posa-hi el teu nom!)*

### 3. Configuració inicial
- Configura l’usuari i contrasenya d’administrador (apunta-te’ls per no oblidar-los).  
- Utilitza el **correu de l’escola**, per exemple:  
  `cristian.gonzalez@mataro.epiaedu.cat`  
- Nom d’usuari: igual que el correu, però sense la part final (`@mataro.epiaedu.cat`).  
  Exemple: `cristian.gonzalez`
- ⚠️ **Contrasenya:** fàcil de recordar. No hi ha sistema de recuperació.  
- Mantén la configuració per defecte de **PHP**, **MySQL** i **servidor web**.  
- Finalment, fes clic a **Add Site** i espera que acabi la instal·lació.

---

## 🔑 Accedir al tauler d’administració

Un cop creat el lloc, arriba el moment d’accedir al **tauler d’administració**, on podràs gestionar pàgines, entrades, menús, disseny i configuracions.

### Què és el `wp-admin`?
És l’adreça (URL) que porta al panell de control intern de WordPress:  
`http://web_proves_nom.local/wp-admin`

És com la porta privada de la teva web, des d’on pots:
- Crear i editar pàgines i entrades.  
- Canviar l’aspecte del web (temes, menús, ginys...).  
- Configurar opcions generals (nom del lloc, idioma, comentaris, etc.).  
- Gestionar usuaris i rols.

💡 **Pensa-hi així:**  
El `wp-admin` és com la *cuina d’un restaurant*: no la veu el públic, però és on es prepara tot.

---

## 🌍 Distingir entre vista d’administrador i vista pública

| Vista | URL aproximada | Descripció |
|-------|----------------|-------------|
| 🧑‍💻 **Vista d’administrador** | `http://web_proves_nom.local/wp-admin` | Zona privada per gestionar i configurar el web. |
| 👀 **Vista pública** | `http://web_proves_nom.local` | El que veuen els visitants del teu lloc. Només mostra contingut publicat. |

💡 **Canviar de vista fàcilment:**
- Des del tauler → clic al nom del web → “**Visita el lloc**”.
- Des del lloc públic → barra negra superior → “**Tauler**”.

---

## ⚙️ Accions inicials

1. Entra a l’URL que et proporciona WP Local (`http://web_proves_nom.local`).  
2. Accedeix al tauler de WordPress amb el teu usuari i contrasenya.

---

## 🎨 Canvi de tema: *Twenty Seventeen*

**Motiu:** Tema oficial de WordPress, clàssic i ideal per a formació bàsica.

**Característiques:**
- Pàgina d’inici amb imatge de capçalera.  
- Suport per a menú principal i menú de peu.  
- Personalització des del *Personalitzador clàssic*.  
- Compatible amb editor clàssic i Gutenberg bàsic.  
- Disseny *responsive* i net.

---

## 🚀 Primers passos amb WordPress

### 1. Crear una primera pàgina de prova
- Títol: **Benvinguts al meu web personal**  
- Contingut: breu presentació sobre tu mateix.  
  💡 Pots fer servir *Lorem Ipsum* si no saps què escriure.  
- Fes clic a **Publica** i després a **Veure pàgina**.

### 2. Crear una segona pàgina: *Les meves mascotes 🐾*
- Títol: **Les meves mascotes**  
- Explica si tens alguna mascota (o inventa-te’n una).  
- Afegeix una imatge.  
  *(Afegeix un bloc → Imatge)*

### 3. Crear una pàgina buida per al blog
- Títol: **Blog**  
- Sense contingut: aquí s’hi mostraran les entrades.

---

## 📝 Crear tres entrades de blog

Ves a **Entrades → Afegir nova** i crea:

1. **Opinió sobre una sèrie - Capítol 1**  
   Explica breument què t’agrada d’una sèrie (One Piece, Stranger Things, The Boys...).  
   Afegeix imatges, imatge destacada, categories i etiquetes.  

2. **Opinió sobre una sèrie - Capítol 2**

3. **Opinió sobre una sèrie - Capítol 3**

💡 Pots generar el text amb ChatGPT per fer-lo més complet.

---

## 🔍 Diferència entre pàgines i entrades

| Tipus | Funció | Exemple |
|-------|---------|----------|
| **Pàgines** | Contingut fix i atemporal. | “Benvinguts”, “Contacte”, “Les meves mascotes” |
| **Entrades** | Contingut dinàmic, ordenat cronològicament. | Articles del blog, notícies, opinions |

---

## 📬 Crear una pàgina de contacte

1. Ves a **Pàgines → Afegir nova**.  
2. Títol: **Contacte**  
3. Escriu un petit text:  
   > Si vols contactar amb mi per parlar de sèries, tecnologia o gats, pots escriure’m.

💡 Més endavant afegirem formularis reals, però de moment n’hi ha prou amb el text.

---

## ⚙️ Configuració bàsica del lloc

Per defecte, WordPress mostra les **entrades recents** a la pàgina principal.  
Nosaltres configurarem una **pàgina fixa com a inici** i una altra per a les entrades.

### Passos
1. Entra al tauler (**wp-admin**).  
2. Ves a **Configuració → Lectura**.  
3. A “La pàgina d’inici mostra”, marca:
   - 🔘 **Una pàgina estàtica (selecciona a sota)**  
   - **Pàgina d’inici:** *Benvinguts al meu web personal*  
   - **Pàgina de les entrades:** *Blog*  
4. Fes clic a **Desa els canvis**.

---

## 🧾 Documentació de la tasca

Crea el fitxer:  
`T11_wordpress_local.md` dins la carpeta `T11/` del teu repositori GitHub.

### Contingut del document:
- Nom de la web creada.  
- Captures de pantalla del procés:  
  - Creació amb WP Local.  
  - Tauler de WordPress.  
  - Pàgina i entrada creades.  
- Explicació de la diferència entre pàgines i entrades.  
- Descripció dels ajustaments configurats.

---

