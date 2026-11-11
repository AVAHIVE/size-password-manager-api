# SIZE Vault — adaptations initiales

Brouillon de rebranding de Passbolt Community Edition pour SIZE. Le serveur du dépôt reste le code Passbolt en amont ; les correctifs ci-dessous s'appliquent aux dépôts distincts indiqués.

## Sources et références exactes

- Serveur : passbolt/passbolt_api @ 5de65b8491b925fdf500e1b06e1f6fafa3b7bc29.
- Interface : passbolt/passbolt_styleguide @ 2265f62500e8a5f7f6ed5fffeb53e1e6a7dacf5b — interface.patch.
- Extension : passbolt/passbolt_browser_extension @ 9db5c2856c23a97819f1d7875afba7fc35b75a0b — extension.patch.
- Android : passbolt/mobile-passbolt-android @ 4523788c4dae3cd531d2f27db6037cb9ff8b9e22 — android.patch.
- iOS : passbolt/mobile-passbolt-ios @ d76a1c7e790d5f404a6307f99f9e2fdb4d154d49 — ios.patch.

Appliquer chaque correctif au dépôt et à la révision correspondants, puis intégrer l'interface modifiée dans la chaîne de compilation de l'extension et du serveur. Une compilation locale de l'interface et de l'extension Chromium MV3 avec l'interface adaptée a réussi, avec des avertissements sur la taille des fichiers. Les fichiers JSON, XML et plist modifiés ont été vérifiés. Aucun test fonctionnel de connexion, de partage, de chiffrement ou sur téléphone n'a encore été effectué.

## État et limites

- Cette branche est un **brouillon**, pas une version à utiliser avec de vrais mots de passe.
- Les correctifs portent sur le logo principal de l'interface, le nom de l'extension et les noms affichés par les applications mobiles. D'autres textes, icônes, écrans, e-mails et éléments de marque restent à adapter.
- Les identifiants d'application, certificats, signatures, services de notification et distribution n'ont pas été configurés. Les applications mobiles ne sont pas compilées ni publiées.
- Passbolt fournit une application Windows ; une application desktop autonome macOS et Linux n'est pas incluse dans ce périmètre. Les extensions de navigateur restent disponibles sur ces plateformes.
- Un serveur configuré, des sauvegardes, les mises à jour, des tests de sécurité et une validation des flux sont nécessaires avant tout déploiement.
- Respecter les licences et mentions d'origine. Passbolt indique que son nom est une marque déposée ; ne pas supposer qu'une licence logicielle donne des droits sur la marque. L'AGPL-3.0 s'applique aux composants correspondants, y compris les obligations pertinentes de mise à disposition du code modifié.
