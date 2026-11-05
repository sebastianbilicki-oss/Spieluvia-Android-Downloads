# Spieluvia – Android-Downloads

Hier findest du die aktuelle signierte Android-Testversion und die Updateinformationen. Zum Herunterladen ist **keine GitHub-Anmeldung** erforderlich.

## Aktuell: Testversion 9

**[APK herunterladen](https://github.com/sebastianbilicki-oss/Spieluvia-Android-Downloads/raw/refs/heads/main/aktuell/Spieluvia.apk)** · **[ZIP herunterladen](https://github.com/sebastianbilicki-oss/Spieluvia-Android-Downloads/raw/refs/heads/main/aktuell/Spieluvia-Android.zip)**

Android ab Version 8/API26, Version `0.9.0-preview+0d3facab8e0e`, Versionscode **9**. Vorschau mit echten Zeitbegrenzungsfunktionen, keine reine Demo und keine Google-Play-Freigabe. Neue Funktionen brauchen weiterhin Tests auf echten Geräten.

### Prüfergebnisse und bekannte Probleme · Stand 04.11.2026

- **[VirusTotal: 0/67 Erkennungen](https://www.virustotal.com/gui/file/888def7cb5f2a16b74f4e89d649ffd70b047abef9af0fe3d4065fac50ed0eb87/detection)** für die unveränderte V9-APK zum Prüfzeitpunkt. Ein unauffälliger Scan ist keine Sicherheitsgarantie oder Play-Protect-Freigabe.
- **136 automatisierte Androidtests bestanden**, Core-Regression und Release-Build erfolgreich; Lint 0 Fehler / 36 Hinweise.
- **[Übersicht der vier gemeldeten Handys, Ergebnisse und offenen Prüfungen](https://github.com/sebastianbilicki-oss/Spieluvia-Android-Downloads/blob/main/downloads/android-test-9/TESTERGEBNISSE.md)**. Die Rückmeldungen betreffen teilweise ältere App-Versionen; eine vollständige V9-Geräteabnahme liegt nicht vor.
- **Bekannt:** Bedienungshilfedienst auf einem Redmi ausgefallen; Erstinstallation auf einem Xiaomi fehlgeschlagen; Play Protect blockiert die Installation auf einem Samsung. Google-Einspruch für V9 abgesendet, Entsperrung noch nicht bestätigt.

### Einmal auf V9 wechseln

1. APK herunterladen oder ZIP entpacken und `Spieluvia.apk` öffnen.
2. **Als Update installieren, vorher nicht deinstallieren und keine App-Daten löschen.** Bei gleicher Paketkennung und Signatur bleiben Eltern-PIN, Regeln und Verbrauch erhalten.
3. V8 und ältere Versionen haben keinen Updatecheck. Deshalb ist der erste Wechsel auf V9 manuell nötig.

### Updates ab V9

V9 prüft bei Appstart/Rückkehr automatisch die öffentliche Versionsdatei. Schnelle Rückkehrvorgänge sind auf eine Abfrage pro 60 Sekunden begrenzt. Unter **App-Updates** lässt sich das abschalten oder manuell prüfen.

Nur eine höhere passende Version wird angeboten. **Der APK-Download startet erst nach Antippen.** Danach Paket, Version, Dateigröße, Prüfsumme und erwarteten Signierer kontrollieren. „Geprüftes Update installieren“ übergibt die Datei bewusst an Android. Falls nötig, die Installationsfreigabe für Spieluvia in Android erlauben, zurückkommen und erneut Installieren antippen. Android prüft und bestätigt die eigentliche Installation. **Keine stille oder erzwungene Installation.** Ein fehlgeschlagener Updateabruf stoppt die Aufsicht nicht.

Bei der Versionsprüfung erhält GitHub die Netzwerkadresse und übliche Verbindungsdaten; keine Geräte-ID, PIN, Regeln oder Nutzungsdaten. Kein Anmeldetoken wird verwendet. APKs liegen im privaten Updatecache. Die neue Installationsberechtigung dient nur eigenen App-Updates; nur diese geprüfte APK erhält vorübergehenden Lesezugriff für den Android-Installer. Kein Hintergrunddienst oder Werksreset nötig.

### Neu in V9

- Updateprüfung bei Appstart aus der öffentlichen Spieluvia-Downloadablage; abschaltbar.
- Neue passende Versionen anzeigen und nach Antippen herunterladen, mit Fortschritt und Abbruch.
- Größe, SHA-256, Paket, Versionscode/-name und gepinnten Signierer prüfen.
- Geprüfte APK bewusst an Android übergeben; Installationsfreigabe und Bestätigung bleiben erforderlich.
- Bisherige Skins, Offline-Ratgeber und Zeitbegrenzung bleiben enthalten.

Die Zeitmessung benötigt die bewusst erteilten Freigaben für Nutzungszugriff, Bedienungshilfe und sichtbare Benachrichtigungen. Telefon, Einstellungen und Startseite bleiben erreichbar; die App bietet keine manipulationsfeste Deinstallations-/Stoppsperre. Die neue Updatefunktion ist von der lokalen Aufsicht getrennt.

## Downloads und Prüfdaten

- [Archiv Testversion 9](https://github.com/sebastianbilicki-oss/Spieluvia-Android-Downloads/tree/main/downloads/android-test-9)
- [Archiv Testversion 8](https://github.com/sebastianbilicki-oss/Spieluvia-Android-Downloads/tree/main/downloads/android-test-8)
- [Versionsdatei latest.json](https://raw.githubusercontent.com/sebastianbilicki-oss/Spieluvia-Android-Downloads/main/latest.json)
- [Aktuelle APK-Prüfsumme](https://github.com/sebastianbilicki-oss/Spieluvia-Android-Downloads/raw/refs/heads/main/aktuell/Spieluvia.apk.sha256)
- [Prüfdaten V9](https://github.com/sebastianbilicki-oss/Spieluvia-Android-Downloads/blob/main/downloads/android-test-9/verification.json)
- [Änderungsverlauf](CHANGELOG.md)

APK SHA-256: `888def7cb5f2a16b74f4e89d649ffd70b047abef9af0fe3d4065fac50ed0eb87`.
Signierzertifikat SHA-256: `cea146b07d0283bfac7696366e72fe1f8ffc7a865abdc128a538d5bc3639c716`.

Gleicher Android-Testsignierer und Paket `de.spieluvia.android` wie bisher, steigender Versionscode. 136 automatisierte Androidfälle, Core-Regressionsprüfung, Release-Build und technische Policy-Prüfungen bestanden. Lint: 0 Fehler / 36 Hinweise. Neue Updateabläufe noch nicht vollständig auf einem physischen Gerät abgenommen; Budgetende, Neustart und längerer Hintergrundbetrieb bleiben separat zu prüfen. Öffentliche Store-/Berechtigungsfreigabe ist nicht bestätigt; einen Play-Vertriebsweg separat bewerten.

## Inhalt dieses Repositorys

Nur ausdrücklich veröffentlichte Installationsdateien, Prüfsummen, Versionsinformationen und Anleitungen. Kein Quellcode der App, keine Signierschlüssel, Passwörter, privaten Nutzerbilder oder Nutzungsdaten. Die APK enthält ihre zum Betrieb benötigten Ressourcen und Texte.

Fragen, Anregungen oder Bedenken: **spieluvia@gmail.com**.

## Entwicklungsplan & kommende Updates

[**Entwicklungsplan & Updates ansehen**](web/entwicklungsplan.html) – mit Statuslegende (✓ eingebaut, ! nächstes Update, ✕ Planung), Kurzbeschreibungen und bekannten Einschränkungen. Die HTML-Seite liegt im Repository; eine öffentliche Homepage-URL erfordert eine passende Website-Veröffentlichung.
