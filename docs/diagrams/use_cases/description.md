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

| UC2: Vragenlijst kopen | |
| --- | --- |
| Stakeholders | MHM Games, wilt dat spelers een vragenlijst kunnen kopen |
| Primary Actors | Speler |
| Precondities | Is ingelogd. Speler heeft voldoende munten |
| Postcondities | Speler heeft een nieuwe vragenlijst gekocht |
| Models | Use Case Diagram Vagado |
| **Main Success** | **Scenario (Basic Flow)** |  
|Description | Speler heeft een vragenlijst gekocht met de beschikbare munten en kan nu de vragenlijst beantwoorden |
| Actor Action | System Action |
| 1. Gebruiker is bij de Vagado-shop | |
| 2. Gebruiker kiest gewenste vragenlijst | |
| | 3. Systeem geeft vragenlijst weer met opties om deze aan te schaffen |
| 4. Gebruiker koopt gewenste vragenlijst | |
| | 5. Systeem controlleerd of gebruiker genoeg munten heeft |
| | 6. Systeem trekt de waarde in munten van de vragenlijst af van de aantal munten van de speler|
| | 7. Systeem voegt de vragenlijst toe aan de informatie van de speler |
| | 8. Systeem laat scherm zien met informatie van de voltooide aankoop |
| **Extensions** | **(Alternative Flow)** |  
| Description| Speler heeft niet genoeg munten en krijgt een foutmelding |
| Actor action | System Action |
| | 3a.1 Systeem controlleerd of speler genoeg munten heeft |
| | 3a.2 Systeem laat foutmelding zien aan speler dat de speler geen genoeg munten heeft | 


[Use case diagram]: http://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/Jelmergu/ooad-casus-vagado/master/docs/diagrams/use_cases/use_cases.puml?cache=no