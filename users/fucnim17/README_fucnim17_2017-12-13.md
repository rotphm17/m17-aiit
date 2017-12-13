# Textdateien

## Codierung

Als **Codierung** bezeichnet man den Vorgang, bei dem man aus einem Zeichen eine Bitkette macht. Decodierung ist genau der Umgekehrte Vorgang, also von einer Bitkette zu einem Zeichen. 
Früher wurde der American Standard Code for Information Interchange, kurz [ASCII-Code](https://de.wikipedia.org/wiki/American_Standard_Code_for_Information_Interchange) verwendet.
Heutzutage verwendet man nur noch Unicode, da er ständig erweitert werden kann. ([UTF-8](https://de.wikipedia.org/wiki/UTF-8) ist eine vereinfachte Variante mit 8 Bit (Unicode hat 32 Bit d.h. ca. 100000 Zeichen!))

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
Der UTF8-Code ist in den ersten 128 Zeichen itent mit dem ASCII-Code, doch er kann wie jeder Unicode beliebig oft erweitert werden.
Er kann bestehen aus:

| 1 Byte | 2 Bytes | 3 Bytes | 4 Bytes | 
| ----------- | ------------ | ------------------ | ----------------- |
| **0**0101010 | 
