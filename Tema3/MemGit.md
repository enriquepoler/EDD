### 1. Memòria dels exemples pràctics amb Git

El primer sera fer un git clone per a copiar el nostre repositori a una carpeta local i poder treballar desde ahi en local:
```bash
1 $ git clone https://github.com/enriquepoler/EDD.git
```
En aquest cas, he clonat el meu repositori de GitHub, pero es pot modificar per descarregar cualsevol.

##### Hi han varios comandos que utilizarem per a poder fer pujades al ripositori, descarregar les actualitzacions, fer commits, i altres coses:
```bash
2 $ git add . 
```
Per a afegir tots els canvis que hem fet en la carpeta i poder actualitzarlos en el repositori.
```bash
2 $ git commit -a -m "comentari" 
```
Per a fer un commit de lo que hem afegit/modificat.
```bash
2 $ git push
```
Per a acabar d'enviar els canvits al repositori de GitHub.
```bash
2 $ git pull
```
Per a descarregar la ultima actualització del repositori, per si treballem mes d'una persona en el repositori, o amb varios equips, poder decarregar els canvits.