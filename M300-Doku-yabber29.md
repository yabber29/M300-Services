M300 Dokumentation von Ramon Christen (yabber29)
==========================================================

### Lernziele
Die nachstehende Dokumentation zeigt alle Schritte auf, die es zur Einrichtung einer vollständig funktionsfähigen Toolumgebung benötigt werden.

### Inhaltsverzeichnis
* 01 - Github
* 02 - Git Client
* 03 - VirtualBox
* 04 - Vagrant
* 05 - Visual Studio Code

---

01 - Github
======

> [⇧ **Nach oben**](#inhaltsverzeichnis)

Als erstes durften wir einen Github Account erstellen und zudem ein Git Repository erstellen. Die beiden Schritte gingen schnell und unkompliziert.
Ich hatte noch einen SSH-Key erstellt in dem Terminal. Als dieser erstellt wurde konnte ich den SSH-Key im GitHub hinzufügen. Dies hat sehr schnell funktioniert und konnten und dadurch konnte ich mich immer direkt anmelden, da ich einen Privat-Key auf meinem Laptop habe.

---

02 - Git Client
======

> [⇧ **Nach oben**](#inhaltsverzeichnis)

### Was ist Git
Git ist eine weit verbreitete Open-Source-Software zur verteilten Versionskontrolle von Software. Lesen Sie hier, wie das Tool unter Windows funktioniert. Git ist ein Versionskontrollsystem, das vom Linux-Erfinder Linus Torvalds entwickelt wurde.

### Wieso wird Git oft von Programmierern gebraucht?
Einige Vorteile von Git
- Paralleles Arbeiten
- Flexibilität
- Performance
- Einfache Beiträge
- Robustheit
- Gemeinschaft und Freiheit
- etc.

### Die wichtigsten Befehle in Git
**Client Konfigurieren**

Informationen mit Hilfe von Git ändern des GitHub Accounts
``` 
$ git config --global user.name "<username>"
$ git config --global user.email "<e-mail>"
```
**Repository clone/pull**

Clone und Pull eines Reporitorys
```
$ git clone https://gitlab.com/ch-tbz-it/Stud/m300/
$ cd M300           # In das Verzeichniss wechseln
$ git pull
```
**Repository Push**

Git push wird üblicherweise verwendet, um lokale Änderungen in einem zentralen Repository zu veröffentlichen und hochzuladen. Nachdem Änderungen an einem lokalen Repository vorgenommen wurden, werden die Änderungen per Push für Remote-Teammitglieder freigegeben.
```
$ git add -A
$ git commit -m "Mein Kommentar"
$ git push
```
**How to Push**

Hier habe ich noch einige Befehle die man beherschen sollte. 
```Shell 
$  cd Pfad/zu/meinem/Repository    # Zum lokalen GitHub-Repository wechseln

$  git status                      # Geänderte Datei(en) werden rot aufgelistet
$  git add -A                      # Fügt alle Dateien zum "Upload" hinzu
$  git status                      # Der Status ist nun grün > Dateien sind Upload-bereit (Optional) 
$  git commit -m "Mein Kommentar"  # Upload wird "commited" > Kommentar zu Dokumentationszwecken ist dafür notwendig
$  git status                      # Dateien werden nun als "zum Pushen bereit" angezeigt
$  git push                        #Upload bzw. Push wird durchgeführt
```

