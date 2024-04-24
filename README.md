## AuD_Projekt_Team02

Ein Filmproduzent plant das Drehen von Szenen für einen Kinofilm, insbesondere soll festgelegt werden, an welchen Tagen welche Szenen gedreht werden. 


Dabei gilt:

**Szenen**
- $S$ ist die Menge der Szenene
- jede Szene $s$ hat einen gegebene Dauer $d(s)$ in Tagen

**Schauspieler**
- $A$ ist die Menge der Schauspieler
- $c(a)$ sind die Kosten von Schauspieler*in $a$ pro Tag
- $a(s)$ ist die Menge der Schauspieler, die für den Dreh von Szene $s$ benötigt werden

**Zu beachten:**
- ein*e Schauspieler*in bleibt von der ersten Szene, an der er/sie beteiligt ist, bis zur letzten Szene, an der er/sie beteiligt ist, am Drehort(und verursacht für die ganze Zeit Kosten)
- eine Szene wird immer am Stück gedreht


**Gesucht:** 
- eine Abfolge von Szenen, die Gesamtkosten für die Schauspieler*innen minimiert

### The format of the instances are;
*https://people.eng.unimelb.edu.au/pstuckey/talent/*

- Name of data file on the first line
- Number of scenes
- Number of actors
- For each actor a line of  1s and 0s 
	 - 1 indicating the scenes in which the actor appears,followed by the cost of the actor. 
- A line of  integers the duration of each scene

#### Example_film105:
```
film105.dat
18
8

0 0 0 1 1 1 0 1 1 0 0 0 1 0 1 0 0 0	10
1 1 0 0 0 0 0 0 0 0 1 1 1 0 0 0 1 0 	4
0 0 1 1 1 1 1 0 0 0 1 1 1 0 1 0 0 0 	5
0 0 0 0 0 0 0 0 0 0 0 0 0 1 0 0 1 0 	5
0 0 0 0 0 0 0 0 0 1 0 1 0 0 0 0 0 1 	5
0 0 1 1 0 1 0 0 1 1 0 0 1 0 1 1 0 1 	40
1 0 0 0 0 1 1 1 0 0 1 0 1 0 0 1 0 1 	4
0 0 0 1 0 0 1 0 0 1 0 1 0 1 0 0 0 1 	20

2 1 1 1 1 1 1 1 1 1 1 1 1 1 2 1 1 1 
```

#### Talent Scheduling Result for film105:
```
cost = 849;
s = [2,1,11,17,14,7,12,18,10,4,13,16,3,9,15,6,5,8];
```
### Vorgehen
Eine Klasse wurde erstellt, die Methoden(a.k.a. "Public Methods") der Klasse müssen ergänzt werden("_..."-Methoden sind für die Klasse essenziell und sollten nicht ständig verändert werden).

