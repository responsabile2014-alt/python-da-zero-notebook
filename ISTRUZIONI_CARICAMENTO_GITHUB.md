# Come caricare il kit su GitHub

Repository di destinazione: **responsabile2014-alt/python-da-zero-notebook**

Questa cartella (`repo/`) è già pronta da caricare. Contiene:
- `README.md` (root del repository)
- `bonus-ai-ready-premium-kit/` (il kit completo, con il suo README.md)

## Metodo 1 - Da interfaccia web GitHub (più semplice)

1. Vai su https://github.com/responsabile2014-alt/python-da-zero-notebook
2. Se il repository non esiste ancora, crealo con questo nome esatto: `python-da-zero-notebook` (sotto l'account `responsabile2014-alt`).
3. Clicca **Add file > Upload files**.
4. Trascina la cartella `bonus-ai-ready-premium-kit` e il file `README.md` di root.
5. Scrivi un messaggio di commit (es. "Aggiunto AI Ready Premium Kit") e conferma con **Commit changes**.
6. Verifica che la cartella `bonus-ai-ready-premium-kit` sia visibile e che il README si veda nella pagina principale.

NOTA: l'upload via web di intere cartelle funziona trascinandole; assicurati che la struttura interna (le sottocartelle 00-13) sia mantenuta.

## Metodo 2 - Da riga di comando (git)

```bash
# 1. clona il repository (o inizializzalo se vuoto)
git clone https://github.com/responsabile2014-alt/python-da-zero-notebook.git
cd python-da-zero-notebook

# 2. copia dentro la cartella del bonus e il README di root
#    (copia qui bonus-ai-ready-premium-kit/ e README.md)

# 3. aggiungi, committa, carica
git add .
git commit -m "Aggiunto AI Ready Premium Kit"
git push origin principale
```

## Dopo il caricamento: verifica dei link

1. Apri il README del kit su GitHub: https://github.com/responsabile2014-alt/python-da-zero-notebook/blob/principale/bonus-ai-ready-premium-kit/README.md
2. Clicca su uno dei link "Apri in Colab": deve aprire il notebook in Google Colab.
3. Se un link dà errore 404, controlla che:
   - il repository sia **pubblico**;
   - il branch si chiami **principale**;
   - il percorso `bonus-ai-ready-premium-kit/06_Notebook_Colab/` sia corretto.

## Importante sul branch

I link "Apri in Colab" usano il branch **principale**. Se il tuo repository usa un branch diverso da **principale**, sostituisci `blob/principale/` con il nome effettivo del branch nei link del README.
