# Classificazione di Spettrogrammi di Target Spaziali

Questo progetto riguarda la classificazione di spettrogrammi di target spaziali in tre classi, basandosi sulla grandezza del segnale. Il modello utilizza reti neurali costruite con PyTorch e altre librerie di supporto per il preprocessing e l'analisi dei dati.

## Struttura del Progetto

### 1. Importazione delle Librerie
Il progetto utilizza le seguenti librerie principali:
- **Pandas**: Per la manipolazione dei dati.
- **NumPy**: Per operazioni matematiche e matriciali.
- **Matplotlib e Seaborn**: Per la visualizzazione dei dati.
- **Pillow (PIL)**: Per la gestione delle immagini.
- **PyTorch e Torchvision**: Per la costruzione, il training e la valutazione della rete neurale.
- **Scikit-learn**: Per metriche di valutazione come matrici di confusione, precisione, richiamo e accuratezza.

### 2. Configurazione
- **Rilevamento del dispositivo**: Il progetto è ottimizzato per funzionare su GPU (CUDA o MPS su dispositivi Apple) o CPU, con un controllo automatico delle disponibilità hardware.
- **Percorsi dei dati**:
  - Training set: `/Users/roberto/Desktop/FINALP/TargetSpaziali/train`
  - Test set: `/Users/roberto/Desktop/FINALP/TargetSpaziali/test`

### 3. Dataset
Il dataset contiene spettrogrammi di segnali, che sono suddivisi in tre classi in base alla loro grandezza. 

### 4. Architettura del Modello
Il progetto implementa una rete neurale profonda per classificare gli spettrogrammi. L'architettura include:
- Livelli convolutivi per l'estrazione delle caratteristiche.
- Livelli completamente connessi per la classificazione finale.

### 5. Valutazione del Modello
Metriche utilizzate:
- **Matrice di confusione**
- **Precisione**
- **Richiamo**
- **Accuratezza**

## Requisiti
- **Python** (versione specificata nel progetto).
- Librerie richieste:
  - torch
  - torchvision
  - pandas
  - numpy
  - matplotlib
  - scikit-learn
  - pillow

## Esecuzione
1. Assicurati che i dati siano organizzati nei percorsi indicati.
2. Installa le librerie richieste con:
   ```bash
   pip install -r requirements.txt
   ```
3. Esegui il notebook per allenare e testare il modello:
   ```bash
   jupyter notebook ClassificazioneTargetSpaziali.ipynb
   ```

## Risultati
Il modello raggiunge un'accuratezza elevata sulla classificazione dei dati di test, dimostrando la capacità di distinguere efficacemente i segnali nelle tre classi previste.

---

Sviluppato da: [Il tuo Nome]
