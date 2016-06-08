name: titleslide
class: center, middle

# GIT en GitHub voor GEO

Rob van Loon

@rob_vl // http://github.com/borrob

---

# Inhoud

- Wie ?
- Wat ?
- Waarom ?
- Hoe ?

*TODO: voeg leuk plaatje toe*

---

# Wie ?

Wie ben ik ?

*TODO: voeg foto toe en een paar keywords over mijzelf*

--

Wie zijn jullie ?

- Voorstelronde

---

# Wat?

Wat gaan we in deze cursus doen?

--

- GIT
- GIT als versiebeheersysteem
- GIT als code delen *(of meer dan alleen code)* <-- zoals deze curus
- GIT om een bijdrage te leveren
	* code
	* tickets en bugreports

**TODO: ** aanvullen met de inhoud

---

# Wat ? - Wat is GIT ?

Versiebeheer

- bijhouden geschiedenis
- geschiedenis: wie heeft wat gedaan

--

commit

- kleinste, logische eenheid

--

branche

- verschillende versies van hetzelfde
- samenstellen releases

--

samenwerken

- gedistribueerd systeem
- groei van de code

---

# Voor wat ?

- source code

--

- setup scripts

--

- data conversies

--

- documenten

--

- boeken

--

    - [gitbook](https://www.gitbook.com)
    - [Read the docs](https://readthedocs.org)

---

# Alternatieven ?

- losse directories
- Mercurial, Subversion
- Source Safe, Team Foundation

---

# REPO

**Waar zit ik de code neer ? **

- lokaal
- gedeelde netwerkschijf
- GitHub
- GitLab
- Bitbucket
- codeCorner

---

# Gedistribueerd versiebeheer

- Repo
- Lokaal
- Push and pull

**TODO:** Brug: van push/pull naar techniek

---

# Repo

![fig 1](img/distributed_fig01.jpg)

TODO: fix center

---

# Fetch

![fig 2](img/distributed_fig02.jpg)

---

# Checkout

![fig 3](img/distributed_fig03.jpg)

---

# Branches

![fig 4](img/distributed_fig04.jpg)

---

# Stage en commit (1)

![fig 5](img/distributed_fig05.jpg)

---

# Stage en commit (2)

![fig 6](img/distributed_fig06.jpg)

---

# Commit van teamleden

![fig 7](img/distributed_fig07.jpg)

---

# Fetch

![fig 8](img/distributed_fig08.jpg)

---

# Merge

![fig 9](img/distributed_fig09.jpg)

---

# Push

![fig 10](img/distributed_fig10.jpg)

---

# Remotes- Origin: schrijfrechten

![fig 11](img/distributed_fig11.jpg)

---

# Remotes- Upstream: leesrechten

![fig 12](img/distributed_fig12.jpg)

---

# Github: fork en pull request

![fig 13](img/distributed_fig13.jpg)

---

class: center, middle

# Techniek

---

# Terminologie (a.k.a. talk the talk)

- branch (master, gh-pages, dev, release, hotfix)
- commit (sha)
- pull and push (origin, upstream)
- merge (cherrypick)
- remotes (distributed)
- tag
- log
- blame

---

# Branch

*Zelfde code, maar net even anders...*

- Gescheiden houden van OTAP straat.
- Snel en makkelijk schakelen (bijv. van implementatie feature naar bugfix)
- "Even wat uitproberen" zonder schade toe te brengen

---

# Commit

Kleinste, zelfstandige verandering

- werkende functie
- fix typo
- werkende unit-test

Commit: wegschrijven van de delta's ten opzichte van de vorige commit (dus ook verwijderen is toevoegen).

Elke commit krijgt een unieke sha (handig als referentie).

Denk ook aan het schrijven van een goede commit-message.

---

# Commit message

1e regel: Header / samenvatting

2e regel: Leeg

-e regel: Beschrijvende tekst

Schrijf een zinvolle commit-message (je bent jezelf later dankbaar).

---

# Vóór de commit

git diff <file> -- toont de wijzigingen in die file sinds de laatste commit


Voor wijzigingen in de hele repo:

    git status

---

# Push en pull

- Pull: geef mij de laatste versie van de repo en merge met mijn versie
- Push: mijn versie wegschrijven naar de server

Push alleen OK als gebasseerd op de laatste versie

*TODO:* brug maken: als niet laatste versie, dan mergen.

---

# Merge

Het samenvoegen van twee branches:
- bugfix in prod
- feature branch in dev

Maar ook:
- remote met locale versie

Let op: merge conflits

---

# Cherrypick

TODO: leuk plaatje

"Ik vind die ene commit in die andere branch wel leuk, maar de rest hoeft ik niet."

---

# Rebase / Squash

Please don't

--

Zoek de gemeenschappelijke voorouder en pas de delta's van de ene branch toe op de andere.

---

# Remotes

Origin: de originele repo (met schrijfrechten)

Upstream: de origele repo waar jij een clone van hebt gemaakt (zonder schrijfrechten)

---

# Tag

Als je door alle commits de bomen in het bos niet meer ziet: hang er een label aan.

Gebruik voor:
- aanwijzen release
- opgeven versienummer (git describe)

---

# Log

Geeft een overzicht van alle commits.

Opties:
- alle branches
- oneline of gehele commit-message
- grafiek

---

# Blame

Niet zo zeer om de schuld af te schuiven, maar wel goed om te achterhalen wie wat wanneer heeft gedaan.
---

class: center, middle

# Workflow

---

# Vanaf begin

1. git init
2. add .gitignore
3. bestanden toevoegen
4. git add .
5. git commit
6. [repeat]
7. git push
8. branch, merge, ...
9. tag
10. release

---

class: center, middle

# Cloud

---

# Voordelen

- open (als je wilt)
- delen
- samenwerken
- commit-hooks
- online editing
- issues en tickets
- overzicht branches, commits, merges

- readthedocs, gitbook

---

# Hosts

GitHub:
- www.github.com
- gh-pages
- erg populair

Bitbucket:
- www.bitbucket.com
- JIRA
- private repositories

GitLab:
- www.gitlab.com
- GitLab CE: open source
- host your own

...

---

class: center, middle

# Extra's

---

# Kanban / Scrum

- Visualiseer
- Deel met anderen
- Feedback

- backlog -> todo -> in progress -> test -> done
- In de cloud: vaak ingebouwd

---

# Issuetracker

- issues, bugs, wensen
- discussies

---

# Bugs

- wat gaat er precies mis
- wat is het verwachte resultaat, wat is het daadwerkelijke resultaat
- welke versie (en welke versie van OS, libraries, ...)
- minimale stappen om het te reproduceren
- foutmeldingen / logbestanden

---

class: center, middle

# GEO

---

# Git en GEO

Git is niet super met binary files --> geen shapes

--

Wél met tekstbestanden -- WKT, GML, GeoJSON

--

Alternatief: GeoGig: shp, geojson, geopkg, sl, sqlserver, oracle

---

# Github

Github ondersteunt geojson

    - leaflet
    - openstreetmap
    - WGS84

TODO: screenshot

---

class: center, middle

# Aan de slag

---

# Hands on (a.k.a walk the walk)

1. Installeer GIT
2. Clone een repo (deze ?)
3. Doe een aanpassing
4. Commit
5. Creeer een branch
6. Doe een aanpassing + commit
7. Merge
