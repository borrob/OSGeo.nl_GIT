# Overview #

## Doel en publiek ##

Het doel van deze cursus is om geintresseerden een eerste kennismaking te geven met GIT (en GitHub). Het doelpubliek zijn mensen die wel te maken hebben met computer broncode en software, maar zelf geen programmeur zijn.

## Indeling slides ##

Hieronder staat een ruwe indeling voor de presentatie.

**INTRO**

Slide: Title slide

Slide: Inhoud

    - waar gaat deze cursus over
    - wat leer je / kun je na deze cursus

Slide: Voorstellen

Slide: Inhoud - specifieker

Slide: Wat is GIT

    - versiebeheer [vertel over hele rudimentair versiebeheer, belang van versiebeheer]
        * bijhouden geschiedenis / opbouw van versies
        * wie heeft wat gedaan [blame]
        * commit als logische eenheid
        * onderscheid via branches
        * samenstellen release
    - samenwerken
        * gedistribueerd systeem
        * groei van code zien

Slide: Alternatieven

    - losse directories
    - Mercurial, Subversion
    - Source Safe, Team Foundation

Slide: Voor wie en voor wat?

    - source code
    - setup scripts
    - data conversies
    - documenten
    - boeken? --> [gitbook](https://www.gitbook.com)

Slide: REPO

    - lokaal
    - gedeelde netwerkschijf
    - GitHub
    - GitLab
    - Bitbucket
    - codeCorner
    - ...
    - uitleg distributed versiebeheer (zometeen meer)
        - repo
        - lokaal

**TECHNIEK**

Slide: Termen (elk aparte slide)

    - branch (master, gh-pages, dev, release, hotfix)
    - commit (sha)
    - pull and push (origin, upstream)
    - merge (cherrypick)
    - tag
    - remotes

Slide: Hoe gebruiken

    - code
    - platte tekst
        - markdown
        - restructured text
        - latex
        - html

Slide: versiebeheer

    - bladeren door branches
    - bladeren door geschiedenis
        - mooie graph
    - blame

Slide: workflow

    - branching: [nvie](http://nvie.com/posts/a-successful-git-branching-model/)
    - not branching: [Dziuba](http://widgetsandshit.com/teddziuba/2011/12/process.html)

Slide: Cloud

    - Voordelen:
        - open
        - delen
        - samenwerken
        - commit-hooks
        - online editing
    - issues en tickets
    - overzicht branches, commits, merges
    - github & geo (werkt met geojson, of was het gml)
    - github met gh-pages
    - readthedocs, gitbook

Slide: Do/Dont

    - ...

...
*TODO: aanvullen*
...

Losse termen en ideeen:

- reference sha of ticket nummer --> automatische link
- branch structuur
- GUI vs CLI
- enkel aanvullingen (ook verwijderen is aanvullen)
- squash vs sausage making (merge en rebase)

# E-mails #

Van de OSGeo.nl lijst zijn een aantal suggestie binnen gekomen over de cursus. De belangrijkste punten:

- wat is versiebeheer en waarom is het belangrijk ?
- wat is GIT (en wat zijn de alternatieven) ?
- wat betekenen de termen: commit, branch, push, pull ?
- hoe gebruik je GitHub, GitLab, Bitbucket, … ?
- hoe kan ik GIT gebruiken ?
- hoe kan ik een bijdrage leveren aan open source projecten?
- hoe meld je een bug? Is de bug al een keer gemeld? Wat gebeurd er na het melden van een bug?
- GitHub samenwerkings-mogelijkheden, ook voor niet-programmeurs, bijv:
- documentatie en zelfs website en app-hosting via GH-pages, Jekyll, Readthedocs.org etc
- GH issue tracker als aktie/discussie-lijst
- Waar vind ik meer informatie?
