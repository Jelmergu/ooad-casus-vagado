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
| Precondities | Speler heeft voldoende munten |
| | Speler is in de shop|
| Postcondities | Speler heeft een nieuwe vragenlijst gekocht |
| **Main Success** | **Scenario (Basic Flow)** |
| **Actor Action** | **Systeem Action** |
| 1. Speler kiest gewenste vragenlijst | |
| | 2. Systeem geeft vragenlijst weer met opties om deze aan te schaffen |
| 3. Speler koopt gewenste vragenlijst | |
| | 4. Systeem controleert of Speler genoeg munten heeft |
| | 5. Systeem controleert of Speler lijst al niet bezit |
| | 6. Systeem trekt de waarde in munten van de vragenlijst af van het aantal munten van de speler|
| | 7. Systeem voegt de vragenlijst toe aan de informatie van de speler |
| | 8. Systeem toont melding '*U heeft de vragenlijst met success gekocht*' |
| | **Alternate Flows** |
| **Actor action** | **Systeem Action** |
| | 4.a. [Speler heeft niet genoeg munten] |
| | 4.a.1 Systeem toont foutmelding '*niet genoeg munten*' | 
| --- | --- |
| |  5.a. [Speler heeft vragenlijst al in bezit] |
| | 5.a.1. Systeem toont foutmelding '*U heeft deze lijst al in uw bezit*' |

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
| | 2.a. [Antwoord is leeg] |
| | 2.a.1 Systeem slaat antwoord over |
| | 2.a.2 Ga naar Main flow actie 4 |
| --- | --- |
| | 4.a. [Niet alle vragen zijn beantwoord] |
| | 4.a.1 Systeem toont volgende vraag |
| | 4.a.2 Ga naar Main flow actie 1 | 

### Use Case 4: Vragen beheren
| UC4: Vragen wijzigen | | 
| --- | --- |
| Stakeholders | MHM Games |
| Primary Actors | Medewerker |
| Precondities | Medewerker is bij paneel voor vragen beheren |
| Postcondities | Vraag is aangepast |
| **Main Success** | **Scenario (Basic Flow)** |
| **Actor Action** | **Systeem Action** |
| 1. Medewerker kiest een vragenlijst om aan te passen | | 
| | 2. Systeem toont vragenlijst met bijbehorende vragen |
| 3. Medewerker wijzigt een vraag en wijzigt hiervan het antwoord | |
| | 4. Systeem slaat vragenlijst op |
| | 5. Systeem toont melding dat vragenlijst successvol is opgeslagen |
| | **Alternative Flows** |
| | 4.a. [Fout bij het opslaan van vragenlijst] |
| | 4.a.1. Systeem toont foutmelding '*Er is iets fouts gegaan*'|
| --- | --- |
| 3.a.1. [Medewerker annuleert wijzigen] | | 
| | 3.a.2. Systeem toont paneel voor vragen beheren |


| UC4: Vragen aanmaken | | 
| --- | --- |
| Stakeholders | MHM Games |
| Primary Actors | Medewerker |
| Precondities | Medewerker is bij paneel voor vragen beheren |
| Postcondities | Vraag/vragen aangemaakt |
| **Main Success** | **Scenario (Basic Flow)** |
| **Actor Action** | **Systeem Action** |
| 1. Medewerker klikt op de knop '*Lijst aanmaken*' | | 
| | 2. Systeem toont scherm om vragen aan te maken |
| 3. Medewerker voert vragen met bijbehorende antwoorden in | |
| | 4. Systeem slaat vragenlijst op |
| | 5. Systeem toont melding dat vragenlijst successvol is opgeslagen |
| | **Alternative Flows** |
| 3.a.1. [Medewerker annuleert aanmaken] | | 
| | 3.a.2. Systeem toont paneel voor vragen beheren |
| --- | --- |
| | 4.a. [Fout bij het opslaan van vragenlijst] |
| | 4.a.2. Systeem toont foutmelding '*Er is iets fouts gegaan*'|


| UC4: Vragen verwijderen | | 
| --- | --- |
| Stakeholders | MHM Games |
| Primary Actors | Medewerker |
| Precondities | Medewerker is bij paneel voor vragen beheren |
| Postcondities | Vraag/vragen verwijderd|
| **Main Success** | **Scenario (Basic Flow)** |
| **Actor Action** | **Systeem Action** |
| 1. Medewerker kiest een lijst om aan te passen | | 
| | 2. Systeem toont scherm met bijbehorende vragen en antwoorden van de lijst |
| 3. Medewerker verwijderd een vraag met bijbehorende antwoord | |
| | 4. Systeem slaat vragenlijst op |
| | 5. Systeem toont melding dat vragenlijst successvol is verwijderd |
| | **Alternative Flows** |
| | 3.a.1. [Medewerker annuleert verwijderen] |
| | 3.a.2. Systeem toont paneel voor vragen beheren |
| --- | --- |
| 4.a. [Fout bij het verwijderen van vragenlijst] | | 
| | 4.a.2. Systeem toont foutmelding '*Er is iets fouts gegaan*'|

### Use case 5: Thema's Beheren
| UC5: Thema wijzigen | | 
| --- | --- |
| Stakeholders | MHM Games |
| Primary Actors | Medewerker |
| Precondities | Medewerker is bij paneel voor thema's beheren |
| Postcondities | Thema is aangepast |
| **Main Success** | **Scenario (Basic Flow)** |
| **Actor Action** | **Systeem Action** |
| 1. Medewerker kiest een thema om aan te passen | | 
| | 2. Systeem toont thema met bijbehorende informatie |
| 3. Medewerker wijzigt een de informatie van een thema | |
| | 4. Systeem slaat thema op |
| | 5. Systeem toont melding dat thema successvol is opgeslagen |
| | **Alternative Flows** |
| 3.a.1. [Medewerker annuleert wijzigen] | | 
| | 3.a.2. Systeem toont paneel voor thema's beheren |
| --- | --- |
| | 4.a. [Fout bij het opslaan van thema] |
| | 4.a.1. Systeem toont foutmelding '*Er is iets fouts gegaan*'|


| UC5: Thema aanmaken | | 
| --- | --- |
| Stakeholders | MHM Games |
| Primary Actors | Medewerker |
| Precondities | Medewerker is bij paneel voor thema's beheren |
| Postcondities | Thema aangemaakt |
| **Main Success** | **Scenario (Basic Flow)** |
| **Actor Action** | **Systeem Action** |
| 1. Medewerker klikt op de knop '*Thema aanmaken*' | | 
| | 2. Systeem toont scherm om thema aan te maken |
| 3. Medewerker voert thema met informatie in | |
| | 4. Systeem slaat thema op |
| | 5. Systeem toont melding dat thema successvol is opgeslagen |
| | **Alternative Flows** |
| 3.a.1. [Medewerker annuleert aanmaken] | | 
| | 3.a.2. Systeem toont paneel voor thema beheren |
| --- | --- |
| | 4.a. [Fout bij het opslaan van thema] |
| | 4.a.2. Systeem toont foutmelding '*Er is iets fouts gegaan*'|


| UC5: Thema verwijderen | | 
| --- | --- |
| Stakeholders | MHM Games |
| Primary Actors | Medewerker |
| Precondities | Medewerker is bij paneel voor thema's beheren |
| Postcondities | Thema verwijdert |
| **Main Success** | **Scenario (Basic Flow)** |
| **Actor Action** | **Systeem Action** |
| 1. Medewerker kiest een thema om aan te passen | | 
| | 2. Systeem toont thema met informatie |
| 3. Medewerker verwijdert een thema | |
| | 4. Systeem verwijdert thema |
| | 5. Systeem toont melding dat thema successvol is verwijderd |
| | **Alternative Flows** |
| | 3.a.1. [Medewerker annuleert verwijderen] |
| | 3.a.2. Systeem toont paneel voor thema beheren |
| --- | --- |
| 4.a. [Fout bij het verwijderen van thema] | | 
| | 4.a.2. Systeem toont foutmelding '*Er is iets fouts gegaan*'|

### Use case 6: Vragenlijsten beheren
| UC6: Vragenlijst verwijderen | | 
| --- | --- |
| Stakeholders | MHM Games |
| Primary Actors | Medewerker |
| Precondities | Medewerker is bij paneel voor vragen beheren |
| Postcondities | Vragenlijst verwijderd |
| **Main Success** | **Scenario (Basic Flow)** |
| **Actor Action** | **Systeem Action** |
| 1. Medewerker kiest een lijst om te verwijderen en klikt op de knop '*Verwijderen*' | | 
| | 2. Systeem toont een melding '*Weet u het zeker dat u [vragenlijst] wilt verwijderen**' |
| 3. Medewerker klikt op '*Ja*' | |
| | 4. Systeem verwijderd lijst |
| | 5. Systeem toont melding dat vragenlijst successvol is verwijderd |
| | **Alternative Flows** |
| | 3.a.1. Fout bij het verwijderen van vragenlijst |
| | 3.a.2. Systeem toont foutmelding '*Er is iets fouts gegaan*'|
| --- | --- |
| 3.a.1. Medewerker klikt op knop '*Nee*' | | 
| | 3.a.2. Systeem toont paneel voor vragen beheren |

| UC6: Vragenlijst wijzigen | | 
| --- | --- |
| Stakeholders | MHM Games |
| Primary Actors | Medewerker |
| Precondities | Medewerker is bij paneel voor vragen beheren |
| Postcondities | Vragenlijst gewijzigd |
| **Main Success** | **Scenario (Basic Flow)** |
| **Actor Action** | **Systeem Action** |
| 1. Medewerker kiest een lijst om te wijzigen en klikt op de knop '*Wijzigen*' | | 
| | 2. Systeem toont vragenlijst met bijbehorende informatie |
| 3. Medewerker wijzigt de gekozen gegevens | |
|  4. Medewerker klikt op '*Opslaan*' ||
| | 5. Systeem toont melding dat vragenlijst successvol is opgeslagen |
| | **Alternative Flows** |
| | 4.a.1. Fout bij het opslaan van vragenlijst |
| | 4.a.2. Systeem toont foutmelding '*Er is iets fouts gegaan*'|
| --- | --- |
| 4.b.1. Medewerker klikt op knop '*Annuleren*' | | 
| | 4.b.2. Systeem toont paneel voor vragenlijsten beheren |


| UC6: Vragenlijst aanmaken | | 
| --- | --- |
| Stakeholders | MHM Games |
| Primary Actors | Medewerker |
| Precondities | Medewerker is bij paneel voor vragen beheren |
| Postcondities | Vragenlijst gewijzigd |
| **Main Success** | **Scenario (Basic Flow)** |
| **Actor Action** | **Systeem Action** |
| 1. Medewerker klikt op de knop '*Vragenlijst aanmaken*' | | 
| 3. Medewerker voert bijbehorende gegevens in | |
| 4. Medewerker klikt op '*Opslaan*' | |
| | 5. Systeem toont melding dat vragenlijst successvol is opgeslagen |
| | **Alternative Flows** |
| | 4.a.1. Fout bij het opslaan van vragenlijst |
| | 4.a.2. Systeem toont foutmelding '*Er is iets fouts gegaan*'|
| --- | --- |
| 4.b.1. Medewerker klikt op knop '*Annuleren*' | | 
| | 4.b.2. Systeem toont paneel voor vragenlijsten beheren |





[Use case diagram]: http://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/Jelmergu/ooad-casus-vagado/master/docs/diagrams/use_cases/use_cases.puml?cache=no