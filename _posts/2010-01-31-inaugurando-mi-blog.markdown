---
layout: post
title: Inaugurando mi blog
categories:
- jekyll
tags:
- jekyll
- markdown

---

Después de mucho tiempo pensando en empezar a escribir, por fin me he decidido. Pretendo escribir sobre mi día a día en el mundo del desarrollo web en [The Cocktail](http://the-cocktail.com/) y como freelance, y también sobre otras idas y venidas de olla.

A modo de introducción decir que éste site esta desarrollado con [jekyll](http://github.com/mojombo/jekyll) por recomendación directa de [pantulis](http://hronia.blogalia.com/) lo que me costo tirar a la basura toda una tarde de desarrollo en rails. La gracia de jekyll esta en que los posts los escribes en [markdown](http://en.wikipedia.org/wiki/Markdown) y los deployas directamente a producción, jekyll se encarga de generarte los html estáticos para ti. He incluido un par de widgets de facebook, tanto para compartir cualquier contenido, como para comentarlo.

Para el deploy en producción de cada post he creado un alias en mi .bash_login:

	alias deploy_blog="cd path/to/jekyll/code && echo 'Creando Html...' && jekyll --pygments 
	&& echo 'Pushing...' && rsync -avz --delete _site/ user@server.domain:path/to/directory "
	

El código al completo del blog lo tenéis disponible [aquí](http://github.com/cantorrodista/my-jekyll-blog).













