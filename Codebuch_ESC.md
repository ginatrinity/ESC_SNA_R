# Datensatz ESC Eurovision Song Contest #
Codebuch Stand 18.11.2025
erstellt von Gina Grad

## Ursprung und Datenerhebung
Die Daten stammen aus der offiziellen Website des ESC. Weitere Bestimmungen zu den Ländern: 

Das Netzwerk ist ein *gerichtetes one-mode Akteursnetzwerk*.

**Umgang mit fehlenden Werten**
Fehlende Werte werden nicht erfasst. Nicht "NA", stattdessen wird kein Wert eingetragen.

## Inhalt
- ESC_edges_final_1.csv (Edgelist)
- ESC_nodes_final.csv (Nodelist)

## Vertex-Attribute

**id**  
Abkürzung des Landes nach ISO (ISO 3166-1 alpha2) (bsp.: DE) siehe Nodelist

**name**
Landname deutsch

**region**
1 - 10, Falls in bestimmter Region Zugehörigkeit zu anderen Ländern besteht (bsp.: 1)
1 = Nordeuropa
2 = Zentraleuropa
3 = Westeuropa
4 = Südeuropa
5 = Südosteuropa
6 = Osteuropa
7 = Europa und Asien (Schnittstellen)
8 = Asien
9 = Australien 
10 = Afrika 


## Edge-Attribute

**from**  
ID des Knotens Land (bsp.: DE) -> Land gibt Punkte an, Land stimmt für

**to**
ID des Knotens Land (bsp.: DE) -> Land bekommt Punkte

**weight**
Punkteverteilung Gesamt von 1975 bis 2015 und Punkteverteilung der Jury von 2016 bis 2025 des ESC (1 = 1 Punkt, 2 = 2 Punkte, [...] 12 = 12 Punkte) 

**year**    
2025 als Jahr

**neighbor**
1 = Ja, es ist ein Nachbarland, 2 = Nein

##