[README_compra.md](https://github.com/user-attachments/files/27962055/README_compra.md)
# 🛒 Llista de la Compra Familiar

App per gestionar la llista de la compra de casa, compartida entre tots els membres de la família en temps real gràcies a la sincronització amb Dropbox.

---

## 📱 Instal·lació al mòbil

1. Obre Safari i accedeix a la URL de l'app
2. Prem el botó de compartir (quadrat amb fletxa cap amunt)
3. Selecciona **"Afegir a pantalla d'inici"**
4. Posa-li el nom **"Compra"** i prem **"Afegir"**

> ⚠️ Cal obrir-la sempre des de Safari (no Chrome ni cap altre navegador) perquè les dades es guardin correctament.
> Repeteix el procés a cada mòbil de casa que vulgui compartir la llista.

---

## ⚙️ Configuració inicial (primer ús)

Per sincronitzar la llista entre dispositius cal configurar el token de Dropbox:

1. Ves a **[dropbox.com/developers/apps](https://dropbox.com/developers/apps)**
2. Entra a l'app **LlistaCompra**
3. Pestanya **Settings** → apartat **OAuth 2** → prem **"Generate"**
4. Copia el token generat
5. A l'app, ves a **Ajustos** → enganxa el token → prem **"Guardar token"**
6. El punt de la barra superior es posarà **verd** si la connexió és correcta

> Repeteix el pas 5 a cada mòbil de casa amb el **mateix token**.

> ⚠️ El token és com una contrasenya. No el comparteixis públicament.

---

## 🗂️ Estructura de l'app

L'app té tres pestanyes:

### Llista
La llista de la compra activa. Mostra els articles pendents i els ja agafats.

### Habituals
Articles que es compren sovint. Un sol toc els afegeix directament a la llista.

### Ajustos
Configuració del token de Dropbox i gestió de les categories.

---

## ➕ Afegir un article a la llista

1. Prem el botó **+** (part inferior dreta de la pestanya Llista)
2. Escriu el nom de l'article
3. Afegeix la quantitat o notes si cal (p.ex. "2 litres", "sense lactosa")
4. Selecciona la categoria
5. Prem **"Afegir"**

---

## ✅ Marcar un article com a agafat

Prem sobre qualsevol article de la llista per marcar-lo com a agafat. Es mourà a la secció **"Ja agafats"** de la part inferior.

Per desmarcar-lo, torna a prémer-lo.

---

## 🗑️ Netejar els articles agafats

Un cop acabada la compra, prem la icona ✓✓ de la part superior dreta per eliminar tots els articles marcats com a agafats.

---

## ⭐ Articles habituals

Els habituals són articles que compres sovint i que vols poder afegir ràpidament a la llista.

**Afegir un habitual:**
1. Ves a la pestanya **Habituals**
2. Prem el botó **+**
3. Omple el nom, la quantitat habitual i la categoria
4. Prem **"Guardar"**

**Afegir un habitual a la llista:**
- Prem sobre qualsevol article habitual → s'afegeix directament a la llista
- Els articles que ja són a la llista es mostren amb fons verd

---

## 🔄 Sincronització

L'app es sincronitza automàticament amb Dropbox:
- En obrir l'app
- Cada 30 segons mentre l'app és oberta
- En tornar a l'app després d'estar en segon pla
- Manualment prement la icona 🔄 de la part superior dreta

L'estat de la sincronització es mostra a la barra sota el títol:
- 🟢 **Verd** — sincronitzat correctament
- 🟠 **Taronja** — sincronitzant...
- 🔴 **Vermell** — error de connexió
- ⚪ **Gris** — sense token configurat

---

## 📂 Categories per defecte

Fruita i verdura, Làctics, Carn i peix, Pa i cereals, Conserves, Neteja, Higiene, Begudes, Congelats, Altres

Les categories es poden afegir, editar o eliminar des de **Ajustos → Categories → Editar**.

---

## 💾 Emmagatzematge de dades

- Les dades es guarden a **Dropbox** (fitxer `llista_compra.json` a la carpeta de l'app)
- També es guarden localment al dispositiu com a còpia de seguretat
- Si no hi ha connexió, els canvis es guarden localment i es sincronitzen quan es recupera la connexió

---

## 🛠️ Actualitzar l'app

Si es publica una nova versió del fitxer `index.html` a GitHub, les dades existents es conserven ja que estan a Dropbox, independent del codi de l'app.
