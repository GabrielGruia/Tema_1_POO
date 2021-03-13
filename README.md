# Tema 16 - POO:

1. Clasa "Individ", avand:  
  
   * membrii privati:  
            - i (intreg) = pozitia (dintr-un tablou unidimensional de 30 de elemente declarat static in main);  
            - tip (char) = „numele” speciei ('+' sau '0');  
            - varsta (intreg) = varsta (de la 0 la o valoare maxima fixa aleasa de programator);  
            - energie (double) = energia;  
            - viu (unsigned char) = este 1 daca e viu si 0 daca e mort;  
  
    * constructor care primeste ca parametrii pozitia si tipul si initializeaza corespunzator membrii respectivi:  
            - varsta se initializeaza cu 0;  
            - energia cu o valoare fixa aleasa de programator;  
            - viu cu 1;  
  
    * metode private:  
            - hraneste = creste energia proprie cu o valoare random intre 1 si 10;  
            - inmulteste = adauga un fiu in stanga sau in dreapta individului daca pozitia este libera (fiul are acelasi tip, varsta este 0, iar energia este de doua ori mai mare fata de cea a parintelui);  
            - ataca = pentru fiecare individ x invecinat si de alt tip, daca energia proprie este mai mare decat energia lui x, din energia proprie se scade energia lui x iar x este omorat (i se aplica metoda "moare");  
            - imbatraneste = creste varsta cu 1; scade energie cu o valoare constanta aleasa de programator; daca a atins o varsta maxima aleasa de programator sau daca energia sa a devenit <= 0, individul curent este omorat (i se aplica metoda "moare");  
            - moare = viu devine 0;  
  
    * metode publice:  
            - actualizare = aplica succesiv metodele: hraneste, inmulteste, ataca, imbatraneste;  
            - esteviu = returneaza 1 daca viu = 1 si 0 altfel;  
            - gettip = returneaza tipul;  
  
  
2. Se citesc maxim 30 de indivizi (supraincarcare pentru >> si <<);  
  
3. Realizare meniu cu functia de:  
            - citire indivizi (se citeste si numarul de indivizi aici);  
            - actualizare;  
            - este viu;  
            - get tip;  
  
4. Alte cerinte:  
            - implementare in C++ folosind clase;  
            - datele membre private;  
            - constructori de initializare (cu si fara parametri), constructor de copiere, destructor, operator de atribuire;  
            - get, set pentru toate datele membre;  
            - supraincarcarea operatorilor << si >> pentru iesiri si intrari de obiecte, dupa indicatiile de mai jos, astfel incat sa fie permise (si ilustrate in program);  
            - sa existe metode publice prin care se realizeaza citirea si afisarea informațiilor complete a n obiecte, memorarea și afisarea acestora;  
            - programul sa aiba un meniu interactiv;
