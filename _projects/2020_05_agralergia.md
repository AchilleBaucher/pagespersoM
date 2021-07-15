---
title: "Implementation of a Grammatical Inference algorithm"
date: 2020-05-01
type: 'personal'
what: 'autonomous personal project'
summary: 'I implemented in C++ a grammatical inference algorithm, tested it and tried to bring some improvment, for mitigate results.'
logo: logo_agralergia.png
logo_desc: "'An infered probabilistic automatata'"
languages: "C++"
---
{% include base_path %}
The code is available on my [framagit](https://framagit.org/Acquilles/graphes).

## Context
Grammatical inference ([1](#1.)) aims at building an probabilistic automata from a given collection of words (succession of symbols). The studied algorithm, ALERGIA, begins by creating the Prefix Tree Acceptor, then progessively merge states of the automata acccording to some criteria, as described in ([2](#2.)).

## Project
I started from a existing C++ graph class ([3](#3.)), and then changed it to adapt it to represent finite probabilistic automata, able to manipulate symbols and transition probabilities. I implemented the ALERGIA algorithm, and tested it by trying to infer automata from sequences written by randomly generated automata. Inference worked for small automata (2 states) but not for bigger ones. I tried to bring an improvment by using an other criterium to merge 2 states, which worked better in some very few cases.

## Note
I wasn't familiar with the good practices of coding at this time, and the comments in the code are really messy (and in french). I'm not able to fully understand how it works anymore.

[1.](#) Pierre Dupont, Laurent Miclet. Inférence grammaticale régulière : fondements théoriques et princi-paux algorithmes. [Rapport de recherche] RR-3449, INRIA. 1998. inria-00073241

[2.](#) Carrasco, Rafael & Oncina, Jose. (2002). Learning Stochastic Regular Grammars by Means of a State Merging Method. 10.1007/3-540-58473-0_144.

[3.](#) NGraph, a simple (Network) Graph library in C++, https://math.nist.gov/~RPozo/ngraph/
