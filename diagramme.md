```mermaid
flowchart TD
    A[Page chargee] --> B[DOM et CSS charges]
    B --> C[Script JavaScript initialise]

    C --> D[Objet audio cree]
    D --> E[Donnees initialisees]

    E --> F[Texte par defaut affiche]

    F --> G{Action utilisateur}

    G -->|Emotion| H[Lancer emotion]
    H --> I[Reinitialiser etat]
    I --> J[Changer fond]
    J --> K[Afficher texte]
    K --> L[Creer particules]
    L --> M[Creer ondes]
    M --> F

    G -->|Reset| N[Reinitialiser]
    G -->|Pause| O[Pause musique]
    G -->|Play| P[Reprendre musique]
    G -->|Stop| Q[Stop musique]

    C --> R[Mouvement souris]
    R --> S[Trails lumineux]
