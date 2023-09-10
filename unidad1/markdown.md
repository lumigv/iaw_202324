# TUTORIAL DE MARKDOWN

En este taller de introducción a Markdown aprenderemos los comandos básicos para empezar a trabajar. 

1. [Encabezados](#encabezados)
2. [Bloques de texto](#bloques-de-texto)
3. [Formato de texto](#formato-de-texto)
4. [Código](#código)
5. [Listas](#listas)
6. [Vínculos o enlaces](#vículos-o-enlaces)
7. [Imágenes](#imágenes)
8. [Tablas](#tablas)


## Sintaxis básica


### Encabezados

# H1 o primer nivel
## H2 o segundo nivel
### H3 o tercer nivel
#### H4 o cuarto nivel

### Bloques de texto

#### Párrafos
Para crear un nuevo párrafo basta con dejar una línea en blanco entre una o más líneas de texto:

Esto es un párrafo.

Esto es otro párrafo.

#### Saltos de línea

Para añadir un salto de línea basta con dejar dos o mas espacios en blanco al final de la línea y luego pulsas INTRO.  

Esto es una línea.  
Y esta es otra línea.
 
#### Cita o Blockquote

> "cita 1"
> > "cita 2"


### Formato de Texto

#### Negrita

**Texto en negrita**  
__Texto en negrita__

#### Itálica o cursiva

*Texto en itálica*  
_Texto en itálica_

#### Negrita cursiva

***Texto en negrita cursiva***  
___Texto en negrita cursiva___


### Código

#### Código en línea

`codigo`


#### Bloque de código

```
Creando códigos de bloque.  
Puedes añadir tantas líneas como quieras.
```

### Listas

#### Lista ordenada

1. Primer elemento
2. Segundo elemento
3. Tercer elemento

#### Lista ordenada 2

1. Elemento 1
    1.1. Elemento 1.1
	1.2. Elemento 1.2
2. Elemento 2
3. Elemento 3
    3.1. Elemento 3.1
    3.2. Elemento 3.2
    
#### Lista desordenada

- Primer elemento
- Segundo elemento
- Tercer elemento

#### Lista desordenada 2

* Primer elemento
* Segundo elemento
* Tercer elemento

#### Lista desordenada 3

+ Primer elemento
+ Segundo elemento
+ Tercer elemento

#### Listas desordenada 4

- Elemento 1
- Elemento 2
    - Elemento 2.1
    - Elemento 2.2



### Línea horizontal

---
***
___

### Vínculos o enlaces
Para crear un enlace debes situar entre corchetes el texto que quieres enlazar, también conocido como anchor. Seguidamente, debes usar paréntesis para definir la URL a la que debe enlazar en texto del enlace

#### Enlace

[Markdown Guide](https://www.markdownguide.org)

#### Enlace de un artículo a otro

[articulo1](articulo1.md)  
[articulo2](../articulo2.md)  
[articulo3](directorio/articulo3.md)


#### Enlace de marcador
Use un símbolo de almohadilla seguido de las palabras del título en minúscula. Quite los signos de puntuación del título y reemplace los espacios por guiones:

[Bloques de texto](#bloques-de-texto)  
[Párrafo1](../articulo1.md#parrafo1)


#### URL

<https://www.markdownguide.org>


#### Correo electrónico

<me@email.com>

### Imágenes

#### Imágenes desde un archivo

![Markdown](images/logomarkdown.png "logo Markdown")

Ó

<image src="images/logomarkdown.png" alt="logo Markdown">


Hay que tener mucho cuidado al subir la imagen a un servidor web, en este caso sería recomendable incluir la / al principio. Podría mostrarse en el ordenador, pero no al servidor web.

![Markdown](/images/logomarkdown.png "logo Markdown")

Ó

<image src="/images/logomarkdown.png" alt="logo Markdown">

#### Imágenes desde un enlace

![Linux](https://www.markdownguide.org/assets/images/tux.png)

Ó

<image src="https://www.markdownguide.org/assets/images/tux.png" alt="Linux">


#### Añadir un pie de foto a una imagen

![Markdown](images/logomarkdown.png "logo Markdown")

Ó

<image src="images/logomarkdown.png" alt="logo Markdown" caption="logo Markdown">



### Tablas


#### Crear tabla

| Column 1 | Column 2 | Column 3 |
|----------|----------|----------|
| Row 1    | Cell 2   | Cell 3   |
| Row 2    | Cell 5   | Cell 6   |
| Row 3    | Cell 8   | Cell 9   |


#### Alineación

| Left-Aligned  | Center Aligned  | Right Aligned |
|:------------- |:---------------:| -------------:|
| Row 1         | Cell 2          | Cell 3        |
| Row 2         | Cell 5          | Cell 6        |
| Row 3         | Cell 8          | Cell 9        |






