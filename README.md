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

i paragrafi sono in <code>14pt</code> e i titoli > <code>18pt</code>, non ho verificato che i contrasti rispettassero le linee guida del W3C, però ho messo in pratica ciò che ho imparato nel corso di Visualizzazione Scientifica, in particolare rendere del materiale facile da leggere e studiare, evitando contrasti eccessivi per non affaticare la vista e mirando ad una grafica minimale.

<code>epub.css</code> contiene lo stylesheet dell'ebook. Faccio notare che il background è un grigio scuro (simile alla modalità notte, o Dark Theme) e il font è un bianco meno brillante del bianco <code>rgb(255,255,255)</code>.

<code>stylesheet.css</code>
```css
  @font-face {
  font-family: OpenSans;
  font-style: normal;
  font-weight: normal;
  src:url("OpenSans-Regular.ttf");
}

@font-face {
  font-family: OpenSans;
  font-style: normal;
  font-weight: bold;
  src:url("OpenSans-Bold.ttf");
}

@font-face {
  font-family: OpenSans;
  font-style: normal;

  src:url("OpenSans-Light.ttf");
}

@font-face {
  font-family: Oswald;
  font-style: normal;
  font-weight: normal;
  src:url("Oswald-Regular.ttf");
}

@font-face {
  font-family: Oswald;
  font-style: normal;
  font-weight: bold;
  src:url("Oswald-Bold.ttf");
}

@font-face {
  font-family: Oswald;
  font-style: normal;
  src:url("Oswald-Light.ttf");
}

body {
  background-color:rgb(29, 29, 29);
  color: rgb(254, 247, 238);
  margin: 0;
  padding: 12%; 
  text-align: justify;
  font-size: 14pt;
  font-family: OpenSans;
  line-height: 1.75;
}
code { 
  font-family: monospace;
  background-color:rgb(63, 63, 63);
  color: rgb(254, 247, 238);
  
       
 }
h1 { text-align: left; color: #FF7F50; font-size:2.5em;}
h2 { text-align: left; color: #fff981; }
h3 { text-align: left; }
h4 { text-align: left; }
h5 { text-align: left; }
h6 { text-align: left; }
h1, h2, h3, h4, h5, h6 {
  font-family: Oswald;
}
h1.title { }
h2.author { }
h3.date { }
ol.toc { padding: 0; margin-left: 1em; }
ol.toc li { list-style-type: none; margin: 0; padding: 0; }
```
<code>sgc-index.css</code> generato dall'indice.
```css
body {
  background-color:rgb(29, 29, 29);
  color: rgb(254, 247, 238);
  margin: 0;
  padding: 12%; 
  text-align: justify;
  font-size: 14pt;
  font-family: Oswald;
  line-height: 1.75;
}
div.sgc-index-title {
    color: #FF7F50;
    font-size: 2.5em;
    font-weight: bold;
    margin-bottom: 1em;
    text-align: left;
}

div.sgc-index-body {
    margin-left: -2em;
}

div.sgc-index-entry {
    margin-top: 0em;
    margin-bottom: 0.5em;
    margin-left: 3.5em;
    text-indent: -1.5em;
}

div.sgc-index-new-letter {
    margin-top: 1.5em;
    margin-left: 1.3em;
    margin-bottom: 0.5em;
    font-size: 1.5em;
    font-weight: bold;
    border-bottom: solid black 4px;
    width: 50%;
}
```
