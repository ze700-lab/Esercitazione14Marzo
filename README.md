# Git-tutorial
Introduzione a git

## PortableGit
Scaricare l'ultima versione di PortableGit: https://github.com/git-for-windows/git/releases/
![](PortableGit.png)
Eseguire il file exe scaricato.
![](exe.png)
Aprire il programma `git-bash` nella cartella di PortableGit appena creata.
![](git-bash.png)

## Creazione progetto
Creare una cartella per il progetto sul Desktop chiamata `Esercitazione16maggio`.
Su git-bash eseguire
```
cd  $HOME/path/to/Esercitazione16maggio
```
dove `path/to/` rappresenta il percorso della cartella `Esercitazione16maggio`.

Creare un file `README.md` in Blocco note, che sarà il readme file del repository Git, e scrivere al suo interno la traccia dell'esercitazione indicata su Classroom.
Salvare il file.

### Creazione repository su Github
- Aprire il sito github.com
- Effettuare il login
- Cliccare su `New` ![](newRepo.png)
- Creare un nuovo repository `Esercitazione16maggio`, prestando attenzione a non creare un Readme di default ![](repo.png)

### Configurazione del repository locale e sincronizzazione
Da `git-bash` eseguire i seguenti comandi:
```
git init  # Inizializza il repository locale
git add README.md  # Inserimento del file README.md nell'area di staging
git commit -m "first commit"  # Creazione del primo commit, che serve a sincronizzare il repository locale con lo stage
git branch -M main  # Creazione del branch main, da usare come default
git remote add origin git@github.com:<username>/Esercitazione16maggio.git  # Connessione del repository remoto al repository locale
git push -u origin main  # Sincronizzazione del repository remoto con quello locale
```
## Aggiunta di nuovi file al repository
1. Creare un nuovo file `main.c` nel workspace
2. Implementare un programma che, dati in input 10 numeri positivi, trovi il massimo e lo visualizzi a video
3. Aggiungere il nuovo file nell'area di staging
4. Sincronizzare l'area di staging con il repository locale (usando un messaggio di commit congruo)
5. Sincronizzare il repository remoto con quello locale

## Migioramento del file README.md
- Aggiungere la traccia dell'esercizio svolto
- Aggiungere una descrizione del codice
- Inserire una sezione in cui vengono spiegati i comandi utilizzati per la creazione di questo repository in stile tutorial
- Spiegare, in una nuova sezione, le funzioni base di Git

Per ognuno dei punti, effettuare, separatamente, i punti da 2 a 5 per sincronizzare i repository.

Di seguito vi sono delle istruzioni per migliorare la formattazione del file README.md

**NOTA: Il repository che creerete in questa esercitazione vi sarà utile per le prossime esercitazioni.**

## Inserire immagini nel README.md
Aggiungere l'immagine `img.jpg` al progetto ed inserirla nel testo con il seguente comando:
```![](img.png)```

## Inserire sezioni
Le sezioni possono essere create inserendo un `#` prima del titolo della sezione. Si può modificare il tipo di sezione usando da uno a sei `#`. È importante separare i `#` dal titolo con uno spazio.

## Inserire codice e citazioni
Il codice può essere inserito delimitandolo con tre backtick `.

Le citazioni possono essere fatte aggiungendo `>` prima del testo.
