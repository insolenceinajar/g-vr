# G:VR RoadMap

## Inhalt
**Einführung**

**RoadMap: Essentials**
1. Die Welt / Statische Assets **[?%]**
1. Grafik **[?%]**
1. Der Spieler: Physik und Bewegung **[0%]**
1. Menü-Führung: GUI und FS **[0%]**
1. Entities
    1. Dynamische Objekte **[0%]**
    1. Interaction-System **[0%]**
    
**RoadMap: Non-Essentials**
1. Kampf-System **[0%]**
1. Dialog-System **[0%]**
1. Follower und Companions **[0%]**
1. Quest-Baum **[0%]**
1. Items: Inventare und Kisten **[0%]**
1. Stats: Fähigkeiten und andere Eigenschaften **[0%]**
1. Handels-System **[0%]**
1. Puzzel und interaktive Objekte **[0%]**
1. Spezielle Interaktionen (Magie) **[0%]**
    

## Einführung
Die RoadMap enthält die wichtigsten Teil-Pakete von G:VR. Einige der Pakete bauen aufeinander auf, deshalb beschreibt die Reihenfolge der RoadMap die Pakete in etwa in absteigender Wichtigkeit, aber sie dient vor allem der Orientierung, zumal sich manche der Pakete auch gegenseitig beeinflussen.
Als "***Essential***" gelten Teile, die für eine grundlegende Funktionalität unentbehrlich sind, während die "***Non-Essentials***" zwar auch teilweise aufeinander aufbauen (so ist zum Beispiel das Follower-System vom Kampf-System abhängig), aber keine notwendigen Elemente darstellen und sich im Zweifel leichter wieder entfernen ließen.

## RoadMap: Essentials
### 1. Die Welt / Statische Assets
Dieses Paket beinhaltet alle unbeweglichen Assets. Die Welt bildet die Grundlage aller Interaktionen, hat selbst nur ein Minimum an Skripten und interagiert mit dem Spieler und Entities nur durch Collision oder NavMeshes.
- Import der Welt
- Anpassung der Meshes unter Unity
- Materials und Textures
- ???

### 2. Grafik
- Statische Effekte (Partikel etc.)
- Idle-Animationen
- Shader (?)

### 3. Der Spieler: Physik und Bewegung
Dieses Paket enthält unter anderem:
- Bewegung durch Locomotion, Teleport, Snap/Smooth-Turning
- Leitern hochklettern
- Springen/Akrobatik
- Rennen (?)
- Item-Physik

### 5. Entities
#### 5.1 Dynamische Objekte
Hier werden in erster Linie alle beweglichen oder veränderlichen Objekte (Entitäten) ins Leben gerufen. Neben Mobs und NPCs sind das interaktive Objekte wie Türen, Kisten, Crafting-Stations, Betten oder auch Kurbeln. In Abstimmung mit Unterpunkt 5.2 sollten die Entities so vorbereitet werden, dass sie mit dem Interaction-System Hand-in-Hand gehen.
#### 5.2 Interaction-System
Das grundlegende Interaction-System, das den Spieler in Bezug zu Entities setzt. In Abstimmung mit Unterpunkt 5.1 erhält jede Entity (oder Gruppe von Entities) eigene Methoden, wenn mit ihnen interagiert wird.

## RoadMap: Non-Essentials
### 3. Follower und Companions
Hängt von Interaction-System, Kampf-System und Dialog-System ab.

### 9. Spezielle Interaktionen (Magie)
Spezielle Events, die nur sehr situativ vorkommen, vor allem durch Magie: Item-Teleport, Levitation, Verwandlung, etc.
