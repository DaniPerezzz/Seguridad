# Práctica: Cifrado y descifrado con GPG
## Dani Perez
### ASIR 2


- Contraseñas: dinosaurio111D

![img](./img/1.png)


 ## Crear el archivo de texto

 Primero se crea un archivo llamado `mensajeDani.txt`:

```
touch mensajeDani.txt
```

---

 ## Cifrado simétrico

 Para cifrar el archivo se utiliza:

```
gpg --symmetric mensajeDani.txt
```

 GPG solicita una contraseña para proteger el archivo.

 Al terminar, se crea un nuevo archivo:

```
mensajeDani.txt.gpg
```

---

 ## 3. Comprobar el archivo cifrado


 podemos comprobar que existen los archivos:

```
mensajeDani.txt
mensajeDani.txt.gpg
```

 El archivo `.gpg` es el que contiene la información cifrada.


---

 ## Cifrado en formato ASCII

 También se ha utilizado:

```
gpg -c --armor mensajeDani.txt
```

 La opción `-c` indica que queremos realizar un **cifrado simétrico**.

 La opción `--armor` hace que el resultado se guarde utilizando un formato de texto ASCII, en lugar del formato binario habitual.

 Por eso se genera:

```
mensajeDani.txt.asc
```

---

