Title: Curry Generator 1
Category: Programming
Lang: de
Date: 2017-01-25
Tags: elm, random, curry, functional programming
Status: draft

__Achtung:__ Lass diesen Artikel ruhig aus, wenn du lieber etwas mit Substanz liest, und nicht so gerne Meta Gerede.

# Curry ist was Feines

## Das Buch
Kurz nachdem mein Kollege und guter Freund [Gregor](www.gregor.codes) mir die funktionale Programmierung näher gebracht hatte, war ich auf der Suche nach einem guten Buch als Überblick über das Thema. Meine Wahl fiel auf das [Curry Buch](http://currybuch.de/) von Stefanie Schirmer, Hannes Mehnert und Jens Ohlig, ich bin nicht mehr sicher wie ich darauf kam. Aber es ist ein sehr schönes Buch, kurzweilig und voller interessanter Informationen. Manches schien mir etwas zu akademisch, um mir als Einstieg zu helfen; aber etwas Neues zu lernen, ohne das man es direkt anwenden kann ist in meiner Welt nichts Schlechtes! Und nachdem ich zwei der Autoren letztes Jahr bei der [Bobkonf](http://bobkonf.de/2016/en/) getroffen habe, weiß ich auch, dass deren Wissen über Curry sicherlich genau so fundiert ist, wie das über Programmierung.

## Der Generator
Aber darum geht es eigentlich gar nicht. Als Einstieg in ihr Buch stellen die Autoren einen Curry Generator vor, der aus einer Reihe Zutaten zufällige Curry Rezepte generieren kann, die vermutlich sogar alle schmecken (ich konnte noch nicht alle testen...). Da das Programm so schön schlicht, aber doch erweiterbar ist, wählte ich es als meinen ersten Spielplatz um [Elm](http://elm-lang.org/) näher kennen zu lernen. In erster Fassung sollten nur die Rezepte generiert werden. Als weiteres Feature konnte man sich Rezepte merken, allerdings nur während der Session. Man hat reichlich Bedarf an Zufälligkeit; noch ein Grund, dass sich das Projekt als Einsteig in die funktionale Programmierung eignet, oder in diesem Fall als Sprung und dunkles, verwirrendes Wasser.

## Zufälligkeit in _purely functional languages_
Was mir vorher nicht so klar war: Wenn man eine Sprache nutzt, in der Seiteneffekte so weit es geht aus dem Weg genommen und an den Rand des Programms geschoben werden (eines der Kernfeatures, die ich an Elm liebe), dann ist das gar nicht so einfach etwas Zufälliges zu bekommen. Wenn mein Programm vornehmlich auf _pure functions_ basiert, will ich ja, dass immer etwas Erwartetes passiert, nichts Unerwartetes. Das war der erste _mind bender_, der mir zeigte, wie grundlegend anders ich lernen muss zu denken.

## Aktueller Stand
Hier ist übrigens der [Curry Generator](playground/curry). Was du hier siehst ist allerdings noch in Elm 0.16 geschrieben. Damals gab es ein schönes community package, mit dem man Listen mischen konnte; sehr praktisch für meine Zwecke. Da sich seit dem allerdings einiges an der Handhabung von Zufallszahlen in Elm getan hat, war die Portierung zu aktuellen Versionen zu aufwändig. Das werde ich aber in nächster Zeit mal nachholen. Mehr dazu in Kürze.