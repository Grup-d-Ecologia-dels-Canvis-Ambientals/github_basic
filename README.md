# Conceptes bàsics GitHub

## Instalació Git Windows

1. Descarregar Git Windows

    [Link descàrrega](https://git-scm.com/downloads/win)

2. Passos post instalació:

    Establir nom d'usuari (link)[https://docs.github.com/en/get-started/git-basics/setting-your-username-in-git]

    ```
    git config --global user.name "Sarah Smith"
    git config --global user.email "sarah.smith@email.com"
    ```

    En windows, la primera vegada que es clona un repositori https si es dóna autorització 3rd party al programari de github
    no cal tornar a entrar credencials per fer push.

## Què és Git?

## Creació de repositoris
### Creació d'un repositori des d'un directori ja existent

    1. Creem un repositori des de github 

        1.2. Anem al nostre perfil -> "Repositories"
        1.3. Cliquem a "New"
        1.4. Deixem totes les opcions per defecte (posem un nom al repositori)

    2. Anem al directori que volem pujar i executem les comandes següents (o similars):

        ```
        echo "# test_create_repo" >> README.md
        git init
        git add README.md
        git commit -m "first commit"
        git branch -M main
        git remote add origin https://github.com/aescobarr/test_create_repo.git
        git push -u origin main
        ```

### Creació d'un repositori des de zero
