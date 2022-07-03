---
name: CibNav

clients:
  - Affaires Maritimes

period:
  fr: début 2019

type:
  fr:
    - Aide à la décision algorithmique
    - Redevabilité des algorithmes publiques

description:
  fr: |
    Outil de priorisation des visites de sécurité pour les navires professionnels français.

    Basé sur des données d'accidentologie, l'outil cible les navires les plus accidentogènes et les remonte aux inspecteurs de sécurité. Ceux-ci planifient leurs visites grâce à cette priorisation, d'éventuels facteurs aggravants et leur expertise. Une brique exploration de données permet également de mettre en avant cette expertise.

    Le projet a démarré dans le cadre du programme Entrepreneur d'Intérêt Général. Il a ensuite été développé sous contrat et est maintenant internalisé.


approach:
  fr:
    - Vulgarisation sur le thème de la data-science
    - Accent mis sur l'algorithme et son appropriation par les utilisateurs
    - Algorithme développé dans une démarche d'interprétabilité

resources:
  fr:
    - 1 data scientist

technos: [InterpretML, Python, Embulk, Airflow, MLFlow, Postgres]

refs:
  - name: eig
    link: https://eig.etalab.gouv.fr/defis/cibnav/
    fr: Présentation du projet CibNav sur le site d'Etalab

code:
  - name: Modèle
    link: https://github.com/interpretml/interpret
    fr: Modèle Machine Learning utilisé



images:
  - ./images/references/cibnav/cibnav-01.png
  - ./images/references/cibnav/cibnav-02.png
  - ./images/references/cibnav/cibnav-03.png

---
