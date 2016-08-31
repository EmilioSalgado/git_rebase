#¿Qué es git rebase?

####Al igual que merge, rebase es una herramienta de git que nos permite realizar la unión entre ramas.

#¿Qué hace rebase de especial?

####Cuando nosotros utilizamos esta herramienta para unir ramas, git sencillamente reproduce los cambios que consolidamos uno a uno en nuestra rama de trabajo y los lleva a la rama a donde queremos unirlos, es decir, genera una especie de archivos virtuales que vienen siendo nuevas consolidaciones en la rama a la que se le unirán los cambios y los ubica uno detrás del otro en el mismo orden que se realizaron. Utilizando la estrategia de "rebase" al unir ramas, nos puede ayudar a evitar conflictos, siempre y cuando se realice con commits que no se hayan hecho públicos, es decir, que no se encuentren en un servidor remoto. Si dichos cambios se encontraran abiertos al público y existiera gente trabajando sobre ellos y a nosotros se nos ocurre aplicar un rebase, puede que los compañeros que están compartiendo el repositorio nos lleguen a odiar, ya que estamos modificando todos los commits y posiblemente el conflicto posterior al rebase sea más difícil de reparar de lo que piensan. Por lo tanto como regla de oro jamas utilicen "rebase" posterior a la realización de un "git push" o sobre "commits" que ya se encuentren en el repositorio remoto.
