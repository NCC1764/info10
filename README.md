<!--
author:   Dirk Koehler

email:    koehler.di@gykl.lernsax.de

version:  0.0.1

language: de

narrator: DE Deutsch Male

comment:  Informatik Klasse 10

link:     https://cdn.jsdelivr.net/chartist.js/latest/chartist.min.css

script:   https://cdn.jsdelivr.net/chartist.js/latest/chartist.min.js

translation: Deutsch  translations/German.md

mode: Presentation

dark: false

@style
.lia-effect__circle {
    display: none !important;
}

@media (min-width: 600px) {
    .newspaper {
        column-count: 2;
        column-gap: 40px;
        column-rule: 1px solid lightblue;
    }
}

h1, h2, h3, h4, h5, h6 {
    column-span: all;
    font-family: Arial, Helvetica, sans-serif;     
}

figurecaption {
    font-size: 0.8em;
    font-family: Arial, Helvetica, sans-serif;
    font-style: italic;
    font-weight: 600;
}

.kasten {
    background-color:rgba(162,67,8,0.8);    
    color:#FFFFFF;
    padding: 1em;
    margin: 1em 0em 1em 0em;
    border-radius:10px;    
    font-family: Arial, Helvetica, sans-serif;
    font-weight: 400;
}

.kasten0 {
    background-color:#399193;
    border-radius:10px;
    color:#FFFFFF;
    padding: 1em;
    font-family: Arial, Helvetica, sans-serif;
    font-weight:400;
}
.kasten1 {
    background-color:#A24308;
    border-radius:10px;
    color:#FFFFFF;
    padding: 1em;
    font-family: Arial, Helvetica, sans-serif;
    font-weight:400;
}

.cb {
    break-before: column;
}

.flexz { 
    display: flex; 
    justify-content: center; 
    align-items: center;
}

@end

@onload
window.LIA.settings.font_size = 2
@end
-->

# 1 Datenbanken

## 1.1 Datenbanken im Alltag

## 1.2 Datenbanken vs. Tabellenkalkulation

## 1.3 Definition

## 1.4 Modellierung

### 1.4.1 Grundbegriffe

### 1.4.2 ER-Modell

### 1.4.3. Transformation ER-Modell in Relationenmodell

> - Transformationsregeln erlauben das automatische Überführen des semantischen Modells (ER-Modell) ins Relationenmodell (Tabellen).
> - Wir nutzen 5 Regeln.

#### Regel 1

![Regel 1](./img/1-Regel.svg)<!-- style="width: 40%; padding:1em;" -->

<p class="kasten">
Jede Entitätsklasse wird in eine Relation (Tabelle) mit Primärschlüssel(n) transformiert.
</p>

![Regel 1](./img/r1.svg)<!-- style="width: 30%; padding:1em;" -->

#### Regel 2

![Regel 2](./img/2-Regel.svg)<!-- style="width: 40%; padding:1em;" -->

<p class="kasten">
Eine 1 : 1 Beziehung im ER – Modell wird umgesetzt, indem ein beliebiger Primärschlüssel einer Entitätsklasse zum Fremdschlüssel der anderen Entitätsklasse wird.
</p>

![Regel 2](./img/r2.svg)<!-- style="width: 40%; padding:1em;" -->

#### Regel 3

![Regel 3](./img/3-Regel.svg)<!-- style="width: 40%; padding:1em;" -->

<p class="kasten">
Eine 1 : n Beziehung wird so umgesetzt, dass der Primärschlüssel der 1-Entitätsklasse Fremdschlüssel der n-Entitätsklasse wird.
</p>

![Regel 3](./img/r3.svg)<!-- style="width: 40%; padding:1em;" -->

#### Regel 4

![Regel 4](./img/4-Regel.svg)<!-- style="width: 40%; padding:1em;" -->

<p class="kasten">
Jede m : n Beziehung im ER – Modell wird umgesetzt, indem eine zusätzliche Relation gebildet wird, welche die Primärschlüssel beider Entitätsklassen als Fremdschlüssel beinhaltet.
</p>

![Regel 4](./img/r4.svg)<!-- style="width: 30%; padding:1em;" -->

#### Regel 5

![Regel 5](./img/5-Regel.svg)<!-- style="width: 40%; padding:1em;" -->

<p class="kasten">
Jede beliebige Beziehung mit Beziehungsattribut wird ins Relationenmodell umgesetzt, indem eine zusätzliche Relation gebildet wird, welche die Primärschlüssel beider Entitätsklassen als Fremdschlüssel und die Beziehungsattribute beinhaltet.
</p>

![Regel 5](./img/r5.svg)<!-- style="width: 50%; padding:1em;" -->

## 1.5 Implementierung

## 1.6 Abfragen

# 2 Programmierung