# Politique de confidentialité — ArrowTrack

**Dernière mise à jour :** 2026-05-20
**Responsable du traitement :** Morten Jacobsen, Norvège
**Contact :** galge.vender.0a@icloud.com

---

## Version courte

ArrowTrack stocke **toutes vos données localement sur votre appareil**. Nous n'avons aucun
serveur qui reçoit vos tirs, vos séances ou vos objectifs. Lorsque vous désinstallez
l'application, toutes les données disparaissent.

Les seuls tiers qui reçoivent des informations sont :
- **Apple** — gère les achats App Store et les notifications
- **RevenueCat** (après votre achat Pro) — vérifie votre achat

Vous disposez de l'intégralité des droits RGPD : accès, effacement et portabilité des données.

---

## Ce que nous stockons

### Sur votre appareil (en local, ne quitte jamais le téléphone)
- **Données de tir :** séances, manches, placements de flèches, scores, étiquettes, objectifs, arcs et jeux de flèches
- **Préférences :** langue sélectionnée, thème, main de tir, catégorie de compétition, options de notification
- **Historique de l'app :** statut des coach-marks (les astuces que vous avez vues), indicateurs de tutoriels complétés

Toutes ces données sont stockées dans une base de données SQLite et dans AsyncStorage sur votre iPhone.
Ni ArrowTrack, ni aucun tiers, n'a accès à ces données.

### iCloud (uniquement si iCloud Drive est activé)
ArrowTrack prévoit d'utiliser iCloud Key-Value Storage à une seule fin précise :
mémoriser si vous avez déjà démarré la période d'essai. Cela se synchronise
via votre compte iCloud pour empêcher qu'une désinstallation + réinstallation
n'accorde une nouvelle période d'essai gratuite.

- Apple est le sous-traitant (notre accord est soumis à leurs conditions standard)
- Les valeurs stockées sont **uniquement** : la date de début d'essai et un statut « essai utilisé »
- Cette fonctionnalité s'active lorsque nous lancerons le modèle Pro (Phase 4b)

Si vous avez désactivé iCloud Drive, ou désactivé iCloud Drive spécifiquement
pour ArrowTrack, iCloud n'est pas utilisé.

---

## Tiers

### Apple App Store
Tous les achats intégrés sont gérés par Apple. Nous ne recevons jamais d'informations
bancaires, d'adresses ou d'autres détails de paiement. La
[politique de confidentialité d'Apple](https://www.apple.com/fr/legal/privacy/) s'applique au
processus d'achat.

### Apple Push Notification Service (APNS)
ArrowTrack envoie des notifications locales (RP atteint, expiration de la période d'essai,
rappels d'objectifs). Pour les livrer, iOS enregistre un jeton d'appareil anonyme
auprès d'Apple. Nous n'avons aucun serveur qui envoie des messages push — toutes les notifications
sont générées localement sur votre appareil en fonction de l'état de l'app.

### RevenueCat (uniquement après achat Pro)
Lorsque vous achetez ArrowTrack Pro, RevenueCat enregistre votre reçu et un
`appUserId` anonyme (UUID généré sur votre appareil). Cela est nécessaire
pour que l'app puisse vérifier votre achat lors d'utilisations ultérieures et lors de la
« restauration des achats ». La
[politique de confidentialité de RevenueCat](https://www.revenuecat.com/privacy) s'applique. Nous n'envoyons jamais
votre nom, votre e-mail ou d'autres données personnelles.

### Apple Analytics / rapports de plantage
Si vous avez activé « Partager l'analyse de l'app » dans les Réglages iOS, Apple envoie
des données agrégées anonymes sur l'utilisation et les plantages au développeur.
ArrowTrack utilise cela pour la correction de bugs et l'optimisation des performances. Vous pouvez
désactiver cela via :
**Réglages iOS → Confidentialité et sécurité → Analyse et améliorations**.

---

## Ce que nous NE collectons PAS

- Aucun compte utilisateur, adresse e-mail ou mot de passe
- Aucune donnée GPS ou de localisation
- Aucun accès aux contacts, au calendrier, à l'appareil photo ou au microphone
- Aucun traqueur tiers (Firebase, Google Analytics, Facebook Pixel, etc.)
- Aucun identifiant publicitaire (IDFA)
- Aucun suivi vidéo ni empreinte d'appareil

---

## Vos droits (RGPD)

Vous disposez des droits suivants au titre du Règlement général sur la protection des données :

**Droit d'accès (Art. 15) :** Toutes vos données sont stockées localement sur votre appareil.
Vous avez une visibilité totale via :
- Réglages → Mes séances (toutes les manches historiques)
- Réglages → Mes objectifs (tous les objectifs actifs et archivés)
- Réglages → Arcs / Jeux de flèches / Terrains (gestion du matériel)

**Droit à la portabilité des données (Art. 20) :** Utilisez
**Réglages → Exporter mes données** pour télécharger toutes vos données sous forme de fichier
JSON. Le fichier peut être partagé via la feuille de partage iOS vers e-mail, AirDrop, Fichiers, etc.
C'est l'intégralité de votre historique de tir dans un format standard.

**Droit à l'effacement (Art. 17) :**
- *Supprimer une séance individuelle :* balayez la séance sur l'écran d'accueil → Supprimer
- *Supprimer toutes les données :* désinstallez ArrowTrack — iOS supprime automatiquement
  toute la base de données SQLite et AsyncStorage. Le reçu RevenueCat (si vous
  avez acheté Pro) est conservé par Apple et RevenueCat pour les besoins de remboursement et de
  support.

**Droit à la limitation et d'opposition (Art. 18–21) :** ArrowTrack ne prend
aucune décision automatisée à votre sujet. Le moteur Smart Insights analyse uniquement
vos propres données d'entraînement localement sur votre appareil et présente
des observations — il ne prend aucune décision en votre nom.

**Droit de retirer son consentement (Art. 7) :** L'opt-in d'Apple Analytics se contrôle
via les Réglages iOS. Les données RevenueCat sont supprimées lorsque vous supprimez votre identifiant Apple.

---

## Modifications

Nous mettrons à jour cette politique lorsque des changements significatifs surviendront dans la manière dont nous
traitons les données. Les modifications sont communiquées via :
1. La date « Dernière mise à jour » en haut de cette page
2. Une bannière in-app au premier lancement suivant la mise à jour si le changement est substantiel
   (ex. nouveaux tiers, nouvelle collecte de données)

---

## Réclamations

Si vous estimez que nous traitons vos données personnelles en violation du RGPD,
vous avez le droit de déposer une réclamation auprès de votre autorité nationale de protection des données :

- **France :** [Commission nationale de l'informatique et des libertés (CNIL)](https://www.cnil.fr/)
- **UE/EEE :** trouvez votre autorité sur
  [edpb.europa.eu](https://www.edpb.europa.eu/about-edpb/about-edpb/members_en)

Nous vous encourageons à nous contacter en premier à galge.vender.0a@icloud.com — nous prenons
toutes les demandes de confidentialité au sérieux.
