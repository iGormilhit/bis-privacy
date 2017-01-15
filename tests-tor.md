# Tests Tor

**version `0.01`** (15.01.2017)

## Objectifs

Cette petite expérience a pour objectifs de voir si les catalogues de bibliothèques web déjà testés (HTTPS, mouchards) sont accessibles avec Tor Browser.

## Protocole de test

Les sites web ont été visités avec Tor Browser 6.0.8 (sur Mac OS X). Le navigateur se présente au serveur comme suit:   

`Mozilla/5.0 (Windows NT 6.1; rv:45.0) Gecko/20100101 Firefox/45.0`

En toute logique, [Whichbrowser](https://whichbrowser.net/) a considéré qu'il s'agit de Firefox 45 sur Windows 7.

## Résultats

Le tableau ci-dessous liste les résultats des tests.
   
### Bibliothèques académiques

| Site | accessible avec Tor Browser |
| :--- | :-------------------------: |
| OPAC RERO GE [1] | oui |
| RERO Explore GE [2] | oui |
| RenouVaud [3] | oui |
| OPAC NEBIS [4] | non |
| NEBIS Recherche [5] | oui |
| Wissensportal ETH [6] | oui |
| Rechercheportal ZB/UZH [7] | oui |
| BEAST [8] | oui |
| Swissbib [9] | oui |
| Swissbib Basel Bern [10] | oui |

**[1]** opac.rero.ch/gateway?skin=ge   
**[2]** explore.rero.ch/ge   
**[3]** sp.renouvaud.ch   
**[4]** http://opac.nebis.ch/F?local_base=nebis&func=option-update-lng&p_con_lng=FRE&file_name=find-b   
**[5]** recherche.nebis.ch   
**[6]** www.library.ethz.ch/en   
**[7]** www.recherche-portal.ch   
**[8]** library.epfl.ch/beast   
**[9]** www.swissbib.ch   
**[10]** baselbern.swissbib.ch   


### Bibliothèques publiques (scolaires + municipales)

| Site | accessible avec Tor Browser |
| :--- | :-------------------------: |
| BM Lausanne [101] | oui |
| BM Genève [102] | oui |
| BM Pully [103] | oui |
| Médiathèque [104] | oui |
| BM Morges [105] | oui |

**[101]** bavl.lausanne.ch/iguana/www.main.cls   
**[102]** collectionsbmu.ville-ge.ch   
**[103]** bibliotheque.pully.ch   
**[104]** www.mediatheque.ch   
**[105]** biblio.morges.ch   



--
*v0.01 - fichier créé le 15 janvier 2017*



