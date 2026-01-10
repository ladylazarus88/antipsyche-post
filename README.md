# Antipsyche – Contenuti editoriali

**Guida per la redazione di nuovi contenuti**

Questo repository contiene **esclusivamente** i testi (articoli, recensioni, saggi) destinati alla pubblicazione sul sito **Antipsyché**, scritti come file **Markdown (.md)**.

---

##  1. Struttura del repository

```
antipsyche-post/
├─ .obsidian/       [CARTELLA SYSTEM NASCOSTA PRIVATA]
├─ .git/            [CARTELLA SYSTEM NASCOSTA PRIVATA]
├─ posts/ 
├─ info
	└─ _README.md
└─templates/
	├─ _template-contrappunti.md
	└─ _template-recensione.md

```

### Significato delle cartelle

- `posts/`  
    Dove devi inserire tutti i **nuovi articoli da pubblicare**.
- `templates/`  
    Contiene i **modelli obbligatori** da copiare per ogni nuovo articolo.
- `info/`  
    Contiene **ME**: la guida che stai leggendo.
---

## 2. Come creare un nuovo articolo (OBBLIGATORIO)

### Duplica il template e sposta il nuovo file nella cartella post

- **Seleziona** uno dei due template disponibili nella cartella `templates`
    
- **Duplica** il file (tasto destro, "Crea una copia").
	
- **Rinominalo** in **kebab-case**, ad esempio:
    prova-di-post.md
    
- **Spostalo** nella cartella **posts**.

---

## 3. Compilare il frontmatter (la parte in alto tra `---`)

**Il frontmatter è obbligatorio**.  Il frontmatter contiene tutti i dati necessari perché il post possa essere correttamente "indicizzato" dal sito. Un file senza frontmatter **non può essere pubblicato**.

Esempio:

```yaml
---
title: Le voci del mondo
slug: le-voci-del-mondo
author: Robert Schneider
editor: Claudio Oreste Menafra
date: 2026-01-05


image: https://example.com/immagine.webp
image_alt: Descrizione dell’immagine

excerpt: Breve riassunto di 1–2 frasi dell’articolo.

categories:
  - Recensione
type: 
  - recensione
tags:
  - Letteratura
  - Romanzo
  - Musica

lang: it
draft: true

---
```

---
## 4. Scrivere il testo

- Usa **solo Markdown**. Obsidian ti aiuta a formattare senza stare a pensare a quali sono i caratteri da usare prima e dopo per determinare le strutture.
     
- I simboli più comuni comunque per formattare il testo sono:  
    - `*corsivo*`
        
    - `**grassetto**`
        
    - `>` per citazioni
    
- Le immagini nel testo sono opzionali ma tendezialmente sarebbe auspicabile avere sempre in apertura un'immagine di copertina. (Quelle del frontmatter servono a gestire il contenuto su altre pagine, quindi anche se le inserisci non le vedrai sulla pagina dell'articolo).
	- ``` ![brevissima caption immagine](URL) ```
---
##  5. Come fare commit e push (workflow base)

Quando hai finito di scrivere o aggiornare un testo da Obsidian, questo viene automaticamente salvato nella tua cartella locale. Adesso:

1. Apri **GitKraken**
       
2. Scrivi un **messaggio di commit** chiaro, es:
    
  ```
   Aggiunta recensione su Robert Schneider
   ```
    
3. Fai **Commit**.
	
	
4. Fai **Push**. 
	
	
5. Fine
---

## 7. Cose da NON fare

- Non modificare niente se non il contenuto della cartella **posts**.
- **Non cambiare la struttura delle cartelle**.
- Non cancellare file di sistema.  
- Non usare Word / Google Docs.
- **Non rimuovere campi dal frontmatter**

---
