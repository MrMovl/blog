Title: Curry Generator
Category: Programming
Lang: de
Date: 2017-01-25
Tags: rambling, elm, random, curry, functional programming

# Curry ist was Feines
http://currybuch.de/
## Das Buch
Kurz nachdem mein Kollege und Freund [Gregor](www.gregor.codes) mir die funktionale Programmierung näher gebracht hatte, war ich auf der Suche nach einem netten Buch als Überblick über das Thema. Meine Wahl fiel auf das Curry Buch von Mehnert et al, ich bin nicht mehr sicher warum. Aber es ist ein sehr schönes Buch, kurzweilig und voller interessanter Informationen. Manches schien mir etwas zu akademisch um mir als Einstieg zu helfen, aber etwas Neues zu lernen, ohne das man es direkt anwenden kann ist in meiner Welt nichts Schlechtes! Und nachdem ich zwei der Autoren letztes Jahr bei der [Bobkonf]() getroffen habe, weiß ich auch, dass deren Wissen über Curry sicherlich genau so fundiert ist wie das über Programmierung.

## Der Generator
Aber darum geht es eigentlich gar nicht. Als Einstieg in ihr Buch stellen die Autoren einen Curry Generator vor, der aus einer Reihe Zutaten zufällige Curry Rezepte generieren kann, die vermutlich sogar alle schmecken (ich konnte noch nicht alle testen...). Da das Program so schön schlicht, aber doch erweiterbar ist, wählte ich es als meinen ersten Spielplatz und [Elm]() näher kennen zu lernen. In erster Fassung sollten nur die Rezepte generiert werden. Als weiteres Feature konnte man sich Rezepte merken, allerdings nur während der Session. Man hat reichlich Bedarf an Zufälligkeit; noch ein Grund, dass sich das Projekt als Einsteig in die funktionale Programmierung eignet, oder in diesem Fall als Sprung und dunkles, verwirrendes Wasser.

## Zufälligkeit in _purely functional languages_
Was mir vorher nicht so klar war: Wenn man eine Sprache nutzt, in der Seiteneffekte so weit es geht aus dem Weg genommen und an den Rand des Programs geschoben werden (eines der Kernfeatures, die ich an Elm liebe), dann ist das gar nicht so einfach etwas zufälliges zu bekommen. Wenn mein Programm vornehmlich auf _pure functions_ basiert, will ich ja, dass immer etwas erwartetes passiert, nichts unerwartetes. Das war der erste _mind bender_, der mir zeigte, wie grundlegend anders ich lernen muss zu denken.

## Aktueller Stand
Hier ist übrigens der [Curry Generator](playground/curry). Was du hier siehst ist allerdings noch in Elm 0.16 geschrieben. Damals gab es ein schönes community package, mit dem man Listen mischen konnte; sehr praktisch für meine Zwecke. Da sich seit dem allerdings einiges an der Handhabung von Zufallszahlen in Elm getan hat, war die portierung zu aktuellen Versionen zu aufwändig. Das werde ich aber in nächster zeit mal nachholen. Mehr dazu in Kürze.