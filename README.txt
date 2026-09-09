Garagenprotokoll PWA V1
Schlankes mobiles Abnahme-/Übergabeprotokoll für Garagen.
Enthält: Garagenadresse/-nummer, Mieter/Nachmieter-Kontaktanschriften, Schlüssel Tor/Box, Zustand/Bemerkungen, Unterschriften, PDF-Druck, verschlüsselte lokale Speicherung, Protokollbibliothek und Kopierfunktion.
Für GitHub Pages die sechs Dateien einzeln in ein eigenes Repository hochladen.

Version 1.1: Fehler beim erstmaligen Einrichten der lokalen Verschlüsselung behoben.


Version 1.2: Neues Garagen-/Auto-App-Icon; alle Funktionen aus V1.1 inkl. Passwortschutz/Verschlüsselung bleiben erhalten.

Version 1.3: Bugfix für Datenschutz-Login: Nach erfolgreichem Einrichten/Entsperren wird der Sperrbildschirm jetzt korrekt ausgeblendet.

Version 1.4: Login robuster gemacht: fester Button-Eventhandler, sichtbarer Entsperrstatus, direkte Ausblendung des Sperrbildschirms und klare Passwort-Fehlermeldung.

Version 1.5: Neuer Kopfbereich mit App-Icon, Titel „Garagenprotokoll“ und Untertitel „Abnahme/Übergabe“. Alle bisherigen Funktionen inkl. Verschlüsselung/Login bleiben erhalten.

Version 1.6: Fotodokumentation ergänzt: je ein Foto „Garagentor außen“ und „Garage innen“. Fotos werden mit dem Protokoll verschlüsselt gespeichert, beim Öffnen wieder angezeigt, beim Kopieren übernommen und beim neuen Protokoll geleert.

Version 1.7: 12-Stunden-Arbeitssitzung (Passwort nur einmal pro Sitzung), manueller „Sperren“-Button und automatischer Zeitstempel beim Unterschreiben. Fotodokumentation bleibt erhalten.

Version 1.8: 12-Stunden-Freigabe bleibt über vollständiges Schließen der PWA erhalten; manueller Sperren-Button löscht sie sofort. Neue schreibgeschützte Vorschau vor der Unterschrift; beide Fotofelder werden angezeigt.

V1.9: Korrigierte 12-Stunden-Freigabe über App-Neustarts ohne Speicherung des Passworts; nicht exportierbarer WebCrypto-Schlüssel mit Ablaufzeit in IndexedDB. Vorschau-Button jetzt sichtbar in der unteren Leiste.

V2.0: Vorschau vollständig überarbeitet. Sie zeigt nun eine schreibgeschützte Bildschirmansicht im gleichen Drucklayout wie die spätere PDF-/Druckausgabe.

V2.1: Fehler im Fenster „Meine Garagenprotokolle“ behoben. Nach „Öffnen“ wird das Fenster nun zuverlässig geschlossen; der Schließen-Button und ein Tipp auf den abgedunkelten Hintergrund schließen es ebenfalls.

V2.2: Unterschriftenfunktion repariert. In V2.1 wurde beim ersten Berühren des Unterschriftenfeldes eine nicht vorhandene Funktion aufgerufen, wodurch das Zeichnen abbrach. Zeitstempel-Funktionen ergänzt und Pointer-Eingabe für Android/PWA robuster gemacht.

V2.3: In der PDF-Vorschau wird die gewählte Protokollart (Übergabe / Einzug oder Abnahme / Auszug) jetzt eindeutig als Text angezeigt; die beiden unmarkierten Auswahlfelder werden in der Vorschau nicht mehr gezeigt. Unterschriftenfix aus V2.2 bleibt erhalten.

V2.4: Fotoausgabe repariert. Aufgenommene Fotos werden vor PDF/Druck explizit aus dem internen Fotospeicher in die Bildfelder geschrieben und vollständig geladen. Auch die PDF-Vorschau übernimmt die gespeicherten Fotos jetzt ausdrücklich. Leere Foto-Platzhalter werden bei vorhandenen Fotos im PDF ausgeblendet. Unterschriftenfix und eindeutige Protokollart aus V2.2/V2.3 bleiben erhalten.

V2.5: Fotodokumentation hat pro Bild zwei eindeutige Aktionen: „Foto aufnehmen“ öffnet die Kamera; „Vorhandenes Foto auswählen“ öffnet die Bild-/Dateiauswahl. Die Bildvorschau ist davon getrennt. PDF-Fotofix aus V2.4 bleibt erhalten.

V2.6: Fehler nach Einführung der getrennten Kamera-/Galerie-Schaltflächen behoben. Die Vorschau synchronisiert keine Datei-Inputs mehr positionsabhängig, sondern nur stabile Protokollfelder; Unterschriften werden separat übernommen. Vorschau wartet auf die Fotodarstellung. Speichern/Vorschau melden Fehler nun sichtbar statt scheinbar ohne Reaktion zu bleiben. Foto-, Unterschriften- und Protokollart-Fixes bleiben erhalten.

V2.7: Protokollspeicher von localStorage auf IndexedDB umgestellt, damit Fotos nicht mehr am kleinen localStorage-Limit scheitern. Bestehende gespeicherte Protokolle werden beim ersten Öffnen automatisch aus dem alten Speicher übernommen. Nach erfolgreichem Speichern wird der alte localStorage-Eintrag entfernt. Verschlüsselung bleibt erhalten.

V2.8: Ursache des Speicherfehlers mit Fotos behoben. Die Base64-Konvertierung der verschlüsselten Protokolldaten arbeitet nun in kleinen Blöcken statt die komplette große Bytefolge auf einmal an JavaScript zu übergeben. Dadurch können Protokolle mit Fotos auf mobilem Chrome gespeichert werden. IndexedDB-Speicher aus V2.7 bleibt erhalten.

V2.9: Der gebrandete blaue Kopfbereich mit Garagen-Icon, Titel, Eigentümer und Domoconzept wird wieder in PDF-Vorschau und PDF/Druck ausgegeben. Er ist für A4 kompakter formatiert. Alle V2.8 Speicher-/Fotofixes bleiben erhalten.

V2.10: Fotos werden in Vorschau und PDF vollständig ohne Beschnitt dargestellt. Die feste Bildhöhe und object-fit: cover wurden entfernt; Bilder passen sich nun proportional an ihre Originalmaße an.
