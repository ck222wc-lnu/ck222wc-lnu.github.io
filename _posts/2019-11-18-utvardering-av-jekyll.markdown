---
layout: post
title:  "Utvärdering av Jekyll"
date:   2019-11-18 23:32:45 +0100
comments: true
categories: personal
---
## Statiska generatorer

Statiska generatorer har både fördelar och nackdelar.

Fördelen är att statiska generatorer som Jekyll ger sidor som är enkla att lägga upp. För att jämföra Jekyll med Wordpress så kräver Wordpress PHP och SQL, medans Jekyll inte har några andra krav, det hade funkat på en version av Apache från 90-talet.

Nackdelen är att processen inte är lätt för 'vanliga' användare. Att sätta upp miljön för Jekyll med Docker gick inte på grund av något Ruby-fel som jag inte kunde lösa, så jag fick installera det manuellt.

## Kommentarer

Jag använde [Isso](https://posativ.org/isso/) för kommentarer. Jag hostar Isso temporärt på en VPS för denna examinationen. Det var lätt att modifiera Disqus-mallen som följer med Jekyll-temat att fungera.

## Open Graph

Open Graph är ett protokoll för metadata. Metadatan kan sedan användas av webbapplikationer för att visa t.ex. en bild och text för en URL.

Jekyll gör det mesta åt mig med SEO-taggen, men jag lade in en bild manuellt.

## Robotar

robots.txt är en fil som ligger i rooten på en webbserver. Filen innehåller information om vilka sidor som robotar (t.ex. spindlar) ska kolla på.

Mitt exempel är väldigt enkelt, jag ber alla robotar att inte kolla på min sida.

```
User-agent: *
Disallow: /
```

Ett mer avancerat exempel är [Wikipedias robots.txt](https://sv.wikipedia.org/robots.txt), med kommentarer och regler för speciella URL:er och robotar som belastar sidan ofta.

## Människor

humans.txt är också en fil i rooten på en webbserver. Denna filen innehåller information om personer som har gjort sidan och är inte till för att läsas av ett program.

Mitt exempel har bara mitt namn och land, samt grundläggande info om sidan. Du kan ha en mycket mer detaljerad fil med email och sociala medier, men jag vill inte få spam och jag gillar inte att ha personlig information på nätet...

```
/* AUTHOR */
Name: Carl
Location: Sweden

/* SITE */
Last update: 2019/11/19
Language: Swedish
Doctype: HTML 5
```
