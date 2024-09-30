# **Anleitung**

1. ***Git*** muss zuerst runtergeladen und auf deinem Rechner installiert werden.
Prüfe anschließend ob git richtig installiert wurde mit dem Befehl **git --version**
Initialisiere ein neues ***Git-Repository*** mit dem Befehl **git init**

2. Um deinen Namen und die Email-Adresse für git zu identifizieren musst du dies einmal in einer ***globalen*** Konfiguration bestätigen
Nutze hierfür folgende Befehle :
**git config --global user.name "Dein Name"**
**git config --global user.email "deine.email@beispiel.com"**

## **3. Verwaltung von Änderungen mit Git:**

    * 1.Erstelle eine neue Datei mit dem Befehl:  **touch "Dateiname"** 
    * 2.Datei zum Staging-Bereich hinzufügen mit dem Befehl: **git add "Dateiname"**
    * 3.Erstelle einen Commit, um die Änderungen zu speichern mit dem Befehl: **git commit -m "Kommentar"**

## **4. Verbindung zu einem Remote-Repository:**

    * 1.Füge das Remote-Repository deinem lokalen Repository hinzu mit dem Befehl: **git remote add origin git@github.com:user.name/Anleitung.git**
    * 2. Überprüfe, ob das Remote korrekt hinzugefügt wurde mit dem Befehl: **git remote -v**
    * 3.Clonen des Repositories mit dem Befehl: **git clone git@github.com:user.name/Anleitung.git**

## **5. Synchronisieren von Änderungen :**

Falls es Änderungen im Remote-Repository gibt, können diese durch den Befehl ***git pull*** heruntergeladen werden.
Nun hat man die aktuelle Datei lokal und kann ebenfalls Änderungen durchführen.
Nachdem eine Änderung vorgenommen wurde, können diese mit dem ***git push*** Befehl von lokal auf das Remote-Repository "hochgeladen" werden.

## **6. Branching und Feature-Entwicklung**

Um einen separaten Branch in einem Feature zu erstellen müssen wir **git checkout -b feature-branchname** in unsere Konsole eingeben.
Damit wird ein neuer Branch erstellt und ebenfalls direkt in diesen gewechselt.
Anschließend müssen wir die Datei durch ein **git add "Dateiname"** in unsere ***Staging-Area*** bringen. 
Wenn die Datei dann bearbeitet wurde ist es notwendig diese zu commiten um sie zu sichern
und gleichzeitig zu kommentieren was man getan oder verändert hat. Dies erfolgt mit dem Befehl **git commit -m "Änderung"**

## **7. Zusammenführunen von Branches:**

Ist ein Feature fertig, kann es durch einen ***Merge*** oder ***Pull*** Request
in den***Main-Branch*** des lokalen Repositorys eingebunden werden. Mit **git merge**
kann man den ***lokalen*** Feature-Branch zum lokalen Main-Branch hinzufügen
und mit **git pull** kann man bspw. neue Features aus dem remote repository
in das lokale Repository einbinden. 
