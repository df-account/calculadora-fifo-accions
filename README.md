# 📈 Calculadora FIFO d'Accions

Una aplicació web d'una sola pàgina (HTML) per calcular guanys i pèrdues fiscals en la venda d'accions d'una única empresa, seguint el mètode **FIFO** (*First In, First Out*).

Dissenyada per a ús personal, funciona completament al navegador, sense servidor ni instal·lació. Optimitzada per a mòbil.

---

## ✨ Característiques

- **Mètode FIFO**: consumeix automàticament els lots de compra més antics en cada venda
- **Resum per any fiscal**: guany/pèrdua, ingressos i rendiment de cada any
- **Detall de lots**: cada venda mostra quines compres ha consumit i a quin preu
- **Posició en cartera**: accions restants i cost mitjà FIFO actual
- **Exportació a PDF** completa amb tots els detalls, sense connexió a internet
- **Multiidioma**: detecció automàtica de l'idioma del sistema operatiu (Català · Castellà · Anglès)
- **Sense internet**: totes les llibreries estan incrustades al fitxer HTML
- **Sense instal·lació**: un sol fitxer `.html`, funciona amb doble clic

---

## 🌍 Idiomes suportats

L'aplicació detecta automàticament l'idioma configurat al sistema operatiu:

| Idioma | Codi |
|--------|------|
| Català | `ca` |
| Castellà | `es` |
| Anglès | `en` (per defecte) |

---

## 🚀 Ús

1. Descarrega el fitxer `calculadora-fifo-accions.html`
2. Obre'l amb qualsevol navegador modern (Chrome, Firefox, Safari, Edge)
3. Afegeix les teves compres i vendes indicant l'**any**, el nombre d'**accions** i el **preu per acció**
4. Els resultats apareixen automàticament per any fiscal
5. Prem **PDF** per exportar l'informe complet

> ⚠️ Les dades **no es guarden** en tancar el navegador. Si necessites conservar-les, exporta el PDF abans de tancar.

---

## 📊 Com funciona el mètode FIFO

Quan vens accions, el sistema assigna el cost de compra seguint l'ordre cronològic: primer es consumeixen les accions comprades més antigues.

**Exemple:**

| Any | Operació | Accions | Preu |
|-----|----------|---------|------|
| 2021 | Compra | 100 | 10,00 € |
| 2022 | Compra | 50 | 14,00 € |
| 2023 | Venda | 120 | 18,00 € |

La venda de 120 accions consumeix:
- 100 accions comprades a 10,00 € → cost 1.000 €
- 20 accions comprades a 14,00 € → cost 280 €

**Ingressos:** 120 × 18,00 € = 2.160 €  
**Cost FIFO:** 1.000 € + 280 € = 1.280 €  
**Guany:** 2.160 € − 1.280 € = **880 €**

---

## 📄 Contingut del PDF exportat

1. **Resum per any fiscal** — ingressos, guany/pèrdua i rendiment de cada any
2. **Posició actual en cartera** — accions restants i cost mitjà FIFO (si n'hi ha)
3. **Detall de vendes per lots** — cada venda desglossada per lots de compra, amb preu de compra, any de compra, preu de venda i resultat de cada lot

---

## 🛠️ Tecnologia

- HTML5 + CSS3 + JavaScript (Vanilla)
- [jsPDF](https://github.com/parallax/jsPDF) v2.5.1 — generació de PDF
- [jsPDF-AutoTable](https://github.com/simonbengtsson/jsPDF-AutoTable) v3.8.2 — taules al PDF

Totes les llibreries estan incrustades al fitxer HTML. **No cal connexió a internet.**

---

## 📱 Compatibilitat

| Plataforma | Navegador | ✓ |
|------------|-----------|---|
| Android | Chrome | ✅ |
| iOS | Safari | ✅ |
| Windows | Chrome, Edge, Firefox | ✅ |
| macOS | Safari, Chrome | ✅ |
| Linux | Firefox, Chrome | ✅ |

---

## ⚖️ Llicència

MIT — lliure per a ús personal i comercial.

---

## 🤝 Contribucions

Les contribucions són benvingudes. Obre un *issue* o envia un *pull request*.
