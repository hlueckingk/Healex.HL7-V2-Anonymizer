### Postman vorbereiten
vgl. https://gitlab.ub.uni-bielefeld.de/medfak-diz/koop-plattform/wiki/-/wikis/Postman
* Die Software Postman kann hier bezogen werden: https://www.postman.com/downloads/
* In Postman, im Menü Datei „File“ und da „Import“ kann die
  Postman Colletion Datei `FHIR Vonk OWL.postman_collection.json`
  aus dem Ordner `/customer-owl-ops/deployment/test/Postman` importiert werden.
* Es erscheint ein Abschnitt „FHIR Vonk OWL“ mit drei Postman Requests
  * `Patient. Create` – dient dem manuellen Anlegen eines Patienten
  * `Patients. Read` – dient der Abfrage von Patienten
  * Bitte Collection FHIR Vonk OWL auswählen und für den lokalen Gebrauch
  * die `FHIR_URL` mit dem Wert `http://localhost:4080` verwenden.

als nächstes: [Patient als FHIR Ressourcen einspeisen](training_1_patient_FHIR.md)
