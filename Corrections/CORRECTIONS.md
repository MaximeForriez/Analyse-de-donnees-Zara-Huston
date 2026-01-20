# Élements de corrections

## Séance 2.

### Questions

- **Question 8.** Il n'existe aucune hiérarchie entre les caractères qualitatifs et les caractères quantitatifs.

- Vous survolez les questions.

### Code

- Quelques problèmes d'exécution en utilisant la colonne `"Libellé du département"` au lieu de `"Code du département"`.

## Séance 3.

### Questions

- **Question 1.** Le caractère le plus général est le caractère qualitatif, car il est possible de transformer le caractère quantitatif en caractère qualitatif.

- **Question 6.** Le moment centré utilise l'écart à la moyenne. Le moment absolu ne l'utilise pas.

- Questions survolées.

### Code

- Excellent !

## Séance 4

### Questions

- Questions survolées.

### Code

- Excellent !

## Séance 5

### Questions

- **Question 5.** Une statistique portant sur la population totale est une statistique exhaustive.

- Questions survolées.

### Code

- Il manque la valeur du test de Shapiro. Vous auriez vu qu'il était élevé pour la distribution test1 que pour la distribution test2.

- La distribution test1 est normale. Il y a effectivement un problème avec le calcul de la *p-value*.

- La distribution test2 est exponentielle ou parétienne.

## Séance 6

### Questions

- Questions survolées.

### Code

- Le calcul des tests est faux. Vous avez écrit :

```
    coef_spear_2007, p_spear_2007 = spearmanr(rangs_pop_2007, rangs_dens_2007)
    coef_kendall_2007, p_kendall_2007 = kendalltau(rangs_pop_2007, rangs_dens_2007)
    print("Spearman :", coef_spear_2007, "p-value :", p_spear_2007)
    print("Kendall :", coef_kendall_2007, "p-value :", p_kendall_2007)

    coef_spear_2025, p_spear_2025 = spearmanr(rangs_pop_2025, rangs_dens_2025)
    coef_kendall_2025, p_kendall_2025 = kendalltau(rangs_pop_2025, rangs_dens_2025)
    print("Spearman :", coef_spear_2025, "p-value :", p_spear_2025)
    print("Kendall :", coef_kendall_2025, "p-value :", p_kendall_2025)
```

Il fallait écrire :

```
    coef_spear_pop, p_spear_pop = spearmanr(rangs_pop_2007, rangs_pop_2025)
    coef_kendall_pop, p_kendall_pop = kendalltau(rangs_pop_2007, rangs_pop_2025)
    print("Spearman :", coef_spear_pop, "p-value :", p_spear_pop)
    print("Kendall :", coef_kendall_pop, "p-value :", p_kendall_pop)

    coef_spear_dens, p_spear_dens = spearmanr(rangs_dens_2007, rangs_dens_2025)
    coef_kendall_dens, p_kendall_dens = kendalltau(rangs_dens_2007, rangs_dens_2025)
    print("Spearman :", coef_spear_dens, "p-value :", p_spear_dens)
    print("Kendall :", coef_kendall_dens, "p-value :", p_kendall_dens)
```

## Humanités numériques

- Aucun rendu.

## Remarques générales

- Aucun dépôt régulier sur `GitHub`.

- Attention ! Vous devez appeler votre fichier de code `main.py`. Vous comprendrez si vous faites un jour du `Python` avancé.

- Vous avez le droit d'avoir votre opinion, mais je n'ai pas arrêté de le dire en cours. Je vous forme pour atteindre le niveau professionnel.

    - Vous avez eu de la chance que l'installation `Python` se passe bien. Ce n'est pas toujours le cas, notamment sur les MAC. Si j'ai mis en place la solution `Docker`, c'est parce que j'ai déjà vécu l'expérience d'étudiants ne pouvant pas installer `Python` dans leur système d'exploitation.

    - Le rôle d'un enseignant est de vous dire ce que vous devez faire, pas de le faire à votre place. J'ai à récupérer 500 fichiers. Désolé Moodle n'est pas adapté. Vous rêvez en vous centrant trop sur vous-même que la logistique est simple.
    
    - L'objectif de `GitHub` est de créer un portfolio. J'ai demandé dès la deuxième séance si `GitHub` posait problème, je n'ai eu aucune réponse, donc tout va bien. Je ne peux pas courir après tout le monde. Si vous ne sollicitez pas, je ne peux pas savoir. Je n'ai jamais envoyé bouler personne, sauf lorsque j'étais occupé. Je ne peux pas me dédoubler. 
    
    - Mettre en place un outil de travail vous prendra toujours davantage de temps que le reste de votre travail.

    - Mon ressenti lorque les étudiants prennent peur, est que vous ne voulez pas vous y mettre. Il n'y avait rien à comprendre, il y avait à faire.

- Il faut vous endurcir, si vous pensez que mes propos étaient durs ou déplacés, c'est que vous connaissez très mal le milieu des cadres dans les secteurs public ou privé. Je suis un bisounours par rapport à ce que vous allez entendre ou devoir faire dans le cadre de votre futur emploi de la part de vos managers. Je ne fais que vous y préparez en parlant ainsi et en vous proposant un projet ambitieux.

- Le cours est exhaustif. Je l'ai dit dès la première séance. Un simple survol du contenu pour les textes longs en repérant ce qui est demandé pour les manipulations, était suffisant. Il est exhaustif pour ceux qui ont fait un peu de mathématiques. Ces étudiants apprécient ce contenu, contrairement à vous.
