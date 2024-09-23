# projet Mermaid
Projet ou que l'on deplace un levier de gauche a droite avec un bouton au top. Le projet incarne le jeu populaire d'arcade rétro Spaceship

```mermaid
graph TD;
    A[Accueil] --> B{Prendre le levier, Appuyer pour tirer};

    B -->|Tirer| C;
    B -->|Pas tirer| A;

    C{Expérience commence};

    C -->|Perdre une vie| E;
    C -->|Prendre un PowerUp| F[Buff temporaire tu tirs];
    C -->|Perdre 3 vie| H;

    E[Jeu continue avec 3 secondes d'invicibilité];

    I -->|Perdre 3 vie| H;


    H[Game Over];

    

    
```