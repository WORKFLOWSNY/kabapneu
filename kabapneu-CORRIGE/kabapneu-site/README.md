# Kaba Pneus — Site web complet

Site statique HTML/CSS prêt à déployer.

## 📁 Structure

```
kabapneu-site/
├── index.html              ← Page d'accueil
├── contact.html
├── tarifs.html
├── a-propos.html
├── marque-iris.html
├── mecanique.html
├── blog.html
├── mentions-legales.html
├── cgv.html
├── confidentialite.html
├── cookies.html
├── centres/
│   ├── vermelles.html
│   └── harnes.html
├── pneus/
│   ├── voiture.html
│   ├── poids-lourd.html
│   ├── agricole.html
│   ├── 4x4-suv.html
│   ├── utilitaire.html
│   ├── moto-scooter.html
│   └── occasion.html
├── services/
│   ├── pneus-montage.html
│   ├── direction-parallelisme.html
│   ├── suspension.html
│   ├── moteur-vidange.html
│   ├── freinage.html
│   └── depannage-pl.html
├── blog/
│   └── comment-lire-dimensions-pneu.html
├── .htaccess               ← URLs propres + HTTPS + cache
├── robots.txt              ← Pour Google
└── sitemap.xml             ← Plan du site (Google)
```

## 🚀 Déploiement — 3 options

### Option 1 : Hébergement statique classique (le plus simple)
1. Acheter un hébergement (ex. o2switch, OVH mutualisé, ~3-7€/mois)
2. Connecter le domaine **kabapneu.fr** dans l'interface
3. Uploader le contenu du dossier en FTP/SFTP à la racine
4. Le `.htaccess` gère automatiquement les URLs propres (sans .html visible)

### Option 2 : WordPress (recommandé pour gérer le contenu facilement)
Voir le fichier **DEPLOIEMENT-WORDPRESS.md** ci-joint.

### Option 3 : Test en local
```bash
cd kabapneu-site
python3 -m http.server 8000
# Ouvrir http://localhost:8000
```

## ✅ Tous les liens internes fonctionnent

28 pages HTML interconnectées, tous les liens cliquables mènent à une page existante.

## 📋 Ce qui reste à faire après déploiement

1. **Google Business Profile** — Optimiser les 2 fiches (Vermelles + Harnes)
   - Photos pros (15+ par fiche)
   - Description complète avec mots-clés
   - Liste exhaustive des services
   - Demander 50 avis par fiche

2. **Google Search Console** — Soumettre le sitemap.xml
   - https://search.google.com/search-console

3. **Compléter les blog articles à venir** :
   - pneus-hiver-pas-de-calais.html
   - quand-changer-pneus.html
   - iris-vs-grandes-marques.html
   - pneus-occasion-arnaques.html
   - parallelisme-3d-pourquoi.html
   - entretien-poids-lourd.html

4. **Remplacer les avis "exemples"** par les vrais avis Google une fois collectés

5. **Mettre vos vraies photos** sur :
   - Hero homepage
   - Sections produit
   - Pages centres
   - Article de blog

## 📞 Coordonnées du site

- **Vermelles** : 24 boulevard de la Fosse 4, 62980 — 07 82 28 49 79
- **Harnes** : 5002F route de Lille, 62440 — 06 52 34 33 54
- **Email** : kabapneus@gmail.com

## 📊 Données entreprise

SARL Kaba Pneus — SIRET 919 802 710 — Gérant Mohamed KABA
