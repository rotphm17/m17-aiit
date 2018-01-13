# Textdateien

## Publizieren

Als [***Publizieren**](https://de.wikipedia.org/wiki/Publikation)* bezeichnet man den Vorgaang, bei dem man Informationen bzw. Dateien über das Internet weiter- bzw. freigibt.

**Möglichkeiten:**

* Soziale Netzwerke: (Whatsapp, Facebook, Twitter, Snapchat, Youtube, etc.)
* Word Dokumente: veröffentlicht in einer Cloud oder auf einer Website
* PDF-Dokument: Vorteil gegenüber Word-Dokumente → sie sind genormt (alle Versionen gleich)
* als Website (in HTML-Format): beste Lösung → passt sich automatisch an die Bildschirmgröße an*-


## Codierung

Als **Codierung** bezeichnet man den Vorgang, bei dem man aus einem Zeichen eine Bitkette macht. Decodierung ist genau der umgekehrte Vorgang, also von einer Bitkette zu einem Zeichen. 
Früher wurde der American Standard Code for Information Interchange, kurz [ASCII-Code](https://de.wikipedia.org/wiki/American_Standard_Code_for_Information_Interchange) verwendet.
Heutzutage verwendet man nur noch Unicode, da er ständig erweitert werden kann. ([UTF-8](https://de.wikipedia.org/wiki/UTF-8) ist eine vereinfachte Variante mit 8 Bit.)

### ASCII-Code

Der ASCII-Code umfasst 8 Bits (256 Zeichen).  
Die ersten 128 Zeichen sind immer die gleichen. In den ersten 128 Zeichen enthalten sind:

* 32 Steuerzeichen (z.B.: Zeilenvorschub)
* a........z
* A........Z
* 0........9
* Sonderzeichen (z.B.: # , ! -)

Die weiteren 128 Zeichen können je nach Land mit sogennanten ***Code Pages*** verschieden genutz werden.
z.B Griechische Alphabet, Deutsche Umlaute,...)

### UTF8-Code
Der UTF8-Code ist in den ersten 128 Zeichen ident mit dem ASCII-Code, doch er kann wie jeder Unicode beliebig oft erweitert werden.
Er kann bestehen aus:

| 1 Byte | 2 Bytes | 3 Bytes | 4 Bytes | 
| ----------- | ------------ | ------------------ | ----------------- |
| {**0**0101010} | {**110**01010} {**10**010101} | {**1110**01010} {**10**0101010} {**10**010101} | {**11110**01} {**10**010101} {**10**0101010} {**10**0101010} |  
| 2⁷ | 2¹¹ | 2¹⁶ | 2²¹ |
| 128 Zeichen | 2048 Zeichen | 65536 Zeichen | 2097152 Zeichen |

Man erkennt: Bytes die mit 01 anfangen sind Nachfolgebytes. Stehen am ersten Byte am Anfang zwei Einsen, dann ist dies ein zweistelliges Byte. Stehen 3 am Anfang, dann ein Dreistelliges usw.  

#### Übungen zum UTF-8 Code

