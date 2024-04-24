## AuD_Projekt_Team02

### The format of the instances are;

- Name of data file on the first line
- Number of scenes
- Number of actors
- For each actor a line of  1s and 0s 
	 - 1 indicating the scenes in which the actor appears,followed by the cost of the actor. 
- A line of  integers the duration of each scene

#### Example_105:
'''
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
'''
