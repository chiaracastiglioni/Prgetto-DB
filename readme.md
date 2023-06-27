# Come usare questo repository
Usare questo repository come template e crearne uno nuvo sul vostro account

# set di una java app
**nelle operazioni da fare usare solo il terminale e NON avviare l'applicazione usando l'abiente grafico di sviluppo**
eseguire comandi da terminale in ambiente bash quindi munirsi di gitbash su windows 
mentre zsh non dovrebbe dare problemi

0. verificare che il file gradlew abbia permessi di esecuzione.
1. usare il comando `./gradlew create-dirs` per creare le directory corrette
2. definire i pkg aggiuntivi e la MainClass che rappresenta l'entrypoint di avvio dell'aplicazione
3. modificare il file `buid.gradle.kts` nello specifico andare nei task "application" e "task.jar" e modificare il contenuto dei parametri che iniziano con "my" con il percorso ai pkg che porta alla classe principale (si confronti con quello fatto per l'elaborato) ricordarsi che i pkg partono dalla cartella "java" e che non bisogna mettere l'estensione del file
4. scrivere un hello world nel main e verificare che `./gradlew run` stampi correttamente

## impostazione di vscode per un cooding sereno
nella cartella .vscode ci sono file di configurazione per chi intendesse 
usare quest'ultimo come ambiente di sviluppo.
Nella cartella sono inclusi un java formatter che serve a rendere standar la scrittura del codice

0. **launch.json** permette di attuare impostazioni avanzate nel caso si voglia usare il debugger ad esempio
in questo file è necessario fare qualcosa di simile a quanto fatto per il file gradle:
    - modificare il parametro `mainClass` mettendo lo stesso argomento passato alla mainClass del file gradle
    - modificare il parametro `project` con un nome appropriato

fatti questi passaggi verificare che venga lanciato correttamente il debugger di vscode mettendo unbrakepoint sulla stampa.

1. **setting.json** permette la configurazione di azioni dell' editor vscode approfondire su internet se interessati


Una volta configurata l'app createvi un nuovo repo dove intendete salvare l'app cambiare l'origine della repo 

0. `git remote rm origin`
1. `git remote add origin "link alla vostra repo"`
2. `git remote show origin ` per verificare sia tutto ok

