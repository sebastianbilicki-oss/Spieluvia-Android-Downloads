# Spieluvia V9 – Prüfberichte und Handytests

Stand: **04.11.2026**. Version `0.9.0-preview+0d3facab8e0e`, Versionscode **9**. Die nachfolgend geprüfte APK ist unverändert; die Veröffentlichung dieser Übersicht ist kein neuer App-Build.

**[V9-APK herunterladen](https://raw.githubusercontent.com/sebastianbilicki-oss/Spieluvia-Android-Downloads/main/downloads/android-test-9/Spieluvia.apk)** · **[V9 als ZIP herunterladen](https://raw.githubusercontent.com/sebastianbilicki-oss/Spieluvia-Android-Downloads/main/downloads/android-test-9/Spieluvia-Android.zip)** · **[VirusTotal-Bericht öffnen](https://www.virustotal.com/gui/file/888def7cb5f2a16b74f4e89d649ffd70b047abef9af0fe3d4065fac50ed0eb87/detection)**

## VirusTotal: 0/67 Erkennungen zum Prüfzeitpunkt

| Prüfung | Ergebnis |
| --- | --- |
| Geprüfte Datei | `Spieluvia.apk`, 6.010.261 Byte |
| Identität | SHA-256 stimmt mit der hier angebotenen V9-APK überein |
| Angezeigtes Scanergebnis am 04.11.2026 | **0/67 Erkennungen**; kein Scanner meldete die Datei als schädlich |
| Einzelne Scanner | 67 Ergebnisse „Undetected“; weitere 8 Scanner konnten den Dateityp nicht verarbeiten |
| Aussagegrenze | Ein unauffälliger Scan ist keine Garantie vollständiger Sicherheit und keine Play-Protect- oder Store-Freigabe |

Der verlinkte Bericht kann sich durch spätere Analysen ändern. Maßgeblich für die Zuordnung ist die vollständige APK-Prüfsumme:

`888def7cb5f2a16b74f4e89d649ffd70b047abef9af0fe3d4065fac50ed0eb87`

## Bisherige Rückmeldungen von vier Handys

Die Tabelle sammelt gemeldete Installations- und Funktionsversuche. Die installierte beziehungsweise ausgewählte App-Version ist nicht auf jedem Gerät bestätigt. Deshalb ist sie **keine pauschale V9-Kompatibilitätsfreigabe**.

| Handy | Android | Bisheriges Ergebnis | Noch offen |
| --- | --- | --- | --- |
| **Redmi Note 11 Pro 5G** | 13, laut Rückmeldung | Installation und Nutzung möglich. Zählung ohne Tastatur nach V6 bestätigt; später Ausfall des Bedienungshilfedienstes trotz aktivierter Freigabe. | Nach Neustart und aufgehobener Energiesparbeschränkung längeren Betrieb prüfen. Version beim jüngsten Abbruch nicht bestätigt. |
| **Xiaomi „15c 6g“** – genaue Modellbezeichnung offen | 15, Versionsanzeige im Screenshot | Erstinstallation scheitert mit „App wurde nicht installiert“. Vollständiger Download und keine vorhandene Vorversion gemeldet. | Genauen Installationsfehler per PC auslesen. Play Protect dort nicht als Ursache bestätigt. |
| **Redmi Note 14 5G** | 16, Modell und Version im Screenshot | Positive Rückmeldung: App funktioniert. | App-Version, Messdauer/-abweichung, Budgetende, Neustart und Hintergrundbetrieb einzeln dokumentieren. |
| **Samsung Galaxy S25+** | 17, Modell/Version laut Rückmeldung | Installation durch **Google Play Protect blockiert**, im Sperrbild bestätigt. | Noch keine Entsperrung und kein anschließender Funktionstest bestätigt. Die Android-Version ist im Sperrbild nicht überprüfbar. |

**Auf keinem dieser Geräte ist bisher ein vollständiger, dokumentierter Langzeittest abgeschlossen.** Positive Rückmeldungen gelten für den beschriebenen Umfang. Energiesparen ist beim Dienstabbruch ein möglicher Einfluss, keine nachgewiesene Ursache oder bestätigte Behebung. Wiederholte Rückmeldungen zum selben Handy werden nicht als weitere Geräte gezählt.

## Automatisierte und technische V9-Prüfungen

| Bereich | Ergebnis |
| --- | --- |
| Automatisierte Androidtests | **136 erfolgreich** |
| Regelkern / Core-Regression | Bestanden |
| Release-Build | Erfolgreich |
| Android Lint | **0 Fehler, 36 Hinweise** |
| Technische Berechtigungs-/Policy-Prüfungen | Bestanden; keine Google-Richtlinienfreigabe |
| APK-Signatur und Ausrichtung | Geprüft, APK-v2/v3-Signatur mit bisherigem Android-Testsignierer |
| Öffentlicher Download | Dateigröße und SHA-256 von APK/ZIP nach Bereitstellung erneut bestätigt |
| Vollständige Geräteabnahme / Store-Freigabe | **Offen** |

Maschinenlesbare ursprüngliche Build-/Signaturprüfdaten: [verification.json](verification.json).

ZIP SHA-256: `44ead0a6f1c2c8dc0c66060ba807c0ce4032975ce866cb5e6c431af822921ba5`.

Signierzertifikat SHA-256: `cea146b07d0283bfac7696366e72fe1f8ffc7a865abdc128a538d5bc3639c716`.

## Play Protect und noch erforderliche Gerätetests

Auf mindestens einem gemeldeten Gerät verhindert Play Protect die Installation. Die Warnung passt zu Googles dokumentierter Behandlung heruntergeladener Apps mit sensiblen Rechten wie der Bedienungshilfe. Spieluvia nutzt sie für die Rückkehr zur Startseite bei Budgetende; eine individuelle Google-Begründung für diese APK liegt nicht vor. Ein **Play-Protect-Einspruch für die öffentliche V9 wurde abgesendet**. Eine Aufhebung der Sperre ist noch nicht bestätigt. [Offizielle Google-Hinweise](https://developers.google.com/android/play-protect/warning-dev-guidance).

Nicht als Lösung voraussetzen, dass Schutzfunktionen abgeschaltet werden. Ein vorhandener gültiger Signierschlüssel ersetzt keine Prüfung durch Google.

Noch systematisch prüfen: Zeitmessung mit/ohne Tastatur und bei externem App-Start, Sperre bei Budgetende, Elternfreigaben, Bildschirm sperren/entsperren, Neustart, längerer Hintergrundbetrieb sowie Updates unter Erhalt von PIN, Regeln, Verbrauch und Skins.

Support und Test-Rückmeldungen: **spieluvia@gmail.com**. Hilfreich sind Modell, Android-Version, Spieluvia-Version, genauer Ablauf und Fehlermeldung. Keine PINs, Zeitcodes oder privaten Nutzungsdaten mitsenden.
