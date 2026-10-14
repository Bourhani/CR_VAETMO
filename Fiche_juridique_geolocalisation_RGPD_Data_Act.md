# Fiche juridique : géolocalisation des véhicules des salariés, RGPD et Data Act

**Textes de référence**
- CNIL, fiche pratique *« La géolocalisation des véhicules des salariés »* (cnil.fr).
- Règlement (UE) 2016/679 du 27 avril 2016, dit **RGPD** : articles 4, 6 et 35.
- Règlement (UE) 2023/2854 du 13 décembre 2023, dit **Data Act** (règlement sur les données).
- Code du travail : articles L.1121-1 (proportionnalité), L.1222-4 (information préalable du salarié) et L.2312-38 (consultation du CSE).

---

## 1. La fiche CNIL : géolocalisation des véhicules des salariés

### 1.1 Le principe
Un employeur peut géolocaliser les véhicules qu'il met à disposition de ses salariés, **mais seulement pour des finalités précises et légitimes**. Le dispositif doit rester **proportionné** et ne doit **pas conduire à une surveillance permanente** du salarié (art. L.1121-1 du Code du travail).

### 1.2 Finalités admises
- **Suivre, justifier ou facturer** une prestation de transport de personnes ou de marchandises, ou une prestation de service liée à l'utilisation du véhicule (preuve d'intervention, par exemple).
- **Assurer la sécurité** du salarié, des marchandises ou des véhicules dont il a la charge (travailleur isolé, vol, etc.).
- **Mieux répartir les moyens** pour des prestations à réaliser en des lieux dispersés (interventions d'urgence, optimisation des tournées).
- **Contrôler le respect des règles d'utilisation du véhicule** définies par l'employeur.
- **Suivre le temps de travail, à titre subsidiaire seulement**, c'est-à-dire uniquement **s'il ne peut pas être réalisé par un autre moyen**, même moins efficace.

### 1.3 Usages interdits ou encadrés
- **Pas de contrôle permanent** du salarié.
- **Pas de contrôle des limitations de vitesse** au moyen de la géolocalisation.
- **Pas de suivi du temps de travail des salariés autonomes dans l'organisation de leurs déplacements**, comme les VRP ou les commerciaux (Cass. soc., 3 nov. 2011, n° 10-18.036 ; Cass. soc., 19 déc. 2018, n° 17-14.631).
- **Pas de géolocalisation en dehors du temps de travail** : le salarié doit pouvoir **désactiver** la collecte ou la transmission de sa position pendant ses pauses et ses trajets privés, quand l'usage personnel du véhicule est autorisé.
- **Pas de collecte de la position des représentants du personnel** lorsqu'ils exercent leur mandat.

### 1.4 Durées de conservation
| Finalité | Durée maximale |
|---|---|
| Principe général | **2 mois** |
| Optimisation des tournées, ou preuve des interventions quand elle ne peut pas être apportée autrement | **1 an** |
| Suivi du temps de travail (si admis) | **5 ans** |

### 1.5 Accès, information et formalités
- **Accès limité** aux seules personnes habilitées, selon leurs fonctions : responsable logistique, RH, direction, etc.
- **Information individuelle préalable** de chaque salarié (art. L.1222-4 du Code du travail et art. 13 du RGPD) : finalités, base légale, destinataires, durée de conservation, droits, possibilité de désactiver le dispositif.
- **Information et consultation du CSE** avant la mise en place (art. L.2312-38 du Code du travail).
- **Inscription au registre des traitements** (art. 30 du RGPD) et association du **délégué à la protection des données (DPO)**.
- **Analyse d'impact (AIPD)** à mener le plus souvent : voir la section 2.3.
- **Sécurité des données** : authentification, journalisation des accès, chiffrement.

> **Sanction en cas de non-respect :** la CNIL peut infliger une amende administrative (art. 83 du RGPD). Devant les prud'hommes, des données obtenues par un dispositif illicite peuvent être écartées comme preuve, ou rendre la sanction disciplinaire injustifiée.

---

## 2. Les articles clés du RGPD

### 2.1 Article 4 : les définitions
Ce sont les notions qui permettent de qualifier juridiquement la géolocalisation.

| Notion (art. 4) | Contenu | Application à la géolocalisation |
|---|---|---|
| **Donnée à caractère personnel** (4.1) | Toute information se rapportant à une personne physique identifiée ou identifiable, directement ou indirectement, notamment par référence à un identifiant tel que… **des données de localisation**. | La position d'un véhicule attribué à un salarié est une donnée personnelle. Le texte cite expressément les données de localisation. |
| **Traitement** (4.2) | Toute opération appliquée à des données : collecte, enregistrement, conservation, consultation, utilisation, etc. | La collecte des positions par le boîtier, leur stockage et leur consultation constituent un traitement. |
| **Profilage** (4.4) | Traitement automatisé visant à évaluer certains aspects d'une personne, notamment ses **déplacements**, son rendement ou son comportement. | Noter la conduite ou analyser les trajets d'un salarié peut constituer un profilage. |
| **Responsable du traitement** (4.7) | Celui qui détermine **les finalités et les moyens** du traitement. | L'**employeur**. |
| **Sous-traitant** (4.8) | Celui qui traite des données **pour le compte** du responsable. | Le **prestataire de télématique** ou de gestion de flotte (contrat obligatoire, art. 28). |
| **Consentement** (4.11) | Manifestation de volonté **libre**, spécifique, éclairée et univoque. | Dans une relation de travail, le consentement est rarement libre à cause du lien de subordination (voir art. 6). |
| **Violation de données** (4.12) | Atteinte à la sécurité entraînant destruction, perte, divulgation ou accès non autorisé. | Une fuite des historiques de trajets doit être notifiée à la CNIL sous 72 h (art. 33). |

### 2.2 Article 6 : la licéité du traitement
Un traitement n'est licite que s'il repose sur **l'une des six bases légales** :

| Base (art. 6.1) | Pertinence pour la géolocalisation des salariés |
|---|---|
| a) **Consentement** | **À éviter.** Le salarié n'est pas en position de refuser librement (lien de subordination), et il pourrait retirer son consentement à tout moment. |
| b) **Exécution d'un contrat** | Peu adaptée : la géolocalisation n'est généralement pas *nécessaire* à l'exécution du contrat de travail. |
| c) **Obligation légale** | Possible seulement si un texte impose le dispositif, par exemple le chronotachygraphe dans le transport routier. Ce n'est pas le cas d'un traceur GPS classique. |
| d) **Intérêts vitaux** | Exceptionnelle (urgence vitale). |
| e) **Mission d'intérêt public** | Réservée aux employeurs publics agissant dans le cadre de leurs missions. |
| f) **Intérêt légitime** | **C'est la base habituelle** pour un employeur privé : facturation, sécurité, organisation. Elle exige une **mise en balance** avec les droits et libertés des salariés, d'où les limites fixées par la CNIL (pas de surveillance permanente, désactivation possible, conservation limitée). Le salarié dispose d'un **droit d'opposition** (art. 21). |

Points complémentaires :
- **Art. 6.4** : une donnée collectée pour une finalité, par exemple la facturation, **ne peut pas être réutilisée** pour une finalité incompatible, comme sanctionner un salarié pour ses trajets, sans nouvelle analyse de compatibilité.
- **Art. 5** : la licéité s'ajoute aux principes de **limitation des finalités, de minimisation, de limitation de la conservation** et de **transparence**.
- **Art. 88** : les États membres peuvent prévoir des règles particulières pour le contexte de l'emploi. En France, ce sont notamment les dispositions du Code du travail citées plus haut.

### 2.3 Article 35 : l'analyse d'impact relative à la protection des données (AIPD)
- **Principe (35.1)** : le responsable mène une AIPD **avant** de mettre en œuvre un traitement **susceptible d'engendrer un risque élevé** pour les droits et libertés des personnes, en particulier en cas de nouvelles technologies.
- **Cas obligatoires (35.3)** : (a) évaluation systématique et approfondie, y compris par profilage, qui fonde des décisions produisant des effets juridiques ; (b) traitement à grande échelle de données sensibles ou relatives aux infractions ; (c) **surveillance systématique à grande échelle** d'une zone accessible au public.
- **Listes des autorités (35.4)** : la CNIL publie la liste des traitements pour lesquels une AIPD est requise. Elle y inclut les traitements de **surveillance constante de l'activité des employés**.
- **Critères du CEPD (lignes directrices WP248)** : une AIPD est en principe requise dès que **deux critères** sur neuf sont réunis. La géolocalisation des salariés en réunit généralement au moins deux : **surveillance systématique** et **personnes vulnérables** (les salariés, en position de dépendance). S'y ajoutent souvent des **données de localisation**, qui sont des données à caractère hautement personnel, et l'usage de **technologies innovantes**.
- **Contenu minimal (35.7)** : description du traitement et de ses finalités ; évaluation de sa **nécessité et de sa proportionnalité** ; évaluation des **risques** pour les salariés ; **mesures** prévues (désactivation hors temps de travail, durées de conservation, habilitations, chiffrement, etc.).
- **Acteurs** : avis du **DPO** (35.2), et si possible avis des personnes concernées ou de leurs représentants (35.9), par exemple le CSE.
- **Suite** : si le risque résiduel reste élevé, **consultation préalable de la CNIL** (art. 36).

**Conclusion pratique :** pour un dispositif de géolocalisation des véhicules des salariés, **l'AIPD doit être considérée comme nécessaire par défaut**. Si l'employeur décide de ne pas en faire, il doit le justifier et documenter cette décision.

---

## 3. Situer le Data Act (règlement (UE) 2023/2854)

### 3.1 Objet et calendrier
Le Data Act fait partie de la stratégie européenne pour les données. Il vise à **répartir équitablement la valeur des données** produites par les **produits connectés** (véhicules, machines, objets connectés) et les **services connexes**.

| Étape | Date |
|---|---|
| Entrée en vigueur | 11 janvier 2024 |
| Application générale (droits d'accès et de partage, etc.) | **12 septembre 2025** |
| Obligation de **conception** permettant l'accès direct aux données (art. 3.1) pour les produits mis sur le marché | **après le 12 septembre 2026** |

### 3.2 Principaux mécanismes
- **Accessibilité dès la conception (art. 3)** : les produits connectés doivent être conçus pour que les données générées par leur usage soient accessibles à l'utilisateur, si possible directement. Le vendeur doit informer l'utilisateur **avant** l'achat ou la location.
- **Droit d'accès de l'utilisateur (art. 4)** : l'utilisateur, c'est-à-dire le propriétaire du produit ou celui qui en a l'usage par contrat (locataire, crédit-bailleur), peut obtenir du **détenteur des données**, souvent le constructeur, les données générées par l'usage du produit. L'accès est **gratuit** et se fait dans un format structuré et lisible par machine.
- **Droit de partage avec un tiers (art. 5)** : l'utilisateur peut demander que ses données soient transmises à un tiers de son choix, par exemple un réparateur indépendant, un assureur ou un gestionnaire de flotte. Les grandes plateformes désignées « contrôleurs d'accès » sont exclues comme bénéficiaires.
- **Protection des secrets d'affaires** et interdiction de développer un **produit concurrent** à partir des données obtenues.
- **Conditions équitables entre entreprises** : mise à disposition dans des conditions équitables, raisonnables et non discriminatoires (FRAND), et protection des PME contre les **clauses contractuelles abusives** (art. 13).
- Autres volets : accès des **organismes publics** en cas de besoin exceptionnel, **changement de fournisseur de cloud** (*switching*), **interopérabilité**.

### 3.3 Articulation avec le RGPD
- **Le RGPD prime** : le Data Act s'applique **sans préjudice** du RGPD. En cas de conflit sur des données personnelles, c'est le RGPD qui l'emporte (art. 1.5 du Data Act).
- Le Data Act **ne crée pas de base légale** pour traiter des données personnelles. Lorsque l'utilisateur **n'est pas** la personne concernée, le détenteur ne peut lui transmettre des données personnelles que s'il existe une **base légale au titre de l'article 6 du RGPD** (art. 4.12 du Data Act). La même règle vaut pour un tiers destinataire.
- Les deux textes sont **complémentaires** : le RGPD protège la **personne** dont les données sont traitées, tandis que le Data Act organise **l'accès économique aux données des objets**, qu'elles soient personnelles ou non.

### 3.4 Application au cas de la flotte de véhicules

```
 Constructeur (détenteur des données)
        │  Data Act art. 4 / 5 : accès et partage
        ▼
 Entreprise propriétaire ou locataire de la flotte = « utilisateur » (Data Act)
        │                          = « responsable du traitement » (RGPD, art. 4.7)
        ▼
 Salarié conducteur = « personne concernée » (RGPD)
        → protégé par les art. 5, 6, 13, 21 et 35 du RGPD et par la fiche CNIL
```

- Grâce au Data Act, l'entreprise peut **obtenir du constructeur** les données de ses véhicules (kilométrage, consommation, codes de panne, et parfois **position GPS**) sans dépendre de l'offre télématique propriétaire du constructeur. Elle peut aussi les faire transmettre à son prestataire de gestion de flotte.
- Mais **dès que ces données permettent de localiser un salarié**, leur exploitation reste entièrement soumise au **RGPD** et aux **recommandations de la CNIL** : finalité légitime, intérêt légitime mis en balance, pas de surveillance permanente, désactivation hors temps de travail, conservation limitée, information des salariés et du CSE, AIPD.
- En pratique, le Data Act **élargit l'accès** aux données, mais il **n'élargit pas ce que l'employeur a le droit d'en faire**.

---

## 4. Synthèse

| Question | Texte applicable | Réponse |
|---|---|---|
| La position d'un véhicule de service est-elle une donnée personnelle ? | RGPD, art. 4.1 | **Oui**, les données de localisation sont expressément citées. |
| Sur quelle base l'employeur peut-il géolocaliser ? | RGPD, art. 6.1.f | En général l'**intérêt légitime**, et non le consentement. |
| Pour quoi faire ? | Fiche CNIL | Facturation et preuve, sécurité, organisation des interventions, règles d'utilisation, et temps de travail seulement à titre subsidiaire. |
| Qu'est-ce qui est interdit ? | Fiche CNIL, jurisprudence | Surveillance permanente, contrôle de la vitesse, suivi hors temps de travail, suivi des salariés autonomes, suivi des représentants du personnel pendant leur mandat. |
| Combien de temps conserver les données ? | Fiche CNIL | 2 mois en principe, 1 an ou 5 ans selon la finalité. |
| Faut-il une AIPD ? | RGPD, art. 35, liste CNIL, WP248 | **Oui en pratique** (surveillance systématique de salariés). |
| Qui peut accéder aux données brutes du véhicule ? | Data Act, art. 3 à 5 | L'**utilisateur** (propriétaire ou locataire de la flotte) et les tiers qu'il désigne. |
| Le Data Act autorise-t-il à suivre les salariés ? | Data Act, art. 1.5 et 4.12 | **Non** : le RGPD prime et une base légale de l'art. 6 reste nécessaire. |

---

### Sources
- CNIL, « La géolocalisation des véhicules des salariés » : https://www.cnil.fr/fr/la-geolocalisation-des-vehicules-des-salaries
- Règlement (UE) 2016/679 (RGPD), EUR-Lex : https://eur-lex.europa.eu/eli/reg/2016/679/oj
- Règlement (UE) 2023/2854 (Data Act), EUR-Lex : https://eur-lex.europa.eu/eli/reg/2023/2854/oj
- Groupe de travail « Article 29 » / CEPD, *Lignes directrices concernant l'analyse d'impact relative à la protection des données* (WP248 rév. 01, 2017).
- Cass. soc., 3 novembre 2011, n° 10-18.036 ; Cass. soc., 19 décembre 2018, n° 17-14.631.

*Ces informations sont à jour à la date de rédaction. Certains textes européens font l'objet de propositions de modification (notamment le paquet « omnibus numérique »). Vérifiez leur état d'avancement avant toute utilisation.*
