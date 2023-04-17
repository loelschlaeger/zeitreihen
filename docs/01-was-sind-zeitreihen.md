# Was sind Zeitreihen?





Eine *Zeitreihe* ist eine Abfolge von Beobachtungen über die Zeit. Zum Beispiel ist der Bitcoinpreis eine Zeitreihe:

<img src="01-was-sind-zeitreihen_files/figure-html/example-ts-births-1.png" width="672" />

Ein anderes Beispiel ist die Anzahl an Geburten in Deutschland:

<img src="01-was-sind-zeitreihen_files/figure-html/example-ts-bitcoin-1.png" width="672" />

Zwei wesentliche Unterschiede zwischen diesen Beispielen können wir hervorheben:

1. **Zeitabstände der Beobachtungen:** Die Beobachtungen können täglich oder monatlich sein, oder andere *Frequenzen* wie stündlich, quartalsweise oder jährlich aufweisen. Wenn die Beobachtungen in gleichmäßigen Abständen vorliegen (*äquidistant* sind), erleichtert das die Analyse.

2. **Struktur in der Zeitreihe:** Die untere Zeitreihe weist eine besondere Struktur auf, wir sehen sich wiederholende Muster. Konkret können wir vermuten, dass manche Monate besonders geburtenstark und andere eher geburtenschwach sind.^[Solche Muster finden wir leider nicht in Finanzzeitreihen, sonst wäre es ziemlich einfach, Kursbewegungen vorherzusagen. 😄]

Bei der Analyse einer Zeitreihe interessieren wir uns für

- den grundsätzlichen *Trend* (und *Änderungen* im Trend),

- *Saisonalitäten* (und andere Muster),

- Bereinigung von zufälligen *Störungen*,

- und natürlich *Prognosen* über den weiteren Verlauf.

::: {.rmdnote} 
Eine Zeitreihe notieren wir als $\{y_t\}_{t\in I}$, wobei $y_t$ die Beobachtung zum Zeitpunt $t$ ist und $I$ die Menge aller Zeitpunkte beschreibt. Wir konzentrieren uns auf endliche Mengen $I$ mit äquidistanten Elementen, daher können wir die Menge $I = \{1,2,\dots,T\}$ verwenden, wobei $T$ die Gesamtanzahl an Beobachtungen ist. 
:::
