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
