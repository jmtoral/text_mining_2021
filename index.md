---
title: '¡Hola mundo!'
subtitle: <h4 style="font-style:normal">Curso de minería de texto en R</h4>
author: <h4 style="font-style:normal">Manuel Toral</h4>
date: <h4 style="font-style:normal">2021-08-01</h4>
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

</style>



\



¡Hola! Bienvenida al curso de análisis cuantitativo de texto del verano de 2021:

* Un syllabus con las sesiones y temas que veremos
* El código que usaremos en las sesiones
* Laboratorios y tareas
<br>
<br>
<br>
<br>


## Acerca del curso

La idea de este curso es que las personas que los tomen puedan enfrentarse a los problemas más comunes de procesamiento, análisis y visualización de datos provenientes del lenguaje natural.

Es por eso que se utilizará el lenguaje humano como insumo para poder entender ciertos patrones del lenguaje. Algunas habilidades que se podrán adquirir de este curso son las siguientes:

- Procesar textos de diversas fuentes digitales para usarlos como insumos de análisis.
- Clasificar de manera sistemática documentos en categorías conocidas o desconocidas.
- Identificar el sentimiento de ciertas palabras para conocer el tono de ciertos textos
- Analizar qué tan parecidos son algunos textos

<br>
<br>
<br>
<br>


## Fechas 📆, horarios ⏱ y costo 💸 

El curso tiene una duración de 16 horas clase + asesoría para proyectos propios.

- **Sábados 21, 28 agosto y 4 y 11 de septiembre.**

- De **10 am a 2 pm** (4 horas por sesión)

El curso tiene un costo de **3,000** pesos mexicanos en total (se emiten facturas).

<br>
<br>
<br>
<br>

<br>


## 📚 Materiales y referencias

Los principales materiales que usaremos son los  siguientes:


- [Silge & Robinson - Text Mining with R](https://www.tidytextmining.com/)

- [Benoit - quanteda: An R package for the quantitative analysis of textual data](https://quanteda.io/index.html)

- [BNOSAC - UDPipe Natural Language Processing - Text Annotation](https://bnosac.github.io/udpipe/docs/doc0.html)

- [Hvitfeldt y Silge - Supervised Machine Learning for Text Analysis in R](https://smltar.com/)

- [Clark - Text Analysis in R](https://m-clark.github.io/text-analysis-with-R/intro.html)

- [Cornelius Puschmann - Advancing Text Mining with R and quanteda](https://www.mzes.uni-mannheim.de/socialsciencedatalab/article/advancing-text-mining/)

- [Marín Benjumea - Expresiones regulares](https://rpubs.com/ydmarinb/429756)

- [Urdinez y Cruz Labrín - AnalizaR Datos Políticos](https://arcruz0.github.io/libroadp/index.html)

<br>
<br>
<br>
<br>

## 🤓 Artículos académicos 

John Wilkerson and Andreu Casas (2017), Large-Scale Computerized Text Analysis in Political Science: Opportunities and Challenges *Annual Review of Political Science*, 20:1, 529-544 [enlace](https://www.annualreviews.org/doi/pdf/10.1146/annurev-polisci-052615-025542) 

Grimmer, J., & Stewart, B. (2013). Text as Data: The Promise and Pitfalls of Automatic Content Analysis Methods for Political Texts. *Political Analysis*, 21(3), 267-297. doi:10.1093/pan/mps028 [enlace](https://www.cambridge.org/core/services/aop-cambridge-core/content/view/F7AAC8B2909441603FEB25C156448F20/S1047198700013401a.pdf/text-as-data-the-promise-and-pitfalls-of-automatic-content-analysis-methods-for-political-texts.pdf) 

🔥 El trabajo de Dan Berliner [enlace](http://www.danielberliner.com/research.html)



<br>
<br>
<br>
<br>

<br>
<br>
<br>
<br>


## ¿ Cómo instalo (y uso) `R`?

Para este curso vamos a trabajar, desde el principio, con código en `R`. Es necesario tener **la última versión** de este lenguaje, al momento de escribir este repositorio ésta es la versión **4.1.1**.

Para instalarlo, es necesario entrar a [*The Comprehensive R Archive Network*](https://cran.r-project.org/) y seguir las instrucciones para cada sistema operativo.

### MAC OSX

- Basta con descargar el archivo `.pkg` [de este link](https://cran.r-project.org/bin/macosx/R-4.1.1.pkg), descomprimir el archivo, abrir el archivo y seguir las instrucciones.

### Windows

- Basta con descargar el archivo `.exe` [de este link](https://cran.r-project.org/bin/windows/base/R-4.1.1-win.exe), abrir el archivo y seguir las instrucciones.

### Linux

En Terminal, escribir las siguientes dos líneas:

`sudo apt-get update`

`sudo apt install r-base r-base-core r-recommended r-base-de`

<div style="margin-bottom:25px;">
</div>
<br>


## ¿Cómo instalar RStudio?

Para instalar RStudio (plataforma que usaremos para el uso de `R`), es necesario acudir a [esta página](https://www.rstudio.com/products/rstudio/download/) y seleccionar nuestro sistema operativo en el menú *Installers for Supported Platforms*. 

Para Ubuntu, hay que correr estas líneas en Terminal:

`sudo apt-get install gdebi-core`

`wget https://download2.rstudio.org/server/xenial/amd64/rstudio-server-1.3.1093-amd64.deb`

`sudo gdebi rstudio-server-1.3.1093-amd64.deb`

<div style="margin-bottom:25px;">
</div>
<br>


## ¿Cómo instalo LaTeX?

Es importante tener LaTeX para crear documentos en PDF. Para instalarlo, hay que entrar a [este sitio](https://www.latex-project.org/get/) y seleccionar nuestro sistema operativo. 

<br>

<br>
<br>
<br>
<br>


## Textos, libros y materiales

### Para aprender R

Hay, realmente, miles de materiales excelentes para aprender `R`. En mi experiencia éstos han sido los más útiles.

- [**Wickham y Grolemund** - R for Data Science](https://r4ds.had.co.nz/): Este el libro sagrado de los que usamos `R` a través del `tidyverse`. Es el mejor y más completo libro para aprender a usar en lenguaje. Les recomiendo mucho terminarlo.
  
- [Cotton - Learning R A Step-by-Step Function Guide to Data Analysis](http://shop.oreilly.com/product/0636920028352.do)

- [Phillips - YaRrr! The Pirate’s Guide to R](https://ndphillips.github.io/piratesguide.html): Una guía introductoria (y bastante divertida) de aprender `R`. Altamente recomendable también para aprender métodos bayesianos. Yo aprendí `R` con este manual. Phillips también tiene gran material introductorio [en su canal de YouTube](https://www.youtube.com/watch?v=Vkv7-nw3wwU&list=PL9tt3I41HFS9gmeZFEuNrnu_7V_NFngfJ)

- [What They Forgot to Teach You About R - Bryan & Hester](https://whattheyforgot.org/)
  
- [Burns - R's Inferno](https://www.burns-stat.com/pages/Tutor/R_inferno.pdf): La premisa del autor es simple "si estás usando R y piensas que es un infierno, este libro es para ti".

- [Privé - Advanced R Course](https://privefl.github.io/advr38book/index.html):Un buen libro avanzado sobre el tema.

### Para resolver (y buscar dudas)

- [Stack Overflow](https://stackoverflow.com/): No hay de otra, **es crucial preguntar**.
  
- [Statistical tools for high-throughput data analysis](http://www.sthda.com/english/)

- [UC Business Analytics R Programming Guide](https://uc-r.github.io/)
  
- [Prabhakaran - Top 50 ggplot2 Visualizations - The Master List (With Full R Code)](http://r-statistics.co/Top50-Ggplot2-Visualizations-MasterList-R-Code.html)
  
- [Sebastián Garrido - Recursos para R](http://segasi.com.mx/cursos/recursos_r/recursos/index.html): "Segasi" ha recolectado un montón de recursos introductorios (y no tanto) en su página personal.

<div style="margin-bottom:25px;">
</div>

<br>


<br>
<br>
<br>
<br>

#### RMarkdown y otras herramientas

En este curso se pretende que podamos presentar resultados en reportes profesionales y muy elegantes que puean ser leídos (y usados) por cualquiera. Así, usaremos *Markdown* "con sabor" a `R` para generar código y resultados.

- [Xie, Allaire & Grolemund - R Markdown: The Definitive Guide](https://bookdown.org/yihui/rmarkdown/): La Guía definitiva para usar *Markdown* "con sabor" a R.
  
- [A simple guide to LaTeX - Step by Step](https://www.latex-tutorial.com/tutorials/): Si bien no usaremos *LaTeX* directamente, sí es importante tenerlo instalado y conocer su existencia y su sintaxis básica para usarla en *RMarkdown*.

### Para estadística en R

Este curso está construido en mayor o menor medida con base en siguientes materiales:

- [Ismay & Kim - Statistical Inference via Data Science: A ModernDive into R and the Tidyverse](https://moderndive.netlify.com/index.html). 

- [Navarro - Learning statistics with R: A tutorial for psychology students and other beginners.](https://learningstatisticswithr.com/book/). El código del libro disponible [aquí](https://learningstatisticswithr.com/).
  
- [Hanck et al. - Introduction to Econometrics with R](https://www.econometrics-with-r.org/1-introduction.html)

- [Field et a. - Discovering Statistics Using R](https://uk.sagepub.com/en-gb/eur/discovering-statistics-using-r/book236067). Este libro es bastante didáctico, pero un poco infantil para personas más maduras.

- [Sheather - A Modern Approach to Regression with R](https://www.springer.com/la/book/9780387096070). El código se encuentra [aquí](https://www.stat.tamu.edu/~sheather/book/).

- [James, et al. -  An Introduction to Statistical Learning with Applications in R](https://www-bcf.usc.edu/~gareth/ISL/). El PDF y el código se encuentran en el link.

- [Bruce & Bruce - Practical Statistics for Data Scientists 50 Essential Concepts](http://shop.oreilly.com/product/0636920048992.do): El código de este libro se encuentra en [este repositorio](https://github.com/andrewgbruce/statistics-for-data-scientists/tree/master/src).

- [Hastie, et al. - The Elements of Statistical Learning](https://web.stanford.edu/~hastie/ElemStatLearn/). El PDF y el código se encuentran en el link.
  
- [Teetor - R Cookbook Proven Recipes for Data Analysis, Statistics, and Graphics](http://shop.oreilly.com/product/9780596809164.do)

- [Noli Brazil - Quantitative Methods in Community Research](https://crd150.github.io/index.html)
  
- [Manuel Gimond - Intro to GIS and Spatial Analysis](https://mgimond.github.io/Spatial/index.html)

- [Claudia Engel - Using Spatial Data in R](https://cengel.github.io/R-spatial/)

- [Corey Sparks](https://rpubs.com/corey_sparks)

<br>
<br>
<br>
<br>


## Repositorios de bases de datos

Algunos repositorios recomendados para buscar buenas bases de datos.

- [Awesome Public Datasets](https://github.com/awesomedata/awesome-public-datasets)
- [TidyTuesday Datasets](https://github.com/rfordatascience/tidytuesday)
- [FiveThirtyEight](https://github.com/rudeboybert/fivethirtyeight)
- [Las bases de datos del programa de competencias *Kaggle*](https://www.kaggle.com/datasets)
- [Harvard Dataverse](https://dataverse.harvard.edu/)
- [Datos abiertos del Gobierno Federal](https://datos.gob.mx/)
- [Datos abiertos de la Ciudad de México](https://datos.cdmx.gob.mx/)
- [Datos abiertos del Estado de Jalisco](https://datos.jalisco.gob.mx/)
- [Banco de Información del LNPP del CIDE](http://datos.cide.edu/)
- [Google Dataset Search](https://datasetsearch.research.google.com/)
- [Open ICPSR](https://www.openicpsr.org/openicpsr/)
- [UK Data Service](http://reshare.ukdataservice.ac.uk/)
- [Empirical Studies of Conflict](https://esoc.princeton.edu/)
- [datamx - La plataforma cívica de datos abiertos de México](http://datamx.io/)


<br>



***
<a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/">Creative Commons Attribution-NonCommercial 4.0 International License</a>.




