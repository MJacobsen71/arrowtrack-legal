# Support — ArrowTrack

**Dernière mise à jour :** 2026-05-20
**Version couverte :** v1.0+
**Contact :** galge.vender.0a@icloud.com

---

## Aide rapide

### Comment enregistrer une volée ?

1. Ouvrez ArrowTrack → touchez **Nouvelle séance** dans l'onglet Accueil
2. Choisissez le terrain, le blason et le format de manche → touchez **Démarrer la séance**
3. **Touchez le blason** pour placer chaque flèche — utilisez le pinch-zoom et la loupe de précision pour la précision
4. Touchez **Enregistrer la volée** quand toutes les flèches sont placées
5. Répétez pour chaque volée jusqu'à ce que la manche soit terminée

### Quelle est la différence entre X et 10 ?

La zone X est l'anneau le plus interne et vaut 10 points — comme l'anneau 10. ArrowTrack suit le X séparément car le X sert de départage en compétition. Touchez le bouton « X » lorsqu'une flèche atteint la zone X en mode score-pad.

### Comment corriger une flèche mal placée ?

1. Appuyez longuement sur la flèche sur le blason → la loupe de précision s'active
2. Glissez la flèche vers la nouvelle position → relâchez
3. OU touchez la flèche pour la sélectionner → touchez **Supprimer** pour la retirer

En mode score-pad : touchez le badge de flèche dans le score-pad et choisissez une nouvelle valeur.

### Qu'est-ce que la post-saisie (l'icône 📋) ?

L'icône 📋 marque les séances saisies manuellement avec le score-pad, sans être enregistrées sur le blason avec des coordonnées. La carte des impacts, la constellation et l'analyse de dispersion ne sont pas disponibles pour les séances post-saisies — seuls les totaux de score.

### Comment acheter Pro ?

1. Touchez une fonctionnalité verrouillée Pro (ex. un thème avec un badge Pro)
2. La page d'achat apparaît avec le bouton **Acheter Pro (299 NOK)**
3. Le modal d'achat standard d'Apple apparaît → confirmez avec Face ID / code
4. Pro s'active immédiatement — toutes les fonctionnalités se débloquent

**Prix :** 299 NOK en achat unique, à vie. Pas d'abonnement, pas de prélèvement récurrent.

### Comment restaurer les achats sur un nouvel iPhone ?

1. Téléchargez ArrowTrack sur le nouvel iPhone (version gratuite)
2. Connectez-vous avec le même identifiant Apple utilisé pour acheter Pro
3. Ouvrez ArrowTrack → **Réglages → Licence → Restaurer les achats**
4. Pro se réactive automatiquement

Si vous avez changé d'identifiant Apple : contactez galge.vender.0a@icloud.com et nous vous aiderons.

### Comment exporter mes données ?

**Réglages → À propos de l'app → Exporter mes données** → la feuille de partage iOS apparaît. Choisissez AirDrop, Mail, Fichiers ou tout autre destinataire pour le fichier JSON.

Le JSON contient toutes les séances, manches, flèches, objectifs, configurations d'arc et préférences — portabilité complète au titre de l'article 20 du RGPD.

### Comment supprimer toutes mes données ?

Désinstallez ArrowTrack → iOS supprime automatiquement toute la base de données SQLite et toutes les préférences. Aucune donnée résiduelle ne reste sur l'appareil.

Si vous avez acheté Pro : le reçu reste chez Apple (pour les besoins de remboursement et de support). La désinstallation n'affecte pas les réinstallations futures — Pro se réactive automatiquement via la restauration des achats.

### Quels formats de manche sont supportés ?

- **WA 720** (extérieur, 6 volées × 12 flèches = 72 flèches)
- **WA 18 m salle** (10 volées × 3 flèches)
- **WA 1440** (4 distances successives)
- **Vegas Shoot** (10 volées × 3 flèches salle 18 m)
- **AGB Portsmouth** (10 volées × 3 flèches salle 20 yd)
- **NFAA Indoor** (12 volées × 5 flèches salle 20 yd)
- **Entraînement libre** (aucune limite de format)

Tous les formats incluent la conformité officielle WA Book 3 : règle du cordon, suivi X séparé, rayons d'anneaux corrects.

### Quels blasons sont supportés ?

- **Blason WA 122 cm 10 anneaux** (standard extérieur)
- **Blason WA 80 cm 10 anneaux** (extérieur longue distance)
- **Blason WA 40 cm 10 anneaux** (salle, mono-spot)
- **Blason WA 40 cm Vegas 3-spot triangulaire** (compétition salle)
- **Blason WA 40 cm Vegas 3-spot vertical** (alternative salle)
- **Blason AGB Portsmouth 60 cm 10 anneaux** (salle Royaume-Uni)
- **Blason NFAA salle 1 spot bleu 40 cm** (USA)
- **Blason NFAA salle 5-spot bleu 40 cm** (compétition USA)

---

## Problèmes techniques

### L'app plante au démarrage

1. Éteignez l'iPhone et rallumez-le
2. Si le problème persiste : désinstallez et réinstallez ArrowTrack (les données d'achat ne sont PAS perdues — le reçu reste chez Apple)
3. Envoyez le journal de plantage à galge.vender.0a@icloud.com : **Réglages → Confidentialité et sécurité → Analyse et améliorations → Données d'analyse** → trouvez le journal ArrowTrack → partagez-le avec nous

Si vous avez choisi de partager les analyses avec le développeur via iOS, les journaux de plantage nous sont envoyés automatiquement.

### Les données de score ont disparu après une mise à jour

ArrowTrack stocke tout localement dans SQLite. Les mises à jour migrent la base de données uniquement vers l'avant — les anciennes données sont converties au nouveau format, jamais supprimées.

Si vous constatez une perte de données :
1. Vérifiez que vous êtes connecté avec le même identifiant Apple
2. Vérifiez **Réglages → À propos de l'app → Numéro de version** — est-il à jour ?
3. Envoyez-nous une description à galge.vender.0a@icloud.com

Nous avons une règle stricte selon laquelle les migrations publiées sont immuables — la perte de données suite à une mise à jour ne devrait jamais arriver. Si cela se produit, c'est un bug et nous voulons en être informés.

### Le pinch-zoom ne fonctionne pas sur le blason

1. Essayez avec deux doigts, pas un
2. Vérifiez que « Réduire les animations » n'est pas activé dans **Réglages iOS → Accessibilité → Mouvement** — cela peut limiter les gestes dans certaines apps
3. Fermez l'app complètement (balayez vers le haut depuis le bas, balayez ArrowTrack vers le haut) et rouvrez-la

### La constellation vibre lors du glissement

C'était un bug en v0.28.2 et antérieures — corrigé en v0.28.3. Mettez l'app à jour vers la dernière version sur l'App Store.

---

## Retours et demandes

### Suggérer une nouvelle fonctionnalité

Envoyez un e-mail à galge.vender.0a@icloud.com avec :
- **Quoi** vous voulez (brève description)
- **Pourquoi** (qu'est-ce que cela améliorerait dans votre entraînement ?)
- **À quelle fréquence** vous l'utiliseriez (quotidiennement / par séance / moins souvent)

Nous lisons chaque demande et publions les fonctionnalités priorisées dans le flux « Quoi de neuf » de l'app.

### Signaler un bug

Envoyez un e-mail à galge.vender.0a@icloud.com avec :
- **Ce qui s'est mal passé** (aussi détaillé que possible)
- **Ce que vous attendiez**
- **Étape par étape** pour reproduire
- **Version iOS** et **modèle d'iPhone** (Réglages → Général → Informations)
- **Version d'ArrowTrack** (Réglages → À propos de l'app)
- Capture d'écran si pertinent

### Général
Nous répondons à toutes les demandes sous 3 jours ouvrés. Les problèmes urgents (plantages vous empêchant de tirer) sont prioritaires.

---

## RGPD et confidentialité

Pour la politique de confidentialité complète : [Confidentialité](https://mjacobsen71.github.io/arrowtrack-legal/privacy-fr)

Pour exporter vos données, supprimer une séance ou exercer d'autres droits RGPD : voir la Politique de confidentialité.

Réclamations de confidentialité : contactez-nous **d'abord** à galge.vender.0a@icloud.com. Si nous ne pouvons pas résoudre la question, vous pouvez vous plaindre auprès de votre autorité nationale de protection des données. Pour la France : [CNIL](https://www.cnil.fr/).

---

## À propos d'ArrowTrack

**Développeur :** Morten Jacobsen, Norvège
**Site web :** [mjacobsen71.github.io/arrowtrack-legal](https://mjacobsen71.github.io/arrowtrack-legal)
**Politique de confidentialité :** [Confidentialité](https://mjacobsen71.github.io/arrowtrack-legal/privacy-fr)
**Licences (open source) :** voir Réglages → À propos de l'app → Licences dans l'app

ArrowTrack est un projet solo d'un seul développeur, conçu pour les archers qui prennent les règles World Archery au sérieux. Construit avec React Native + Expo + TypeScript + SQLite. Pas de backend, pas de cloud, pas de tracking.

Merci d'utiliser l'app. 🏹
