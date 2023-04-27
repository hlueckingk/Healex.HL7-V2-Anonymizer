### Patient als FHIR Ressourcen einspeisen

* Postman Request `Patients. Read` ausführen und vergewissern, dass der Testpatient nicht vorliegt:
  * Vorname: „Max“, Nachname: „Mustermann”.
* Postman Collection `Patient. Create` verwenden und Patient einspielen.
  * Wir notieren uns aus dem Ergebnis die ID (z.B. „f1325484-9ba4-45a5-a877-170cae29d37a“).
* Anschließend Postman Request `Patients. Read` öffnen
  * In der URL hinter `/Patient` die ID ergänzen, sodass in der Adresszeile hinter GET die URL `/Patient/f1325484-9ba4-45a5-a877-170cae29d37a` steht (ID bitte entsprechend anpassen).
  * Postman Request ausführen und vergewissern, dass der Testpatient als Ergebnis zurückgegeben wird.

als nächstes: [Patient in CDS suchen](training_2_search_patient_CDS.md)