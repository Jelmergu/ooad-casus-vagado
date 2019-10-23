# Usecase beschrijvingen

![Use case diagram]

### Use case 2: Vragenlijst Kopen
| UC1: Registreren | |
| --- | --- |
| Primary Actor | Speler | 
| Precondities | - |
| Postconditie | Speler is geregistreerd en ingelogd en aangekomen op zijn dashboard |
| **Main Success scenario** | |
| **Actor Actions** | **Systeem Actions** |
| 1. Speler vult gegevens in |  |
| 2. Speler verstuurt formulier | |
| | 3. Systeem controleert gegevens zijn ingevuld |
| | 4. Systeem controleert of gebruikersnaam niet in gebruik is |
| | 5. Systeem controleert of wachtwoord voldoet aan eisen |
| | 6. Systeem slaat gegevens op |
| | 7. Systeem geeft speler start items |
| | 8. Systeem logt speler in |
| | 9. Systeem toont dashboard |
| | **Alternate Flows** |
| **Actor Actions** | **Systeem Actions** |
| | 3.a. [Gegevens zijn niet allemaal ingevuld] |
| | 3.a.1 Systeem toont melding '*gegevens niet allemaal ingevuld*' | 
| | 3.a.2 Systeem toont registratieformulier |
| --- | --- |
| | 4.a. [Gebruikersnaam is in gebruik] |
| | 4.a.1 Systeem toont melding '*gebruikersnaam in gebruik*' | 
| | 4.a.2 Systeem toont registratieformulier |
| --- | --- |
| | 5.a. [Wachtwoord voldoet niet aan eisen] |
| | 5.a.1 Systeem toont melding wachtwoord niet correct |
| | 5.a.2. Systeem toont registratieformulier |

### Use case 2: Vragenlijst Kopen
| UC2: Vragenlijst kopen | |
| --- | --- |
| Stakeholders | MHM Games, wilt dat spelers een vragenlijst kunnen kopen |
| Primary Actors | Speler |
| Precondities | Speler is ingelogd |
| | Speler heeft voldoende munten |
| | Gebruiker is in de shop|
| Postcondities | Speler heeft een nieuwe vragenlijst gekocht |
| **Main Success** | **Scenario (Basic Flow)** |
| **Actor Action** | **Systeem Action** |
| 1. Gebruiker kiest gewenste vragenlijst | |
| | 2. Systeem geeft vragenlijst weer met opties om deze aan te schaffen |
| 3. Gebruiker koopt gewenste vragenlijst | |
| | 4. Systeem controleert of gebruiker genoeg munten heeft |
| | 5. Systeem trekt de waarde in munten van de vragenlijst af van het aantal munten van de speler|
| | 6. Systeem voegt de vragenlijst toe aan de informatie van de speler |
| | 7. Systeem toont scherm met informatie over de voltooide aankoop |
| | **Alternate Flows** |
| **Actor action** | **Systeem Action** |
| | 4.a. [Speler heeft niet genoeg munten] |
| | 4.a.1 Systeem toont foutmelding '*niet genoeg munten*' | 



### Use case #: <UC naam>
| UC#: <UC naam> | |
| --- | --- |
| Stakeholders | MHM Games |
| Primary Actors | <Actor> |
| Precondities | <preconditie 1> |
| | ... |
| Postcondities | <Postconditie> |
| **Main Success** | **Scenario (Basic Flow)** |
| **Actor Action** | **Systeem Action** |
| 1. <Actor> | |
| | 2. <Systeem>
| | **Alternate Flows** |
| **Actor action** | **Systeem Action** |
| | 2.a. [<Conditie>] |
| | 4.a.1 <acties> | 


[Use case diagram]: http://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/Jelmergu/ooad-casus-vagado/master/docs/diagrams/use_cases/use_cases.puml?cache=no