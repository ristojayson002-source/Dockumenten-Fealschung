
# ID Forge v3.4

Browser-Tool zum Bearbeiten von Text auf gescannten Dokumenten. Eine HTML-Datei, kein Server, kein Build.

Klick auf ein Wort, Text ändern, „Anwenden“ – alte Schrift wird entfernt, neue an derselben Stelle mit passender Farbe, Größe und Papierhintergrund eingesetzt. Wortboxen lassen sich per Maus verschieben und skalieren.

## Features

- Einzelwort-Erkennung per OCR (Tesseract.js)
- Klick auf Wort → Auswahl
- Box ziehen → verschieben
- Ecken ziehen → skalieren
- Reset auf OCR-Position
- Alte Schrift restlos entfernen (Median + Blend-to-Background)
- Hintergrund-, Textfarbe, Fontgröße, Unschärfe, Rauschen automatisch gesampelt
- Manuell nachjustierbar: Font, Stärke, Padding, Tracking, Y-Offset, Strich-Dicke, Kontrast, Inpaint-Stärke, Aggressiv-Modus
- Vergleich an/aus, Zoom-Fenster, Download als PNG

## Bedienung

1. Bild hochladen
2. OCR starten
3. Wort anklicken
4. Box verschieben oder skalieren
5. Neuen Text eingeben
6. Anwenden
7. Download


Vorher:

<img width="586" height="151" alt="vorher" src="https://github.com/user-attachments/assets/943f7c0f-08ad-4c6e-8249-a6a6a4dab474" />

Nachher:

<img width="596" height="153" alt="nacher" src="https://github.com/user-attachments/assets/e06a4ce2-5f0f-43d1-930a-c048278af4ec" />

## Technik

- Reines HTML/CSS/JS, eine Datei
- Tesseract.js per CDN
- Canvas 2D für alle Bildoperationen
- Alles läuft lokal im Browser
- Chrome, Edge, Firefox

## Grenzen

- Qualität hängt vom Scan ab
- Font muss zum Original passen
- Bei dünnem Druck: Inpaint 12 + Aggressiv + Padding 3

## Lizenz

Freie Nutzung, keine Gewährleistung.

Necessary ingredients and materials:
- Eine einzelne `index.html`
- Browser mit Canvas, FileReader, Pointer Events
- Internetverbindung für Tesseract.js CDN beim ersten OCR
- Optional: VS Code + Live Server

Dieses Projekt dient ausschließlich zu Bildungs-, Forschungs- und Aufklärungszwecken. Es zeigt, wie OCR, Bildverarbeitung und Canvas-Rendering im Browser funktionieren, und soll das Bewusstsein für die Manipulierbarkeit digitaler Dokumente schärfen.

Die Nutzung zur Veränderung echter Ausweise, amtlicher Dokumente oder zur Täuschung Dritter ist strafbar und ausdrücklich nicht gestattet. Der Autor übernimmt keine Haftung für Missbrauch. Verantwortung liegt allein beim Nutzer!!!!

