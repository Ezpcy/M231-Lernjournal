# Verschlüsselung

## Cäsar-Verschlüsselung

Die Cäsar-Verschlüsselung, benannt nach Julius Cäsar, der sie angeblich benutzte, ist eine der einfachsten und bekanntesten Verschlüsselungstechniken. Es handelt sich um eine Art der Substitutionsverschlüsselung, bei der jeder Buchstabe im Klartext um eine festgelegte Anzahl von Stellen im Alphabet verschoben wird.

### **Funktionsweise der Cäsar-Verschlüsselung**

**Grundprinzip:**

- Du wählst eine Verschiebungszahl (oft als "Schlüssel" bezeichnet). Zum Beispiel könnte die Zahl 3 sein.
- Jeder Buchstabe in deinem Klartext wird um diese Anzahl von Stellen im Alphabet verschoben.

**Beispiel:**

- Verschiebungszahl (Schlüssel): 3
- Klartext: **`HALLO`**
- Verschlüsselung:
    - **`H`** wird zu **`K`** (H->I->J->K)
    - **`A`** wird zu **`D`**
    - **`L`** wird zu **`O`**
    - **`L`** wird zu **`O`**
    - **`O`** wird zu **`R`**
- Verschlüsselter Text: **`KDOOR`**

### **Entschlüsselung**

Um eine Nachricht, die mit der Cäsar-Verschlüsselung kodiert wurde, zu entschlüsseln, machst du die Verschiebung rückgängig. Das heißt, du verschiebst die Buchstaben des verschlüsselten Textes in die entgegengesetzte Richtung um denselben Schlüsselwert.

**Beispiel:**

- Verschlüsselter Text: **`KDOOR`**
- Schlüssel: 3
- Entschlüsselung:
    - **`K`** wird zu **`H`**
    - **`D`** wird zu **`A`**
    - **`O`** wird zu **`L`**
    - **`O`** wird zu **`L`**
    - **`R`** wird zu **`O`**
- Ursprünglicher Text: **`HALLO`**

### **Anwendung und Sicherheit**

- **Anwendung:** Die Cäsar-Verschlüsselung wird heute hauptsächlich für pädagogische Zwecke im Bereich der Kryptographie genutzt, um die Grundlagen der Verschlüsselung zu vermitteln.
- **Sicherheit:** Sie bietet kaum Sicherheit gegen moderne Entschlüsselungsmethoden. Sie kann leicht durch sogenannte Brute-Force-Methoden (Ausprobieren aller möglichen Schlüssel) oder durch Frequenzanalyse (Analyse der Häufigkeit von Buchstaben) gebrochen werden.

Obwohl sie nicht für ernsthafte oder sensible Kommunikation geeignet ist, bleibt die Cäsar-Verschlüsselung ein interessantes Beispiel für die Anfänge der Kryptographie.

## Vigenère-Verschlüsselung

Die Vigenère-Verschlüsselung ist eine Methode der polyalphabetischen Substitution, die im 16. Jahrhundert von Blaise de Vigenère entwickelt wurde. Sie ist eine Erweiterung der einfachen Caesar-Verschlüsselung und bietet eine höhere Sicherheit durch die Verwendung eines Schlüsselwortes.

### **Funktionsweise der Vigenère-Verschlüsselung**

**Grundprinzip:**

- **Schlüsselwort:** Wähle ein Wort oder eine Phrase, das/die als Schlüssel dient. Dieses Schlüsselwort wird wiederholt, bis es die Länge des Klartextes erreicht.
- **Verschlüsselung:** Jeder Buchstabe im Klartext wird anhand einer Verschiebung verschlüsselt, die durch den entsprechenden Buchstaben im Schlüsselwort bestimmt wird. Diese Verschiebung ist vergleichbar mit der Caesar-Verschlüsselung, aber der Schlüssel ändert sich mit jedem Buchstaben.

**Beispiel:**

- Schlüsselwort: **`VIGENERE`**
- Klartext: **`HALLO`**
- Verschlüsselung:
    - Das Schlüsselwort wird über den Klartext geschrieben: **`VIGEN`**.
    - **`H`** (verschoben um **`V`**, also um 21 Stellen) wird zu **`C`**.
    - **`A`** (verschoben um **`I`**, also um 8 Stellen) wird zu **`I`**.
    - **`L`** (verschoben um **`G`**, also um 6 Stellen) wird zu **`R`**.
    - **`L`** (verschoben um **`E`**, also um 4 Stellen) wird zu **`P`**.
    - **`O`** (verschoben um **`N`**, also um 13 Stellen) wird zu **`X`**.
- Verschlüsselter Text: **`CIRPX`**

### **Entschlüsselung**

Die Entschlüsselung erfolgt durch die Umkehrung des Verschlüsselungsprozesses. Man nutzt das Schlüsselwort, um die Verschiebung rückgängig zu machen.

**Beispiel:**

- Verschlüsselter Text: **`CIRPX`**
- Schlüsselwort: **`VIGENERE`**
- Entschlüsselung:
    - **`C`** (zurückverschoben um **`V`**, also um 21 Stellen) wird zu **`H`**.
    - **`I`** (zurückverschoben um **`I`**, also um 8 Stellen) wird zu **`A`**.
    - **`R`** (zurückverschoben um **`G`**, also um 6 Stellen) wird zu **`L`**.
    - **`P`** (zurückverschoben um **`E`**, also um 4 Stellen) wird zu **`L`**.
    - **`X`** (zurückverschoben um **`N`**, also um 13 Stellen) wird zu **`O`**.
- Ursprünglicher Text: **`HALLO`**

### **Anwendung und Sicherheit**

- **Anwendung:** Die Vigenère-Verschlüsselung war bis zum Ende des 19. Jahrhunderts als "unbrechbar" bekannt und wurde für militärische und diplomatische Kommunikation verwendet.
- **Sicherheit:** Obwohl sicherer als die Caesar-Verschlüsselung, kann die Vigenère-Verschlüsselung durch moderne kryptanalytische Methoden, wie die Kasiski-Examination oder die Frequenzanalyse, gebrochen werden.

Die Vigenère-Verschlüsselung bleibt ein beliebtes Beispiel in der Lehre der Kryptographie und ist ein interessanter Einstiegspunkt in die Welt der Verschlüsselungsalgorithmen.