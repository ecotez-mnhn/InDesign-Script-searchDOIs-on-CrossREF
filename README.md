# InDesign-Script-searchDOIs-on-CrossREF
That script "reads" the bibliography of your publication and add DOI (for Digital Object Identifier) to each entry

—————————————————————————————————————————————————————————————————————————————————————————————————————————————————————————————————
## searchDOIs.jsx | Auteur : Emmanuel Côtez (emmanuel.cotez@mnhn.fr / emmanuel.cotez@teznet.fr) | https://github.com/ecotez-mnhn ##
—————————————————————————————————————————————————————————————————————————————————————————————————————————————————————————————————

Version : 1.04

Works with Adobe InDesign CC

———————————————————————————————————————————————————————————————————————————————————————————————

[FR]
Script d'ajout automatique des DOI aux entrées de la bibliographie via l'API fournie par CrossREF.

- Le programme nécessite de sélection un style de paragraphe (Journaux du Muséum, EJT, Mémoires du Muséum ou "Other") et analyse ensuite le contenu de chaque entrée de bibliographie (qui doit être dans un unique paragraphe), en extrait les données et les envoie à CrossREF pour récupérer le DOI correspondant, s'il existe.
- Les DOIs ajoutés sont automatiquement liés et stylés en style "Lien hypertexte" ; si un DOI existe déjà, le lien existant est supprimé et recréé ;
- Les entrées bibliographiques non trouvées apparaissent soulignées en vert, et celles dont les données n'ont pas pu être extraites soulignées en rouge ;
- Les couleurs et le style de caractère sont automatiquement créés s'ils n'existent pas ;
- L'entrée "Other" permet de sélectionner un style de paragraphe personnalisé pour les références ; les expressions régulières permettant d'extraire les données sont configurables ci-dessous.
 
Dépendances :
- collator.jsxinc
- extendables/extendables.jsx
- getURLs.jsx
- functionsEc.js
———————————————————————————————————————————————————————————————————————————————————————————————

[EN]
Script for automatically adding DOIs to bibliography entries via the API provided by CrossREF.

The program requires you to select a paragraph style (Journals of the Museum, EJT, Memoirs of the Museum or Other) and then analyses the content of each bibliography entry (which must be in a single paragraph), extract the data and send them to CrossREF and get back the DOI if exists.
- DOIs added are automatically linked and styled in "Lien hypertexte" character style; if a DOI already exists, the existing link is deleted and recreated;
- Bibliographic entries not found appear underlined in green, and those from which data could not be extracted underlined in red;
- Colours and character style are automatically created if they do not exist;
- The "Other" entry allows the selection of a personalised paragraph style for the references; regular expressions allowing the data to be extracted can be configured below.

Dependencies:
collator.jsxinc
extendables/extendables.jsx
getURLs.jsx
functionsEc.js
