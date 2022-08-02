JavaScript fornisce otto diversi tipi di dati che sono:
 undefined, null, boolean, string, symbol, bigint, number e object.

I computer distinguono tra numeri, come il numero 12,
 e stringhe, come "12", "cane" o "123 gatti", che sono raccolte di caratteri.
Le variabili consentono ai computer di archiviare e manipolare i dati in modo dinamico. Lo fanno utilizzando un'"etichetta" per indicare i dati anziché utilizzare i dati stessi. Uno qualsiasi degli otto tipi di dati può essere memorizzato in una variabile.

Le variabili sono un nome semplice per rappresentare i dati a cui vogliamo fare riferimento. 
Diciamo a JavaScript di creare o dichiarare una variabile mettendo la parola chiave var davanti ad essa, in questo modo: var ourName;
var a;
---
Memorizzazione dei valori con l'operatore di assegnazione
In JavaScript, puoi memorizzare un valore in una variabile con l'operatore di assegnazione (=).

miaVariabile = 5;
Questo assegna il valore Number 5 a myVariable.

Se sono presenti calcoli a destra dell'operatore =, questi vengono eseguiti prima che il valore venga assegnato alla variabile a sinistra dell'operatore.

var miaVar;
miaVar = 5;
Innanzitutto, questo codice crea una variabile denominata myVar. Quindi, il codice assegna 5 a myVar. Ora, se myVar appare di nuovo nel codice, il programma lo tratterà come se fosse 5.

Assegna il valore 7 alla variabile a.
a = 7
---
Assegnare il valore di una variabile a un'altra
Dopo che un valore è stato assegnato a una variabile utilizzando l'operatore di assegnazione, è possibile assegnare il valore di quella variabile a un'altra variabile utilizzando l'operatore di assegnazione.

var miaVar;
miaVar = 5;
var myNum;
mioNum = miaVar;
Quanto sopra dichiara una variabile myVar senza valore, quindi le assegna il valore 5. Successivamente, viene dichiarata una variabile denominata myNum senza valore. Quindi, il contenuto di myVar (che è 5) viene assegnato alla variabile myNum. Ora, myNum ha anche il valore di 5.
---

Inizializzazione di variabili con l'operatore di assegnazione
È comune inizializzare una variabile su un valore iniziale nella stessa riga in cui viene dichiarata.

var miaVar = 0;
Crea una nuova variabile chiamata myVar e le assegna un valore iniziale di 0.

var myVar = 0;
Definire una variabile a con var e inizializzarla su un valore di 9.
var a = 9;
---
Dichiara variabili stringa
In precedenza hai utilizzato il seguente codice per dichiarare una variabile:
var mioNome;
Ma puoi anche dichiarare una variabile stringa come questa:
var myName = "il tuo nome";
"il tuo nome" è chiamato una stringa letterale.

 Una stringa letterale, o stringa, è una serie di zero o più caratteri racchiusi tra virgolette singole o doppie.

Crea due nuove variabili stringa: myFirstName e myLastName e assegna loro rispettivamente i valori del tuo nome e cognome.
var myFirstName = "mauro"
var myLastName = "veronese"
---
Comprensione delle variabili non inizializzate
Quando le variabili JavaScript vengono dichiarate, hanno un valore iniziale di undefined. Se esegui un'operazione matematica su una variabile non definita, il tuo risultato sarà NaN che significa "Non un numero". Se concateni una stringa con una variabile undefined, otterrai una stringa di undefined.

Inizializzare le tre variabili a, b e c rispettivamente con 5, 10 e "Io sono a" in modo che non siano indefinite.
var a = 5;
var b = 10;
var c = "io sono a";
---
Comprendere la distinzione tra maiuscole e minuscole nelle variabili
In JavaScript tutte le variabili e i nomi delle funzioni fanno distinzione tra maiuscole e minuscole. Ciò significa che la capitalizzazione conta.
Scrivi i nomi delle variabili in JavaScript in camelCase. In camelCase, i nomi delle variabili con più parole hanno la prima parola in minuscolo e la prima lettera di ogni parola successiva è in maiuscolo. Esempi:
---

Esplora le differenze tra le parole chiave var e let
Uno dei maggiori problemi con la dichiarazione di variabili con la parola chiave var è che puoi facilmente sovrascrivere le dichiarazioni di variabili:

var camper = "Giacomo";
var camper = "David";
console.log(camper);
Nel codice sopra, la variabile camper è originariamente dichiarata come James e viene quindi sovrascritta come David. La console visualizza quindi la stringa David.

In una piccola applicazione, potresti non riscontrare questo tipo di problema. Ma man mano che la tua base di codice diventa più grande, potresti sovrascrivere accidentalmente una variabile che non intendevi. Poiché questo comportamento non genera errori, la ricerca e la correzione dei bug diventa più difficile.

Una parola chiave chiamata let è stata introdotta in ES6, un importante aggiornamento di JavaScript, per risolvere questo potenziale problema con la parola chiave var. Imparerai altre funzionalità di ES6 nelle sfide successive.
---
Dichiara una variabile di sola lettura con la parola chiave const
La parola chiave let non è l'unico nuovo modo per dichiarare le variabili. In ES6, puoi anche dichiarare variabili usando la parola chiave const.
const ha tutte le fantastiche funzionalità che consente, con il bonus aggiuntivo che le variabili dichiarate utilizzando const sono di sola lettura. Sono un valore costante, il che significa che una volta assegnata una variabile con const, non può essere riassegnata:

const FAV_PET = "Gatti";
FAV_PET = "Cani";
La console visualizzerà un errore dovuto alla riassegnazione del valore di FAV_PET.
Dovresti sempre nominare le variabili che non vuoi riassegnare usando la parola chiave const. Questo aiuta quando si tenta accidentalmente di riassegnare una variabile che dovrebbe rimanere costante.
Nota: è comune per gli sviluppatori utilizzare identificatori di variabili maiuscole per valori immutabili e minuscoli o camelCase per valori mutabili (oggetti e matrici).
--
Aggiungi due numeri con JavaScript
Numero è un tipo di dati in JavaScript che rappresenta dati numerici.

JavaScript utilizza il simbolo + come operatore di addizione quando posizionato tra due numeri. Esempio:
const myVar = 5 + 10;
myVar ora ha il valore 15.
---
Sottrai un numero da un altro con JavaScript
Possiamo anche sottrarre un numero da un altro.
JavaScript utilizza il simbolo - per la sottrazione. Esempio:
const myVar = 12 - 6;
myVar avrebbe il valore 6.
---
Moltiplica due numeri con JavaScript
Possiamo anche moltiplicare un numero per un altro.
JavaScript utilizza il simbolo * per la moltiplicazione di due numeri. Esempio:
const myVar = 13 * 13;
myVar avrebbe il valore 169.
---
Dividi un numero per un altro con JavaScript
Possiamo anche dividere un numero per un altro.
JavaScript usa il simbolo / per la divisione. Esempio:
const myVar = 16 / 2;
myVar ora ha il valore 8.
---
Incrementa un numero con JavaScript
Puoi facilmente incrementarne o aggiungerne uno a una variabile con l'operatore ++.
i++;
è l'equivalente di
io = io + 1;
Nota: l'intera riga diventa i++;, eliminando la necessità del segno di uguale.
(ovviamente va prima assegnatogli il valore NUMERICO alla variabile.
let myVar = 87;
myVar++;
---
Decrementa un numero con JavaScript
Puoi facilmente decrementare o diminuire una variabile di uno con l'operatore --.
io--;
è l'equivalente di
io = io - 1;
Nota: l'intera riga diventa i--;, eliminando la necessità del segno di uguale.
let myVar = 11;
myVar --;
---
Crea numeri decimali con JavaScript
Possiamo anche memorizzare numeri decimali nelle variabili. I numeri decimali sono talvolta indicati come numeri in virgola mobile o float.
Nota: quando si calcolano i numeri, vengono calcolati con precisione finita. Le operazioni che utilizzano virgola mobile possono portare a risultati diversi rispetto al risultato desiderato. Se ottieni uno di questi risultati, apri un argomento sul forum di freeCodeCamp.
let myDecimal = 5.7;
---
Moltiplica due decimali con JavaScript
In JavaScript, puoi anche eseguire calcoli con numeri decimali, proprio come i numeri interi.
Moltiplichiamo due decimali insieme per ottenere il loro prodotto.
Modificare 0.0 in modo che il prodotto sia uguale a 5.0.
const product = 2.0 * 2.5; (ris: 5.0)
---
Dividi un decimale per un altro con JavaScript
Ora dividiamo un decimale per un altro.
Modificare 0,0 in modo che il quoziente sia uguale a 2,2.
4.4 / 2.0; (ris:2,2)
---
Trovare un resto in JavaScript
L'operatore resto % fornisce il resto della divisione di due numeri. Esempio:
5 % 2 = 1 perché
Math.floor(5 / 2) = 2 (Quoziente)
2 * 2 = 4
5 - 4 = 1 (Resto)
Utilizzo
In matematica, un numero può essere verificato come pari o dispari controllando il resto della divisione del numero per 2.

17 % 2 = 1 (17 è dispari)
48 % 2 = 0 (48 è pari)
Nota: l'operatore resto viene talvolta erroneamente chiamato operatore modulo. È molto simile al modulo, ma non funziona correttamente con i numeri negativi.
Impostare il resto uguale al resto di 11 diviso per 3 utilizzando l'operatore resto (%).
const remainder = 11 % 3; (abbiamo assegnato lo scarto di 2 alla variabile)
---
 Ricordiamo che tutto ciò che si trova a destra del segno di uguale viene valutato per primo, quindi possiamo dire: myVar = myVar + 5;. Esistono operatori che eseguono sia un'operazione matematica che un'assegnazione in un unico passaggio.
Uno di questi è l'operatore +=. let myVar = 1;
myVar += 5;

let a = 3;
let b = 17;
let c = 12;
// Only change code below this line
a += 12;
b += 9;
c +=7;
---
Assegnazione composta con sottrazione aumentata
Come l'operatore +=, anche -= sottrae un numero da una variabile.
myVar = myVar - 5;          sottrae 5 da myVar.
 Questo può essere riscritto come: myVar -= 5;
let a = 11;
let b = 9;
let c = 3;
// Only change code below this line
a -= 6;
b -= 15;
c -= 1;
---
L'operatore *= moltiplica una variabile per un numero.
myVar = myVar * 5;  moltiplica myVar per 5.
 Questo può essere riscritto come:  myVar *= 5;
let a = 5;
let b = 12;
let c = 4.6;
// Only change code below this line
a *= 5;
b *= 3 ;
c *= 10;
---
Assegnazione Composta Con Divisione Aumentata
L'operatore /= divide una variabile per un altro numero.
miaVar = miaVar / 5;
Dividerà myVar per 5. Questo può essere riscritto come:
miaVar /= 5;
// Only change code below this line
a /= 12;
b /= 4;
c /= 11;
---
Quando si definisce una stringa è necessario iniziare e terminare con virgolette singole o doppie.
In JavaScript, puoi evitare che una citazione la consideri come una virgoletta di fine stringa inserendo una barra rovesciata (\) davanti alla virgoletta.
const sampleStr = "Alan ha detto, \"Peter sta imparando JavaScript\".";
Console: = Alan ha detto, "Peter sta imparando JavaScript".
(notare la barra a sinistra che si usa in questi casi)
---
Stringhe di citazioni con virgolette singole
I valori stringa in JavaScript possono essere scritti con virgolette singole o doppie, purché inizi e finisca con lo stesso tipo di virgolette.
const myStr = "<a href=\"http://www.example.com\" target=\"_blank\">Link</a>";
const myStr = '<a href="http://www.example.com" target="_blank">Link</a>'; (corretto)
----
Sequenze di escape nelle stringhe
Le virgolette non sono gli unici caratteri a cui è possibile eseguire l'escape all'interno di una stringa. Ci sono due ragioni per usare i caratteri di escape:

Per consentirti di utilizzare caratteri che potresti non essere altrimenti in grado di digitare, come un ritorno a capo.
Per consentirti di rappresentare più virgolette in una stringa senza che JavaScript interpreti erroneamente ciò che intendi.
Lo abbiamo imparato nella sfida precedente.

Code	Output
\'	single quote
\"	double quote
\\	backslash
\n	newline
\r	carriage return
\t	tab
\b	word boundary
\f	form feed

Si noti che la barra rovesciata stessa deve essere sottoposta a escape per essere visualizzata come barra rovesciata.
const myStr = 
"FirstLine\n\t\\SecondLine\nThirdLine";

Console:
FirstLine
	\SecondLine
ThirdLine
---
Stringhe concatenate con operatore Plus +
In JavaScript, quando l'operatore + viene utilizzato con un valore String, viene chiamato operatore di concatenazione. Puoi creare una nuova stringa da altre stringhe concatenandole insieme.
const myStr = "This is the start." + " " + "This is the end.";
console:
This is the start. This is the end.
---
Stringhe concatenate con l'operatore Plus Equals
Possiamo anche usare l'operatore += per concatenare una stringa alla fine di una variabile stringa esistente. Questo può essere molto utile per spezzare una lunga stringa su più righe.
let myStr = "This is the first sentence. ";
myStr += "This is the second sentence.";
Console: "This is the first sentence. ";
myStr += This is the first sentence. This is the second sentence.
---
Costruire stringhe con variabili
A volte sarà necessario costruire una stringa. Utilizzando l'operatore di concatenazione (+), puoi inserire una o più variabili in una stringa che stai creando.
const myName = "mauro";
const myStr = "My name is" + myName + "I am well!";
---
Proprio come possiamo costruire una stringa su più righe da stringhe letterali, possiamo anche aggiungere variabili a una stringa usando l'operatore più uguale (+=).
esempio:
const someAdjective = "awesome";
let myStr = "Learning to code is ";
myStr += someAdjective;
---
Trova la lunghezza di una stringa
Puoi trovare la lunghezza di un valore String scrivendo .length dopo la variabile stringa o la stringa letterale.
console.log("Alan Peter".length);
console: 10 (conta effettivamente quante lettere ci sono nella stringa comp spazi bianchi)
exercise:
// Setup
let lastNameLength = 0;
const lastName = "Lovelace";
// Only change code below this line
lastNameLength = lastName.length;
---
Usa la notazione tra parentesi per trovare il primo carattere in una stringa
La notazione tra parentesi è un modo per ottenere un carattere in un indice specifico all'interno di una stringa.
La maggior parte dei linguaggi di programmazione moderni, come JavaScript, non iniziano a contare da 1 come fanno gli umani. Iniziano da 0. Questa operazione viene definita indicizzazione in base zero.
// Setup
let firstLetterOfLastName = "";
const lastName = "Lovelace";

// Only change code below this line
firstLetterOfLastName = lastName[0];
console.log(firstLetterOfLastName)
console: L (riferito alla prima lettera della costante lastName("lovelace")
---
Comprendere l'immutabilità delle stringhe
In JavaScript, i valori String sono immutabili, il che significa che non possono essere modificati una volta creati.
Ad esempio, il seguente codice:
let myStr = "Bob";
myStr[0] = "J";
non è possibile modificare il valore di myStr in Job, perché il contenuto di myStr non può essere modificato. Si noti che questo non significa che myStr non può essere modificato, ma solo che i singoli caratteri di una stringa letterale non possono essere modificati. L'unico modo per cambiare myStr sarebbe assegnarlo con una nuova stringa, come questa:
let myStr = "Bob";
myStr = "Lavoro";

example:
let myStr = "jello World";
myStr = "Hello World";  (semplicemente la riassegnamo)
console.log(myStr) (result: Hello World)
---
Usa la notazione tra parentesi per trovare il  carattere in una stringa
Puoi anche usare la notazione tra parentesi per ottenere il carattere in altre posizioni all'interno di una stringa.
const lastName = "Lovelace";  (0L, 1o,2v,3e ecc ecc)
Trova la lettera V

const thirdLetterOfLastName = lastName[2]; 
console: v
---
Usa la notazione tra parentesi per trovare l'ultimo carattere in una stringa
Per ottenere l'ultima lettera di una stringa, puoi sottrarne una dalla lunghezza della stringa.

const lastName = "Lovelace";
const lastLetterOfLastName = lastName[lastName.length - 1];
---
Puoi ottenere il valore della terzultima lettera della stringa const firstName = "Augusta" utilizzando firstName[firstName.length - 3]

esempio:
const lastName = "Lovelace";
const secondToLastLetterOfLastName = lastName[lastName.length - 2];
Console: C
----
Spazi vuoti di parole
Ti vengono fornite frasi con alcune parole mancanti, come nomi, verbi, aggettivi e avverbi. Quindi riempi i pezzi mancanti con parole a tua scelta in modo che la frase completata abbia un senso. Exercise: Formiamo una frase compiuta che abbia un senso

const myNoun = "dog";
const myAdjective = "big";
const myVerb = "ran";
const myAdverb = "quickly";

const wordBlanks  =  myNoun + " " + "is very" + " " + myAdjective + " " + "and" + " " + myVerb + " " + "fast and" + " " + myAdverb;";

console: dog is very big and ran fast and quickly
---
Memorizza più valori in una variabile utilizzando gli array JavaScript
Con le variabili array JavaScript, possiamo archiviare diversi dati in un unico posto.
(crea una stringa ed un numero nell'array)

const myArray = ["macchine", 8];
---
Annida un array all'interno di un altro array
Puoi anche annidare array all'interno di altri array, come di seguito:
const squadre = [["Bulls", 23], ["White Sox", 45]];
Questo è anche chiamato un array multidimensionale.
const myArray = [["macchine", 10], ["ruote", 20]];
console: (2) [Array(2), Array(2)]
---
Accedi ai dati dell'array con gli indici
Possiamo accedere ai dati all'interno degli array usando gli indici.
Gli indici di matrice vengono scritti con la stessa notazione tra parentesi utilizzata dalle stringhe, tranne per il fatto che invece di specificare un carattere, specificano una voce nella matrice. Come le stringhe, gli array utilizzano l'indicizzazione in base zero, quindi il primo elemento in un array ha un indice di 0.

Crea una variabile chiamata myData e impostala in modo che sia uguale al primo valore di myArray usando la notazione tra parentesi.

const myArray = [50, 60, 70];
const myData = myArray[0];
console.log(myData) result: 50
---
Modifica i dati dell'array con gli indici
A differenza delle stringhe, le voci degli array sono mutabili e possono essere modificate liberamente, anche se l'array è stato dichiarato con const.
Esempio:

const ourArray = [50, 40, 30];
ourArray[0] = 15;
ourArray ora ha il valore [15, 40, 30].
---
Accedi a matrici multidimensionali con indici
Un modo per pensare a un array multidimensionale è come un array di array. Quando utilizzi le parentesi per accedere all'array, il primo set di parentesi si riferisce alle voci nell'array più esterno (il primo livello) e ogni coppia aggiuntiva di parentesi si riferisce al livello successivo di voci all'interno.
Example:

const arr = [
  [1, 2, 3],
  [4, 5, 6],
  [7, 8, 9],
  [[10, 11, 12], 13, 14]
];
arr[3];
arr[3][0];
arr[3][0][1];
arr[3] is [[10, 11, 12], 13, 14], arr[3][0] is [10, 11, 12], and arr[3][0][1] is 11.

exercise:
Usando la notazione tra parentesi, seleziona un elemento da myArray in modo tale che myData sia uguale a 8.

const myArray = [
  [1, 2, 3],
  [4, 5, 6],
  [7, 8, 9],
  [[10, 11, 12], 13, 14],
];

const myData = myArray[2][1]; (il primo valore sta per il terzo array ed il secondo per il num 8)
console.log(myData) (risultato 8);
---
Manipola gli array con push()
Un modo semplice per aggiungere dati alla fine di un array è tramite la funzione push().
.push() prende uno o più parametri e li "spinge" alla fine dell'array.
Esempi:

const arr1 = [1, 2, 3];
arr1.push(4);
console: 1,2,3,4
altro es:
const arr2 = ["Stimpson", "J", "gatto"];
arr2.push(["felice", "gioia"]);
arr1 ora ha il valore [1, 2, 3, 4] e arr2 ha il valore ["Stimpson", "J", "cat", ["happy", "joy"]].

exercise:
Spingere ["dog", 3] alla fine della variabile myArray.

const myArray = [["John", 23], ["cat", 2]];
myArray.push(["dog", 3]);
Console: (3) [Array(2), Array(2), Array(2)]
---
Manipola gli array con pop()
Un altro modo per modificare i dati in un array è con la funzione .pop().

.pop() viene utilizzato per estrarre un valore dalla fine di un array. Possiamo memorizzare questo valore saltato assegnandolo a una variabile. In altre parole, .pop() rimuove l'ultimo elemento da un array e restituisce quell'elemento.
Qualsiasi tipo di voce può essere estratto da un array: numeri, stringhe, persino array nidificati.

const treArr = [1, 4, 6];
const oneDown = threeArr.pop(); (sottrae l'ultimo array, ovvero il 6)
console.log(oneDown);
console.log(treArr);
Il primo console.log visualizzerà il valore 6 e il secondo visualizzerà il valore [1, 4].

Utilizzare la funzione .pop() per rimuovere l'ultimo elemento da myArray e assegnare il valore estratto a una nuova variabile, removedFromMyArray.
const myArray = [["John", 23], ["cat", 2]];
const removedFromMyArray = myArray.pop();
console.log(myArray) [Array(2)]
----
Manipola gli array con shift()
pop() rimuove sempre l'ultimo elemento di un array. E se volessi rimuovere il primo?
È qui che entra in gioco .shift(). Funziona proprio come .pop(), tranne per il fatto che rimuove il primo elemento anziché l'ultimo.
Esempio:
const ourArray = ["Stimpson", "J", ["cat"]];
const rimossoFromOurArray = ourArray.shift();

removeFromOurArray avrebbe un valore della stringa Stimpson e ourArray avrebbe ["J", ["cat"]].

Exercise:
Utilizzare la funzione .shift() per rimuovere il primo elemento da myArray e assegnare il valore "shifted off" a una nuova variabile, removedFromMyArray.

const myArray = [["John", 23], ["dog", 3]];
const removedFromMyArray = myArray.shift();
console.log(myArray):  [Array(2)]
----
Manipola gli array con unshift()
Non solo puoi spostare gli elementi dall'inizio di un array, puoi anche annullare lo spostamento degli elementi all'inizio di un array, ovvero aggiungere elementi davanti all'array.
.unshift() funziona esattamente come .push(), ma invece di aggiungere l'elemento alla fine dell'array, unshift() aggiunge l'elemento all'inizio dell'array.
Esempio:
const ourArray = ["Stimpson", "J", "cat"];
ourArray.shift();
ourArray.unshift("Felice");
Dopo lo spostamento, ourArray avrà il valore ["J", "cat"]. Dopo lo spostamento, ourArray avrà il valore ["Happy", "J", "cat"].
Aggiungi ["Paul", 35] all'inizio della variabile myArray usando unshift().
const myArray = [["John", 23], ["dog", 3]];
myArray.shift();
myArray.unshift(["Paul", 35]);
===
Crea una lista della spesa nella variabile myList. L'elenco dovrebbe essere un array multidimensionale contenente diversi sottoarray.
Il primo elemento in ogni sottoarray dovrebbe contenere una stringa con il nome dell'elemento. Il secondo elemento dovrebbe essere un numero che rappresenta la quantità, ad es.
["Barra di cioccolato", 15]
Dovrebbero esserci almeno 5 sottoarray nell'elenco.
Exercise:
const myList = [["Pane", 1], ["farina", 2], ["pesce", 15], ["succhi", 2], ["acqua",2]];
=======
Scrivi JavaScript riutilizzabile con Funzioni
In JavaScript, possiamo dividere il nostro codice in parti riutilizzabili chiamate funzioni.
Ecco un esempio di una funzione:
funzione nomefunzione() {
   console.log("Hello World");
}
Puoi chiamare o invocare questa funzione usando il suo nome seguito da parentesi, in questo modo: functionName(); Ogni volta che la funzione viene chiamata, verrà stampato il messaggio Hello World sulla console di sviluppo. Tutto il codice tra parentesi graffe verrà eseguito ogni volta che viene chiamata la funzione.
Crea una funzione chiamata reusableFunction che stampa la stringa Hi World sulla console di sviluppo, e chiama la funzione.
function reusableFunction() {
  console.log("Hi World");
}
function reusableFunction(); (richiamiamo la funzione)
====
Passaggio di valori a funzioni con argomenti
I parametri sono variabili che fungono da segnaposto per i valori che devono essere immessi in una funzione quando viene chiamata.
Quando viene definita una funzione, in genere viene definita insieme a uno o più parametri. I valori effettivi che vengono immessi (o "passati") in una funzione quando viene chiamata sono noti come argomenti.
Ecco una funzione con due parametri, param1 e param2:

funzione testFun(param1, param2) {
  console.log(param1, param2);
}
Quindi possiamo chiamare testFun in questo modo: testFun("Hello", "World");. Abbiamo passato due argomenti stringa, Hello e World. All'interno della funzione, param1 sarà uguale alla stringa Hello e param2 sarà uguale alla stringa World. Nota che potresti chiamare nuovamente testFun con argomenti diversi e i parametri assumerebbero il valore dei nuovi argomenti.
Crea una funzione chiamata functionWithArgs che accetta due argomenti e restituisce la loro somma alla console di sviluppo.
Chiama la funzione con due numeri come argomenti.
(Waiting:functionWithArgs(1,2) dovrebbe produrre 3.
Waiting:functionWithArgs(7,9) dovrebbe produrre 16.
In attesa: dovresti chiamare functionWithArgs con due numeri dopo averlo definito.)
function functionWithArgs(param1, param2) {
console.log(param1 + param2);
}
functionWithArgs(7, 9);
===
Restituire un valore da una funzione con Return
Possiamo passare valori in una funzione con argomenti. È possibile utilizzare un'istruzione return per inviare un valore da una funzione.
Esempio
function plusThree(num) {
  return num + 3;
}
---
const answer = plusThree(5); (esempio di riassegnazione)
answer has the value 8.

plusThree accetta un argomento per num e restituisce un valore uguale a num + 3.
----
Crea una funzione timesFive che accetti un argomento, lo moltiplichi per 5 e restituisca il nuovo valore.
function timesFive(num) {
return num * 5;
}
===
Ambito e funzioni globali
In JavaScript, l'ambito si riferisce alla visibilità delle variabili. Le variabili definite al di fuori di un blocco funzione hanno l'ambito globale. Ciò significa che possono essere visti ovunque nel tuo codice JavaScript.
Le variabili dichiarate senza le parole chiave let o const vengono create automaticamente nell'ambito globale. Ciò può creare conseguenze indesiderate altrove nel codice o quando si esegue nuovamente una funzione. Dovresti sempre dichiarare le tue variabili con let o const.
Usando let o const, dichiara una variabile globale denominata myGlobal al di fuori di qualsiasi funzione. Inizializzalo con un valore di 10.
All'interno della funzione fun1, assegna 5 a oopsGlobal senza usare le parole chiave var, let o const.
exercise:
// Declare the myGlobal variable below this line
let myGlobal = 10
function fun1() {
  // Assign 5 to oopsGlobal Here
      oopsGlobal = 5
}
// Only change code above this line
function fun2() {
  var output = "";
  if (typeof myGlobal != "undefined") {
    output += "myGlobal: " + myGlobal;
  }
  if (typeof oopsGlobal != "undefined") {
    output += " oopsGlobal: " + oopsGlobal;
  }
  console.log(output);
}
====
Ambito e funzioni locali
Le variabili dichiarate all'interno di una funzione, così come i parametri della funzione, hanno un ambito locale. Ciò significa che sono visibili solo all'interno di quella funzione.
Ecco una funzione myTest con una variabile locale chiamata loc.
funzione mioTest() {
   const loc = "foo";
   console.log(loc);
}
mioTest();
console.log(loc);
La chiamata alla funzione myTest() visualizzerà la stringa foo nella console. La riga console.log(loc) (al di fuori della funzione myTest) genererà un errore, poiché loc non è definito al di fuori della funzione.

L'editor ha due console.logs per aiutarti a vedere cosa sta succedendo. Controlla la console mentre codifichi per vedere come cambia. Dichiara una variabile locale myVar all'interno di myLocalScope ed esegui i test.
Nota: la console visualizzerà ancora ReferenceError: myVar non è definito, ma ciò non causerà il fallimento dei test.

function myLocalScope() {
  // Only change code below this line
var myVar;
  console.log('inside myLocalScope', myVar);
}
myLocalScope();

// Run and check the console
// myVar is not defined outside of myLocalScope
console.log('outside myLocalScope', myVar);
===
Ambito globale e locale nelle funzioni
È possibile avere sia variabili locali che globali con lo stesso nome. Quando si esegue questa operazione, la variabile locale ha la precedenza sulla variabile globale.
In questo esempio:
const someVar = "Hat";

funzione myFun() {
   const someVar = "Head";
   return someVar;
}
La funzione myFun restituirà la stringa Head perché è presente la versione locale della variabile.
Aggiungi una variabile locale alla funzione myOutfit per sovrascrivere il valore di outerWear con la stringa string sweater..

const outerWear = "T-Shirt";
function myOutfit() {  
const outerWear = "sweater"  
  return outerWear;
}
myOutfit();
===
Comprensione del valore non definito restituito da una funzione
Una funzione può includere l'istruzione return ma non è necessario. Nel caso in cui la funzione non abbia un'istruzione return, quando la chiami, la funzione elabora il codice interno ma il valore restituito non è definito.
Esempio
let sum = 0;

function addSum(num) {
  sum = sum + num;
}

addSum(3);
addSum è una funzione senza un'istruzione return. La funzione cambierà la variabile di somma globale ma il valore restituito della funzione non è definito.

Crea una funzione addFive senza argomenti. Questa funzione aggiunge 5 alla variabile sum, ma il suo valore restituito non è definito.

let sum = 0;
function addThree() {
  sum = sum + 3;
}
function addFive() {
  sum += 5;  
}
addThree();
addFive();
===
Assegnazione con valore restituito
Se ricorderete dalla nostra discussione sulla memorizzazione dei valori con l'operatore di assegnazione, tutto ciò a destra del segno di uguale viene risolto prima che il valore venga assegnato. Ciò significa che possiamo prendere il valore di ritorno di una funzione e assegnarlo a una variabile.
Supponiamo di aver predefinito una funzione somma che somma due numeri insieme, quindi:
ourSum = sum(5, 12);
chiamerà la funzione sum, che restituisce un valore di 17 e lo assegna alla variabile ourSum.
exercise:
Chiama la funzione processArg con un argomento di 7 e assegna il suo valore di ritorno alla variabile elaborata.

let processed = 0;
function processArg(num) {
  return (num + 3) / 5;
}
processed = processArg(7)
===
Stare in fila
In Informatica una coda è una struttura dati astratta in cui gli elementi sono tenuti in ordine. Nuovi elementi possono essere aggiunti in fondo alla coda e quelli vecchi vengono rimossi dalla prima fila.

Scrivi una funzione nextInLine che accetta un array (arr) e un numero (item) come argomenti.
Aggiungi il numero alla fine dell'array, quindi rimuovi il primo elemento dell'array.

La funzione nextInLine dovrebbe quindi restituire l'elemento che è stato rimosso.

function nextInLine(arr, item) {
  arr.push(item)
  const removed = arr.shift()
  return removed;
}
const testArr = [1, 2, 3, 4, 5];

console.log("Before: " + JSON.stringify(testArr));
console.log(nextInLine(testArr, 6));
console.log("After: " + JSON.stringify(testArr));
Console: 
Before: [1,2,3,4,5]
1
After: [2,3,4,5,6]
=============
Comprendere i valori booleani
Un altro tipo di dati è il booleano. I booleani possono essere solo uno di due valori: vero o falso. Sono fondamentalmente piccoli interruttori on-off, dove true è attivo e falso è disattivato. Questi due stati si escludono a vicenda.
Nota: i valori booleani non vengono mai scritti tra virgolette. Le stringhe "true" e "false" non sono booleane e non hanno alcun significato speciale in JavaScript.
Modificare la funzione welcomeToBooleans in modo che restituisca true anziché false quando si fa clic sul pulsante Esegui.

function welcomeToBooleans() {
  return true; 
}
==============
Usa la logica condizionale con le istruzioni If
se le istruzioni vengono utilizzate per prendere decisioni nel codice. La parola chiave if indica a JavaScript di eseguire il codice tra parentesi graffe in determinate condizioni, definite tra parentesi. Queste condizioni sono note come condizioni booleane e possono essere solo vere o false.
Quando la condizione restituisce true, il programma esegue l'istruzione tra parentesi graffe. Quando la condizione booleana restituisce false, l'istruzione tra parentesi graffe non verrà eseguita.
Pseudocodice

if (la condizione è vera) {
  l'istruzione viene eseguita
}
Esempio

function test(myCondition) {
  if (la mia condizione) {
    return "Era vero";
  }
  return "Era falso";
}

test (vero);
test(falso);
test(true) restituisce la stringa Era vero e test(falso) restituisce la stringa Era falso.

Quando test viene chiamato con un valore true, l'istruzione if valuta myCondition per vedere se è true o meno. Poiché è vero, la funzione restituisce Era vero. Quando chiamiamo test con un valore di false, myCondition non è true e l'istruzione tra parentesi graffe non viene eseguita e la funzione restituisce Era false.

Crea un'istruzione if all'interno della funzione per restituire Sì, era vero se il parametro wasThatTrue è vero e restituisce No, altrimenti era falso.

function trueOrFalse(wasThatTrue) {
if(wasThatTrue === true) {
  return "Yes, that was true"
} return "No, that was false"
}
=============================
Confronto con l'operatore di uguaglianza
Ci sono molti operatori di confronto in JavaScript. Tutti questi operatori restituiscono un valore booleano vero o falso.
L'operatore più semplice è l'operatore di uguaglianza ==. L'operatore di uguaglianza confronta due valori e restituisce true se sono equivalenti o false in caso contrario. Si noti che l'uguaglianza è diversa dall'assegnazione (=), che assegna il valore a destra dell'operatore a una variabile a sinistra.

function equalityTest(myVal) {
  if (myVal == 10) {
    return "Equal";
  }
  return "Not Equal";
}

Se myVal è uguale a 10, l'operatore di uguaglianza restituisce true, quindi il codice tra parentesi graffe verrà eseguito e la funzione restituirà Equal. In caso contrario, la funzione restituirà Non uguale. Affinché JavaScript possa confrontare due diversi tipi di dati (ad esempio numeri e stringhe), deve convertire un tipo in un altro. Questo è noto come tipo coercizione. Una volta fatto, tuttavia, può confrontare i termini come segue:

1 == 1 // vero
1 == 2 // falso
1 == '1' // vero
"3" == 3 // vero

Aggiungi l'operatore di uguaglianza alla riga indicata in modo che la funzione restituisca la stringa Equal quando val è equivalente a 12.
function testEqual(val) {
  if (val == 12) { 
    return "Equal";
  }
  return "Not Equal";
}
testEqual(10);
=========================
Confronto con l'operatore Strict Equality
Strict Equality(===) è la controparte dell'operatore di uguaglianza (==). Tuttavia, a differenza dell'operatore di uguaglianza, che tenta di convertire entrambi i valori rispetto a un tipo comune, l'operatore di uguaglianza rigorosa non esegue una conversione di tipo.
Se i valori confrontati hanno tipi diversi, vengono considerati disuguali e l'operatore di uguaglianza rigorosa restituirà false.
Esempi
3 === 3 // vero
3 === '3' // falso
Nel secondo esempio, 3 è un tipo Numero e '3' è un tipo String.
Utilizzare l'operatore di uguaglianza rigorosa nell'istruzione if in modo che la funzione restituisca la stringa Equal quando val è rigorosamente uguale a 7.

function testStrict(val) {
  if (val === 7) { 
    return "Equal";
  }
  return "Not Equal";
}
testStrict(10);
============================
Esercitati a confrontare valori diversi
Nelle ultime due sfide, abbiamo appreso dell'operatore di uguaglianza (==) e dell'operatore di uguaglianza rigorosa (===). Facciamo una rapida rassegna e facciamo pratica usando questi operatori ancora un po'.
Se i valori confrontati non sono dello stesso tipo, l'operatore di uguaglianza eseguirà una conversione di tipo e quindi valuterà i valori. Tuttavia, l'operatore di uguaglianza rigorosa confronterà sia il tipo di dati che il valore così com'è, senza convertire un tipo nell'altro.
Esempi
3 == '3' restituisce true perché JavaScript esegue la conversione del tipo da stringa a numero. 3 === '3' restituisce false perché i tipi sono diversi e la conversione del tipo non viene eseguita.
Nota: in JavaScript, puoi determinare il tipo di una variabile o un valore con l'operatore typeof, come segue:
typeof 3
typeof '3'
typeof 3 restituisce il numero della stringa e typeof '3' restituisce la stringa stringa.
La funzione compareEquality nell'editor confronta due valori utilizzando l'operatore di uguaglianza. Modificare la funzione in modo che restituisca la stringa Uguale solo quando i valori sono rigorosamente uguali.

function compareEquality(a, b) {
  if (a === b) { 
    return "Equal";
  }
  return "Not Equal";
}
compareEquality(10, "10");
=================================
Confronto con l'operatore di disuguaglianza
L'operatore di disuguaglianza (!=) è l'opposto dell'operatore di uguaglianza. Significa non uguale e restituisce falso dove l'uguaglianza restituirebbe vero e viceversa. Come l'operatore di uguaglianza, l'operatore di disuguaglianza converte i tipi di dati dei valori durante il confronto.
Esempi
1 != 2 // vero
1 != "1" // falso
1 != '1' // falso
1 != vero // falso
0 != falso // falso
Aggiungi l'operatore di disuguaglianza != nell'istruzione if in modo che la funzione restituisca la stringa Non uguale quando val non è equivalente a 99.
function testNotEqual(val) {
  if (val!=99) { 
    return "Not Equal";
  }
  return "Equal";
}

testNotEqual(10);
=============================
Confronto con l'operatore Strict Inequality
L'operatore di disuguaglianza rigorosa (!==) è l'opposto logico dell'operatore di uguaglianza rigorosa. Significa "Strictly Not Equal" e restituisce false dove l'uguaglianza rigorosa restituirebbe true e viceversa. L'operatore di disuguaglianza rigorosa non convertirà i tipi di dati.
Esempi
3 !== 3 // falso
3 !== '3' // vero
4 !== 3 // vero
Aggiungi l'operatore di disuguaglianza rigorosa all'istruzione if in modo che la funzione restituisca la stringa Not Equal quando val non è rigorosamente uguale a 17

function testStrictNotEqual(val) {
  if (val!==17) {
    return "Not Equal";
  }
  return "Equal";
}
testStrictNotEqual(10);
========================================
Confronto con l'operatore Greater Than
L'operatore maggiore di (>) confronta i valori di due numeri. Se il numero a sinistra è maggiore del numero a destra, restituisce true. In caso contrario, restituisce false.
Come l'operatore di uguaglianza, l'operatore maggiore di convertirà i tipi di dati dei valori durante il confronto.
Esempi
5 > 3 // vero
7 > '3' // vero
2 > 3 // falso
'1' > 9 // falso
Aggiungi l'operatore maggiore di alle righe indicate in modo che le istruzioni di ritorno abbiano senso.
function testGreaterThan(val) {
  if (val>100) {  
    return "Over 100";
  }
  if (val>10) {  
    return "Over 10";
  }
  return "10 or Under";
}
testGreaterThan(10);
===============================================
Confronto con l'operatore maggiore di o uguale a
L'operatore maggiore o uguale a (>=) confronta i valori di due numeri. Se il numero a sinistra è maggiore o uguale al numero a destra, restituisce true. In caso contrario, restituisce false.
Come l'operatore di uguaglianza, l'operatore maggiore o uguale a convertirà i tipi di dati durante il confronto.
Esempi
6 >= 6 // vero
7 >= '3' // vero
2 >= 3 // falso
'7' >= 9 // falso
Aggiungi l'operatore maggiore o uguale a alle righe indicate in modo che le istruzioni di ritorno abbiano senso.
function testGreaterOrEqual(val) {
  if (val>=20) {  // Change this line
    return "20 or Over";
  }
  if (val>=10) {  // Change this line
    return "10 or Over";
  }
  return "Less than 10";
}
testGreaterOrEqual(10);
============================================
Confronto con l'operatore Less Than
L'operatore minore di (<) confronta i valori di due numeri. Se il numero a sinistra è minore del numero a destra, restituisce true. In caso contrario, restituisce false. Come l'operatore di uguaglianza, l'operatore minore di converte i tipi di dati durante il confronto.
Esempi
2 < 5 // vero
'3' < 7 // vero
5 < 5 // falso
3 < 2 // falso
'8' < 4 // falso
Aggiungi l'operatore minore di alle righe indicate in modo che le istruzioni di ritorno abbiano senso.
function testLessThan(val) {
  if (val<25) {  // Change this line
    return "Under 25";
  }
  if (val<55) {  // Change this line
    return "Under 55";
  }
  return "55 or Over";
}
testLessThan(10);
=========================================
Confronto con l'operatore  Less Than Or Equal to
L'operatore minore o uguale a (<=) confronta i valori di due numeri. Se il numero a sinistra è minore o uguale al numero a destra, restituisce true. Se il numero a sinistra è maggiore del numero a destra, restituisce false. Come l'operatore di uguaglianza, l'operatore minore o uguale a converte i tipi di dati.
Esempi
4 <= 5 // vero
'7' <= 7 // vero
5 <= 5 // vero
3 <= 2 // falso
'8' <= 4 // falso
Aggiungi l'operatore minore o uguale a alle righe indicate in modo che le istruzioni di ritorno abbiano senso.
function testLessOrEqual(val) {
  if (val<=12) {  // Change this line
    return "Smaller Than or Equal to 12";
  }
  if (val<=24) {  // Change this line
    return "Smaller Than or Equal to 24";
  }
  return "More Than 24";
}
testLessOrEqual(10);
================================================
Confronti con l'operatore logico and (&&)
A volte dovrai testare più di una cosa alla volta. L'operatore logico e (&&) restituisce true se e solo se gli operandi a sinistra ea destra di esso sono veri.
Lo stesso effetto potrebbe essere ottenuto annidando un'istruzione if all'interno di un'altra if:

if (num > 5) {
  if (num < 10) {
    return "Yes";
  }
}
return "No";restituirà Sì solo se num è maggiore di 5 e minore di 10. La stessa logica può essere scritta come:

if (num > 5 && num < 10) {
  return "Yes";
}
return "No";

Sostituisci le due istruzioni if ​​con un'unica istruzione, utilizzando l'operatore &&, che restituirà la stringa Sì se val è minore o uguale a 50 e maggiore o uguale a 25. In caso contrario, restituirà la stringa No.

function testLogicalAnd(val) {
  if (val <= 50 && val >= 25) {
      return "Yes";
    }
  return "No";
}
testLogicalAnd(10);
=======================================================
Confronti con l'operatore logico or
L'operatore logico or (||) restituisce true se uno degli operandi è true. In caso contrario, restituisce false.
L'operatore logico o è composto da due simboli pipe: (||). Questo può essere generalmente trovato tra i tasti Backspace e Invio.
Lo schema seguente dovrebbe sembrare familiare dai waypoint precedenti:

if (num > 10) {
  return "No";
}
if (num < 5) {
  return "No";
}
return "Yes";
will return Yes only if num is between 5 and 10 (5 and 10 included). The same logic can be written as:

if (num > 10 || num < 5) {
  return "No";
}
return "Yes";
Combina le due istruzioni if ​​in un'unica istruzione che restituisce la stringa Outside se val non è compreso tra 10 e 20 inclusi. Altrimenti, restituisci la stringa Inside.

function testLogicalOr(val) {
  if (val < 10 || val > 20) {
    return "Outside";
  }
  return "Inside";
}
testLogicalOr(15);
===============================
Introducing Else Statements
Quando una condizione per un'istruzione if è vera, viene eseguito il blocco di codice che la segue. E quando quella condizione è falsa? Normalmente non succederebbe nulla. Con un'istruzione else, è possibile eseguire un blocco di codice alternativo.

if (num > 10) {
  return "Bigger than 10";
} else {
  return "10 or Less";
}
Combina le istruzioni if in una singola istruzione if/else.
function testElse(val) {
  let result = "";
  
  if (val > 5) {
    result = "Bigger than 5";
  } else {
    result = "5 or Smaller";
  }
  
  return result;
}
testElse(4);
===================================
Introducing Else If Statements
Se hai più condizioni che devono essere affrontate, puoi concatenare le istruzioni if insieme alle istruzioni else if.

if (num > 15) {
  return "Bigger than 15";
} else if (num < 5) {
  return "Smaller than 5";
} else {
  return "Between 5 and 15";
}
Converti la logica per usare le istruzioni else if.

function testElseIf(val) {
  if (val > 10) {
    return "Greater than 10";
  } else if(val < 5) {
     return "Smaller than 5";
  }else {
     return "Between 5 and 10";
  }
}
testElseIf(7);
==================================
Ordine logico nelle istruzioni If Else
L'ordine è importante nelle affermazioni if, else if.
La funzione viene eseguita dall'alto verso il basso, quindi dovrai stare attento a quale istruzione viene prima.
Prendi queste due funzioni come esempio.
Ecco il primo:
function foo(x) {
  if (x < 1) {
    return "Less than one";
  } else if (x < 2) {
    return "Less than two";
  } else {
    return "Greater than or equal to two";
  }
}
E il secondo cambia semplicemente l'ordine delle affermazioni:
function bar(x) {
  if (x < 2) {
    return "Less than two";
  } else if (x < 1) {
    return "Less than one";
  } else {
    return "Greater than or equal to two";
  }
}
Sebbene queste due funzioni sembrino quasi identiche, se passiamo un numero a entrambe otteniamo output diversi.
pippo(0)
barra(0)
foo(0) restituirà la stringa Minore di uno e bar(0) restituirà la stringa Minore di due.

Modificare l'ordine della logica nella funzione in modo che restituisca le istruzioni corrette in tutti i casi.
function orderMyLogic(val) {
  if (val < 5) {
    return "Less than 5";
  } else if (val < 10) {
    return "Less than 10";
  } else {
    return "Greater than or equal to 10";
  }
}
orderMyLogic(7);
======================================
Concatenamento If Else Statements
Le istruzioni if/else possono essere concatenate insieme per una logica complessa. Ecco lo pseudocodice di più istruzioni if / else if concatenate:
if (condition1) {
  statement1
} else if (condition2) {
  statement2
} else if (condition3) {
  statement3
. . .
} else {
  statementN
}
Scrivi concatenate le dichiarazioni if/else if che soddisfano le seguenti condizioni:
function testSize(num) {
if(num < 5){
  return"Tiny";
} else if(num < 10){
  return"Small";
} else if(num < 15){
  return"Medium";
} else if(num < 20){
  return"Large";
} else {
  return"Huge";
}
}
testSize(7);
====================================
Codice del golf
Nel gioco del Golf, ogni buca ha un par, ovvero il numero medio di colpi che un giocatore dovrebbe fare per affondare la pallina nella buca per completare il gioco. A seconda di quanto sono al di sopra o al di sotto del par i tuoi colpi, c'è un soprannome diverso.

Alla tua funzione verranno passati argomenti par e strokes. Restituisce la stringa corretta secondo questa tabella che elenca i tratti in ordine di priorità; dall'alto (il più alto) al basso (il più basso):

Strokes	Return
1	"Hole-in-one!"
<= par - 2	"Eagle"
par - 1	"Birdie"
par	"Par"
par + 1	"Bogey"
par + 2	"Double Bogey"
>= par + 3	"Go Home!"

par e tratti saranno sempre numerici e positivi. Abbiamo aggiunto una serie di tutti i nomi per tua comodità.

const names = ["Hole-in-one!", "Eagle", "Birdie", "Par", "Bogey", "Double Bogey", "Go Home!"];

function golfScore(par, strokes) {
  
if (strokes == 1) {
  return "Hole-in-one!";
} else if (strokes <= par -2) {
  return "Eagle";
} else if (strokes == par - 1) {
  return "Birdie";
} else if (strokes == par) {
  return "Par";
} else if (strokes == par + 1) {
  return "Bogey"
} else if (strokes == par + 2) {
  return "Double Bogey";
} else {
  return "Go Home!"
}
}
golfScore(5, 4);
========================================
Selezione da molte opzioni con le istruzioni Switch
Se hai molte opzioni tra cui scegliere, usa un'istruzione switch. Un'istruzione switch verifica un valore e può avere molte istruzioni case che definiscono vari valori possibili. Le istruzioni vengono eseguite dal primo valore case corrispondente fino a quando non viene rilevata un'interruzione.

Ecco un esempio di un'istruzione switch:

switch (lettera minuscola) {
   case "a":
     console.log("A");
     break;
   case "b":
     console.log("B");
     break;
}
i valori case sono testati con uguaglianza stretta (===). L'interruzione dice a JavaScript di interrompere l'esecuzione delle istruzioni. Se l'interruzione viene omessa, verrà eseguita l'istruzione successiva.

Scrivi un'istruzione switch che verifica val e imposta la risposta per le seguenti condizioni:
1 - alfa
2 - beta
3 - gamma
4 - delta

function caseInSwitch(val) {
  let answer = "";
  
switch(val) {
  case 1:
  answer = "alpha";
  break
  case 2:
  answer = "beta"
  break
  case 3:
  answer = "gamma"
  break
  case 4:
  answer = "delta"
  break
}
  return answer;
}
caseInSwitch(1);
======================
Aggiunta di un'opzione predefinita nelle istruzioni Switch
In un'istruzione switch potresti non essere in grado di specificare tutti i valori possibili come istruzioni case. Invece, puoi aggiungere l'istruzione predefinita che verrà eseguita se non vengono trovate istruzioni case corrispondenti. Pensala come l'ultima dichiarazione else in una catena if/else.
Un'istruzione predefinita dovrebbe essere l'ultimo caso.

switch (num) {
  case value1:
    statement1;
    break;
  case value2:
    statement2;
    break;
...
  default:
    defaultStatement;
    break;
}
Scrivi un'istruzione switch per impostare la risposta per le seguenti condizioni:
a - apple
b - bird
c - cat
default - stuff
exercise:
function switchOfStuff(val) {
  let answer = "";
switch (val) {
  case "a":
    answer="apple";
    break;
  case "b":
    answer="bird";
    break;
  case "c":
    answer="cat";
    break;
    default:
    answer="stuff";
}
  return answer;
}
switchOfStuff(1);
=========
Opzioni identiche multiple nelle istruzioni Switch
Se l'istruzione break viene omessa dal caso di un'istruzione switch, le seguenti istruzioni case vengono eseguite fino a quando non viene rilevata un'interruzione. Se hai più input con lo stesso output, puoi rappresentarli in un'istruzione switch come questa:
let result = "";
switch (val) {
  case 1:
  case 2:
  case 3:
    result = "1, 2, or 3";
    break;
  case 4:
    result = "4 alone";
}
I casi per 1, 2 e 3 produrranno tutti lo stesso risultato.
Scrivi un'istruzione switch per impostare la risposta per i seguenti intervalli:
1-3 - Basso
4-6 - Mezzo
7-9 - Alto
Nota: sarà necessario disporre di un'istruzione case per ogni numero nell'intervallo.
exercise:
function sequentialSizes(val) {
  let answer = "";  
let result = "";
switch (val) {
  case 1:
  case 2:
  case 3:
    answer = "Low";
    break;
  case 4:
  case 5:
  case 6:
  answer = "Mid"
  break;
  case 7:
  case 8:
  case 9:
  answer = "High";
  break;    
}
  return answer;
}
sequentialSizes(1);
=====
Sostituzione delle catene If Else con Switch
Se hai molte opzioni tra cui scegliere, un'istruzione switch può essere più facile da scrivere rispetto a molte istruzioni if/else if concatenate. Il seguente:
if (val === 1) {
  answer = "a";
} else if (val === 2) {
  answer = "b";
} else {
  answer = "c";
}
può essere sostituito con:
switch (val) {
  case 1:
    answer = "a";
    break;
  case 2:
    answer = "b";
    break;
  default:
    answer = "c";
}
Cambia le istruzioni if/else if concatenate in un'istruzione switch.
function chainToSwitch(val) {
  let answer = "";
    if (val === "bob") {
    answer = "Marley";
  } else if (val === 42) {
    answer = "The Answer";
  } else if (val === 1) {
    answer = "There is no #1";
  } else if (val === 99) {
    answer = "Missed me by this much!";
  } else if (val === 7) {
    answer = "Ate Nine";
  }

  switch(val) {
    case "bob":
    answer = "Marley";
    break;
    case 42:
    answer = "The Answer";
    break;
    case 1:
    answer = "There is no #1";
    break;
    case 99:
    answer ="Missed me by this much!";
    break;
    case 7:
    answer = "Ate Nine";
    break;
  }
   return answer;
}
chainToSwitch(7);
===================
Restituzione di valori booleani da funzioni
Puoi ricordare da Confronto con l'operatore di uguaglianza che tutti gli operatori di confronto restituiscono un valore booleano vero o falso.
A volte le persone usano un'istruzione if/else per fare un confronto, come questo:
function isEqual(a, b) {
  if (a === b) {
    return true;
  } else {
    return false;
  }
}
Ma c'è un modo migliore per farlo. Poiché === restituisce true o false, possiamo restituire il risultato del confronto:
function isEqual(a, b) {
  return a === b;
}
Correggi la funzione isLess per rimuovere le istruzioni if/else.
function isLess(a, b) {  
    return a < b;
    return a > b;
}
isLess(10, 15);
===
Restituisce il modello iniziale per le funzioni
Quando viene raggiunta un'istruzione return, l'esecuzione della funzione corrente si interrompe e il controllo ritorna alla posizione chiamante.
Esempio
function myFun() {
  console.log("Hello");
  return "World";
  console.log("byebye")
}
myFun();
Quanto sopra visualizzerà la stringa Hello nella console e restituirà la stringa World. La stringa byebye non verrà mai visualizzata nella console, perché la funzione esce all'istruzione di ritorno.
Modificare la funzione abTest in modo che se aob sono minori di 0 la funzione esca immediatamente con un valore di undefined.
Suggerimento
Ricorda che undefined è una parola chiave, non una stringa.
function abTest(a, b) {
if(a<0 || b<0) {
  return undefined;
}
  return Math.round(Math.pow(Math.sqrt(a) + Math.sqrt(b), 2));
}
abTest(2,2);
====
Contare le carte
Nel gioco da casinò Blackjack, un giocatore può determinare se ha un vantaggio sulla mano successiva rispetto al banco tenendo traccia del numero relativo di carte alte e basse rimaste nel mazzo. Questo si chiama conteggio delle carte.
Avere più carte alte rimaste nel mazzo favorisce il giocatore. Ad ogni carta viene assegnato un valore secondo la tabella sottostante. Quando il conteggio è positivo, il giocatore dovrebbe scommettere alto. Quando il conteggio è zero o negativo, il giocatore dovrebbe scommettere basso.
Conta le carte cambio
+1            2, 3, 4, 5, 6
0              7, 8, 9
-1             10, 'J', 'Q', 'K', 'A'
Scriverai una funzione di conteggio delle carte. Riceverà un parametro della carta, che può essere un numero o una stringa, e aumenterà o diminuirà la variabile di conteggio globale in base al valore della carta (vedi tabella). La funzione restituirà quindi una stringa con il conteggio corrente e la stringa Bet se il conteggio è positivo, oppure Hold se il conteggio è zero o negativo. Il conteggio corrente e la decisione del giocatore (Bet o Hold) devono essere separati da un singolo spazio.
Output di esempio: -3 Hold o 5 Bet
Suggerimento
NON reimpostare il conteggio su 0 quando il valore è 7, 8 o 9.
NON restituire un array.
NON includere virgolette (singole o doppie) nell'output.
let count = 0;
function cc(card) {  
if(card <= 6){
  count +=1;
} else if(card == 10 || card == 'J' ||
     card == 'Q' || card == 'K' || card ==  'A') {
       count -= 1;
     }
if(count <=0 ) {
  return count + " Hold";
} else {
  return count + " Bet";
}
  return "Change Me";
}
cc(2); cc(3); cc(7); cc('K'); cc('A');
===
Crea oggetti JavaScript
Potresti aver già sentito il termine oggetto.
Gli oggetti sono simili agli array, tranne per il fatto che invece di utilizzare gli indici per accedere e modificare i loro dati, si accede ai dati negli oggetti tramite quelle che vengono chiamate proprietà.
Gli oggetti sono utili per archiviare i dati in modo strutturato e possono rappresentare oggetti del mondo reale, come un gatto.
Ecco un esempio di oggetto gatto:
const cat = {
  "name": "Whiskers",
  "legs": 4,
  "tails": 1,
  "enemies": ["Water", "Dogs"]
};
In questo esempio, tutte le proprietà vengono archiviate come stringhe, ad esempio nome, gambe e code. Tuttavia, puoi anche usare i numeri come proprietà. Puoi anche omettere le virgolette per le proprietà delle stringhe di una sola parola, come segue:
const anotherObject = {
  make: "Ford",
  5: "five",
  "model": "focus"
};
Tuttavia, se il tuo oggetto ha proprietà non stringa, JavaScript le typecast automaticamente come stringhe.
Crea un oggetto che rappresenti un cane chiamato myDog che contenga le proprietà nome (una stringa), zampe, code e amici.
Puoi impostare queste proprietà dell'oggetto su qualsiasi valore desideri, purché il nome sia una stringa, le gambe e le code siano numeri e gli amici siano un array.
const myDog = {
name: "Hyppo",
legs: 4,
tails: 80,
"friends": ["friends", "child", "cool"]  
};
===
Accesso alle proprietà dell'oggetto con la notazione del punto
Esistono due modi per accedere alle proprietà di un oggetto: notazione punto (.) e notazione parentesi ([]), simile a una matrice.
La notazione a punti è ciò che usi quando conosci il nome della proprietà a cui stai tentando di accedere in anticipo.
Ecco un esempio dell'utilizzo della notazione punto (.) per leggere la proprietà di un oggetto:
const myObj = {
  prop1: "val1",
  prop2: "val2"
};
const prop1val = myObj.prop1;
const prop2val = myObj.prop2;
prop1val avrebbe un valore della stringa val1 e 
prop2val avrebbe un valore della stringa val2.

Leggi i valori delle proprietà di testObj usando la notazione del punto. Impostare la variabile hatValue uguale alla proprietà hat dell'oggetto e impostare la variabile shirtValue uguale alla proprietà shirt dell'oggetto.
const testObj = {
  "hat": "ballcap",
  "shirt": "jersey",
  "shoes": "cleats"
};
const hatValue = testObj.hat;      // Change this line
const shirtValue = testObj.shirt;    // Change this line
===
Accesso alle proprietà dell'oggetto con la notazione tra parentesi
Il secondo modo per accedere alle proprietà di un oggetto è la notazione tra parentesi ([]). Se la proprietà dell'oggetto a cui stai tentando di accedere ha uno spazio nel nome, dovrai utilizzare la notazione tra parentesi.
Tuttavia, puoi ancora utilizzare la notazione tra parentesi sulle proprietà dell'oggetto senza spazi.
Ecco un esempio dell'utilizzo della notazione tra parentesi per leggere la proprietà di un oggetto:
const myObj = {
  "Space Name": "Kirk",
  "More Space": "Spock",
  "NoSpace": "USS Enterprise"
};
myObj["Space Name"];
myObj['More Space'];
myObj["NoSpace"];

Tieni presente che i nomi delle proprietà con spazi devono essere tra virgolette (singole o doppie).
Leggere i valori delle proprietà an entree e drink di testObj utilizzando la notazione tra parentesi e assegnarli rispettivamente a entreeValue e drinkValue.
const testObj = {
  "an entree": "hamburger",
  "my side": "veggies",
  "the drink": "water"
};
const entreeValue = testObj["an entree"];   
const drinkValue = testObj["the drink"];    
===
Accesso alle proprietà degli oggetti con le variabili
Un altro uso della notazione tra parentesi sugli oggetti consiste nell'accedere a una proprietà che è memorizzata come valore di una variabile. Questo può essere molto utile per scorrere le proprietà di un oggetto o quando si accede a una tabella di ricerca.
Ecco un esempio di utilizzo di una variabile per accedere a una proprietà:
const dogs = {
  Fido: "Mutt",
  Hunter: "Doberman",
  Snoopie: "Beagle"
};
const myDog = "Hunter";
const myBreed = dogs[myDog];
console.log(myBreed);
La stringa Doberman verrebbe visualizzata nella console.
Nota che non usiamo le virgolette attorno al nome della variabile quando la utilizziamo per accedere alla proprietà perché stiamo usando il valore della variabile, non il nome.

Imposta la variabile playerNumber su 16. Quindi, usa la variabile per cercare il nome del giocatore e assegnarlo al giocatore.
const testObj = {
  12: "Namath",
  16: "Montana",
  19: "Unitas"
};
const playerNumber = 16;
const player = testObj[playerNumber]; 
===
Aggiornamento delle proprietà dell'oggetto
Dopo aver creato un oggetto JavaScript, puoi aggiornarne le proprietà in qualsiasi momento proprio come aggiorneresti qualsiasi altra variabile. È possibile utilizzare la notazione punto o parentesi per aggiornare.

Ad esempio, diamo un'occhiata al nostro Cane:
const ourDog = {
  "name": "Camper",
  "legs": 4,
  "tails": 1,
  "friends": ["everything!"]
};
Dato che è un cane particolarmente felice, cambiamo il suo nome con la stringa Happy Camper. Ecco come aggiorniamo la proprietà del nome del suo oggetto: ourDog.name = "Happy Camper"; o ourDog["name"] = "Happy Camper"; Ora, quando valutiamo ourDog.name, invece di ottenere Camper, otterremo il suo nuovo nome, Happy Camper.
Aggiorna la proprietà del nome dell'oggetto myDog. Cambiamo il suo nome da Coder a Happy Coder. È possibile utilizzare la notazione punto o parentesi.
const myDog = {
  "name": "Coder",
  "legs": 4,
  "tails": 1,
  "friends": ["freeCodeCamp Campers"]
};
myDog.name = "Happy Coder";
===
Aggiungi nuove proprietà a un oggetto JavaScript
Puoi aggiungere nuove proprietà agli oggetti JavaScript esistenti nello stesso modo in cui li modificheresti.
Ecco come aggiungeremmo una proprietà corteccia al nostro cane:

ourDog.bark = "bow-wow";            or

ourDog["bark"] = "bow-wow";
Ora, quando valutiamo ourDog.bark, otterremo il suo abbaiare, bow-wow.
Example:

const ourDog = {
  "name": "Camper",
  "legs": 4,
  "tails": 1,
  "friends": ["everything!"]
};
ourDog.bark = "bow-wow";

Aggiungi una proprietà corteccia a myDog e impostala su un dog sound, ad esempio "woof". È possibile utilizzare la notazione punto o parentesi.
const myDog = {
  "name": "Happy Coder",
  "legs": 4,
  "tails": 1,
  "friends": ["freeCodeCamp Campers"]
};
myDog.bark = ["dog sound"];
===
Elimina proprietà da un oggetto JavaScript
Possiamo anche eliminare proprietà da oggetti come questo:
elimina ourDog.bark;
Esempio:
const nostro Cane = {
   "nome": "Camper",
   "gambe": 4,
   "code": 1,
   "amici": ["tutto!"],
   "bark": "bow-wow"
};
elimina ourDog.bark;
Dopo l'ultima riga mostrata sopra, ourDog appare come:
{
   "nome": "Camper",
   "gambe": 4,
   "code": 1,
   "amici": ["tutto!"]
}
Elimina la proprietà tails da myDog. È possibile utilizzare la notazione punto o parentesi.
const myDog = {
  "name": "Happy Coder",
  "legs": 4,
  "tails": 1,
  "friends": ["freeCodeCamp Campers"],
  "bark": "woof"
};
delete myDog.tails;
===
Utilizzo di oggetti per le ricerche
Gli oggetti possono essere pensati come una memoria chiave/valore, come un dizionario. Se si dispone di dati tabulari, è possibile utilizzare un oggetto per cercare valori anziché un'istruzione switch o una catena if/else. Questo è molto utile quando sai che i tuoi dati di input sono limitati a un certo intervallo.
Ecco un esempio di una semplice ricerca alfabetica inversa:
const alpha = {
  1:"Z",
  2:"Y",
  3:"X",
  4:"W",
  ...
  24:"C",
  25:"B",
  26:"A"
};
const thirdLetter = alpha[2];
const lastLetter = alpha[24];

const value = 2;
const valueLookup = alpha[value];
thirdLetter è la stringa Y, lastLetter è la stringa C e valueLookup è la stringa Y..
Converti l'istruzione switch in un oggetto chiamato lookup. Usalo per cercare val e assegnare la stringa associata alla variabile di risultato.
function phoneticLookup(val) {
  let result = "";  

  var lookup = {
    "alpha": "Adams",
    "bravo": "Boston",
    "charlie": "Chicago",
    "delta": "Denver",
    "echo": "Easy",
    "foxtrot": "Frank"
  }
   result = lookup[val];
  return result;
}
phoneticLookup("charlie");
===
Testare gli oggetti per le proprietà
A volte è utile verificare se la proprietà di un determinato oggetto esiste o meno. Possiamo usare il metodo .hasOwnProperty(propname) degli oggetti per determinare se quell'oggetto ha il nome della proprietà specificato. .hasOwnProperty() restituisce true o false se la proprietà viene trovata o meno.
Esempio:
const myObj = {
  top: "hat",
  bottom: "pants"
};

myObj.hasOwnProperty("top");
myObj.hasOwnProperty("middle");

Il primo hasOwnProperty restituisce true, mentre il secondo restituisce false.
Modificare la funzione checkObj per verificare se un oggetto passato alla funzione (obj) contiene una proprietà specifica (checkProp). Se la proprietà viene trovata, restituisci il valore di quella proprietà. In caso contrario, restituire "Non trovato".

function checkObj(obj, checkProp) {  
  if(obj.hasOwnProperty(checkProp)) {
    return obj[checkProp];
  } else {
    return "Not Found";
  }  
}}
===
Manipolazione di oggetti complessi
A volte potresti voler archiviare i dati in una struttura dati flessibile. Un oggetto JavaScript è un modo per gestire dati flessibili. Consentono combinazioni arbitrarie di stringhe, numeri, booleani, array, funzioni e oggetti.
Ecco un esempio di una struttura dati complessa:
const ourMusic = [  {
    "artist": "Daft Punk",
    "title": "Homework",
    "release_year": 1997,
    "formats": [ 
      "CD", 
      "Cassette", 
      "LP"
    ],
    "gold": true
  }
];
Questo è un array che contiene un oggetto all'interno. L'oggetto ha vari pezzi di metadati su un album. Ha anche una matrice di formati nidificati. Se desideri aggiungere più record di album, puoi farlo aggiungendo record all'array di livello superiore. Gli oggetti contengono i dati in una proprietà, che ha un formato chiave-valore. Nell'esempio sopra, "artista": "Daft Punk" è una proprietà che ha una chiave di artista e un valore di Daft Punk.
Nota: dovrai inserire una virgola dopo ogni oggetto nell'array, a meno che non sia l'ultimo oggetto nell'array.
Aggiungi un nuovo album all'array myMusic. Aggiungi le stringhe dell'artista e del titolo, il numero dell'anno di rilascio e una matrice di formati di stringhe.
const myMusic = [
  {
    "artist": "Billy Joel",
    "title": "Piano Man",
    "release_year": 1973,
    "formats": [
      "CD",
      "8T",
      "LP"
    ],
    "gold": true
  },
  {
    "artist": "Billy Joel",
    "title": "Piano Man",
    "release_year": 1973,
    "formats": [
      "CD",
      "8T",
      "LP"
    ]  } ];
===
Accesso agli oggetti nidificati
È possibile accedere alle sottoproprietà degli oggetti concatenando insieme la notazione punto o parentesi.
Ecco un oggetto annidato:
const ourStorage = {
  "desk": {
    "drawer": "stapler"
  },
  "cabinet": {
    "top drawer": { 
      "folder1": "a file",
      "folder2": "secrets"
    },
    "bottom drawer": "soda"
  }
};
ourStorage.cabinet["top drawer"].folder2;
ourStorage.desk.drawer;
ourStorage.cabinet["top drawer"].folder2 would be the string secrets, and ourStorage.desk.drawer would be the string stapler.
Accedere all'oggetto myStorage e assegnare il contenuto della proprietà del vano portaoggetti alla variabile gloveBoxContents. Usa la notazione del punto per tutte le proprietà ove possibile, altrimenti usa la notazione tra parentesi.
const myStorage = {
  "car": {
    "inside": {
      "glove box": "maps",
      "passenger seat": "crumbs"
     },
    "outside": {
      "trunk": "jack"
    }
  }
};
const gloveBoxContents = myStorage.car.inside["glove box"];
===
Accesso agli array nidificati
Come abbiamo visto negli esempi precedenti, gli oggetti possono contenere sia oggetti nidificati che array nidificati. Simile all'accesso agli oggetti nidificati, la notazione tra parentesi di matrice può essere concatenata per accedere alle matrici nidificate.
Ecco un esempio di come accedere a un array nidificato:
const ourPets = [
  {
    animalType: "cat",
    names: [
      "Meowzer",
      "Fluffy",
      "Kit-Cat"
    ]
  },
  {
    animalType: "dog",
    names: [
      "Spot",
      "Bowser",
      "Frankie"
    ]
  }
];
ourPets[0].names[1];
ourPets[1].names[0];
ourPets[0].names[1] would be the string Fluffy, and ourPets[1].names[0] would be the string Spot.
Usando la notazione con punto e parentesi, imposta la variabile secondTree sul secondo elemento nell'elenco degli alberi dall'oggetto myPlants.

const myPlants = [  {
    type: "flowers",
    list: [
      "rose",
      "tulip",
      "dandelion"
    ]  },
  {
    type: "trees",
    list: [
      "fir",
      "pine",
      "birch"
    ]  } ];
const secondTree = myPlants[1].list[1];
===
Raccolta di dischi
Ti viene dato un oggetto letterale che rappresenta una parte della tua collezione di album musicali. Ogni album ha un numero ID univoco come chiave e molte altre proprietà. Non tutti gli album hanno informazioni complete.
Inizi con una funzione updateRecords che prende un oggetto letterale, registra, contenente la raccolta di album musicali, un ID, un oggetto di scena (come artista o tracce) e un valore. Completare la funzione utilizzando le regole seguenti per modificare l'oggetto passato alla funzione.
La tua funzione deve sempre restituire l'intero oggetto della raccolta di record.
Se prop non è tracce e value non è una stringa vuota, aggiorna o imposta la prop di quell'album su value.
Se prop è tracce ma l'album non ha una proprietà tracce, crea un array vuoto e aggiungi valore ad esso.
Se prop è tracce e value non è una stringa vuota, aggiungi valore alla fine dell'array di tracce esistenti dell'album.
Se value è una stringa vuota, elimina la proprietà prop specificata dall'album.
Nota: per i test viene utilizzata una copia dell'oggetto recordCollection.
const recordCollection = {
  2548: {
    albumTitle: 'Slippery When Wet',
    artist: 'Bon Jovi',
    tracks: ['Let It Rock', 'You Give Love a Bad Name']
  },
  2468: {
    albumTitle: '1999',
    artist: 'Prince',
    tracks: ['1999', 'Little Red Corvette']
  },
  1245: {
    artist: 'Robert Palmer',
    tracks: []
  },
  5439: {
    albumTitle: 'ABBA Gold'
  } };
---
  function updateRecords(records, id, prop, value) {
      if(value == ""){
          delete records[id][prop];
      } else {
          if (prop != 'tracks'){
              records[id][prop] = value;
          } else {
              if(records[id].hasOwnProperty('tracks')){
                  records[id].tracks.push(value);
              } else {
                  records[id].tracks = [value];
              }  }   }
      return records;
    }  
  updateRecords(recordCollection, 5439, 'artist', 'ABBA');
===
Itera con JavaScript While Loops
Puoi eseguire lo stesso codice più volte usando un ciclo.

Il primo tipo di ciclo che impareremo è chiamato ciclo while perché viene eseguito mentre una condizione specificata è vera e si interrompe una volta che quella condizione non è più vera.

const ourArray = [];
let i = 0;

while (i < 5) {
  ourArray.push(i);
  i++;
}

Nell'esempio di codice sopra, il ciclo while verrà eseguito 5 volte e aggiungerà i numeri da 0 a 4 a ourArray.
Proviamo a far funzionare un ciclo while inserendo i valori in un array.
Aggiungi i numeri da 5 a 0 (inclusi) in ordine decrescente a myArray usando un ciclo while.
const myArray = [];
let i = 5;
while(i >= 0) {
  myArray.push(i);
  i--;
}
===
Iterare con JavaScript For Loops
Puoi eseguire lo stesso codice più volte usando un ciclo.
Il tipo più comune di ciclo JavaScript è chiamato ciclo for perché viene eseguito per un numero specifico di volte.
I cicli For sono dichiarati con tre espressioni facoltative separate da punto e virgola:
per (a; b; c), dove a è l'istruzione di inizializzazione, b è l'istruzione di condizione e c è l'espressione finale.
L'istruzione di inizializzazione viene eseguita una sola volta prima dell'avvio del ciclo. Viene in genere utilizzato per definire e impostare la variabile di ciclo.
L'istruzione di condizione viene valutata all'inizio di ogni iterazione del ciclo e continuerà finché restituisce true. Quando la condizione è falsa all'inizio dell'iterazione, il ciclo interrompe l'esecuzione. Ciò significa che se la condizione inizia come falsa, il tuo ciclo non verrà mai eseguito.
L'espressione finale viene eseguita alla fine di ogni iterazione del ciclo, prima del successivo controllo delle condizioni e viene solitamente utilizzata per incrementare o decrementare il contatore del ciclo.
Nell'esempio seguente inizializziamo con i = 0 e ripetiamo mentre la nostra condizione i < 5 è vera. Incrementeremo i di 1 in ogni iterazione del ciclo con i++ come nostra espressione finale.

const ourArray = [];
for (let i = 0; i < 5; i++) {
  ourArray.push(i);
}
ourArray will now have the value [0, 1, 2, 3, 4].
Utilizzare un ciclo for per inserire i valori da 1 a 5 su myArray.

const myArray = [];
for(let i = 0; i<5; i++) {
  myArray.push(i+1)
}
===
Itera i numeri dispari con un ciclo For
I cicli For non devono iterare uno alla volta. Modificando la nostra espressione finale, possiamo contare per numeri pari.
Inizieremo da i = 0 e ciclo mentre i < 10. Incrementeremo i di 2 ogni ciclo con i += 2.

const ourArray = [];
for (let i = 0; i < 10; i += 2) {
  ourArray.push(i);
}

ourArray ora conterrà [0, 2, 4, 6, 8]. Cambiamo la nostra inizializzazione in modo da poter contare con numeri dispari.
Spingi i numeri dispari da 1 a 9 su myArray usando un ciclo for.

const myArray = [];
for (let i = 1; i<= 9; i+= 2) {
  myArray.push(i);
}
===
Conta alla rovescia con un ciclo For
Un ciclo for può anche contare all'indietro, purché possiamo definire le giuste condizioni.
Per decrementare di due ogni iterazione, dovremo modificare la nostra inizializzazione, condizione ed espressione finale.
Inizieremo da i = 10 e ciclo mentre i > 0. Diminuiremo i di 2 ogni ciclo con i -= 2.

const ourArray = [];
for (let i = 10; i > 0; i -= 2) {
  ourArray.push(i);
}

ourArray ora conterrà [10, 8, 6, 4, 2]. Cambiamo la nostra inizializzazione e l'espressione finale in modo da poter contare all'indietro di due per creare una matrice di numeri dispari decrescenti.
Spingi i numeri dispari da 9 a 1 su myArray usando un ciclo for.

const myArray = [];
for (let i = 9; i >= 1; i -= 2) {
  myArray.push(i);
  }
===
Iterare attraverso un array con un ciclo For
Un'attività comune in JavaScript consiste nell'iterare il contenuto di un array. Un modo per farlo è con un ciclo for. Questo codice visualizzerà ogni elemento dell'array arr sulla console:

const arr = [10, 9, 8, 7, 6];
for (let i = 0; i < arr.length; i++) {
    console.log(arr[i]);
}

Ricorda che gli array hanno un'indicizzazione in base zero, il che significa che l'ultimo indice dell'array è lunghezza - 1. La nostra condizione per questo ciclo è i < arr.length, che interrompe il ciclo quando i è uguale a lunghezza. In questo caso l'ultima iterazione è i === 4 cioè quando i diventa uguale a arr.length - 1 e restituisce 6 alla console. Quindi i aumenta a 5 e il ciclo termina perché i < arr.length è falso.
Dichiara e inizializza una variabile total su 0. Usa un ciclo for per aggiungere il valore di ogni elemento dell'array myArr al totale.

const myArr = [2, 3, 4, 5, 6];
let total = 0;
for (let i = 0; i < myArr.length; i++) {
   console.log(myArr[i]);
   total += myArr[i];
}
===
Nidificazione per loop
Se si dispone di un array multidimensionale, è possibile utilizzare la stessa logica del waypoint precedente per scorrere sia l'array che qualsiasi sottoarray. Ecco un esempio:

const arr = [
   [1, 2], [3, 4], [5, 6]
];

for (let i = 0; i < arr.length; i++) {
   for (let j = 0; j < arr[i].lunghezza; j++) {
     console.log(arr[i][j]);
   }
}
Questo emette ogni sub-elemento in arr uno alla volta. Nota che per il ciclo interno, stiamo controllando la .length di arr[i], poiché arr[i] è esso stesso un array.

Modifica la funzione multiplyAll in modo che restituisca il prodotto di tutti i numeri nei sub-array di arr.

function multiplyAll(arr) {
  let product = 1;
for (let i = 0; i < arr.length; i++) {
  for (let j = 0; j < arr[i].length; j++) {
    product *= arr[i][j];
  }   }  
  return product;
}
multiplyAll([[1, 2], [3, 4], [5, 6, 7]]);
====
Iterare con JavaScript Do...While Loops
Il prossimo tipo di ciclo che imparerai è chiamato ciclo do...while. Si chiama ciclo do...while perché eseguirà prima un passaggio del codice all'interno del ciclo, indipendentemente da cosa, e quindi continuerà a eseguire il ciclo mentre la condizione specificata restituisce true.

const ourArray = [];
let i = 0;
do {
  ourArray.push(i);
  i++;
} while (i < 5);

L'esempio sopra si comporta in modo simile ad altri tipi di loop e l'array risultante sarà simile a [0, 1, 2, 3, 4]. Tuttavia, ciò che rende il fare... mentre diverso dagli altri cicli è il modo in cui si comporta quando la condizione fallisce al primo controllo. Vediamo questo in azione. Ecco un ciclo while regolare che eseguirà il codice nel ciclo finché i < 5:

const ourArray = []; 
let i = 5;
while (i < 5) {
  ourArray.push(i);
  i++; }

In questo esempio, inizializziamo il valore di ourArray su un array vuoto e il valore di i su 5. Quando eseguiamo il ciclo while, la condizione restituisce false perché i non è inferiore a 5, quindi non eseguiamo il codice all'interno il cappio. Il risultato è che ourArray finirà senza alcun valore aggiunto e apparirà ancora come [] quando tutto il codice nell'esempio sopra avrà completato l'esecuzione. Ora, dai un'occhiata a un ciclo do...while:

const ourArray = []; 
let i = 5;
do {
  ourArray.push(i);
  i++;
} while (i < 5);

In questo caso, inizializziamo il valore di i su 5, proprio come abbiamo fatto con il ciclo while. Quando arriviamo alla riga successiva, non c'è alcuna condizione da valutare, quindi andiamo al codice tra parentesi graffe ed eseguiamolo. Aggiungeremo un singolo elemento all'array e quindi incrementeremo i prima di arrivare al controllo delle condizioni. Quando finalmente valutiamo la condizione i < 5 sull'ultima riga, vediamo che ora i è 6, che fallisce il controllo condizionale, quindi usciamo dal ciclo e il gioco è fatto. Alla fine dell'esempio precedente, il valore di ourArray è [5]. In sostanza, un ciclo do...while assicura che il codice all'interno del ciclo venga eseguito almeno una volta. Proviamo a far funzionare un ciclo do...while spingendo i valori in un array.

Cambia il ciclo while nel codice in un ciclo do...while in modo che il ciclo invii solo il numero 10 a myArray e io sarò uguale a 11 quando il tuo codice avrà terminato l'esecuzione.

const myArray = [];
let i = 10;
do {
  myArray.push(i);
  i++;
}
while (i < 5);
===
Sostituisci i loop usando la Recursion
La ricorsione è il concetto che una funzione può essere espressa in termini di se stessa. Per aiutare a capire questo, inizia pensando al seguente compito: moltiplica i primi n elementi di un array per creare il prodotto di quegli elementi. Usando un ciclo for, potresti farlo:

function multiply(arr, n) {
    let product = 1;
    for (let i = 0; i < n; i++) {
      product *= arr[i];
    }
    return product;
  }

Tuttavia, si noti che moltiplica(arr, n) == moltiplica(arr, n - 1) * arr[n - 1]. Ciò significa che puoi riscrivere moltiplicare in termini di se stesso e non è mai necessario utilizzare un ciclo.

 function multiply(arr, n) {
    if (n <= 0) {
      return 1;
    } else {
      return multiply(arr, n - 1) * arr[n - 1];
    }  }

La versione ricorsiva di moltiplicare si scompone in questo modo. Nel caso base, dove n <= 0, restituisce 1. Per valori maggiori di n, chiama se stesso, ma con n - 1. Quella chiamata di funzione viene valutata allo stesso modo, chiamando di nuovo moltiplicare fino a n <= 0. A questo punto, tutte le funzioni possono tornare e la moltiplica originale restituisce la risposta.
Nota: le funzioni ricorsive devono avere un caso base quando ritornano senza chiamare nuovamente la funzione (in questo esempio, quando n <= 0), altrimenti non possono mai terminare l'esecuzione.
Scrivete una funzione ricorsiva, sum(arr, n), che restituisca la somma dei primi n elementi di un array arr.

function sum(arr, n) {  
if (n <= 0) {
  return 0;
} else {
  return sum(arr, n - 1) + arr[n - 1];
}  }
console.log(sum([1,2,3,4,5,6,7,8], 5));
===
Ricerca profilo
Abbiamo una serie di oggetti che rappresentano persone diverse nei nostri elenchi di contatti.
Una funzione lookUpProfile che prende il nome e una proprietà (prop) come argomenti è stata prescritta per te.
La funzione dovrebbe verificare se name è il firstName di un contatto effettivo e la proprietà data (prop) è una proprietà di quel contatto.
Se entrambi sono veri, restituisci il "valore" di quella proprietà.
Se il nome non corrisponde ad alcun contatto, restituire la stringa Nessun contatto di questo tipo.
Se prop non corrisponde ad alcuna proprietà valida di un contatto trovato corrispondente al nome, restituire la stringa No tale proprietà.

const contacts = [
  {
    firstName: "Akira",
    lastName: "Laine",
    number: "0543236543",
    likes: ["Pizza", "Coding", "Brownie Points"],
  },
  {
    firstName: "Harry",
    lastName: "Potter",
    number: "0994372684",
    likes: ["Hogwarts", "Magic", "Hagrid"],
  },
  {
    firstName: "Sherlock",
    lastName: "Holmes",
    number: "0487345643",
    likes: ["Intriguing Cases", "Violin"],
  },
  {
    firstName: "Kristian",
    lastName: "Vos",
    number: "unknown",
    likes: ["JavaScript", "Gaming", "Foxes"],
  },
];

function lookUpProfile(name, prop) {  
    let profile = [];
    for(let i = 0; i<contacts.length; i++) {
      
      if(contacts[i].firstName == name) {
        profile.push(contacts[i]);
      }   }

    if(profile.length == 0) {
      return "No such contact";
    }
    if(profile[0].hasOwnProperty(prop)) {
      return profile[0][prop];
    } else {
      return "No such property"
    }  }
lookUpProfile("Akira", "likes");
===
Genera frazioni casuali con JavaScript
I numeri casuali sono utili per creare comportamenti casuali.
JavaScript ha una funzione Math.random() che genera un numero decimale casuale compreso tra 0 (incluso) e 1 (esclusivo). Quindi Math.random() può restituire uno 0 ma non restituire mai un 1.
Nota: come per la memorizzazione dei valori con l'operatore di assegnazione, tutte le chiamate di funzione verranno risolte prima dell'esecuzione del ritorno, quindi possiamo restituire il valore della funzione Math.random().
Cambia randomFraction per restituire un numero casuale invece di restituire 0.

function randomFraction() {
  return Math.random();
}
===
Genera numeri interi casuali con JavaScript
È fantastico poter generare numeri decimali casuali, ma è ancora più utile se lo usiamo per generare numeri interi casuali.
Usa Math.random() per generare un decimale casuale.
Moltiplica quel decimale casuale per 20.
Utilizzare un'altra funzione, Math.floor() per arrotondare il numero per difetto al numero intero più vicino.
Ricorda che Math.random() non può mai restituire un 1 e, poiché stiamo arrotondando per difetto, è impossibile ottenere effettivamente 20. Questa tecnica ci darà un numero intero compreso tra 0 e 19.
Mettendo tutto insieme, ecco come appare il nostro codice:
Math.floor(Math.random() * 20);
Stiamo chiamando Math.random(), moltiplicando il risultato per 20, quindi passando il valore alla funzione Math.floor() per arrotondare il valore per difetto al numero intero più vicino.
Utilizzare questa tecnica per generare e restituire un numero intero casuale compreso tra 0 e 9.

function randomWholeNum() {
  return Math.floor(Math.random() * 10);
}
===
Genera numeri interi casuali all'interno di un intervallo
Invece di generare un numero intero casuale compreso tra zero e un dato numero come abbiamo fatto prima, possiamo generare un numero intero casuale che rientra in un intervallo di due numeri specifici.
Per fare ciò, definiremo un numero minimo min e un numero massimo max.
Ecco la formula che useremo. Prenditi un momento per leggerlo e prova a capire cosa sta facendo questo codice:
Math.floor(Math.random() * (max - min + 1)) + min
Crea una funzione denominata RandomRange che accetta un intervallo myMin e myMax e restituisce un numero intero casuale maggiore o uguale a myMin ed è minore o uguale a myMax, incluso.

function randomRange(myMin, myMax) {
  return Math.floor(Math.random() * (myMax - myMin + 1)) + myMin;
}
===
Utilizzare la funzione parseInt
La funzione parseInt() analizza una stringa e restituisce un intero. Ecco un esempio:
const a = parseInt("007");
La funzione precedente converte la stringa 007 nell'intero 7. Se il primo carattere nella stringa non può essere convertito in un numero, restituisce NaN.
Utilizzare parseInt() nella funzione convertToInteger in modo che converta la stringa di input str in un intero e la restituisca.

function convertToInteger(str) {
   return parseInt(str);
}
convertToInteger("56");
===
Utilizzare la funzione parseInt con un Radix
La funzione parseInt() analizza una stringa e restituisce un intero. Richiede un secondo argomento per la radice, che specifica la base del numero nella stringa. La radice può essere un numero intero compreso tra 2 e 36.
La chiamata di funzione è simile a:
parseInt(string, radix);
And here's an example:
const a = parseInt("11", 2);
La variabile radix dice che 11 è nel sistema binario, o base 2. Questo esempio converte la stringa 11 in un numero intero 3.
Utilizzare parseInt() nella funzione convertToInteger in modo che converta un numero binario in un intero e lo restituisca.

function convertToInteger(str) {
return parseInt(str, 2)
}
convertToInteger("10011");
===
Utilizzare l'operatore condizionale (ternario).
L'operatore condizionale, chiamato anche operatore ternario, può essere utilizzato come espressione if-else a una riga.
La sintassi è un? b : c, dove a è la condizione, b è il codice da eseguire quando la condizione restituisce true e c è il codice da eseguire quando la condizione restituisce false.
La seguente funzione utilizza un'istruzione if/else per verificare una condizione:

function findGreater(a, b) {
  if(a > b) {
    return "a is greater";
  }
  else {
    return "b is greater or equal";
  }   }
Questo può essere riscritto usando l'operatore condizionale:
function findGreater(a, b) {
  return a > b ? "a is greater" : "b is greater or equal";
}
Utilizzare l'operatore condizionale nella funzione checkEqual per verificare se due numeri sono uguali o meno. La funzione dovrebbe restituire la stringa Uguale o la stringa Non uguale.

function checkEqual(a, b) {
    return a == b ? "Equal" : "Not Equal";
}
checkEqual(1, 2);
===
Utilizzare più operatori condizionali (ternari).
Nella sfida precedente, hai utilizzato un unico operatore condizionale. Puoi anche concatenarli insieme per verificare la presenza di più condizioni.
La seguente funzione utilizza le istruzioni if, else if ed else per verificare più condizioni:
function findGreaterOrEqual(a, b) {
  if (a === b) {
    return "a and b are equal";
  }
  else if (a > b) {
    return "a is greater";
  }
  else {
    return "b is greater";
  }  }
La funzione precedente può essere riscritta utilizzando più operatori condizionali:

function findGreaterOrEqual(a, b) {
  return (a === b) ? "a and b are equal" 
    : (a > b) ? "a is greater" 
    : "b is greater";
}

È considerata una buona pratica formattare più operatori condizionali in modo tale che ogni condizione si trovi su una riga separata, come mostrato sopra. L'utilizzo di più operatori condizionali senza un'adeguata indentazione può rendere difficile la lettura del codice. Per esempio:

function findGreaterOrEqual(a, b) {
  return (a === b) ? "a and b are equal" : (a > b) ? "a is greater" : "b is greater";
}
Nella funzione checkSign, utilizza più operatori condizionali, seguendo il formato consigliato utilizzato in findGreaterOrEqual, per verificare se un numero è positivo, negativo o zero. La funzione dovrebbe restituire positivo, negativo o zero.

function checkSign(num) {
 return (num > 0) ? "positive" 
    : (num < 0) ? "negative" 
    : "zero";
}
checkSign(10);
===
Usa la ricorsione per creare un conto alla rovescia
In una sfida precedente, hai imparato come usare la ricorsione per sostituire un ciclo for. Ora, esaminiamo una funzione più complessa che restituisce una matrice di numeri interi consecutivi che iniziano con 1 fino al numero passato alla funzione.
Come accennato nella sfida precedente, ci sarà un caso base. Il caso base dice alla funzione ricorsiva quando non ha più bisogno di chiamare se stessa. È un caso semplice in cui il valore restituito è già noto. Ci sarà anche una chiamata ricorsiva che esegue la funzione originale con argomenti diversi. Se la funzione è scritta correttamente, alla fine si raggiungerà il caso base.
Ad esempio, supponiamo di voler scrivere una funzione ricorsiva che restituisca un array contenente i numeri da 1 a n. Questa funzione dovrà accettare un argomento, n, che rappresenta il numero finale. Quindi dovrà chiamarsi con valori progressivamente più piccoli di n fino a raggiungere 1. Potresti scrivere la funzione come segue:

function countup(n) {
  if (n < 1) {
    return [];
  } else {
    const countArray = countup(n - 1);
    countArray.push(n);
    return countArray;
  }  }
console.log(countup(5));
Il valore [1, 2, 3, 4, 5] verrà visualizzato nella console.

All'inizio, questo sembra controintuitivo poiché il valore di n diminuisce, ma i valori nell'array finale stanno aumentando. Ciò accade perché il push avviene per ultimo, dopo che la chiamata ricorsiva è tornata. Nel punto in cui n viene inserito nell'array, countup(n - 1) è già stato valutato e restituito [1, 2, ..., n - 1].

Abbiamo definito una funzione chiamata conto alla rovescia con un parametro (n). La funzione dovrebbe utilizzare la ricorsione per restituire un array contenente gli interi da n a 1 in base al parametro n. Se la funzione viene chiamata con un numero inferiore a 1, la funzione dovrebbe restituire una matrice vuota. Ad esempio, chiamando questa funzione con n = 5 dovrebbe restituire l'array [5, 4, 3, 2, 1]. La tua funzione deve utilizzare la ricorsione chiamando se stessa e non deve utilizzare loop di alcun tipo.

function countdown(n){
  if (n < 1) {
    return [];
  } else {
   let countArray = countdown(n-1)
     countArray.unshift(n);
     return countArray;  
}  }
===
Usa la ricorsione per creare un intervallo di numeri
Continuando dalla sfida precedente, ti offriamo un'altra opportunità per creare una funzione ricorsiva per risolvere un problema.

Abbiamo definito una funzione denominata rangeOfNumbers con due parametri. La funzione dovrebbe restituire una matrice di numeri interi che inizia con un numero rappresentato dal parametro startNum e termina con un numero rappresentato dal parametro endNum. Il numero iniziale sarà sempre minore o uguale al numero finale. La tua funzione deve usare la ricorsione chiamando se stessa e non usare loop di alcun tipo. Dovrebbe funzionare anche per i casi in cui startNum e endNum sono gli stessi.

function rangeOfNumbers(startNum, endNum) {
  if(startNum == endNum) {
    return [startNum];

  }else {
    const countArr = rangeOfNumbers(startNum + 1, endNum);
    countArr.push(startNum);
    return countArr;
  }  };
