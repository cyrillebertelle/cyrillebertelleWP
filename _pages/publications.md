---
layout: page
permalink: /publications/
title: publications
description: 
years: [2021, 2020, 2019, 2018, 2017, 2016, 2015, 2014, 2013, 2012, 2011, 2010, 2009, 2008, 2007, 2006, 2005, 2004, 2003, 2002, 2001, 2000, 1999, 1998, 1997, 1991, 1990, 1989, 1988]
nav: true
---

Many publications are available from 
* [my personal Hal repository](https://haltools.archives-ouvertes.fr/Public/afficheRequetePubli.php?auteur_exp=cyrille+bertelle&CB_auteur=oui&CB_titre=oui&CB_article=oui&langue=Anglais&tri_exp=annee_publi&tri_exp2=typdoc&tri_exp3=date_publi&ordre_aff=TA&Fen=Aff&css=../css/VisuRubriqueEncadre.css)
* or [my Google Scholar page](https://scholar.google.com/citations?user=Twj3qDQAAAAJ&hl=fr)

Below many publications are listed by categories in reversed chronological order, generated by jekyll-scholar. It contains 250 references including 7 books, 14 publications of proceedings or special issues of journals, 24 book chapters, 48 journal articles, 148 conference papers (as of end August 2021).

<div class="publications">
 
{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
