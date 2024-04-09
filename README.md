Rezervare online bilete de tren

Interfața Utilizatorului:
Pagină de pornire: O pagină care prezintă utilizatorului opțiunile disponibile, cum ar fi căutarea de trenuri disponibile, vizualizarea și gestionarea rezervărilor existente.
Căutare tren: O interfață care permite utilizatorului să căute trenuri disponibile în funcție de locație de plecare și destinație, dată și oră.
Rezervare: O interfață care permite utilizatorului să selecteze un tren și să facă o rezervare pentru unul sau mai multe locuri pe trenul selectat.
Backend (PHP și Java):
Conectare la bază de date: O conexiune cu baza de date MySQL pentru a accesa și manipula datele.
Procesare solicitări: Scripturi PHP și Java pentru a gestiona cererile utilizatorului, inclusiv căutarea trenurilor disponibile, efectuarea unei rezervări și actualizarea datelor în baza de date.
Bază de Date MySQL:
Tabele:
Utilizatori: Acest tabel va conține informații despre utilizatori, cum ar fi ID-ul utilizatorului, numele, adresa de email și parola.
    Aceste informații sunt esențiale pentru implementarea funcționalităților de autentificare și autorizare.
Trenuri: Informații despre trenuri, cum ar fi numele trenului, tipul de tren (de exemplu, rapid, intercity etc.).
Statii: Lista de stații disponibile, numele stației.
Rute: Informații despre rutele disponibile între stații, inclusiv stația de plecare și de destinație și distanța.
Aceste informații sunt necesare pentru afișarea programului de circulație al trenurilor și pentru calcularea duratei călătoriei.
Tipuri de bilete: Acest tabel va conține informații despre diferitele tipuri de bilete disponibile (de exemplu, bilete de adult, copil, student, elev sau pensionar), denumirea și prețul. Aceste informații sunt utile pentru calcularea prețului total al rezervării și afișarea opțiunilor de bilete disponibile utilizatorilor.
Locuri: locurile disponibile în fiecare tren, inclusiv numele trenului, numărul locului, tipul de loc (de exemplu, loc la fereastră sau la culoar) și disponibilitatea (dacă locul este disponibil sau rezervat).
 Actualizarea disponibilității locurilor este crucială pentru gestionarea rezervărilor și a locurilor libere.
Rezervari: Detalii despre rezervările făcute, cum ar fi ID-ul rezervării, ID-ul utilizatorului, numele trenului, datele de călătorie și locurile rezervate.
Relații între tabele:
Trenuri și Rute ar putea fi legate printr-o cheie străină.
Rute și Staii ar putea fi legate similar, pentru a stabili rutele disponibile între diferite stații.
Funcționalități adiționale:
Autentificare și Autorizare: Pentru a permite utilizatorilor să-și creeze conturi și să-și gestioneze rezervările lor.
Validare și verificare: Validarea datelor introduse de utilizatori pentru a preveni erorile și manipularea incorectă a datelor.
Tranzacții și confirmare: Implementarea unui sistem de confirmare a rezervărilor 
