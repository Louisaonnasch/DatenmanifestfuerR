---
title: "Mein Markdown Meilenstein"
author: "Louisa Onnasch"
date: "11/7/2021"
output: html_document
---

# Das erste Mal RMarkdown
## Meine Erafhrungen mit diesem Meilenstein 

Anfangs war ich etwas skeptisch R gegenüber, da ich von vielen Leuten gehört habe, dass die Lernkurve sehr steil ist und man schnell den Überblick verlieren *kann*. Doch nachdem ich mich ein bisschen in R reingefuchst habe, hat es mir schnell **Spaß** gemacht. Besonders erstaunlich fand ich, das RMarkdown sogar deutlich **leichter** ist, als z.B HTML. Ich bin sehr gespannt was noch alles auf uns zukommen wird und freue mich auf die neuen *Herausforderungen*. 

# Das habe ich bereits gelernt: 

* Wie ich R, RStudio und RMarkdown installiere 
* Wie ich R Pakete installiere und öffne
* Wie ich mit Chunks umgehe 

1. Wie ich eine neue Mardown Datei erstelle 
1. Wie ich meinen Text in RMarkdown layoute 
1. Wie ich eine Abbildng aus Github einfüge 


#Mein Datenmanifest: 






```{r Wie lange muss ich bis zur Rente arbeiten?} 
geburt <- 2001 # bitte Geburtsjahr eingeben [YYYY eingeben]
alter <- 2021 - geburt
# wir berechnen Ihr Alter im Jahr 2020 (für das gesamte Jahr)
alter

# Wir berechnen Ihr Rentenalter und gehen davon aus, dass Sie mit 69 in  Rente gehen können.
rentenalter <- geburt + 69
rentenalter

# Wir gehen davon aus, dass Sie in drei Jahren anfangen werden zu arbeiten.
arbeitsbeginn <- 2023
arbeitsjahre <- rentenalter - arbeitsbeginn

# Voila: wenn alles klappt, arbeiten Sie so lange.
arbeitsjahre

```
# Variablen im Reporting verwenden
## Variablen in Dokumente einbauen.
Wir können die Ergebnisse von Variablen direkt in unseren Report einbetten, wenn der codechunk zuvor ausgeführt wurde. Schauen Sie sich das Beispiel unten an und ersetzen Sie die letzte Variable davon. 

### Einsatz von dynamischen Variablen im Dokument
Ich bin im Jahr `r geburt` geboren und werde im Jahr 2021 `r alter` Jahre alt sein. Das bedeutet, dass ich wahrscheinlich `r arbeitsjahre` Jahre arbeiten darf. Wenn Sie mal nachdenken, wie das Leben vor `r arbeitsjahre` Jahren, also im Jahr `r 2021-arbeitsjahre` aussah (ohne Smartphone oder Netflix), dann kommt in den nächsten `47` Jahren ganz schön viel Veränderung auf mich zu!  

### Eine kleine Geschichte mit Text- und Zahlen-Variablen

Schreiben Sie eine  kleine Geschichte mit den Werten, die Sie in dieses Dokument einbauen. 

```{r Mini-Geschichte}
Rudi <- "dog"
Chilli <- "cat"
google_trefferanzahl <- 3847
```
