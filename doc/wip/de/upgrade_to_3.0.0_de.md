# Upgrade auf die aktuelle Version

Um das Upgrade anzustoßen:

- HA → Einstellungen → Geräte & Dienste → HACS → Waste Collection Schedule

- im Bereich `Diagnose` auf +1 `deaktivierte Entität` klicken
  ![deaktivierte Entität(en) in WCS](pictures/deaktivierte_Entität_ok.png)
  *Abbildung: deaktivierte Entität*

- im Bereich `Diagnose` den Schalter `Pre-release` anklicken
  ![Schalter Pre-Release](pictures/Pre-release_ok.png)
  *Abbildung: Schalter Pre-release*

- auf das Zahnrad-Symbol klicken → die Option `aktiviert` aktivieren → auf `aktualisieren` klicken
  ![Schalter des Pre-Release-Sensors aktivieren](pictures/Pre-release_aktivieren_ok.png)
  *Abbildung: Schalter des Pre-release Sensors aktivieren*

- die Aktivierung bestätigen
  ![Aktivierung bestätigen](pictures/Bestätigung_Pre-Release_aktivieren_ok.png)
  *Abbildung: Aktivierung des Schalters bestätigen*

- Pre-Release Sensor unter WCS aktivieren
  ![Pre-Release Sensor unter WCS aktivieren](pictures/Pre-release_aktivieren_2_ok.png)
  *Abbildung: Pre-release Sensor aktivieren*

- Das Upgrade ist jetzt verfügbar
  ![Upgrade ist verfügbar](pictures/Pre-release_aktivieren_3_ok.png)
  *Abbildung: Pre-Update verfügbar*

- auf `Update verfügbar` klicken → auf `Aktualisieren` klicken, um WCS anschließend auf die aktuelle Version (hier: V 3.0.0-beta4) zu bringen
  ![Upgrade auf die aktuelle Version](pictures/WCS_upgraden_ok.png)
  *Abbildung: Pre-Update verfügbar*
  
- HA → Einstellungen → HA neu starten
  ![HA neu starten](pictures/WCS_Restart_required_ok.png)
  *Abbildung: HA neu starten*

  ![Neustart bestätigen](pictures/WCS_Restart_bestätigen_ok.png)
  *Abbildung: HA-Neustart bestätigen*
