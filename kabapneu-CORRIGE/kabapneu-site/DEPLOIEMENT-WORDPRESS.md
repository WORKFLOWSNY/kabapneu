# 🚀 Déploiement sur WordPress — Guide pas à pas

## Méthode A : Site statique sur hébergement WordPress (le plus simple)
Si vous voulez juste mettre les fichiers HTML en ligne sans utiliser le CMS WordPress :
- Uploadez le dossier `kabapneu-site/` à la racine de votre hébergement
- C'est terminé, ça marche directement

## Méthode B : Importer dans WordPress comme CMS (recommandé)

### Étape 1 : Installer WordPress
1. Sur votre hébergement (o2switch, OVH, etc.), installer WordPress en 1 clic
2. Une fois installé, accéder à `https://kabapneu.fr/wp-admin`

### Étape 2 : Choisir un thème
Recommandation : **Astra** (gratuit, léger, rapide, optimisé SEO)
1. Apparence → Thèmes → Ajouter
2. Rechercher "Astra"
3. Installer + Activer

### Étape 3 : Plugins essentiels
Installer ces plugins (Extensions → Ajouter) :
- **Elementor** (constructeur de page visuel)
- **Yoast SEO** (référencement)
- **WP Rocket** (cache, optimisation vitesse) — payant mais excellent
- **Complianz GDPR** (bannière cookies conforme RGPD)
- **Wordfence** (sécurité)

### Étape 4 : Créer les pages WordPress
Pour chaque fichier HTML, créer une page WordPress correspondante :

| Fichier HTML | Slug WordPress | Titre |
|--------------|----------------|-------|
| `index.html` | (page d'accueil) | Kaba Pneus |
| `centres/vermelles.html` | `centres/vermelles` | Centre Vermelles |
| `centres/harnes.html` | `centres/harnes` | Centre Harnes |
| `pneus.html` | `pneus` | Nos pneus |
| `pneus/voiture.html` | `pneus/voiture` | Pneus voiture |
| `pneus/poids-lourd.html` | `pneus/poids-lourd` | Pneus PL |
| `pneus/agricole.html` | `pneus/agricole` | Pneus agricole |
| ... | ... | ... |
| `tarifs.html` | `tarifs` | Tarifs |
| `contact.html` | `contact` | Contact |
| `a-propos.html` | `a-propos` | À propos |
| `marque-iris.html` | `marque-iris` | Marque IRIS |

**Pour chaque page** :
1. Pages → Ajouter
2. Définir le titre
3. Dans Réglages → Permalien : entrer le slug correspondant
4. Ouvrir le fichier HTML correspondant dans un éditeur de texte
5. Copier le contenu situé **entre les balises `<main>` ou après `<section class="page-hero">`** (juste le contenu, pas le header/footer)
6. Coller dans l'éditeur WordPress (passer en mode "Texte" ou "HTML" pour conserver la mise en forme)

### Étape 5 : Configurer le menu
Apparence → Menus
- Créer un menu "Principal"
- Ajouter : Pneus (avec sous-menu), Mécanique, Tarifs, À propos, Contact
- Assigner à l'emplacement "Menu principal"

### Étape 6 : Réglages essentiels
**Réglages → Permaliens** : choisir "Nom de l'article" pour avoir des URLs propres

**Yoast SEO** : 
1. Ouvrir l'assistant de configuration
2. Renseigner les infos de l'entreprise (SARL, Mohamed KABA, etc.)
3. Connecter Google Search Console
4. Soumettre le sitemap (généré automatiquement)

### Étape 7 : Migration des produits Shopify → WooCommerce
Si vous voulez vendre les pneus en ligne :
1. Installer **WooCommerce** (gratuit)
2. Utiliser le CSV fourni : `kabapneu-produits-woocommerce.csv` (de votre projet)
3. WooCommerce → Produits → Importer → Sélectionner le CSV

### Étape 8 : Mettre les fiches Google Business à jour
Une fois le site en ligne :
1. Aller sur https://business.google.com
2. Modifier la fiche **Vermelles** : ajouter l'URL https://kabapneu.fr/centres/vermelles
3. Modifier la fiche **Harnes** : ajouter l'URL https://kabapneu.fr/centres/harnes

## 💡 Conseil final

Si vous n'êtes pas à l'aise avec WordPress, l'**option statique** (Méthode A) est largement suffisante pour démarrer. Vous pourrez toujours migrer vers WordPress plus tard quand vous aurez besoin de fonctionnalités CMS (gestion des produits en ligne, blog facile à mettre à jour, etc.).

Pour le démarrage, le plus important est d'avoir le site **en ligne et indexé par Google**, peu importe la techno.
