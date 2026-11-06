TANKLOG 1.0 – Installation und Datenübertragung
================================================

1. Alle Dateien UND den Ordner icons unverändert in ein öffentliches GitHub-Repository hochladen. index.html muss im Hauptverzeichnis liegen.
2. GitHub: Settings > Pages > Deploy from a branch > main > /(root) > Save.
3. Einige Minuten warten, die veröffentlichte HTTPS-Adresse öffnen.
4. Android: Chrome > Menü > App installieren (oder Startbildschirm hinzufügen).
   Samsung Internet: Menü > Seite hinzufügen zu > Startbildschirm.
   iPhone: Safari > Teilen > Zum Home-Bildschirm.
5. Am PC die gleiche Website öffnen. Die Daten sind dort anfangs LEER, weil sie lokal pro Gerät gespeichert werden.
6. Auf dem Handy: Backup > Backup herunterladen. JSON-Datei auf den PC übertragen (USB, Quick Share oder E-Mail).
7. Auf dem PC: TANKLOG im Browser öffnen > Backup > Backup importieren > JSON auswählen.
   ACHTUNG: Import ERSETZT die bisherigen Daten auf diesem Gerät. Vorher ggf. PC-Backup erstellen.
8. Backup regelmäßig wiederholen, um den PC aktuell zu halten. Es findet KEINE automatische Synchronisation statt.
9. CSV für Excel: Backup > CSV-Dateien herunterladen. Es werden drei CSV-Dateien exportiert. Bilder sind nur im JSON-Backup enthalten.

HINWEISE
- Daten liegen lokal im IndexedDB-Speicher des Browsers/der installierten App, nicht auf GitHub.
- Browserdaten löschen, App deinstallieren oder Handy verlieren kann Daten vernichten. Regelmäßige JSON-Backups sind wichtig.
- Ölwechsel- und HU-Erinnerungen werden beim Öffnen der App angezeigt, nicht als automatische Push-Nachricht.
- Verbrauch wird zwischen Volltankungen ermittelt. Bitte Kilometerstände und Volltank-Markierung korrekt eingeben.
- Bei großen Fotobeständen kann der lokale Speicher knapp werden. Fotos werden beim Import verkleinert.
- Kein Konto, kein Server und keine laufenden Cloud-Kosten erforderlich.

NEU in Version 1.2: Fällige HU/TÜV- und Wartungstermine erscheinen beim Öffnen der App als Hinweis und in der Garage. Die Meldung wird pro Browsersitzung und Datum nicht ständig wiederholt. Für Erinnerungen bei geschlossener App wären Push-Benachrichtigungen mit zusätzlicher Infrastruktur nötig.

VERSION 1.3 – FAHRZEUGSCHEIN
- Beim Anlegen/Bearbeiten Bild importieren, lokal speichern und anzeigen.
- Browser mit TextDetector: lokale Erkennung versuchen; andere Browser: manuelle Eingabe oder OCR-Text einfügen.
- KEINE allgemeine automatische OCR-Garantie auf Samsung/iPhone. Keine Cloud-Übertragung.
- FIN-Dublettenprüfung, erweiterte Felder, Dokument im JSON-Backup enthalten.
- Achtung: Fahrzeugscheine enthalten sensible Daten; Backup sicher aufbewahren.
- Vor Updates immer Backup erstellen.


VERSION 1.4 – FAHRZEUGSCHEIN-OCR
Bei Auswahl eines Bildes startet die Texterkennung mit Tesseract.js (Deutsch + Englisch).
WICHTIG: Für den ersten Scan benötigt die App Internet, da die OCR-Bibliothek und
Sprachmodelle von externen CDN-Servern geladen werden. OCR läuft im Browser,
aber vollständige Offline-Verfügbarkeit der OCR-Dateien ist nicht garantiert.
Die Fahrzeugdaten werden weiterhin lokal in IndexedDB gespeichert.
Die Erkennung kann Fehler machen. Vor dem Speichern jedes Feld prüfen.
Vor Updates immer ein JSON-Backup erstellen.
