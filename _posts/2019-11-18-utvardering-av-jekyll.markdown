---
layout: post
title:  "Utvärdering av Jekyll"
date:   2019-11-18 23:32:45 +0100
comments: true
categories: personal
---
## Kommentarer

Jag använde [Isso](https://posativ.org/isso/) för kommentarer. Jag hostar Isso temporärt på en VPS för denna examinationen. Det var lätt att modifiera Disqus-mallen som följer med Jekyll-temat att fungera.

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
