# iris
Semplice algoritmo di machine learning fatto con il K-means

# Descrzione
Questo progetto è stato creato per classificare varie classi di piante, in questo caso iris, utilizzando il K-means. In questo programma abbiamo utilizzato 3 classi differenti di piante, abbiamo quindi utilizzato 3 cluster(centroidi) differenti per classificarli.

Ogni singolo elemento del dataset viene posizionato su un canvas, utilizzando le sue caratteristiche come coordinate (ogni elemento ha 4 caratteristiche), e di conseguenza ogni baricentro viene posizionato casualmente all'interno dell'intervallo di punti, per assicurarsi che tutti siano associati ad almeno un punto.

Per associare un baricentro ai punti corrispondenti, calcoliamo la sua distanza punto-centroide, e assegniamo il punto al baricentro con la distanza più breve, fatto ciò aggiorniamo la posizione del baricentro, calcolando la media delle coordinate dei punti associati , ea questo punto ricalcoliamo le distanze e riassociamo i punti ai propri centroidi fino a che questi ultimi non cambiano più la loro posizione.

Ora controlliamo a quale classe si riferisce il baricentro, semplicemente assegnandogli la classe maggioritaria dei punti ad esso associati, e infine controlliamo se il programma è efficace, verificando quanti elementi rappresentano realmente la classe del baricentro a cui sono stati associati, abbiamo ottenuto la massima precisione, ovvero circa il 91%, utilizzando un grafico 4d, è possibile modificare il numero di dimensioni utilizzate nel programma semplicemente cambiando la linea:
```javascript
var ndim = 4;
```
# Struttura del progetto
Il progetto è suddiviso in 3 file:
 * `dataset.js`: contiene tutti gli elementi del progetto, in questo caso tutte le piante, nel nostro progetto abbiamo 150 elementi, 50 per ogni classe
 * `iris.html`: contiene l'elemento canvas per visualizzare il risultato e collegamenti a vari file js
 * `kmeans.js`: rappresenta il codice che permette di realizzare il progetto

# Run and Test
Per avviare il progetto è necessario aprire il file `iris.html` dal quale sarà possibile visualizzare il risultato finale, ed infine accedendo alla console del browser sarà possibile visualizzarne anche l'esattezza

# Persone
Le persone che hanno collaborato a questo progetto sono:
  * Riccardo Ventrici (https://github.com/v3ntri)
  * Marianna Mileo (https://github.com/merymylo)
  * Federico Marra (https://github.com/Marra-Federico)
  * Frank Dunkan (https://github.com/Fiokkodineve)
