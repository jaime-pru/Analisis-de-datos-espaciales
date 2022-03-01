---
title: 'Spatial data analysis with R: wrangling, visualization and econometric models '

tags:
 -R software
 -Rstats
 -regional science
 -data visualization
 -spatial autocorrelation
 -spatial econometrics

authors:
 - name: Jaime A. Prudencio-Vázquez 
   orcid: 0000-0001-5866-1280
   affiliation: 1

affiliations:
 - name: Economics Department, Universidad Autónoma Metropolitana, Unidad Azcapotzalco, CDMX, México.  
   index: 1

date: 1 March 2022

bibliography: paper.bib

---

# Summary

Spatial data analysis with R: wrangling, visualization and econometric models is a [complete open course](https://github.com/jaime-pru/Analisis-de-datos-espaciales) in Spanish for the analysis of spatial information in R software. The course is aimed at Spanish-speaking economics undergraduate students interested in developing technical skills for the quantitative analysis required by regional sciences and the spatial approach of economics.

Its objective is to guide the reader, from a fundamentally practical approach, in the knowledge and handling of techniques for the exploration, analysis and modeling of spatial information through the use of R [@RSoftware] and RStudio, a computer program and programming language focused on statistical analysis. and information visualization and an integrated development environment (IDE), respectively.

The course appears in the form of an electronic book and is structured in five chapters of gradual learning. In chapter 1, the basic elements of R and RStudio are presented through the use of the exploratory data analysis approach, that is, the student is fully introduced to the use of the software to propose and solve questions related to the data structure through various information visualization and manipulation tools.

Chapter 2 shows how to create various types of choropleth maps and the enormous flexibility of style customization that R has for this purpose. Chapter 3 presents the tools to carry out an exploratory analysis of spatial data where the reader will find a way to define the interrelationships that occur in space through the construction of spatial weight matrices and will learn about spatial autocorrelation and its implications in the analysis of information. Meanwhile, in chapter 4, a very synthetic review of simple regression models is presented, emphasizing the problem of autocorrelation that could occur when estimating a linear model with spatial data. Finally, in chapter 5, some of the different spatial econometric modeling alternatives available in R are shown.

All the exercises that are presented in the course are based on a database about information on the situation of the COVID19 pandemic between March and September 2020 in the Metropolitan Area of Valle de México, the largest metropolitan area in Mexico, integrated by 76 local administrative units or municipalities and that has more than 21 million inhabitants. In addition, the database used provides information on the economic structure at the municipal level and a set of variables of a sociodemographic characteristics coming from the population census.

# Story of the project

The material originates from the Area of Productive Relations in Mexico and its academic offer of a bachelor's degree in its terminal phase, Economics of Innovation: firms, networks and territory, from the Department of Economics, of the Autonomous Metropolitan University Azcapotzalco Unit, in the City of Mexico, where the author is a teacher and researcher under the figure of visiting professor.

As a teacher of spatial econometrics in the economics department of the Universidad Autónoma Metropolitana Azcapotzalco, I frequently found myself in the need to generate materials for teaching the course contents in R in the form of HTML documents that I then shared with the students, in each promotion. Thus, instead of isolated and unstructured materials, I decided to compile and order with a coherent expository logic and gradual learning the set of materials worked up to now and that now make up this course.


# Statement of Need

Regional science are characterized by their multidisciplinary character and their solid quantitative support [@Fischer2014]. Although it is true that in all study programs in economics we find a solid repertoire of quantitative instruments: mathematics, statistics and, of course, econometrics, the tools required for the analysis of reality from a spatial and regional perspective continue to be scarce within the training at the bachelor's level. [Spatial data analysis with R](https://jaime-pru.github.io/Analisis-de-datos-espaciales/index.html) seeks to be a contribution, however minimal, to remedy this situation.

Each chapter contains both theoretical and practical elements relating with the dealing to spatial data in the context of economics. These are illustrated through code segments in R that are explained in their logic and structure so that the reader is able not only to replicate the results, but also to understand what each piece of code does. In addition, throughout the chapter, exercises are proposed to deepen the knowledge about the tools that are exposed. The most appropriate way to follow the course is through the sequence proposed by the structure of the book, from chapter 1 to 5, because the learning process of the tools is exposed gradually; however, if the user of the material already feels comfortable with handling some topic, she can continue to the next one without difficulties.

Besides, a large part of the literature on the data wrangling and analysis of spatial information is still in a language other than Spanish, mostly in English, which makes it difficult for those who have not yet mastered the language to access these tools, since in Mexico English proficiency is still very low [@IMCO2015; @EF2020]. Thus, this material in Spanish becomes a gateway for those interested in these issues and facilitate the learning process.

On the other hand, the student or teacher reader interested in making some correction, modification or contribution to this course, can do so through the instructions located in the repository that contains the source files of the electronic book. All will be welcome.

# Acknowledgements

The author thanks [Montserrat Romero Martínez](vmrm@azc.uam.mx) and [Alvaro Martínez Rodríguez](amr@azc.uam.mx), assistants in the Productive Relations Area, who were respectively in charge of reviewing Preliminary materials for this book and its edition for publication online with Bookdown on GitHub.

# References
