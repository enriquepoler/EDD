# ANT

El primer que hem de fer será crear els archius calcula.java i calculadora.java, els cuals tindrán implementats les funcions principals i faran us de llibreries que crearem.

## 1. Build.xml

Crearem un archiu a l'arrel de la carpeta de ant, anomenat build.xml per poder definir les fases de construccio i com se compilará el programa.

## 2. Compilacio dels archius .java per obtindre els .class

Desde la terminal d'ubuntu, a l'arrel de la carpeta d'ant executarem: 

```
$ javac com/ieseljust/edd/calc/*.java
```

## 3. Executar el programa amb ant

Per a executar el programa, ho farem altra vegada desde l'arrel amb:

```
ant run -Darg0=3 -Darg1=4
```

Son el parametros que li donarem per a executar el programa i que faja els calculs amb eixos dos numeros.