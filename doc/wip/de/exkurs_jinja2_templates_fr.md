# Excursus : modèles Jinja2

Cette petite digression couvre *rudimentaire* la syntaxe et la sémantique du moteur de modèle. Le moteur de template étant très flexible, la configuration de l'application peut différer légèrement du code présenté ici en termes de délimiteurs et de comportement des valeurs non définies.

Un modèle `Jinja2` est simplement un fichier texte. `Jinja2` peut générer n'importe quel format texte (`HTML`, `XML`, `CSV`, `LATEX` et ainsi de suite...). Un modèle `Jinja2` ne nécessite aucune extension spécifique telle que `.html`, `.xml` ou toute autre extension.

Un modèle contient des variables et/ou des expressions qui sont remplacées par des valeurs lors du rendu du modèle.

Un modèle contient également des balises qui contrôlent la logique du modèle. La syntaxe ici est fortement inspirée de  `Django` et `Python`.

Il existe différents types de séparateurs. Les délimiteurs `Jinja2` par défaut sont configurés comme suit:

- `{% ... %}` → für (limitierte `Python`-) Anweisungen
- `{{ ... }}` → für Ausdrücke, die in der Template-Ausgabe angezeigt werden sollen
- `{# ... #}` → für Kommentare, die nicht in der Template-Ausgabe enthalten sind

Les instructions de ligne et les commentaires sont également possibles, mais ne comportent pas de caractères de préfixe standard et ne peuvent être utilisés que si le système (HA) le spécifie.

***Les variables du modèle*** sont définies par le *Dictionnaire* transmis au modèle. Vous pouvez expérimenter les variables dans les modèles, à condition qu'elles soient également transmises par l'application.

Les variables peuvent contenir des attributs ou des éléments également accessibles. Les attributs d'une variable dépendent en grande partie de l'application destinée à fournir cette variable.

Vous pouvez également utiliser un point (`.`) au lieu de la syntaxe *standard* Python `__getitem__`-'subscript' [ ] pour accéder aux attributs d'une variable.

Les lignes suivantes font donc la même chose:

```yaml
{{ foo.bar }}  
{{ foo['bar'] }}
```

**Important**:
les doubles accolades extérieures `{{` ne font pas partie de la variable, mais de l'instruction `print`. Si vous souhaitez accéder aux variables dans les balises, vous ne pouvez pas les mettre entre accolades.

Un signe moins (`-`) coupe l'objet correspondant avant (`{{-`, `{%-`) ou après (`-}}`, `-%}`).

Si une variable ou un attribut n'existe pas, le résultat sera une valeur ***non définie***. Ce que vous pouvez faire avec ce type de valeur dépend entièrement de la configuration de l'application spécifique:  
Le comportement par défaut est qu'après évaluation, lors de l'impression ou de l'itération sur une chaîne vide, le processus est immédiatement abandonné et un message d'erreur est généré.
