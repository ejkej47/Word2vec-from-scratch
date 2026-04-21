WORD2VEC MODEL (SKIP-GRAM, NEGATIVE SAMPLING)

Projekat se bavi implementacijom Word2Vec modela za učenje vektorskih reprezentacija reči, koristeći Skip-gram arhitekturu. Model je razvijen od nule bez upotrebe ML biblioteka, sa ciljem razumevanja načina na koji se uče semantičke relacije između reči.

PODACI

Korišćen je text8 dataset (tekst sa Wikipedije).

-prvih 1.000.000 reči korišćeno za treniranje,
-formiran vokabular i frekvencije reči.

METODOLOGIJA

PRIPREMA PODATAKA

-tokenizacija i formiranje vokabulara

SUBSAMPLING

-smanjenje uticaja često pojavljivanih reči

GENERISANJE PAROVA

-dinamički kontekstualni prozor
-parovi (centralna reč, kontekst)

MODEL

-matrice W1 i W2
-Xavier inicijalizacija

NEGATIVE SAMPLING

-uzorkovanje negativnih primera (unigram distribucija)

TRENING

-SGD optimizacija
-smanjenje learning rate-a

EVALUACIJA

-cosine similarity između reči
REZULTATI
-model uči osnovne semantičke odnose između reči,
-slične reči se grupišu u prostoru,
-loss opada tokom treniranja.
