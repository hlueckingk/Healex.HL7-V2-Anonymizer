## Plattform-Stack für CDR starten
vgl. https://gitlab.ub.uni-bielefeld.de/medfak-diz/koop-plattform/wiki/-/wikis/CDS-Stack

### Konfigurieren für lokale Verwendung

* in Datei `deployment/source/filehandler_interfaces.env`
  * `FILE_WATCH_FOLDER` auf lokalen Hotfolder anpassen
    * Beispiel für Windows: `c:/customer-owl-ops/hotfolder/`
* Datei `deployment/source/swarm-compose.hospital.patient.cds.env`
  * `BACKEND_PUBLIC_BASE_URL=https://localhost:9080`
  * `FRONTEND_URL=https://localhost:8080`
* `deployment/source/swarm-compose.hospital.patient.fhir.env`
  * `FILE_WATCH_FOLDER=c:/customer-owl-ops/hotfolder`
* Mit dem Befehl `docker secret ls` überprüfen, ob folgende Secrets hinterlegt sind (ggf. hinterlegen):
  * `create clinicalsite-api-secret`
  * `create oidc-client-secret`

### CDR starten

* In Repo-Ordner `/customer-owl-ops/deployment/source` wechseln
* Skript `bash deploy-stack-hospital.sh` ausführen

als nächstes: [Postman vorbereiten](training_0_2_postman.md)
