---
title: "Syllabus"
subtitle: <h4 style="font-style:normal">Introducción al análisis cuantitativo de textos en R</h4>
date: <h4 style="font-style:normal">2021-08-12</h4>
output: 
  html_document:
    toc: true
    toc_depth: 3
    toc_float: true
    theme: readable
---


<style>
p.comment {
background-color: #DBDBDB;
padding: 10px;
border: 1px solid black;
margin-left: 25px;
border-radius: 5px;
font-style: italic;
}

.figure {
   margin-top: 20px;
   margin-bottom: 20px;
}

h1.title {
  font-weight: bold;
  font-family: Arial;  
}

h2.title {
  font-family: Arial;  
}

</style>


<style type="text/css">
#TOC {
  font-size: 13px;
  font-family: Arial;
}
</style>

\

## Sesión 1: ¿Cómo proceso cadenas de texto como datos?

### Breve repaso del *tidyverse*

- Repaso breve de las 5 funciones
- Uso de las funciones para cadenas de texto `str_`
- Breve introducción a las expresiones regulares

### Procesamiento y lectura de textos

- ¿Cómo leo datos desde PDF / EPUBs / archivos de texto?
- Ordenar, estructurar y limpiar cadenas de texto
- ¿Qué es un *corpus* y para qué sirve?


### Scraping básico

- ¿Cómo obtengo datos de manera sistemática de algún lugar de internet?

### Introducción a `tidytext`

- Como *desanidar tokens* con `unnest_tokens` y contarlos.

<br/><br/>
<br/><br/>
<br/><br/>

## Sesión 2: ¿Cómo analizar las palabras?

### Introducción al análisis cuantitativo de textos

- Ley de Zipf
- Conteo de tokens y *n-gramas¨*
- Relaciones entre palabras


### El documento como unidad de análisis

- Cálculo y uso del *tf_idf*

### Introducción al análisis de sentimientos

- Análisis de sentimientos por el método de diccionario

### Similitud entre documentos
- Distancias euclideanas

<br/><br/>
<br/><br/>
<br/><br/>

## Sesión 3: Modelos de clasificación

### Preparación para modelar
- Remover palabras vacías (*stopwords*)
- Extraer las stemas
- Etiquetado de elementos del discurso
    
### Métodos de categorías conocidas:
- Impelementación práctica de la regresión lineal
- Implementación práctica Naive Bayes para NLP
- Implementación práctica de Lasso para NLP

<br/><br/>
<br/><br/>
<br/><br/>

## Sesión 4: Más modelos

### Métodos de clasificación con categorías no conocidas
- Distribución latente de Dirichlet
- Distribución latente de Dirichlet con semillas

### Vectorización de textos 
