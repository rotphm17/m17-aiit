# Verzeichnisbaum

Es gibt verschiedene Verzeichnise. Man kann sich das ganze unter einem umgedrehten Baum vorstellen. Bei Windows fängt der "Stamm" mit C: an. Windows stellt z.B einen Usb-Stick auch als eigenes Verzeichnis da. Diese beginnen immer mit einem Großbuchstaben. Von dem Hauptverzeichnis gehen dann alle anderen Dateien/Verzeichnise weg.  
Bei Linux und macOs fängt der Verzeichnisbaum mit ( / <--root ) an. Usb-Sticks etc werden NICHT wie bei Windows unter einen eigenen Verzeichnisbaum dargestellt.

# Multi User / Multi Task

## Multi User:
Die Idee, mehrere Benutzer mit einem Computer arbeiten zu lassen, stammt bereits aus den frühen Zeiten der Großrechner, wo sich viele EDV-Bedarfsträger wenige Ressourcen teilen mussten. Die Rechner waren früher vor allem in Universitäten und wenigen Großbetrieben in Gebrauch. Zu ihrer Bedienung dienten Terminals, die nur aus einer Tastatur und einem Bildschirm bestanden und mit dem Hauptrechner verbunden waren.  
Der Begriff Multiuser stellt nicht unbedingt auf gleichzeitiges Arbeiten ab. Historisch gab es durchaus auch Computer, an denen verschiedene Benutzer in eigenen Arbeitsumgebungen nacheinander, jedoch nicht gleichzeitig arbeiten konnten. Sofern Multitasking vorgesehen war, konnte ein Benutzer immerhin mehrere Aufgaben gleichzeitig ausführen lassen. Wenn gleichzeitig verschiedenen Benutzern eigene Arbeitsumgebungen zur Verfügung stehen, spricht man von Multisession.

## Multi Task:
Der Begriff Multitasking [ˌmʌltiˈtɑːskɪŋ] (engl.) bzw. Mehrprozessbetrieb bezeichnet die Fähigkeit eines Betriebssystems, mehrere Aufgaben (Tasks) (quasi-)nebenläufig auszuführen. Im Allgemeinen bietet der Prozessor hierzu auch unterstützende Hardware-Strukturen. Die verschiedenen Prozesse werden in so kurzen Abständen immer abwechselnd aktiviert, dass der Eindruck der Gleichzeitigkeit entsteht. Multitasking ist somit ein Synonym für Zeit-Multiplexverfahren. Besitzt ein Computer mehrere CPU-Kerne, so dass er mehrere Aufgaben echt-gleichzeitig ausführen kann, so spricht man von Multiprocessing. In modernen Computern werden beide Verfahren kombiniert eingesetzt.
  
Multitasking kann bei verschiedenen Anforderungen nützlich sein, insbesondere bei der Optimierung der Auslastung und für eine je nach Zielsetzung ausgeglichene oder prioritätsbasierte Ressourcenverteilung.  
Jedoch heißt das nicht das die CPU (mit z.B 4 Kernen) nur 4 Aufgaben gleichzeitig erledigen kann. Er kann natürlich auch mehr als 4 Aufgaben gleichzeitig ausführen. Jedoch braucht das mehr Leistung weswegen es längere Wartezeiten gibt wenn man zu viele Aufgaben gleichzeitig ausführt.  
Man kann das Ganze so verstehen: Wie wenn man eine CPU mit 1 Kern hat und die zwei Aufgaben ausführen soll wird jeweils 50% des Kernes für 1 Aufgabe verwendet, weswegen es dann längere Wartezeiten gibt.

# Rechte
Zugriffsrechte bezeichnen in der EDV die Regeln der administrativen Zugriffskontrolle, nach denen entschieden wird, ob und wie Benutzer, Programme oder Programmteile, Operationen auf Objekten (z. B. Netzwerke, Drucker, Dateisysteme) ausführen dürfen. Am geläufigsten ist dieses Konzept bei Dateisystemberechtigungen, bei der festgelegt wird, welche Benutzer welche Dateien und Verzeichnisse lesen, schreiben, ändern oder ausführen dürfen.  
  
Beispielbild: https://upload.wikimedia.org/wikipedia/de/1/19/Zugriffsrecht.png
Die Grafik zeigt beispielhaft, was über Zugriffsrechte festgelegt werden kann. Dies ist im einfachsten Fall, WER WAS tun darf. Unter „WER“ wird häufig nicht eine spezifizierte Person, sondern eine Gruppe/Rolle festgelegt, der einzelne Benutzer zugeordnet sind. Zu „WAS“ können ebenfalls elementare Funktionen oder Gruppierungen davon benannt, sowie erforderlichenfalls spezielle Datenaktionen (Create, Read, Update, Delete) auf bestimmte Datenarten und -Mengen erlaubt werden. Je nach Bedarf können Zusatzfestlegungen wie 4AP etc. geregelt sein.

--> Eigentümer = User = u  
--> Gruppe = Group = g  
--> Alle anderen = Others = o  

Es gibt grundsätzlich 3 verschiedene Rechte:  
r...read (lesen)  
w...write (schreiben, modifizieren)  
x...execute (ausführen, in das Verzeichnis "hineingehen")  

0...nicht erteilt, 1...erteilt  
uuu   ggg   ooo  
rwx   rwx   rwx  
110   100   000 <---Dateirechte  

Das Beispiel würde so viel bedeuten wie: Der User hat die Rechte R,W d.h: er darf Dateien lesen, verändern aber nicht Ausführen. Die Group darf Dateien lesen aber nicht modifizieren. Alle anderen können mit einer Datei nichts machen.

#### Ändern der Rechte:
Gui: Nautilus bei Ubuntu. --> Dateimanager
Shell: (ch = change) Chmod, Chgip, Cham

## Superuser
Ein Superuser bzw. Superadmin hat ALLE Rechte. Wenn man einen Benutzer als Superuser einstellt kann man das NICHT mehr ändern.
Das erste Benutzerkonto das auf dem PC eingerichtet wird kann sich selbst als Superuser einstellen.

