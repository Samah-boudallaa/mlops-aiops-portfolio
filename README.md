# MLOps / AIOps Portfolio | Samah Boudallaa

Portfolio en ligne construit pour répondre à une offre réelle : **MLOps / AIOps Engineer chez RED TIC (Casablanca)**. Chaque section relie une attente de l'annonce à une preuve concrète : projet, dépôt GitHub, chiffre mesuré.

**Voir le portfolio :** https://samah-boudallaa.github.io/mlops-aiops-portfolio/

---

## Contexte

Ce dépôt est un livrable du module **Projet professionnel et insertion professionnelle** (EST Kelâa des Sraghna, Bachelor Sciences des Données, 2026-2027, enseignante : Prof. Oumaima El Bouzidi).

Le groupe joue le rôle d'un cabinet de conseil qui prépare le dossier de candidature complet d'un de ses membres pour un poste précis. Le profil retenu est celui de Samah Boudallaa. Son portfolio habituel reste séparé, dans le dépôt `samah-boudallaa.github.io` ; celui-ci a été créé uniquement pour cet exercice.

### L'équipe (groupe n° 2)

<table>
<tr><td align="center" valign="top" width="20%"><a href="https://github.com/NezhaIdrissi"><img src="https://github.com/NezhaIdrissi.png?size=120" width="96" alt="Nezha Ennaji Idrissi"><br><b>Nezha Ennaji Idrissi</b></a><br><sub>Bloc 1 · Profil</sub></td><td align="center" valign="top" width="20%"><a href="https://github.com/KhadijaElBasri"><img src="https://github.com/KhadijaElBasri.png?size=120" width="96" alt="Khadija El Basri"><br><b>Khadija El Basri</b></a><br><sub>Bloc 2 · CV</sub></td><td align="center" valign="top" width="20%"><a href="https://github.com/Chaymae-El-Bahloul"><img src="https://github.com/Chaymae-El-Bahloul.png?size=120" width="96" alt="Chaymae El Bahloul"><br><b>Chaymae El Bahloul</b></a><br><sub>Bloc 3 · Lettre de motivation</sub></td><td align="center" valign="top" width="20%"><a href="https://github.com/Samah-boudallaa"><img src="https://github.com/Samah-boudallaa.png?size=120" width="96" alt="Samah Boudallaa"><br><b>Samah Boudallaa</b></a><br><sub>Bloc 4 · Profil GitHub (candidate présentée)</sub></td><td align="center" valign="top" width="20%"><a href="https://github.com/khadija-rizqy"><img src="https://github.com/khadija-rizqy.png?size=120" width="96" alt="Khadija Rizqy"><br><b>Khadija Rizqy</b></a><br><sub>Bloc 5 · Portfolio</sub></td></tr>
</table>

Cliquez sur un nom pour ouvrir son profil GitHub. Chaque membre a pris en charge un bloc du dossier ; le candidat étudié est Samah Boudallaa.

Groupe n° 2. Poste visé : [MLOps / AIOps Engineer, RED TIC](https://verscdi.com/jobs/mlops-aiops-engineer-casablanca-n6akag) (offre VersCDI).

---

## Ce que contient le portfolio

- Une accroche orientée MLOps / AIOps et quatre indicateurs : 443 154 enregistrements traités, lecture en moins de 100 ms, 8 métriques Prometheus, 12 tests pytest.
- Un tableau « attente du poste, preuve, dépôt » avec des liens vers les dépôts.
- Trois projets mis en avant, avec leurs limites assumées.
- Des projets à venir : CI/CD d'un modèle, MLflow et suivi de dérive, Kubernetes et cloud.
- Le parcours, les compétences, un bouton de téléchargement du CV et les contacts.

## Correspondance avec l'offre

| Attente du poste | Preuve | Projet |
|---|---|---|
| Conteneurisation et déploiement | Docker Compose (6 services), conteneur non-root avec healthcheck | [Smart Data Pipeline](https://github.com/Samah-boudallaa/smart-data-pipeline-pfe), [GraphGen](https://github.com/Samah-boudallaa/GraphGen) |
| CI/CD et tests | GitHub Actions, 12 tests pytest, linter ruff | [GraphGen](https://github.com/Samah-boudallaa/GraphGen) |
| Monitoring et observabilité | Prometheus (8 métriques), dashboard Grafana | [Smart Data Pipeline](https://github.com/Samah-boudallaa/smart-data-pipeline-pfe) |
| Détection d'anomalies | Isolation Forest sur un flux Kafka | [Smart Data Pipeline](https://github.com/Samah-boudallaa/smart-data-pipeline-pfe) |
| Modèles ML exposés en API | FastAPI (9 endpoints), modèle XGBoost | [NexaDecide](https://github.com/Samah-boudallaa/nexadecide-decision-system) |

**Limites assumées :** les résultats viennent de tests en local ou de données simulées (MAPE de 8,9 % sur données simulées). Il manque encore Kubernetes, MLflow, le suivi de dérive et une expérience cloud en production ; ils figurent dans la feuille de route du portfolio.

---

## Preuves visuelles

Les captures sont dans le dossier [`assets/`](assets/).

| Capture | Ce qu'elle montre |
|---|---|
| `assets/grafana-dashboard.png` | Dashboard Grafana du projet Smart Data Pipeline |
| `assets/docker-compose-ps.png` | Les 6 conteneurs du pipeline en fonctionnement |
| `assets/github-actions-graphgen.png` | Intégration continue GraphGen (exécution réussie) |
| `assets/pytest-graphgen.png` | Les 12 tests pytest qui passent |
| `assets/architecture-smart-data-pipeline.png` | Schéma : Kafka, traitement, Isolation Forest, Prometheus, Grafana |
| `assets/og-image.png` | Aperçu affiché lors du partage du lien (1200 x 630) |

---

## Structure du dépôt

```
mlops-aiops-portfolio/
├── index.html                 Portfolio (HTML, CSS et JavaScript, un seul fichier)
├── CV_Samah_Boudallaa.pdf     CV adapté à l'offre, version validée par le groupe
├── README.md                  Ce fichier
└── assets/                    Captures d'écran, schéma, image de partage
```

## Technologies

HTML, CSS et JavaScript sans framework ni dépendance. Le fond animé (réseau de données) est dessiné avec l'élément `canvas`. Thème clair et sombre, navigation au clavier (Ctrl K) et affichage adapté aux téléphones.

## Lancer en local

```bash
git clone https://github.com/Samah-boudallaa/mlops-aiops-portfolio.git
cd mlops-aiops-portfolio
python -m http.server 8000
```

Puis ouvrir http://localhost:8000.

## Déploiement

Le site est publié avec GitHub Pages : Settings, Pages, branche `main`, dossier `/ (root)`.

---

## Contact

- E-mail : [samahboudallaa@gmail.com](mailto:samahboudallaa@gmail.com)
- LinkedIn : [samah-boudallaa-92409a329](https://www.linkedin.com/in/samah-boudallaa-92409a329)
- GitHub : [Samah-boudallaa](https://github.com/Samah-boudallaa)
-
