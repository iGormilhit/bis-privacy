# Tests de tracking

## Objectifs

Cette petite expérience a pour objectifs de:

1. comparer Privacy Badger, Ghostery et Disconnect
2. tester les mouchards rencontrés sur les sites et catalogues de bibliothèques (en Suisse romande)

## Protocole de test

Les modules ont été testés l'un après l'autre (les autres étant désactivés). Une fois les 3 modules testés, l'expérience a été reconduite avec Lightbeam pour avoir un élément de comparaison (ce dernier, contrairement aux 3 autres, n'étant pas destiné à bloquer les mouchards, seulement à les lister).

## Comparaison de Privacy Badger, Ghostery et Disconnect

Le tableau ci-dessous liste le nombre de mouchards détectés par ces 3 modules + Lightbeam.
   
*Bonus: vérification que la connexion à ces sites se fait (automatiquement) en HTTPS*   
(**auto** = HTTPS supporté et automatique | **oui** = HTTPS supporté mais pas automatique | **non** = HTTPS non supporté)

**Bibliothèques académiques**

| Site | Privacy Badger | Ghostery | Disconnect | Lightbeam | détails | *HTTPS* |
| :--- | :------------: | :------: | :--------: | :-------: | :------ | :---: |
| OPAC RERO GE [1] | 2 | 0 | 0 | 2 | ajax.googleapis.com, cdn.jquerytools.org | *non* |
| RERO Explore GE [2] | 4 | 1 * | 1 * | 1 * | fonts.googleapis.com, fonts.gstatic.com, cdn.jquerytools.org, www.google-analytics.com * | *non* |
| RenouVaud [3] | 0 | 0 | 0 | 0 |  | *oui* |
| OPAC NEBIS [4] | 0 | 0 | 0 | 0 |  | *non* |
| NEBIS Recherche [5] | 1 | 0 | 0 | 1 | www.library.ethz.ch | *non* |
| Wissensportal ETH [6] | 2 | 0 | 0 | 0 | fonts.googleapis.com, fonts.gstatic.com | *oui [a]* |
| Rechercheportal ZB/UZH [7] | 2 | 0 | 0 | 0 | www.library.ethz.ch, www.hbz.uzh.ch | *non* |
| BEAST [8] | 5 | 1 * | 1 * | 2 ** | actu.epfl.ch, jahia-prod.epfl.ch, library.epfl.ch, www.epfl.ch **, www.google-analytics.com * ** | *oui [a]* |
| Swissbib [9] | 4 | 2 * | 2 * | 1 *** | fonts.googleapis.com, fonts.gstatic.com, by2.uservoice.com **, widget.uservoice.com * ** ***, Piwik * | *auto* |
| Swissbib Basel Bern [10] | 5 | 2 * | 2 ** | 2 *** | fonts.googleapis.com, fonts.gstatic.com, by2.uservoice.com **, widget.uservoice.com * ** ***, eu.libraryh3lp.com ***, Piwik * | *auto* |

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

**[a]** ne fournit aucune information au sujet de son identité (pas de certificat SSL?)

**Bibliothèques publiques (scolaires + municipales)**

| Site | Privacy Badger | Ghostery | Disconnect | Lightbeam | détails | *HTTPS* |
| :--- | :------------: | :------: | :--------: | :-------: | :------ | :---: |
| BM Lausanne [101] | 11 | 3 * | 55 [b] | 8 ** | s7.addthis.com * **, m.addthis.com, cdnjs.cloudflare.com **, www.dartfish.tv **, googleads.g.doubleclick.net * **, static.doubleclick.net, www.google.com, fonts.gstatic.com, www.youtube.com, i.ytimg.com, s.ytimg.com, images.amazon.com **, mediaeurope.dartfish.com, multimedia.fnac.com **, ssl.google-analytics.com, www.google-analytics.com * **, Youtube ** | *auto* |
| BM Genève [102] | 0 | 0 | 0 | 0 |  | *auto* |
| BM Pully [103] | 5 | 2 * | 2 * | 5 ** | stats.g.doubleclick.net **, staticxx.facebook.com, www.facebook.com **, marketplace.archimed.fr **, connect.facebook.net *, Google Analytics * **, images-amazon.com ** | *non* |
| Médiathèque [104] | 5 | 2 * | 8 ** | 3 *** | ajax.googleapis.com *, cse.google.com, www.google.com ***, www.google-analytics.com * ***, www.googleapis.com ***, Google ** | *non* |
| BM Morges [105] | 2 | 0 | 0 | 0 | www.meteoblue.com, www.doc-alain.com | *non* |

**[b]** 10 Google, 44 Amazon, 1 AddThis

**[101]** bavl.lausanne.ch/iguana/www.main.cls
**[102]** collectionsbmu.ville-ge.ch
**[103]** bibliotheque.pully.ch
**[104]** www.mediatheque.ch
**[105]** biblio.morges.ch




* v0.01 - fichier mis à jour le 31 décembre 2016*



