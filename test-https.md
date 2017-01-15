# Analyse du HTTPS

## Qu'est-ce que le HTTPS ?

Il s'agit d'une version sécurisée du protocole HTTP, d'où le HTTP**S**. Son implémentation n'est pas toujours des plus simple et le système des autorités de certifications posent certains problèmes. Enfin, les services informatiques en charge de la sécurité des réseaux des grandes institutions et des grandes entreprises ont souvent des pratiques qui amoindrissent grandement la sécurité de ce protocoles, et ce dans le but d'améliorer la sécurité de l'organisation elle-même.

Cela dit, le HTTPS reste à préféré au protocole en clair. Lorsque tout se passe bien, au moins les informations qui sont échangées entre l'utilisateur et le site web sont chiffrées, ce qui signifie que les intermédiaires qui sont en mesure d'intercepter le trafic HTTP, ne seront pas en mesure de lire les données échanges. Ces données comprennent vos identifiants et vos mots de passe.

Dans certains cas, les données échangées entre votre ordinateur et un serveur dépassent de loin ces simples informations. Les objets connectés envoient en général quantité de données à leur véritable propriétaire, à savoir l'entreprise qui vend le service. Il y a déjà eu des exemples de télévision connectée qui transportaient les données de leur client en clair via Internet. Il est arrivé que le logiciel [Adobe Digital Edition](https://en.wikipedia.org/wiki/Adobe_Digital_Editions "Article Wikipedia en anglais"), bien connu dans notre métier, le fasse également.

Une autre application du HTTPS, c'est qu'il permet, dans une certaine mesure, de s'assurer que le site web visité est bien celui qu'il prétend être. C'est une bonne protection contre le [phishing](https://fr.wikipedia.org/wiki/Hame%C3%A7onnage "Article wikipédia sur le phishing ou hameçonnage en bon français").

## Objectifs de l'analyse

Il s'agit d'abord simplement de vérifier dans quelle mesure les catalogues des bibliothèques offre ce genre de sécurité, tout particulièrement pour les fonctionnalités impliquant une connexion de la part des usagers.

Ensuite, il s'agit de vérifier la qualité de l'implémentation de ce protocole.

## Protocole de test

1. Accès par HTTP à la page d'accueil, et vérifier si l'utilisateur est redirigé.
2. Accès par HTTP à la page de connexion, et vérifier si une redirection existe.
3. Si la redirection n'existe pas, refaire les tests en accédant directement via HTTPS.
4. Lorsque le HTTPS est proposé, vérifier dans les outils d'analyse la note obtenu. On été utilisés :
   1. https://tls.imirhil.fr/
   2. https://www.ssllabs.com/

## Bibliothèques académiques

| Site | HTTPS global | Redirection globale | HTTPS pour la connexion | Redirection pour la connexion | Note imirhil | Note SSLlabs |
| :--- | :------------: | :------: | :--------: | :-------: | :------ | :---: |
| [OPAC RERO GE](http://opac.rero.ch/gateway?skin=ge) | Non | Non | Non | Non | NA | NA |
| [Explore GE](http://explore.rero.ch/primo_library/libweb/action/search.do?vid=GE_V1) | Non | Non | NA | NA | NA | NA |
| | | | | | | |
| | | | | | | |
| | | | | | | |
| | | | | | | |
| | | | | | | |
| | | | | | | |
| | | | | | | |
| | | | | | | |
