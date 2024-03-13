---
title: "About"
type: "about"
description: This is the about page
date: 2021-08-01T11:11:11+01:00
---

# Was ist Trekko?

**Trekko ist unser privates Outdoor Journal. Die Aktivitäten-Seiten werden aus den Daten eines GPX Files erstellt. Und ja, natürlich verwendet man für solche Sachen Tools wie Strav oder ähnliche ;-)**

## Wie ist Trekko entstanden?

Der Code für die Analyse und Berechnung sämtlicher Daten im GPX File wurden mit Hilfe von ChatGPT erstellt und haben keinen Anspruch auf Vollständigkeit und Genauigkeit.
Aus den zur Verfügung stehenden Daten im GPX File werden, ebenfalls mit Hilfe der OpenAI ChatGPT API, Beschreibungstexte für die einzelnen Aktivitäten erstellt. Die Teaserbilder auf der Startseite, sowie auf der Übersichtsseite werden automatisch mit der DALL_E API generiert (was teilweise gut zu sehen ist :-)).

## Wer hat Trekko erstellt?

Mein Name ist Michi - www.michimauch.ch - und ich hatte die Idee zu diesem kleinen Projekt. 99% des Codes wurde von ChatGPT erstellt. So wie sämtliche Erklärungen und Anleitungen kamen von ChatGPT. Ich habe für die Erstellung des Projektes kein einziges mal auf Google zurück greifen müssen.

## Webseite

Die Webseite wurde mit dem Static Website Builder Hugo erstellt. Das grundlegende Theme ist AVA (https://github.com/jmau111/hugo-theme-ava) und wurde von mir bzw. ChatGPT angepasst und erweitert. Die Seite ist auf Github gehostet und hat dem entsprechend auch ein eigenes Repository. Es wird natürlich keine Datenbank verwendet.

## GPX Handler

Den GPX Handler habe ich mit GO entwickelt bzw. der Code hat mir ChatGPT zur Verfügung gestellt. Der GPX Handler läuft aktuell nur auf meinem lokalen Gerät. Mittels eines Shell-Scripts kann ich nach dem Upload die neuen Files (für die Hugo Webseite) ins entsprechende Github Repo pushen und direkt das Building der Hugo Seite starten. Der GPX Handler verfügt über ein eigenes Repository auf Github.
Im "Backend" des GPX Handlers können die Schnittstelle zu ChatGPT und Dall_E nach belieben aktiviert oder deaktiviert werden. Dies hilft die Kosten der API möglichst gering zu halten. Dies natürlich vor allem während der Entwicklung.

## Nominate API von OpenStreetMap

Mittels der Nominate API und den entsprechenden Koordinaten aus dem GPX File, war es möglich Daten wie Ort, Kanton, Bundesland oder auch das Land zu lesen und auf der Seite zu publizieren.

## Karte inkl. Routen

Die Karten mit den jeweiligen Routen werden mit dem Leaflet Plugin erstellt und dargestellt. Die jeweils dazu gehörigen JSON Files, werden ebenfalls mit dem GPX Handler erstellt. Zusätzlich wird noch ein "Gesamt JSON" File erstellt. Dies soll mal helfen, wenn es darum geht, Statistiken aus all den Aktivitäten zu erstellen.

## Weitere Ziele

In naher Zukunft möchte ich noch verschiedene Statistiken rund um die Aktivitäten entwickeln. Ein Ziel wäre ebenfalls noch, die Gemeindewappen der Start- und Endpunkte dynamisch und mittels einer Schnittstelle laden zu können (Wikipedia ist nur eine kleine Hilfe).
