# Smarter Patrols

**Auteur** : Monsterfish
**Version** : 1.0.1

Permet aux troupes de patrouille et d'escorte de siège de l'IA d'utiliser réellement tous leurs groupes lors d'une attaque. Les deux volets peuvent être désactivés séparément dans les paramètres.

## Troupes de patrouille

Dans le jeu d'origine, seul le premier groupe de patrouille reçoit des ordres. Le second reste simplement au point de ralliement pendant toute l'attaque.

Avec ce module, chaque groupe de patrouille suit son propre itinéraire autour du château attaqué :

- **Groupe 1** contourne le château dans un sens.
- **Groupe 2** le contourne dans l'autre sens.
- **Groupe 3** fait des allers-retours devant la façade du château (le côté tourné vers l'attaquant).
- **Groupes 4, 5, 6** font de même que 1, 2 et 3, décalés d'un quart de tour derrière eux. Les groupes 7, 8 et 9 suivent derrière, et ainsi de suite.

Ils se déplacent à une distance de marche définie autour du château (12 cases par défaut, comme la patrouille du jeu d'origine), afin de contourner murs et douves plutôt que de foncer dedans. Un groupe qui croise des ennemis combat d'abord puis reprend sa route.

## Troupes d'escorte de siège

Ces troupes vont déjà d'un engin de siège à l'autre, mais les deux groupes suivent exactement le même trajet au même moment et agissent donc comme un seul bloc.

Avec ce module :

- Chaque groupe commence auprès d'un engin de siège différent et un groupe sur deux se déplace en sens inverse, ce qui couvre tous les engins.
- Les groupes composés majoritairement d'unités de mêlée marchent quelques cases devant les engins (vers le château) afin d'attirer les tirs des défenseurs. Les archers restent auprès des engins.
- Lorsque l'assaut des murs commence, tous les groupes passent à l'attaque comme dans le jeu d'origine.

## Davantage de groupes

Le jeu d'origine ne gère que 2 groupes de patrouille et 2 groupes d'escorte de siège. Si un fichier d'IA en demande davantage, les unités en trop se retrouvent dans les mauvaises troupes (creuseurs de douves ou armée principale). Ce module permet d'avoir jusqu'à 12 groupes de chaque type. Le nombre provient du fichier de l'IA sauf si vous le définissez dans les paramètres (escorte de siège : 4 par défaut). Une troupe n'est divisée que tant que chaque groupe conserve au moins 4 unités (réglable).

Les groupes supplémentaires n'existent que pendant l'attaque. Dès qu'une brèche est ouverte, que le seigneur meurt ou que l'IA se replie, ils rejoignent le reste de l'armée et suivent à nouveau les ordres habituels de l'IA.

## Bon à savoir

- Seules les attaques de l'IA sont concernées ; vos propres troupes ne sont pas modifiées.
- Compatible avec Lord Hunt.
- Aucune donnée supplémentaire n'est écrite dans les sauvegardes.
