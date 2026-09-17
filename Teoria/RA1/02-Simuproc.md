# Modul-MP0483. Sistemes informàtics.
**RA1. Avalua sistemes informàtics, identificant els seus components i característiques.**

### Simuproc
**Funcionament d'una CPU**  
Un ordinador està compost per diferents components electrònics pels quals circula electricitat. La distribució de l'electricitat per diferents components permet visualitzar les funcionalitats que se li suposen que ha de realitzar.

Per tal que la distribució de corrent elèctric sigui mesurable i correcta, els sistemes utilitzen rellotges interns, components que permeten calcular durant quant de temps ha de transcórrer per donar validesa a la informació. Aquests components permeten la sincronització entre components i que tot funcioni correctament.

El procés que utilitza el simulador que presentem, i la major part de CPUs del mercat serà semblant, segueix aquestes parts:

>1. Cicle d'obtenció d'informació per processar o cicle de Fetch: consisteix en obtenir dades per realitzar càlculs. En el cas de Simuproc aquest cicle es compon del següent:
>>a. Llegeix un registre anomenat **PC** (Comptador de Programa o **P**rogram **C**ounter)  
>>b. Connecta amb l'adreça de memòria que indica el registre PC  
>>c. Carrega el contingut de la memòria en un registre anomenat IR (Registre d'Instrucció o **I**nstruction **R**egister)  
>>d. Incrementa el PC  
>2. Cicle d'execució: la CPU realitza la funció que té programada amb els conjunts de'instruccions definits. Amb Simuproc serà:
>>a. Si ha de tornar a consultar la memòria per necessitar informació la CPU tornarà a memòria per obtenir dades  
>>b. Executa la instrucció que se li ha definit pel dissenyador de la CPU  
>>c. Emmagatzema els resultats a la memòria

### Llenguatge Assemblador (Assembler)
Els llenguatges de programació s'utilitzen per donar instruccions als ordinadors per tal que resolguin problemes amb unes poques dades introduïdes pels usuaris.  
Aquests llenguatges poden ser molt ràpids i eficients, però molt complexos d'utilitzar per part dels programadors. Són els llenguatges de **baix nivell**: l'ordinador rep ordres en binari i funciona al màxim rendiment.

Per contra, aquests llenguatges de baix nivell són molt propensos a cometre errades per part dels programadors, ja que resulten molt difícils de llegir degut a treballar amb 1 i 0. Per la necessitat de llegir i crear amb certa facilitat els programes, tenim els llenguatges d'**alt nivell**. Aquest tipus de llenguatges intenten apropar el llenguatge humà per facilitar la interacció amb l'ordinador o dispositiu que s'està programant. Són més senzills per a les persones però més lents de cara a executar codi per part de la CPU, ja que molts cops afegeixen generalitzacions i execució de codi no necessari per realitzar segons quines funcions.

El llenguatge assemblador és un llenguatge de baix nivell, no es programa directament amb codi binari ja que utilitza una nomenclatura anomenada mnemònics que ajuden a entendre la instrucció que li facilitem a la CPU, tot i que un programa complet també resulta complicat d'entendre i trobar errors. No obstant, els avantatges que aporta en certs moments fan que sigui el llenguatge preferit per obtenir el màxim rendiment d'un sistema informàtic.

[Instruccions assemblador de Simuproc](https://sites.google.com/site/simuproc/instrucciones-soportadas "Instruccions Simuproc")
