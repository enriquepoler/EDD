# Creacio de l'archiu calcula

El que anem a fer primer será crear diversos archius Calcula per tal de compilar i crear un archiu calcula.o que ens done la eixida dels archius compilats de manera conjunta.

## 1. Crear archius calcula.c i calcula.h

L'archiu calcula.c tindrá imprementat les funcions suma, resta, multiplica, divdeix i a mes afegirem la mitja. I per altra part, l'archiu calcula.h contindrá les capçaleres d'aquestes funcions, per tal de ser utilitzades per altre programa.

## 2. Crear l'archiu calcula.o

El fitxer final 'calcula' necesita tant del seu codi font calcula.c com del fitxer objecte de la llibreria calc.o i per tal d'obtindre aquest fitxer objecte, necessitem del fitxer font de la llibreria calcula.c

Optindrem el fitxer calc.o a partir de calcula.c de la seguent forma:
```
gcc -c calcula.c -o calc.o
```

Ara nem a conseguir el fitxer executable 'calcula'

```
gcc -Wall -g calc.o calcula.c -o calcula
```

Aixi haurem obtingut el fitxer executable 'calcula', amb el coresponent link al calcula.c

# Creacio del Makefile