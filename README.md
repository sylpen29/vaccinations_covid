# vaccinations_covid

Nous avons ouvert un Ubuntu
Créer un dossier `mkdir docker-covid-Brief`
Puis sommes rentré dans le dossier: `cd docker-covid-Brief`
Et enfin nous avons ouvert VS Code avec `code .`

Nous avons créé 4 fichiers:

 - fichier python `vaccins.py` -> ouvrir la connection avec MySQL
 - fichier `Dockerfile` -> paramètrer le code
 - fichier `docker-compose.yml` -> Créer les containers dans Docker et fait le lien entre la bdd et grafana
 - fichier `devcontainer.json` -> Echange de données

Les trois derniers fichiers ce trouve dans un dossier `.devcontainer`

Après cela nous téléchargeons sur VS Code l'extension `VS Code Remote-Containers extension`
Il permet de créer les containers dans Docker.
Nous allons par la suite chercher cette extension dans une ` Command Palette`
Et ouvrir `Remote-Containers: Open Folder in Container ...`
Cela nous envoi nos dossier dans un Workspace du nom de `Dev Container: Develop Python`

Nous ouvrons MySQL avec un `localhost:8080` et nous connectons avec les données fournies dans `vaccins.py`
On import le fichier `vaccination.sql`
Après cela nous pouvons ouvrir Grafana grâce au lien `localhost:3000`
Nous nous connectons, faisons le lien avec la bdd depuis `DATA Sources`

Pour finir nous avons fait deux graphiques avec le dashboard.

Voici les graphiques avec leur requêtes:
<img width="894" alt="dashboard_Grafana" src="https://user-images.githubusercontent.com/61606863/162408729-c87e2282-13c5-43c2-84d0-bdb586fcb8de.png">
<img width="641" alt="somme_vaccinés_country_Grafana" src="https://user-images.githubusercontent.com/61606863/162408803-78cec999-f628-4a72-824c-200526e7359a.png">

<img width="649" alt="somme_personnes_vaccinées" src="https://user-images.githubusercontent.com/61606863/162408846-f90e5919-23de-4b55-9b29-ad57f08a4be9.png">
<img width="625" alt="people_vaccinés_Grafana" src="https://user-images.githubusercontent.com/61606863/162408874-5d97f02c-d716-4234-97fe-6a3ee2852476.png">
