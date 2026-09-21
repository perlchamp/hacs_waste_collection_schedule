# Upgrade auf die aktuelle Version

## Das Upgrade anstoßen

- HA → Einstellungen → Geräte & Dienste → HACS → Waste Collection Schedule

- im Bereich `Diagnose` auf +1 `deaktivierte Entität` klicken  
  ![deaktivierte Entität(en) in WCS](pictures/deaktivierte_Entität_ok.png)  
  *Abbildung: WCS--deaktivierte Entität*

- im Bereich `Diagnose` den Schalter `Pre-Release` anklicken  
  ![Schalter Pre-Release](pictures/Pre-release_ok.png)  
  *Abbildung: WCS--Schalter Pre-Release*

- auf das Zahnrad-Symbol klicken → die Option `aktiviert` aktivieren → auf `aktualisieren` klicken  
  ![Schalter des Pre-Release-Sensors aktivieren](pictures/Pre-release_aktivieren_ok.png)  
  *Abbildung: Schalter des Pre-Release Sensors aktivieren*

- die Aktivierung bestätigen
  ![Aktivierung bestätigen](pictures/Bestätigung_Pre-Release_aktivieren_ok.png)  
  *Abbildung: WCS--Aktivierung des Schalters bestätigen*

- Pre-Release Sensor unter WCS aktivieren  
  ![Pre-Release Sensor unter WCS aktivieren](pictures/Pre-release_aktivieren_2_ok.png)  
  *Abbildung: WCS--Pre-Release Sensor aktivieren*

- Das Upgrade ist jetzt verfügbar  
  ![Upgrade ist verfügbar](pictures/Pre-release_aktivieren_3_ok.png)  
  *Abbildung: WCS--Pre-Update verfügbar*

- auf `Update verfügbar` klicken → auf `Aktualisieren` klicken, um WCS anschließend auf die aktuelle Version (hier: V 3.0.0-beta4) zu bringen  
  ![Upgrade auf die aktuelle Version](pictures/WCS_upgraden_ok.png)  
  *Abbildung: WCS--Pre-Update verfügbar*
  
- HA → Einstellungen → HA neu starten
  ![HA neu starten](pictures/WCS_Restart_required_ok.png)  
  *Abbildung: HA neu starten*

  ![Neustart bestätigen](pictures/WCS_Restart_bestätigen_ok.png)  
  *Abbildung: HA-Neustart bestätigen*

  ## Fazit

  Bisher sind keinerlei Probleme mit der aktuellen Version aufgetreten. Alle Sensoren/Entitäten sind vollständig, und die Anzeigen auf dem Dashboard unverändert geblieben.
