# Datenschutzerklärung für die App „Rollhockey Companion“
**Stand: Oktober 2026**

**1. Verantwortliche Stelle**
Verantwortlich für die Datenverarbeitung im Zusammenhang mit dieser mobilen Applikation (nachfolgend „App“) ist:
Michael Glaus
Juraweg 26
4803 Vordemwald, Schweiz
E-Mail: glausmichael@hotmail.com 
*(Hinweis: Diese App ist ein unabhängiges Projekt und steht in keiner offiziellen Verbindung zum Schweizerischen Rollhockey-Verband oder den Betreibern von rollhockey.ch).*

**2. Grundsatz zur Datenerhebung**
Der Schutz Ihrer Privatsphäre ist uns ein wichtiges Anliegen. Diese App wurde nach dem Prinzip der Datensparsamkeit entwickelt: 
* Die App erfordert keine Registrierung und kein Benutzerkonto. 
* Wir setzen keine Analyse- oder Werbe-Tools (wie z. B. Google Analytics oder Werbe-IDs) zur Nachverfolgung Ihres Nutzungsverhaltens ein. 
* Wenn Sie die App regulär nutzen (Ansehen von Tabellen und Teams), werden keinerlei personenbezogene Nutzungsdaten an den Entwickler der App übermittelt.

**3. Lokale Datenspeicherung auf Ihrem Endgerät**
Damit Sie Ihre bevorzugten Teams, Ligen und abonnierten Spiele nicht bei jedem Start der App neu auswählen müssen, speichert die App folgende Einstellungen ausschliesslich lokal im internen Gerätespeicher Ihres Smartphones (mittels Android Jetpack DataStore): 
* Ausgewählte und gespeicherte Teams, Ligen und Saisons 
* Technisch notwendige Abruf-URLs für Spielpläne und Tabellen 
* IDs der Spiele, für die Sie Live-Benachrichtigungen aktiviert haben 

**Geräte-Backup durch das Betriebssystem:** Sofern Sie in den Systemeinstellungen Ihres Android-Geräts die automatische Datensicherung (Google Drive Backup) aktiviert haben, können diese lokalen App-Einstellungen vom Betriebssystem verschlüsselt in Ihrem persönlichen Google-Konto gesichert werden, um sie bei einem Gerätewechsel wiederherzustellen. Der Entwickler hat keinen Zugriff auf diese Sicherungen. Sie können alle lokal gespeicherten Daten jederzeit löschen, indem Sie in den Android-Systemeinstellungen den Speicher der App löschen bzw. die App deinstallieren.

**4. Push-Benachrichtigungen und Live-Spiele (Backend)**
Um Sie in Echtzeit über Tore, Karten und Spielereignisse zu informieren, nutzt diese App optionale Push-Benachrichtigungen. Wenn Sie ein Spiel abonnieren (Glocken-Symbol), passiert zur technischen Umsetzung Folgendes:

* **AWS Backend:** Die App sendet allgemeine Spieldaten (wie die Spiel-ID und Teamnamen) an unser Server-Backend (gehostet bei Amazon Web Services, AWS, Region Frankfurt). Es werden dabei **keine** personenbezogenen Daten, keine dauerhaften IP-Adressen und keine eindeutigen Nutzer-IDs an unser Backend übermittelt. Das Backend speichert anonymisiert, dass ein bestimmtes Spiel abonniert wurde, um die Webseite der Liga zentral abzufragen. Die Spieldaten werden 24 Stunden nach Spielende automatisch vom Server gelöscht.
* **Firebase Cloud Messaging (FCM):** Für die sichere und akkuschonende Zustellung der Benachrichtigungen an Ihr Smartphone nutzen wir "Firebase Cloud Messaging", einen Dienst von Google. FCM verwendet themenbasierte Abos ("Topics" für die jeweilige Spiel-ID), sodass unser Backend nicht weiss, wer Sie sind oder welches Gerät Sie nutzen. Google erfasst im Rahmen der Bereitstellung von FCM möglicherweise anonymisierte Geräte-Metadaten (z. B. Instance IDs), die für die technische Zustellung der Push-Nachrichten erforderlich sind. Weitere Informationen zum Datenschutz bei Firebase finden Sie hier: [Datenschutz bei Firebase](https://firebase.google.com/support/privacy)

**5. Datenübermittlung an Drittserver (Abruf von Spielplänen & Tabellen)**
Die App zeigt öffentlich zugängliche Spielpläne, Resultate und Ranglisten an. Um diese Informationen beim Öffnen der App aktuell darzustellen, baut die App direkt von Ihrem Endgerät aus eine Verbindung zu den Webservern der jeweiligen Sportplattformen auf – aktuell insbesondere zu: 
* rollhockey.ch (betrieben durch den Schweizerischen Rollhockey-Verband, SRHV) sowie 
* ggf. weiteren durch Sie ausgewählten internationalen Verbands-Websites 

Wenn die App Daten von z.B. www.rollhockey.ch abruft oder Sie über einen Link in der App einen externen Spielbericht im Browser öffnen, werden technisch bedingt folgende Verbindungsdaten direkt von Ihrem Gerät an den Server von rollhockey.ch übermittelt: 
* Ihre aktuelle IP-Adresse 
* Datum und Uhrzeit der Anfrage 
* Die angeforderte Ziel-URL (z. B. Saison- und Liga-Parameter) 
* Technische Informationen zum Browser/System (User-Agent) 

Diese Übermittlung ist technisch zwingend erforderlich (Rechtsgrundlage: Art. 6 Abs. 1 lit. b und f DSGVO sowie Art. 31 nDSG). Auf die weitere Verarbeitung dieser Server-Logdaten durch den Betreiber von rollhockey.ch haben wir keinen Einfluss. Es gelten hierfür die Datenschutzbestimmungen der entsprechenden Webseiten-Betreiber.

**6. App-Berechtigungen**
Für den Betrieb benötigt die App folgende Systemberechtigungen auf Ihrem Android-Gerät: 
* **Internetzugriff (INTERNET):** Erforderlich, um die Spielpläne, Live-Spielstände und Tabellen abzurufen. 
* **Benachrichtigungen (POST_NOTIFICATIONS, optional ab Android 13):** Wenn Sie für ein einzelnes Spiel das Glocken-Symbol (Live-Tracking) aktivieren, fragt die App um Erlaubnis, Ihnen System-Benachrichtigungen über FCM anzeigen zu dürfen. Sie können diese Berechtigung jederzeit in den Android-Systemeinstellungen widerrufen.

**7. Ihre Rechte (nach Schweizer nDSG und EU-DSGVO)**
Nach dem Schweizer Bundesgesetz über den Datenschutz (nDSG) sowie – sofern anwendbar – der Europäischen Datenschutz-Grundverordnung (DSGVO) haben Sie grundsätzlich das Recht auf Auskunft, Berichtigung, Löschung, Einschränkung der Verarbeitung sowie Datenübertragbarkeit. Da der Entwickler dieser App jedoch keinerlei personenbezogene Daten von Ihnen erhebt oder auf den eigenen AWS-Servern personenbezogen speichert, liegen uns keine Daten vor, die Ihrer Person zugeordnet werden könnten. Sämtliche in der App vorgenommenen Einstellungen können Sie jederzeit selbstständig auf Ihrem Gerät durch Deinstallation der App vollständig löschen. Bei Fragen zum Datenschutz im Zusammenhang mit dieser App können Sie sich jederzeit unter der oben angegebenen E-Mail-Adresse an uns wenden.

**8. Änderungen dieser Datenschutzerklärung**
Wir behalten uns vor, diese Datenschutzerklärung anzupassen, falls die App um neue Funktionen erweitert wird oder sich rechtliche Vorgaben ändern. Die jeweils aktuelle Fassung ist jederzeit über den in der App und im Google Play Store hinterlegten Link abrufbar.
