# Ping Monitor — GitHub Actions

Ping automatique d'une URL toutes les 5 minutes, sans serveur, sans navigateur.

## Installation

1. Ajoute le secret PING_URL :
   Settings > Secrets and variables > Actions > New repository secret
   - Nom : PING_URL
   - Valeur : https://ton-app.onrender.com

2. Push ce repo sur GitHub

3. Va dans l'onglet Actions pour verifier que ca tourne

## Changer l'intervalle

Modifie la ligne cron dans .github/workflows/ping.yml :
- toutes les 3 min : */3 * * * *
- toutes les 5 min : */5 * * * *
- toutes les 10 min : */10 * * * *

## Note

GitHub desactive les workflows si le repo est inactif 60 jours.
Fais un petit commit de temps en temps pour eviter ca.
