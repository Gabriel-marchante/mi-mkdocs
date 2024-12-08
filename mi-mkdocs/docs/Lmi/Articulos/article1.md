# Característiques dels llenguatges de marques

Els **llenguatges de marques** s'utilitzen per definir estructures i continguts en documents. A continuació, descrivim alguns dels llenguatges de marques més coneguts: **SVG**, **HTML** i **XML**.

## 1. SVG (Scalable Vector Graphics)

SVG és un llenguatge basat en XML per a descriure gràfics vectorials escalables. Utilitza una àmplia gamma d'elements per definir formes, textos i imatges dins d'un gràfic.

```xml
<svg width="100" height="100">
  <circle cx="50" cy="50" r="40" stroke="green" stroke-width="4" fill="yellow" />
</svg>
```

### **Elements comuns en SVG**:
- `<circle>`: Defineix un cercle amb atributs com **cx** (coordenada X del centre), **cy** (coordenada Y del centre), i **r** (radi).
- `<rect>`: Crea un rectangle amb atributs com **x**, **y** (posicions), **width** (amplada) i **height** (alçada).
- `<line>`: Dibuixa una línia entre dos punts, amb atributs com **x1**, **y1**, **x2**, **y2** (coordenades dels extrems).

**Imatge d'exemple**:  
![Exemple SVG]()

---

## 2. HTML (HyperText Markup Language)

HTML és el llenguatge estàndard per a la creació de pàgines web. Utilitza etiquetes per estructurar el contingut, com encapçalats, paràgrafs, imatges, enllaços, etc.

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Pàgina d'exemple HTML</title>
  </head>
  <body>
    <h1>Hola, món!</h1>
    <p>Aquest és un exemple de pàgina web amb HTML.</p>
    <a href="https://www.example.com">Fes clic aquí per visitar Example</a>
  </body>
</html>
```

### **Elements comuns en HTML**:
- **<h1> a <h6>**: Defineixen encapçalats de diferents nivells.
- **<p>**: Defineix un paràgraf.
- **<a>**: Crea un enllaç amb l'atribut **href** per especificar la URL.
- **<img>**: Insereix imatges amb l'atribut **src** per l'URL de la imatge i **alt** per a una descripció alternativa.

**Enllaç d'exemple**: [Visitar Example](https://www.example.com)

---

## 3. XML (eXtensible Markup Language)

XML és un llenguatge de marques generalment utilitzat per emmagatzemar i transportar dades. A diferència d'HTML, no té etiquetes predefinides.

```xml
<persona>
  <nom>Joan</nom>
  <edat>30</edat>
  <ciutat>Barcelona</ciutat>
</persona>
```

### **Elements comuns en XML**:
- `<persona>`: Element arrel que conté informació d'una persona.
- `<nom>`, `<edat>`, `<ciutat>`: Etiquetes personalitzades que defineixen les propietats d'una persona.

**Característiques principals de XML**:
- **Autodefinit**: L'usuari crea les seves pròpies etiquetes.
- **Estricte en la sintaxi**: Cada etiqueta oberta ha de tenir una etiqueta de tancament corresponent.

---

## Taula comparativa dels llenguatges de marques

| Característica    | **SVG**                   | **HTML**                 | **XML**                   |
|-------------------|---------------------------|--------------------------|---------------------------|
| **Ús principal**  | Gràfics vectorials         | Estructuració de pàgines  | Estructuració de dades     |
| **Estructura**    | Basat en etiquetes XML     | Basat en etiquetes HTML   | Basat en etiquetes XML     |
| **Flexibilitat**  | Limitada a gràfics         | Enfocada a pàgines web    | Molt flexible              |
| **Exemple d'etiqueta** | `<circle>`              | `<h1>`, `<p>`, `<a>`      | Personalitzada (`<nom>`)   |
| **Validació**     | Necessari que sigui ben format | Pot ser laxa           | Estricta validació         |

---
