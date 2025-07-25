---
title: "Erster Beitrag: Eine Anleitung zum Aufbau von 'Wandernder Gezeitensammler'"
date: 2024-07-25T11:00:00+08:00
categories: ["hugo"]
tags: ["hugo"]
summary: "Dies ist nicht nur der erste Beitrag auf dieser Seite, sondern auch ein lebendiges Dokument darüber, wie man neue Beiträge und Bilder hinzufügt – ein Plan für unseren zukünftigen kreativen Arbeitsablauf."
draft: false
---

Hallo, mein zukünftiges Ich, und alle Freunde, die hier zufällig vorbeischauen.

Willkommen am Anfang von „Wandernder Gezeitensammler“. Dieser Raum ist als ein Korb gedacht, um die „Muscheln“ und „Sterne“ aufzubewahren, die ich an den Ufern des Wissens und der Informationen aufsammle. Heute lege ich die erste sorgfältig ausgewählte Muschel hinein – eine Anleitung, wie man hier Inhalte erstellt.

Dieser Beitrag dient sowohl als Erinnerung als auch als Bedienungsanleitung, um sicherzustellen, dass jede zukünftige Schöpfung klar und effizient ist.

## I. Der Ausgangspunkt: Ein einziger Befehl

Wir erstellen Dateien nicht manuell. Stattdessen verwenden wir das elegante Kommandozeilen-Tool von HUGO. Es ist wie ein Zauberstab, der alles für uns vorbereitet.

Öffne dein Terminal, navigiere zum Stammverzeichnis des Blogs und sprich den Zauberspruch aus:

```bash
# Format: hugo new inhaltstyp/JJJJ/MM/dein-beitrags-slug/index.sprache.md
hugo new posts/2024/07/a-new-journey/index.de.md
```

Dieser Befehl vollbringt ein kleines Wunder:

1.  Er erstellt einen Ordner namens `a-new-journey` im Verzeichnis `content/posts/2024/07/`.
2.  In diesem Ordner erstellt er eine Datei `index.de.md`.
3.  Er füllt diese Datei automatisch mit „Identitätsinformationen“ (dem Front Matter), einschließlich Titel, Datum und einem entscheidenden Flag: `draft: true`. Dieses Flag markiert ihn als Entwurf, der in lokalen Vorschauen sichtbar, aber bei der endgültigen Bereitstellung ignoriert wird, was sehr sicher ist.

Wenn wir mit dem Schreiben fertig und bereit sind, es der Welt zu zeigen, ändern wir einfach `draft: true` in `draft: false`.

## II. Ihm eine Seele geben: Worte und Bilder

Ein vollständiger Artikel besteht aus Text und Bildern. In unserer gut durchdachten Struktur wird ihre Verwaltung unglaublich einfach.

### 1. Worte

Unter den „Identitätsinformationen“ der Datei befindet sich der Ort, an dem wir unseren Worten freien Lauf lassen. Hier folgt man der Standard-Markdown-Syntax – prägnant und leistungsstark.

### 2. Bilder: Ein Ende des Chaos

Das ist der schönste Teil unseres Arbeitsablaufs. **Jeder Artikel hat seinen eigenen dedizierten Ordner**, was bedeutet, dass alle im Artikel verwendeten Bilder direkt neben dem Artikel selbst gespeichert werden können!

Nehmen wir an, wir schreiben diesen `a-new-journey`-Beitrag. Seine Verzeichnisstruktur sieht so aus:

```
content/
└── posts/
    └── 2024/
        └── 07/
            └── a-new-journey/          <-- Der dedizierte Ordner des Artikels
                ├── index.de.md         <-- Die Artikeldatei selbst
                └── journey-start.jpg   <-- Das zugehörige Bild!
```

**Wie verweist man auf dieses Bild?**

In deiner `index.de.md`-Datei musst du nur Folgendes schreiben, ohne komplexe Pfade:

```markdown
![Der Beginn der Reise](journey-start.jpg)
```

![Der Beginn der Reise](journey-start.jpg)

So einfach ist das! Bild und Text sind elegant „gebündelt“, was Migration, Sicherung und Verwaltung zu einer sorgenfreien Erfahrung macht.

## III. Der „Personalausweis“ des Artikels: Front Matter

Der Bereich am Anfang jedes Artikels, umschlossen von `---`, sind seine Metadaten. Sie bestimmen, wie der Artikel kategorisiert und angezeigt wird.

-   **`title`**: Der Titel des Artikels.
-   **`date`**: Das Veröffentlichungsdatum, das seine Position in den Archiven bestimmt.
-   **`categories`**: Die Kategorie, normalerweise eine einzelne, breite Klassifizierung wie `["Technische Notizen"]` oder `["Lebensreflexionen"]`.
-   **`tags`**: Die Tags, von denen es mehrere geben kann und die für eine feinere Indexierung verwendet werden, wie `["Go", "Web", "Leistungsoptimierung"]`.
-   **`summary`**:Eine kurze Zusammenfassung, die auf der Artikellistenseite angezeigt wird.
-   **`draft`**: `false` bedeutet, der Artikel ist veröffentlicht; `true` bedeutet, er ist ein Entwurf.

Das sorgfältige Ausfüllen dieser Informationen hält unsere Wissensdatenbank sauber und organisiert.

## Fazit

Der kreative Prozess sollte eine Freude sein, keine Last.

Die Reise mit `hugo new` beginnen, Worte und Bilder in ihrem dedizierten Ordner platzieren und schließlich den `draft`-Staub abwischen. Das ist das ganze Geheimnis, um jede Entdeckung hier bei „Wandernder Gezeitensammler“ festzuhalten.

Möge dieser kleine Korb mit jedem Tag voller werden.