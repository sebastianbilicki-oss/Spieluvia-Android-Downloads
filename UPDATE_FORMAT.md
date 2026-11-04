# Updateinformationen v1

`latest.json` ist die öffentliche Quelle für den späteren Updatecheck. Aktuell wird eine ausdrücklich als Vorschau gekennzeichnete Testversion angeboten; die installierte V8 fragt diese Datei noch nicht ab.

Die Paketkennung muss zur App passen, `versionCode` muss höher als die installierte Version sein, das Gerät muss `minSdk` erfüllen. `downloadUrl` und `zipUrl` zeigen auf die versionierte Ablage. Prüfsummen sind SHA-256 über die vollständigen Dateibytes, Dateigrößen in Byte. Der APK-Zertifikatfingerabdruck ist in der App unabhängig zu prüfen; die Versionsdatei allein ist kein unabhängiger Echtheitsnachweis. `releaseNotes` enthält die Änderungen auf Deutsch. `appHasUpdateCheck` beschreibt nur die hier angebotene Version.

Bei künftigen Versionen zuerst unveränderliche versionierte Dateien veröffentlichen und prüfen, anschließend `aktuell/`, README/Änderungsverlauf und `latest.json` gemeinsam aktualisieren. Gleiche Paketkennung/Signatur, steigender Versionscode. Die bisherigen Archivdateien erhalten. Nur Installationsdateien und öffentliche Metadaten übernehmen, nie den Quellcheckout oder private Signierdateien.

Download oder Updateprüfung installiert nichts automatisch. Für reguläre Android-Handys ist eine bewusste Installationsbestätigung einzuplanen. Kein Gerätemanagement oder Reset wird eingerichtet.
