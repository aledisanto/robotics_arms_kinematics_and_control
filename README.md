# Analisi Cinematica e Controllo Dinamico di Manipolatori Robotici

Questa repository raccoglie i progetti applicativi sviluppati per lo studio dei manipolatori robotici. Il progetto sfrutta **MATLAB App Designer** per creare interfacce grafiche (GUI) che permettono di visualizzare e testare interattivamente la teoria matematica alla base del movimento dei robot.

Possiamo dividere il lavoro in due sezioni principali: 
* **Cinematica** (lo studio della geometria del movimento)
* **Dinamica e Controllo** (lo studio delle forze che generano il movimento e il tracciamento delle traiettorie).

---

## Parte 1: Cinematica dei Manipolatori
In questa sezione, l'obiettivo è studiare la relazione geometrica tra le posizioni dei singoli giunti del braccio robotico e la posizione/orientamento finale del suo "end-effector" (la pinza o l'utensile finale) nello spazio 3D. Non vengono prese in considerazione le forze o le masse, ma solo la geometria.

**Cosa andiamo a fare negli esercizi:**
* **Cinematica Diretta e Matrici Omogenee:** Calcoliamo le matrici di trasformazione omogenea per determinare la posa dell'end-effector conoscendo i valori dei giunti e tracciamo il robot in uno spazio 3D. (**[esercizio_1](esercizio_1/esercizio_1/)**)
* **Convenzione di Denavit-Hartenberg (D-H):** Assegniamo i sistemi di riferimento standard per vari modelli di bracci robotici (es. robot a 4 gradi di libertà) per automatizzare il calcolo delle matrici di trasformazione tra un giunto e l'altro e verso la base. (**[esercizio_2](esercizio_2/esercizio_2/)**) e (**[esercizio_3](esercizio_3/esercizio_3/)**)
* **Cinematica Inversa e Polso Sferico:** Risolviamo il problema inverso, ovvero: data una posizione e un orientamento target che l'end-effector deve raggiungere, calcoliamo gli angoli dei giunti necessari. Sfruttiamo la presenza di un "polso sferico" per disaccoppiare matematicamente il problema in due parti (posizione tramite il calcolo di un punto comune e orientamento), analizzando anche le molteplici soluzioni possibili per raggiungere la stessa posa. ((**[esercizio_4](esercizio_4/esercizio_4/)**) e (**[esercizio_5](esercizio_5/esercizio_5/)**))
* **Manipolabilità e Robot a Cavi:** Per un robot planare a due gradi di libertà mosso da cavi, calcoliamo la relazione non lineare tra la lunghezza dei cavi e la posizione. Successivamente, calcoliamo il Jacobiano per generare e plottare gli ellissoidi di manipolabilità di velocità e forza all'interno dello spazio di lavoro. ((**[esercizio_6](esercizio_6/esercizio_6/)**)

---

## Parte 2: Dinamica e Controllo
In questa sezione, l'obiettivo è far muovere fisicamente il robot nel tempo, tenendo conto delle coppie (torques) applicate ai motori dei giunti e implementando un sistema ad anello chiuso per far seguire al robot una traiettoria specifica in modo automatico. ((**[esercizio_7](esercizio_7/esercizio_7/)**)

**OSS.**
In tutte le cartelle il file pdf presenta la consegna dell'esercizio e i file nominati (_codice) racchiudono solo il codice MATLAB poi implementato in **MATLAB App Designer**

---

*Progetto realizzato da: Alessandro Di Santo*  
*Professore: Seriani Stefano*  
*Corso: Robotics*  
*Computer Engineering — Università degli Studi di Trieste*
