# Meilensteine in openATTIC

Die Evolution eines Projekts von "Bathwater" zu "Wide Open"

---

Lenz Grimmer | [@lenzgrimmer](https://twitter.com/lenzgrimmer)

Kieler Open Source und Linux Tage | 2018-09-14

Note:
* Entstehungsgeschichte eines Open Source Projekts
* Wachstum und Weiterentwicklung eines Teams
* Lose Sammlung von Anekdoten, Schlüsselereignissen, gesammelten Erfahrungen


# $ whoami

Note:
* Home Office seit 2002
* Der Vortrag wird viele Anglizismen enthalten


<!-- .slide: data-background-image="images/openattic-kielux-2015-youtube.png" data-background-size="contain" -->

Note:
* oA-Vortrag auf den Kieler Linuxtagen 2015
* Es ist viel passiert seitdem...


<!-- .slide: data-background-image="images/tweet-vom-2018-06-27.png" data-background-size="contain" -->

Note: 
* Warum dieser Vortrag? 
* Einladung von Felix Kronlage aufgrund dieses Tweets
* Begriffe aus Mozilla/Open Tech Strategies-Studie "Open Source Archetypes: A  Framework For Purposeful Open Source"



# 2010 - 2014
## (The early days)

Note:
* Entstehungsgeschichte openATTIC bei it-novum
* Vor meiner Zeit
* Hörensagen und Web-Archive


<!-- .slide: data-background-image="images/back-scratcher.jpg" data-background-size="contain" -->

Note:
* Dezember 2010: "Scratching an itch"
* it-novum als spin-off Dienstleister
* NetApp alternative, WebUI für Linux Storage-Services 


<!-- .slide: data-background-image="images/openattic-1.x.png" data-background-size="contain" -->

Note:
* Django, ExtJS UI
* XML-RPC API
* NFS, Samba, iSCSI, LVM, XFS
* Später ZFS & Btrfs, Snapshots, DRBD


<!-- .slide: data-background-image="images/openattic_community_blue.svg" data-background-size="contain" -->

Note:
* Enterprise/Community-Version
* Erste Kunden


<!-- .slide: data-background-image="images/openattic-code-einreichen-2014.png" data-background-size="contain" -->

Note:
* Duale Lizenz: CLA erforderlich (Harmony Agreements)
* Dedizierte Websites .com/.org
* User-zentrierte Community-Infrastruktur (Forum, IRC)
* Separate (teilw. interne) Mercurial repos f. Frontent, Backend, Tests
* Symbolfoto für den Projektnamen "Speicher -> Storage/Attic" 


<!-- .slide: data-background-image="images/openattic-support-options-2015-02.png" data-background-size="contain" -->

Note:
* Stand Anfang 2015: Enterprise/Community Edition
* DRBD, SnapApps, Ceph Support (nur für Enterprise Edition)


<!-- .slide: data-background-image="images/Ceph_Logo_Stacked_RGB_120411_fa.png" data-background-size="contain" -->

Note:
* 2014: Erste Ceph-Unterstützung (nur für Enterprise-Kunden)
* Frage: Wer weiß nicht, was Ceph ist? Kurze Erklärung
* Auf Ceph kommen wir später wieder zurück



# 2015
## Das Jahr der großen Veränderungen

Note:
* Juli 2015: Product Manager für openATTIC bei it-novum
* Home Office


<!-- .slide: data-background-image="images/leyre-labarga-700581-unsplash.jpg" data-background-size="contain" -->

Note:
* Öffnung des Projekts
* Zusammenführung aller Mercurial Repositories auf BitBucket
* Development/Stable Branches
* Neuer Release alle 5-6 Wochen
* Rotation des “Release Captain” 


<!-- .slide: data-background-image="images/Jira_Software@2x-blue.png" data-background-size="contain" -->

Note:
* Öffentliche JIRA-Instanz, import der vormals internen Issues
* Pull requests/reviews/approvals öffentlich auf BitBucket
* Jeder PR hat ein dazugehöriges JIRA-Issue


<!-- .slide: data-background-image="images/oa-2.0-dashboard.png" data-background-size="contain" -->

Note:
* openATTIC 2.0
* Neue UI mit AngularJS/Bootstrap statt ExtJS
* REST API statt XML-RPC
* Initial weniger Features als Vorgängerversion
* Status: "Rocket Ship To Mars"


<!-- .slide: data-background-image="images/openattic.svg" data-background-size="contain" -->

Note:
* Neues Logo
* Alle Komponenten unter GPL
* Neues Geschäftsmodell: Support Subscriptions statt Lizenzen
* OEM Business (Thomas-Krenn)



# 2016
## Noch mehr Veränderungen

Note:
* Neue Rolle: Team Lead & PM - schizophren?
* Erster neuer Team-Kollege im Home Office
* Mehr Kollaborationstools: Etherpad / Mumble / Google Group
* English Thursday


<!-- .slide: data-background-image="images/openATTIC-2.0-Storage_Dashboard.png" data-background-size="contain" -->

Note:
* April 2016: UI Redesign
* Notwendig wg. Lizenzproblemen mit einer Komponente


<!-- .slide: data-background-image="images/SUSE_Linux_GmbH_Logo.svg" data-background-size="contain" -->

Note:
* Feb 2016: Kooperation mit SUSE
* Gemeinsame Entwicklung von Ceph-Features für SES 4
* November 2016: Akquisition durch SUSE
* Team weiterhin in den Räumen bei it-novum
* Dezember 2016: SUSE Enterprise Storage 4



# 2017
## Wachstum

Note:
* Integration mit SUSE (Infrastruktur, neues Office)
* Weitere Kollegen stoßen hinzu
* Das Team wird international


<!-- .slide: data-background-image="images/Git-logo.svg" data-background-size="contain" -->

Note:
* Blog und Source Code wechseln von hg zu git
* Entwickler haben häufiger mehr Erfahrung mit git als hg
* Flexibleres Branch-Naming
* Branches können aus dem Repo gelöscht werden 
* Rebasing & Squashing
* Automatisches "Signed-off-by"


<!-- .slide: data-background-image="images/saltstack-logo.svg" data-background-size="contain" -->

Note:
* Exklusiver Focus auf Ceph in Version 3.0 
* Bestehende Architektur skaliert nicht
* Andere OSS-Projekte machen "traditionelles Storage Management" besser - openMediaVault
* Oktober 2017: SUSE Enterprise Storage 5 (SES 5)



<!-- .slide: data-background-image="images/fuse-brussels-273772-unsplash.jpg" data-background-size="contain" -->
# 2018
## Auf zu neuen Höhen


<!-- .slide: data-background-image="images/ceph-mgr-dashboard-healthpage-mimic.png" data-background-size="contain" -->

Note:
* openATTIC wird zum Upstream Ceph Manager Dashboard
* Prototyp als “Proof of Concept”
* Erster Meilenstein: Dashboard v1 ersetzen


<!-- .slide: data-background-image="images/nine-kopfer-578133-unsplash.jpg" data-background-size="contain" -->

Note:
* Juni 2018: Ceph "Mimic" mit Dashboard v2
* Ceph Projekt "Wide Open"
* Coopetition Red Hat / SUSE
* Grüne Wiese - Neuanfang basierend auf Erfahrungen
* Vollwertiger Ersatz für openATTIC mit Ceph "Nautilus" (2019)



<!-- .slide: data-background-image="images/roman-mager-59976-unsplash.jpg" data-background-size="contain" -->

Note:
* Weisheiten am Schluss
* Zuviele, um sie alle anzubringen


## It's a marathon, not a sprint

Note:
* Aufbau einer Community erfordert viel Zeit
* Besondere Pflege der "Early Adopter" und Contributors
* Hauptteil der Arbeit hängt am Core Team
* Unterstützung verschiedener Distributionen ist viel Arbeit


## OSS für Infrastruktur
* Gut: Subscriptions statt Lizenzen
* Branding and Customizing
* Schlecht: Dual Licensing & CLAs


## Offenheit & Transparenz FTW

Note:
* Public feature/issue tracking
* Bitbucket/Mercurial vs. github/git
* Code branches und Pull Requests (incl. reviews)
* Ausführliche commit-Messages m. Referenzen auf issues
* CHANGELOGs (inkl. Referenzen auf Issue-IDs)


## Perfekt ist der Feind von "Gut Genug"

Note:
* Kurze Release-Zyklen und Iterationen
* MVP
* Fail fast
* Funktionalität vor Feintuning


## Embrace Change

Note:
* Veränderungen und Kurskorrekturen sind wichtig und hilfreich
* Kommunikation mit dem Team wichtig


## Plane Zeit für Refactoring

Note:
* Wenn das Fundament bröckelig ist, kann man keinen Wolkenkratzer bauen
* Manchmal ist eine Lösung vielleicht nicht mehr die Richtige


## Alles (Code, Doku, Build-Scripts) in einem git-Repo

Note:
* Vereinfacht Arbeit mit Branches
* Reproducable builds (npm-Cache in git)
* Blog in git senkt die Hürde


### Documentation is like sex: when it is good, it is very, very good; and when it is bad, it is better than nothing

Note:
* Ausführliche Entwickler-Dokumentation
  * Aufbau einer Entwicklungsumgebung
  * Prozess zur Einreichung von Patches


# Vielen Dank!


# Image Credits
* Bear Claw Back scratcher by Ray B (CC BY 2.0) - https://www.flickr.com/photos/raybouk/8095552537/ 
* Open Sign by Leyre Labarga - https://unsplash.com/photos/lfyP9zTgUp0
* Office building in mist by Fuse Brussels - https://unsplash.com/photos/JI01fn0U7Cg
* Lighthouse by Nine Köpfer - https://unsplash.com/photos/7t7wRG90grg
* Formulas on an old blackboard by Roman Mager - https://unsplash.com/photos/5mZ_M06Fc9g
