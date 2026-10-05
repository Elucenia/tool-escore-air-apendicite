<!-- ELUCENIA technical documentation · escore-air-apendicite · fr · no clinical/professional/rights approval -->

# Score AIR (réponse inflammatoire de l’appendicite)

[conditions, sources et autorisations](https://elucenia.org/fr/outils/escore-air-apendicite)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Vomissements

`vomito`

### Douleur de la fosse iliaque droite

`dor`

### Douleur à la décompression ou défense musculaire

`defesa`

- `0` — Absent
- `1` — Léger
- `2` — Modérée
- `3` — Intense

### Température ≥ 38,5 °C

`temp`

### Neutrophiles

`neut`

- `0` — \< 70%
- `1` — 70 à 84%
- `2` — ≥ 85%

### Leucocytes

`leuco`

- `0` — \< 10 000/mm³
- `1` — 10 000 à 14 900/mm³
- `2` — ≥ 15 000/mm³

### Protéine C-réactive

`pcr`

- `0` — \< 10 mg/L
- `1` — 10 à 49 mg/L
- `2` — ≥ 50 mg/L

## Édition de la méthode

AIR d’Andersson (2008), avec les Tableaux 2 et 7 corrigés par l’erratum de 2012 : sept composantes, total 0–12, CRP en mg/L ; groupes d’origine 0–4, 5–8 et 9–12. La modification du seuil inférieur proposée en 2021 n’a pas été appliquée.

## Formule documentée

Vomissements (1) + douleur fosse iliaque droite (1) + irritation péritonéale légère (1), modérée (2), forte (3) + température ≥38,5 °C (1) + neutrophiles 70–84% (1) ou ≥85% (2) + leucocytes 10 000–14 900 (1) ou ≥15 000 (2) + CRP 10–49 (1) ou ≥50 mg/L (2). Total 0 à 12.

## Limites et population

L’AIR de 2008 a été étudié chez des personnes admises pour suspicion d’appendicite ; une partie de la cohorte est restée dans le groupe indéterminé et a nécessité des investigations supplémentaires. Seul le résumé de l’article original de 2008 a été lu. L’erratum de 2012 a été lu directement : ses Tableaux 2 et 7 corrigent les concentrations de CRP et documentent les points, les unités et les groupes d’origine. La vérification numérique se limite à la somme des sept composantes déjà sélectionnées ; elle n’approuve ni les groupes cliniques ni les décisions diagnostiques, d’imagerie ou chirurgicales. La révision de 2021 a proposé un faible risque pour un score \<4, distinct du groupe d’origine 0–4 ; ce changement n’a pas été appliqué dans cette édition. L’âge minimal, les exclusions et le protocole complet n’ont pas été confirmés par la lecture du résumé de 2008. Les éléments non observés ne doivent pas être considérés comme absents. Aucune revue clinique ou linguistique par des professionnels indépendants ni autorisation des droits de l’instrument n’a été effectuée.

## Références

- [Andersson M, Andersson RE. The appendicitis inflammatory response score: a tool for the diagnosis of acute appendicitis that outperforms the Alvarado score. World J Surg, 2008.](https://doi.org/10.1007/s00268-008-9649-y)

- [Di Saverio S et al. Diagnosis and treatment of acute appendicitis: 2020 update of the WSES Jerusalem guidelines. World J Emerg Surg, 2020.](https://doi.org/10.1186/s13017-020-00306-3)

- [Andersson M, Andersson RE. Erratum to: The Appendicitis Inflammatory Response Score: A Tool for the Diagnosis of Acute Appendicitis that Outperforms the Alvarado Score. World J Surg, 2012;36:2269–2270. Corrected Tables 2 and 7.](https://doi.org/10.1007/s00268-012-1679-9)

## Reproduire les tests techniques

Exécutez node test.cjs dans le répertoire racine de ce dépôt pour reproduire les cas synthétiques enregistrés. Les données d’entrée, les résultats attendus et les tolérances d’origine sont conservés. Les tests techniques ne constituent pas une validation clinique.

```sh
node test.cjs
```

tool.json contient les sources, l’édition et le périmètre de la revue. examples.json conserve les données d’entrée et les résultats attendus des cas synthétiques ; results.json consigne les résultats obtenus.

[Fiche et références](../tool.json) · [Code JavaScript](../calculator.js) · [Cas de référence](../examples.json) · [results.json](../results.json)

## Revue et conditions d’utilisation

Aucune révision clinique indépendante n’a été effectuée.

Cette interface est une traduction réalisée par nos soins, et non une édition officielle ou certifiée. La revue clinique indépendante, la révision linguistique professionnelle et l’autorisation des droits sur les instruments n’ont pas été réalisées.

Résultat de la formule ou de la classification. L’interprétation, la conduite et l’applicabilité dépendent de l’évaluation professionnelle et de la source sélectionnée.

## Licence et attribution

Apache-2.0 s’applique uniquement au code d’ELUCENIA. Les droits sur les instruments, publications, traductions et données restent ceux de leurs titulaires respectifs. Conservez LICENSE et NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
