# Diagramme de flux – Voyage spirituel

```mermaid
flowchart TD
    A[Page chargée] --> B[Script JS lancé]
    B --> C[Utilisateur clique sur une émotion]
    C --> D[playEmotion()]
    D --> E[Texte + animations]

# Diagramme de flux – Projet Voyage spirituel

Ce diagramme représente le fonctionnement de l’application web interactive.

```mermaid
flowchart TD
    A[Chargement de la page HTML] --> B[Chargement du DOM et du CSS]
    B --> C[Initialisation du JavaScript]

    C --> D[Création de l'objet Audio]
    D --> E[Initialisation des données\nchant, colors, timeoutList]

    E --> F[Affichage du texte par défaut]

    F --> G{Action utilisateur}

    G -->|Clic sur une émotion| H[playEmotion(type)]
    H --> I[resetEmotion()]
    I --> J[Changement du fond]
    J --> K[Affichage progressif du texte]
    K --> L[Création des particules]
    L --> M[Création des ondes lumineuses]
    M --> F

    G -->|Réinitialiser| N[resetEmotion()]
    G -->|Pause musique| O[pauseMusic()]
    G -->|Reprendre musique| P[resumeMusic()]
    G -->|Stop musique| Q[stopMusic()]

    C --> R[Mouvement souris détecté]
    R --> S[Création des traînées lumineuses]
