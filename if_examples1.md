1. Beispielaufgabe zur Überprüfung auf Geradheit einer Zahl:
   Schreibe ein C-Programm, das den Benutzer nach einer Ganzzahl fragt und überprüft, ob die eingegebene Zahl gerade ist. Wenn die Zahl gerade ist, gib "Die Zahl ist gerade" aus, ansonsten gib "Die Zahl ist ungerade" aus.

2. Beispielaufgabe zur Bewertung von Noten:
   Schreibe ein C-Programm, das die Benutzer nach einer Schulnote von 1 bis 6 fragt. Das Programm soll dann die entsprechende Beschreibung für die Note ausgeben. Zum Beispiel: "1 - Sehr gut", "2 - Gut", usw. Falls eine ungültige Note eingegeben wird, gib "Ungültige Note" aus.

3. Beispielaufgabe zur Überprüfung auf ein Schaltjahr:
   Schreibe ein C-Programm, das den Benutzer nach einer Jahreszahl fragt und überprüft, ob das eingegebene Jahr ein Schaltjahr ist. Gib "Schaltjahr" aus, wenn die Jahreszahl durch 4 teilbar ist und nicht durch 100, es sei denn, es ist durch 400 teilbar. Andernfalls gib "Kein Schaltjahr" aus.

4. Beispielaufgabe zur Überprüfung des größten Wertes:
   Entwickle ein C-Programm, das drei Ganzzahlen vom Benutzer einliest und dann den größten Wert unter den dreien ausgibt. Verwende `if`-Anweisungen, um die Vergleiche durchzuführen und den größten Wert zu ermitteln.


```c
#include <stdio.h>

int main() {
    float gewicht, kosten = 0;

    printf("Geben Sie das Gewicht des Pakets ein (in kg): ");
    scanf("%f", &gewicht);

    if (gewicht <= 0) {
        printf("Ungültiges Gewicht.\n");
    } else if (gewicht <= 1) {
        kosten = 3.5;
    } else if (gewicht <= 5) {
        kosten = 5.5;
    } else if (gewicht <= 10) {
        kosten = 8.5;
    } else {
        kosten = 10.5;
    }

    if (kosten > 0) {
        printf("Die Versandkosten betragen %.2f Euro.\n", kosten);
    }

    return 0;
}
```

Dieses Programm fragt den Benutzer nach dem Gewicht eines Pakets und berechnet dann die entsprechenden Versandkosten. Es werden `if`-Anweisungen verwendet, um das Gewicht zu überprüfen und die Versandkosten entsprechend festzulegen:

- Wenn das Gewicht unter oder gleich 1 kg ist, beträgt die Versandkosten 3,50 Euro.
- Wenn das Gewicht über 1 kg, aber höchstens 5 kg beträgt, beträgt die Versandkosten 5,50 Euro.
- Wenn das Gewicht über 5 kg, aber höchstens 10 kg beträgt, betragen die Versandkosten 8,50 Euro.
- Für Pakete über 10 kg betragen die Versandkosten 10,50 Euro.

Das Programm überprüft auch, ob das eingegebene Gewicht gültig ist, und gibt eine entsprechende Meldung aus, wenn das Gewicht ungültig ist.
