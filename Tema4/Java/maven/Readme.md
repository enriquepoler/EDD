# MAVEN

## Instalacio Maven en ubuntu

Per a instalar maven en ubuntu a traves de terminal posarem el seguent comando:
```
$ sudo apt install maven
```

## Creacio del projecte

Per a començar, elegirem la carpeta on volem crear el projecte de maven i executarem el seguent comando:

```
mvn archetype:generate -DgroupId=com.ieseljust.edd -DartifactId=CalculaMVN -DarchetypeArtifactId=maven-archetype-quickstart -DinteractiveMode=false
```

On posa "-DartifactId=", despres del "=" podem elegir el nom que vuigam per a la carpeta del projecte.

## Modificar el fitxer pom.xml

Dins de l'archiu pom.xml afegirem despres d'on esta la url de "maven.apache.org" el seguent:

```
<properties>
    <maven.compiler.source>1.6</maven.compiler.source>
    <maven.compiler.target>1.6</maven.compiler.target>
  </properties>
```

## Afegir el projecte

Dins del main del src del projecte de maven, haurem de cambiar el app.java per els nostres fitxers, podem gastar els .java que hem creat per a ant.

## Compilar maven

Es hora de compilar la aplicacio. Ens situem en la carpeta on es troba el fitxer pom.xml i executem:

```
$ mvn compile
```

Afegim l'objectiu:

```
$ java cp target/classes com.ieseljust.edd.calcula 3 4
```

Netejar el projecte: 

```
$ mvn clean package
```