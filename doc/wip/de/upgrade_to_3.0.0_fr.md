# Mettre à niveau vers la version actuelle

Pour lancer la mise à niveau:

- HA → Paramètres → Appareils & services → HACS → Waste Collection Schedule

- dans la zone `Diagnostics` cliquez sur +1 `entité désactivée`
  ![entité(s) désactivée(s) dans WCS](pictures/deaktivierte_Entität_ok.png)
  *Image: entité désactivée*

- Cliquez sur le bouton `Pré-release` dans la zone `Diagnostics`
  ![Changer de pré-release](pictures/Pre-release_ok.png)
  *Image: commutateur de pré-release*

- cliquez sur le symbole d'engrenage → activez l'option `activé` → cliquez sur `mettre à jour`.
  ![Activer le commutateur du capteur de pré-release](pictures/Pre-release_aktivieren_ok.png)
  *Image: Activer l'interrupteur du capteur de pré-release*

- confirmer l'activation
  ![Confirmer l'activation](pictures/Bestätigung_Pre-Release_aktivieren_ok.png)
  *Image: Confirmer l'activation du commutateur*

- Activer le capteur de pré-release sous WCS
  ![Activer le capteur de pré-version sous WCS](pictures/Pre-release_aktivieren_2_ok.png)
  *Image: Activer le capteur de pré-release*

- La mise à niveau est maintenant disponible
  ![La mise à niveau est disponible](pictures/Pre-release_aktivieren_3_ok.png)
  *Image: Pré-release est disponible*

- Cliquez sur `Mise à jour disponible` → cliquez sur `Mettre à jour` pour ensuite mettre à jour WCS vers la version actuelle (ici : V 3.0.0-beta4).
  ![Mise à niveau vers la version actuelle](pictures/WCS_upgraden_ok.png)
  *Image: Mise à niveau vers la version actuelle*

- HA → Paramètres → Redémarrer HA
  ![Redémarrer HA](pictures/WCS_Restart_required_ok.png)
  *Image: Redémarrer HA*

  ![Confirmer le redémarrage](pictures/WCS_Restart_bestätigen_ok.png)
  *Image: Confirmer le redémarrage de HA*
