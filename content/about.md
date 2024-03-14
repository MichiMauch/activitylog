---
title: "About"
type: "about"
description: This is the about page
date: 2021-08-01T11:11:11+01:00
---

[English text below](#what-is-trekko)

# Was ist Trekko?

**Trekko ist unser privates Outdoor Journal. Die Aktivitäten-Seiten werden aus den Daten der GPX Files erstellt, welche wir bei den Aktivitäten aufgenommen haben. Und ja, natürlich verwendet man für solche Sachen Tools wie Strav oder ähnliche ;-)**

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

# What is Trekko?

**Trekko is our private outdoor journal. The activities pages are created from the data of the GPX files, which we recoreded on the tours. And yes, of course, tools like Strava or similar are used for such things ;-)**

## How was Trekko created?

The code for analyzing and calculating all the data in the GPX file was created with the help of ChatGPT and does not claim to be complete or accurate.
From the available data in the GPX file, description texts for the individual activities are also created with the help of the OpenAI ChatGPT API. The teaser images on the homepage and on the overview page are automatically generated with the DALL_E API (which is partly clearly visible :-)).

## Who created Trekko?

My name is Michi - www.michimauch.ch - and I had the idea for this small project. 99% of the code was created by ChatGPT. Just like all the explanations and instructions came from ChatGPT. I did not have to use Google even once for the creation of the project.

## Website

The website was created with the static website builder Hugo. The basic theme is AVA (https://github.com/jmau111/hugo-theme-ava) and was adapted and expanded by me or ChatGPT. The site is hosted on Github and accordingly also has its own repository. Of course, no database is used.

## GPX Handler

I developed the GPX Handler with GO, or the code was provided to me by ChatGPT. The GPX Handler is currently only running on my local device. Using a shell script, I can push the new files (for the Hugo website) to the corresponding Github repo and start building the Hugo page directly after uploading. The GPX Handler has its own repository on Github.
In the "backend" of the GPX Handler, the interface to ChatGPT and Dall_E can be activated or deactivated as desired. This helps to keep the API costs as low as possible. This is especially true during development.

## Nominate API by OpenStreetMap

Using the Nominate API and the corresponding coordinates from the GPX file, it was possible to read data such as location, canton, federal state, or even the country and publish it on the site.

## Map incl. Routes

The maps with the respective routes are created and displayed with the Leaflet plugin. The respective JSON files are also created with the GPX Handler. Additionally, a "total JSON" file is created. This should help when it comes to creating statistics from all the activities.

## Further Goals

In the near future, I would like to develop various statistics around the activities. Another goal would also be to dynamically load the municipal coats of arms of the starting and ending points via an interface (Wikipedia is only a small help).
