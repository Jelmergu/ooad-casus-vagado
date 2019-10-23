# Usecase beschrijvingen

![Use case diagram]

Voor alle usecases, behalve UC1 Registreren, geldt als preconditie: `<Actor> is ingelogd`.

### Use case 2: Vragenlijst Kopen
| UC1: Registreren | |
| --- | --- |
| Stakeholders | MHM Games |
| Brief description | Deze usecase beschrijft het registratieprocess |
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
| Stakeholders | MHM Games |
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

### Use case 3: Vragenlijst beantwoorden
| UC3: Vragenlijst beantwoorden | |
| --- | --- |
| Stakeholders | MHM Games |
| Brief description| Deze usecase beschrijft de acties die uitgevoerd worden voor het beantwoorden van een vragenlijst |
| Primary Actors | Speler |
| Precondities | Speler heeft de vragenlijst gekocht |
| | Speler heeft de vragenlijst geopent |
| Postcondities | Speler heeft de vragenlijst volledig goed beantwoordt |
| **Main Success** | **Scenario (Basic Flow)** |
| **Actor Action** | **Systeem Action** |
| 1. Speler beantwoordt vraag | |
| | 2. Systeem valideert antwoord |
| | 3. Systeem bewaart score van antwoord |
| | 4. Systeem toont vragenlijst resultaat |
| | **Alternate Flows** |
| **Actor action** | **Systeem Action** |
| | 4.a. [Niet alle vragen zijn beantwoord] |
| | 4.a.1 Systeem toont volgende vraag |
| | 4.a.2 Ga naar Main flow actie 1 | 
| --- | --- |
| | 2.a. [Antwoord is leeg] |
| | 2.a.1 Systeem slaat antwoord over |
| | 2.a.2 Ga naar Main flow actie 4 |

[Use case diagram]: http://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/Jelmergu/ooad-casus-vagado/master/docs/diagrams/use_cases/use_cases.puml?cache=no