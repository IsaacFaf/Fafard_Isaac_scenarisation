```mermaid
graph TD;
    A[Page d'accueil] --> B[Naviguer dans les sections];
    B --> C{Type de contenu ?};

    C -->|Vidéo| D[Visionner une vidéo];
    C -->|Audio| E[Écouter de l'audio];
    C -->|Image| F[Voir une galerie d'images];
    C -->|Texte| G[Lire du texte interactif];
    C -->|3D| H[Interagir avec un objet 3D];

    D --> I{Vidéo terminée ?};
    I -->|Oui| B;
    I -->|Non| D;

    E --> J{Audio terminé ?};
    J -->|Oui| B;
    J -->|Non| E;

    F --> K{Exploration terminée ?};
    K -->|Oui| B;
    K -->|Non| F;

    G --> L{Texte terminé ?};
    L -->|Oui| B;
    L -->|Non| G;

    H --> M{Interaction 3D terminée ?};
    M -->|Oui| B;
    M -->|Non| H;

    B --> N[Quitter l'expérience];
