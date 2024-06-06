# JOHN THE RIPPER

John the Ripper est l'un des outils de déchiffrement de mots de passe les plus célèbres, les plus appréciés et les plus polyvalents. Il allie une grande rapidité de déchiffrement à une compatibilité étendue avec une variété impressionnante de types de hachage.

Initialement, il a été conçu que pour le système d’exploitation Unix, mais il peut maintenant être utilisé sur plusieurs autres plates-formes, telles que Windows, Mac, etc. Il a été publié pour la première fois en 1996 par OpenWall. Sa dernière version est la 1.9.0 qui a été publiée en 2019.

## Qu’est ce que le Hachage (Hash) ?

Un hachage permet de transformer des données de longueur variable en une représentation de longueur fixe. Cela masque la valeur originale des données en les passant à travers un algorithme de hachage. Parmi les algorithmes de hachage populaires, on trouve MD4, MD5, SHA1 et NTLM.

Illustrons ce concept avec un exemple :

Si nous prenons "adil", une chaîne de 4 caractères - et que nous l'exécutons à travers un algorithme de hachage MD5, nous nous retrouverons avec une sortie de :
`5c3bea5d394835b2af9d2cfd632147f8` un hachage MD5 standard de 32 caractères.

De même, si nous prenons "professeuradil", une chaîne de 14 caractères - et que nous l'exécutons à travers le même algorithme de hachage MD5, nous nous retrouvons avec une sortie de :
`063ad290fafcaac17643cbf488b896a5` un autre hachage MD5 standard de 32 caractères.

## Qu'est-ce qui garantit la sécurité des hashs ?

Les hashs sont sécurisés grâce à plusieurs caractéristiques clés : ils sont résistants aux collisions, ce qui rend presque impossible de trouver deux ensembles de données différents produisant le même hash. Ils offrent une résistance à la préimage, empêchant de retrouver les données d'origine à partir du hash, et ils présentent un effet avalanche, où un petit changement dans les données d'entrée entraîne un changement significatif et imprévisible dans le hash. Ces propriétés assurent la sécurité et la fiabilité des hashs pour des applications comme la protection des mots de passe, l'intégrité des fichiers et les signatures numériques.

## La mission de John …

Même si un algorithme de hachage n'est pas réversible, il est toujours possible de casser des hashs. Par exemple, si vous avez la version hachée d'un mot de passe et que vous connaissez l'algorithme utilisé, vous pouvez créer un dictionnaire en hachant un grand nombre de mots. Ensuite, en comparant ces hashs avec celui que vous essayez de casser, vous pouvez trouver une correspondance. Si une correspondance est trouvée, vous connaissez le mot de passe original. Ce processus est appelé une attaque de dictionnaire. John the ripper (l’éventreur en français), souvent abrégé en John, est un outil permettant de mener des attaques de force brute rapides sur divers types de hashs.

**Le bon tuyau** : certains sites comme [hashes.com](https://hashes.com/en/decrypt/hash) vous permettent de déchiffrer certains hashs.
