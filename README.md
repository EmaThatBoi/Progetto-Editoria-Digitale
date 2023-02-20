# Codice del progetto

## Trasformazione del formato

il codice usato con pandoc per effettuare la trasformazione:

<code>pandoc -o book.epub metadata.txt testo.md</code> <br></br>
<code>testo.md</code> è il testo deli libro in markdown<br></br>
<code>book.epub</code> è stato rinominato successivamente con il titolo del libro <br></br>
<code>metadata.txt</code> è il file txt contenente i metadati in Dublin Core

## Css

dall'editor si vedono due file css:
<code>stylesheet1.css</code> è quello da me sviluppato, mentre <code>sgc-index.css</code> è stato generato con la creazione dell'indice analitico attraverso l'editor Sigil. 

i paragrafi sono in 14pt e i titoli > 18pt, non ho verificato che i contrasti rispettassero le linee guida del W3C, però ho messo in pratica ciò che ho imparato nel corso di Visualizzazione Scientifica, in particolare rendere del materiale facile da leggere e studiare, evitando contrasti eccessivi per non affaticare la vista e mirando ad una grafica minimale.

<code>epub.css</code> contiene lo stylesheet dell'ebook. Faccio notare che il background è un grigio scuro (simile alla modalità notte, o Dark Theme) e il font è un bianco meno brillante del bianco RGB (255,255,255).

