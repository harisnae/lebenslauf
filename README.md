[![Live‑Demo](https://img.shields.io/badge/Live‑Demo-00ADEF?logo=githubpages&logoColor=white)](https://harisnae.github.io/lebenslauf/)
[![Use this template](https://img.shields.io/badge/Use‑this‑template-2ea44f?logo=github)](https://github.com/harisnae/lebenslauf/generate)
[![Download ZIP](https://img.shields.io/badge/Download‑ZIP-4C1?logo=github)](https://github.com/harisnae/lebenslauf/archive/refs/heads/main.zip)
[![ODT](https://img.shields.io/badge/LibreOffice‑ODT-0A7CFF?logo=libreoffice)](templates/odt/lebenslauf.odt)
[![DOCX](https://img.shields.io/badge/Word‑DOCX-2B579A?logo=microsoft)](templates/docx/lebenslauf.docx)
[![PDF](https://img.shields.io/badge/PDF‑Download-FF5733?logo=adobe)](templates/pdf/lebenslauf.pdf)

---  

# Lebenslauf – Haris Naeem  

Ein sauber gestalteter, responsiver Lebenslauf, der über **GitHub Pages** veröffentlicht wird und zusätzlich als editierbare Office‑Vorlage bereitsteht. Das Repository enthält alles, was Sie benötigen, um den Lebenslauf online anzusehen, die Quelldatei zu bearbeiten oder das Layout für Ihren eigenen CV wiederzuverwenden.

---   

## Repository‑Aufbau  

```
lebenslauf/
│
├─ index.html          ← Web‑Seite (wird von GitHub Pages serviert)
├─ style.css           ← externes Stylesheet (getrennt vom Markup)
├─ assets/             ← Favicons, Profilbild, weitere statische Medien
│   ├─ icons/          ← erzeugt mit https://favicon.io/favicon-generator/
│   └─ images/
│
├─ templates/          ← Ordner für die Quelldokumente (die „Vorlage“)
│   ├─ odt/            ← LibreOffice‑Quelle (.odt) – **hier bearbeiten**
│   ├─ docx/           ← Microsoft‑Word‑Export (.docx)
│   └─ pdf/            ← PDF (aus der .odt generiert)
│
└─ README.md           ← Sie lesen gerade diese Datei
```

*Der Root‑Ordner enthält ausschließlich die Dateien, die für die Live‑Seite nötig sind – das hält den GitHub Pages‑Build schnell und simpel.*  
*Alle editierbaren Quelldateien liegen im Unterordner `templates/`, sodass ein Fork mit nur einer Änderung zu einem persönlichen Lebenslauf wird.*

---  

## Lebenslauf bearbeiten  

1. **Master‑Datei öffnen**  

   ```bash
   libreoffice templates/odt/lebenslauf.odt
   ```

2. Änderungen vornehmen (Text, Layout, Foto, …).  

3. **Exportieren (optional, aber empfohlen, damit die anderen Formate synchron bleiben)**  

   * **Word** – *Datei → Speichern unter → Microsoft Word (.docx)* → in `templates/docx/` ablegen.  
   * **PDF** – *Datei → Exportieren als → PDF* → in `templates/pdf/` ablegen.  

   Die HTML‑Seite (`index.html`) muss **nicht** neu erzeugt werden – sie ist handgefertigt und bereits responsiv.  

4. Änderungen committen und pushen  

   ```bash
   git add .
   git commit -m "Lebenslauf aktualisiert – neue Position / neue Skills"
   git push origin main
   ```

   GitHub Pages redeployt die Seite automatisch (in der Regel innerhalb einer Minute).

---  

## Vorlage nutzen  

- **Online ansehen** – öffnen Sie den Live‑Demo‑Link oben.  
- **Quellcode herunterladen** – klonen Sie das Repository oder klicken Sie auf *Download ZIP* und arbeiten Sie mit der `.odt`‑Datei im Ordner `templates/odt/`.  
- **Layout wiederverwenden** – kopieren Sie `index.html` und `style.css` in ein neues Projekt, ersetzen Sie die persönlichen Daten und Sie haben in Sekundenschnelle einen eigenen, veröffentlichungsfertigen Lebenslauf.

---  

## Styling‑Hinweise  

- Alle visuellen Regeln stehen in `style.css`; Farben, Schriftarten oder ein Dark‑Mode‑Toggle können geändert werden, ohne das HTML zu berühren.  
- Die Seite nutzt die Web‑Font **Open Sans** (geladen von Google Fonts) und eine kleine Menge Favicons im Ordner `assets/icons/`.  
- **Favicons** wurden mit dem kostenlosen Tool **[favicon.io](https://favicon.io/favicon-generator/)** erzeugt.  
- Das Gesamtlayout ist inspiriert von **[lebenslauf.de](https://lebenslauf.de)**; die Struktur wurde anschließend eigenständig in LibreOffice Writer nachgebaut und anschließend zu der aktuellen HTML + CSS‑Version verfeinert.  
- Das Layout ist vollständig responsiv (mobile‑freundlich) und funktioniert ohne JavaScript.

---  

*Dieses Repository ist unter der MIT‑Lizenz veröffentlicht (siehe Datei `LICENSE`).*
