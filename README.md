# Sièges au crible

Comparateur personnel de sièges auto pour enfants, publié sur
**https://btrd.github.io/sieges-au-crible/**.

La page est **privée** : elle est chiffrée et ne s'ouvre qu'avec un mot de passe. Ce dépôt ne
contient que la version chiffrée ; le code et les données sont dans un dépôt privé séparé.

## Accès

- Saisir le mot de passe sur la page, ou ouvrir un lien de la forme
  `https://btrd.github.io/sieges-au-crible/#password=…` qui déverrouille directement la page.
  Préférer `#password=` à `?password=` : la partie après `#` n'est jamais envoyée au serveur.
- La page porte une balise `noindex` : les moteurs de recherche ne l'indexent pas.
- Chiffrement : AES-256-GCM, clé dérivée du mot de passe par PBKDF2-SHA256 (600 000 itérations),
  déchiffrement dans le navigateur avec l'API Web Crypto.
