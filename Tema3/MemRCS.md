# Memòria d'RCS
###### 1. Creeu un fitxer anomenat exercici.md, i afegiu-li algun contingut en format Markdwon.
touch exercici.md
nano exercici.md
Hola mundo, Enrique Poler
---
###### 2. Registreu el fitxer per a que el controle RCS.
ci -u exercici.md

---
###### 3. Intenteu modificar el fitxer, per veure si teniu o no permís.
No hi han permisos de modificació

---
###### 4. Feu un checkout del fitxer, ara sí, per afegir canvis.
co -l exercici.md

---
###### 5. Modifiqueu el fitxer i afegiu-li més contingut. Aquesta serà la versió 1.2.
nano exercici.md
###### Hola mundo, Enrique Poler prueba checkout

---
###### 6. Amb un altre usuari, intenteu modificar el fitxer (fent el checkout abans).
No tinc la posibilitat de canviar d'usuari, no soc administrador ni tinc altre compte

---
###### 7. Com a l’usuari original, registreu els canvis al fitxer.


---
###### 8. Amb l’altre usuari de nou, intenteu ara modificar el fitxer (també fent un checkout).

---
###### 9. Si podeu, afegiu més informació al fitxer, ara serà la versió 1.3.
nano exercici.md
###### Hola mundo, Enrique Poler prueba checkout
versio 3, anyadir informacio

---
###### 10. Com a l’usuari original, visualitzeu les diferències entre les versions, i torneu a la versió 1.2.
rcsdiff -r1.1 -r1.2 exercici.md

===================================================================
.
RCS file: ./exercici.md,v
retrieving revision 1.1
retrieving revision 1.2
diff -r1.1 -r1.2
1c1
< Hola mundo, Enrique Poler
---
> ##### Hola mundo, Enrique Poler prueba checkout
---
rcsdiff -r1.2 -r1.3 exercici.md

===================================================================
.
RCS file: ./exercici.md,v
retrieving revision 1.2
retrieving revision 1.3
diff -r1.2 -r1.3
1a2,3
.>
.> versio 3, anyadir informacio.
---
co -r1.2 exercici.md
./exercici.md,v  -->  ./exercici.md
revision 1.2
done

---
###### 11. Apliqueu més canvis i guardeu-los amb la versió 1.4.
nano exercici.md

##### Hola mundo, Enrique Poler prueba checkout
Prova versió 1.4

ci -u exercici.md
./exercici.md,v  <--  ./exercici.md
new revision: 1.4; previous revision: 1.3
enter log message, terminated with single '.' or end of file:
.>> Prova
.>> 
.>> v4 
.>> .
done

