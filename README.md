# Übung 8 - Typecasting, Debugger, Scanner


## 1. Aufgabe

Folgendes Klassendiagramm soll umgesetzt werden:

<p align="center">
  <img src="/assets/images/UML1.png" alt="Bildbeschreibung" />
</p>

**Folgende Bedingungen gelten für die Eigenschaften:**
- `punkte` darf einen Wert von 0 bis 100 annehmen.

**Folgende Bedingungen gelten für die Methoden:**
- Im Konstruktor müssen statt der Zuweisung die `set`-Methoden aufgerufen werden.
- Die Parameternamen des Konstruktors müssen gleich den Eigenschaftsnamen sein. 
- `pruefeNote()`: Gibt aus, welche Note mit den angegebenen Punkten erreicht wurde. Es gilt folgender Notenschlüssel:
	- [90, 100]: Sehr gut
	- [80, 90): Gut
	- [70, 80): Befriedigend
	- [60, 70): Genügend
	- [0, 60): Nicht Genügend

Um Ihr Programm zu testen, erstellen Sie eine `Main`-Klasse, welche die `main`-Methode beinhaltet:
- `main(String[] args)`: Erstellen Sie eine Instanz der `Notenpruefung`-Klasse. Erstellen Sie einen Scanner und lassen Sie den Benutzer die Punkte eingeben. Je nachdem wie viele Punkte eingegeben wurden, soll dann die richtige Note ausgegeben werden.

## 2. Aufgabe

Folgendes Klassendiagramm soll umgesetzt werden:

<p align="center">
  <img src="/assets/images/UML2.png" alt="Bildbeschreibung" />
</p>

**Folgende Bedingungen gelten für die Eigenschaften:**
- `alter` muss größer-gleich 18 sein.

Bei falschen Werten soll eine Fehlermeldung ausgegeben werden.

**Folgende Bedingungen gelten für die Methoden:**
- Im Konstruktor müssen statt der Zuweisung die `set`-Methoden aufgerufen werden.
- Die Parameternamen des Konstruktors müssen gleich den Eigenschaftsnamen sein. 
- `print()`: Gibt alle Eigenschaften schön formatiert aus.


Um Ihr Programm zu testen, erstellen Sie eine `Main`-Klasse, welche die `main`-Methode beinhaltet:
- `main(String[] args)`: Erstellen Sie mit dem Scanner eine Instanz der Studentklasse. Lesen Sie die Werte dafür mittels Scanner ein.

## 3. Aufgabe


Folgendes Klassendiagramm soll umgesetzt werden:

<p align="center">
  <img src="/assets/images/UML3.png" alt="Bildbeschreibung" />
</p>

**Folgende Bedingungen gelten für die Eigenschaften:**
- `wasserFuellstand` muss größer-gleich 0 und kleiner-gleich `wasserKapazitaet` sein.
- `wasserKapazitaet` darf einen Wert von 500.0 bis 2000.0 annehmen.
- `bohnenFuellstand` muss größer-gleich 0 und kleiner-gleich `bohnenKapazitaet` sein.
- `bohnenKapazitaet` darf einen Wert von 100 bis 1000 annehmen.

Wenn falsche Werte übergeben werden, so geben Sie eine Fehlermeldung aus.

**Beschreibung der Methoden:**
- Im Konstruktor müssen statt der Zuweisung die set-Methoden aufgerufen werden. Achten Sie auf die Reihenfolge der Aufrufe. 
- Die Parameternamen des Konstruktors müssen gleich den Eigenschaftsnamen sein.
- `einschalten()`: Die Kaffeemaschine soll eingeschalten werden. Geben Sie dazu auch eine Meldung aus.
- `ausschalten()`: Die Kaffeemaschine soll ausgeschalten werden. Geben Sie dazu auch eine Meldung aus.
- `wasserAuffuellen(double menge)`: Das Wasser soll um `menge` aufgefüllt werden. Geben Sie aus wie viel Wasser aufgefüllt wurde und wie viel Wasser nun in der Maschine ist.
- `bohnenAuffuellen(int menge)`: Die Bohnen sollen um `menge` aufgefüllt werden. Geben Sie aus wie viel an Bohnen aufgefüllt wurde und wie viel an Bohnen nun in der Maschine ist.
- `kochen(int art)`: Es soll Kaffee gekocht werden. Dies soll aber nur möglich sein, wenn die Kaffeemaschine eingeschalten ist. Die `art` gibt an, welcher Kaffee gekocht werden soll. Folgende Arten werden bei der jeweiligen Zahl gekocht:
	- `art= 1`: Espresso: Es werden 30 Wasser und 10 Bohnen benötigt.
	- `art = 2`: Latte: Es werden 100 Wasser und 20 Bohnen benötigt.
	- `art = 3`: Capuccino: Es werden 120 Wasser und 25 Bohnen benötigt.

Sollten die benötigten Mengen nicht in der Maschine sein, kann der Kaffee nicht gekocht werden und eine Fehlermeldung soll ausgegeben werden.

**Zusatz:** Setzen Sie auch das Auffüllen von Wasser und Bohnen mit dem Scanner um.

Um Ihr Programm zu testen, erstellen Sie eine `Main`-Klasse, welche die `main`-Methode beinhaltet:
- `main(String[] args)`: Erstellen Sie eine Instanz der Kaffeemaschinenklasse. Erstellen Sie einen Scanner und testen Sie mit verschiedenen Eingaben Ihr Programm.
