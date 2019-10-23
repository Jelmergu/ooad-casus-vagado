# Usecase beschrijvingen

![Use case diagram]

| UC1: Registreren | |
| --- | --- |
| Primary Actor | Speler | 
| Precondities | - |
| Postconditie | Speler is geregistreed en ingelogd en aangekomen op zijn dashboard |
| Main Success scenario| |
| Actor Actions | System Actions |
| 1. Speler vult gegevens in |  |
| 2. Speler verstuurt formulier | |
| | 3. Systeem controleert gegevens zijn ingevuld |
| | 4. Systeem controleert of gebruikersnaam niet in gebruik is |
| | 5. Systeem controleert of wachtwoord voldoet aan eisen |
| | 6. Systeem slaat gegevens op |
| | 7. Systeem geeft speler start items
| | 8. Systeem logt speler in |
| | 9. Systeem toont dashboard |
| | **Alternate Flows** |
| **Actor Actions** | **System Actions** |
| | 3.a. [Gegevens zijn niet allemaal ingevuld] |
| | 3.a.1 Systeem toont melding gegevens niet allemaal ingevuld | 
| | 3.a.2 Systeem toont registratieformulier |
| --- | --- |
| | 4.a. [Gebruikersnaam is in gebruik] |
| | 4.a.1 Systeem toont melding gebruikersnaam in gebruik | 
| | 4.a.2 Systeem toont registratieformulier |
| --- | --- |
| | 5.a. [Wachtwoord voldoet niet aan eisen] |
| | 5.a.1 Systeem toont melding wachtwoord niet correct |
| | 5.a.2. Systeem toont registratieformulier |




  



[Use case diagram]: http://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/Jelmergu/ooad-casus-vagado/master/docs/diagrams/use_cases/use_cases.puml?cache=no