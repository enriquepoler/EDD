# GRADLE

## Instalacio de Gradle

```
$ sudo apt install gradle
```

## Escomençar el projecte Gradle

```
$ gradle init
```

Elegir les opcions: 
Type: 4 
Build: 1 
Test framework: 1 
Name: calcula
Source package: com.ieseljust.edd

## Modificar el archiu build.gradle

En el arxiu build.gradle, haurem de cambiar en la ultima linea el main class i posar:

```
mainClassName = 'com.ieseljust.edd.calcula'
```

Una vegada fet, haurem de posar els nostres arxius .java en el main del gradle, per a poder compilar el projecte i executarlo.

## Compilar Gradle

```
$ gradle build
```

I per a executar-lo, soles falta:

```
$ gradle run
```