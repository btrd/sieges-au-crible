# Sièges au crible

Comparateur personnel de sièges auto pour enfants, publié sur
**https://btrd.github.io/sieges-au-crible/**.

La page est **privée** : elle est chiffrée et ne s'ouvre qu'avec un mot de passe. Ce dépôt ne
contient que la version chiffrée ; le code et les données sont dans un dépôt privé séparé.

## Ce que montre la page

Les sièges auto crash-testés par l'ADAC, croisés avec trois autres sources :

| Source | Ce qu'elle apporte |
|---|---|
| [ADAC](https://www.adac.de/rund-ums-fahrzeug/ausstattung-technik-zubehoer/kindersitze/kindersitztest/) | Note globale et sous-notes (sécurité, utilisation, ergonomie, substances nocives), traduites de l'allemand |
| [Securange](https://www.securange.fr/) | Sièges recommandés, hors sélection ou à éviter |
| [ConsoBaby](https://www.consobaby.com/) | Avis de parents, résumés en points forts et points faibles |
| [Plus Test (VTI)](https://www.vti.se/en/services/laboratory-and-testing/crash-safety-testing/child-restraint-systems/the-plus-test/plus-tested-models) | Sièges dos à la route ayant réussi le crash-test suédois |

Les textes de Securange et de ConsoBaby sont reformulés, jamais copiés ; chaque siège renvoie vers
ses pages d'origine.

## Accès

- Saisir le mot de passe sur la page, ou ouvrir un lien de la forme
  `https://btrd.github.io/sieges-au-crible/#password=…` qui déverrouille directement la page.
  Préférer `#password=` à `?password=` : la partie après `#` n'est jamais envoyée au serveur.
- La page porte une balise `noindex` : les moteurs de recherche ne l'indexent pas.
- Chiffrement : AES-256-GCM, clé dérivée du mot de passe par PBKDF2-SHA256 (600 000 itérations),
  déchiffrement dans le navigateur avec l'API Web Crypto.
