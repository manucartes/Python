# Notas de Python 🐍 
> Escrito por manu cartes.
> 20 de junio de 2021 

## Manejo de archivos 📁

### Leer un archivo

```python
archivo = open("Datos.txt",'r')
contenido = archivo.read()
print(contenido)
```

### Escribir en un archivo

Para escribir un archivo primero hay que abrirlo y pasarle un parámetro, este puede ser:

* 'w' = Borra el archivo si ya existe y crea uno nuevo
* 'a' = Agrega el contenido al final del archivo
* 'x' = Si ya existiese el archivo devuelve un error

```python
fichero = open("datos_prueba.txt",'a')
print(fichero)
fichero.write("Esta linea fue creada desde codigo")
fichero.close()
```

## Solicitudes a internet 📡

### Obtener código fuente página web

Para esto es necesario agregar la librería `requests`

```python
import requests
res = requests.get('https://scotch.io')

print(res.text)
```

## La libreria NumPy 🧮

```python
import numpy as np
```

### La función arange

Crea un array NumPy

```python
a.np = arange(2,8)
```

> array([2,3,4,5,6,7])



