# Git tutorial

## By: Carlos Chacon
## 27/09/2017

![Git Logo](https://github.com/caedocha/git-tutorial/blob/master/images/logo.png)


## Que es Git?

- Version Control System (VCS) hecho por Linus Torvalds ( Linux )
- Bajar Git aqui: https://git-scm.com/downloads




dddd

## Que es Github?

- Es un servicio que ofrece "hosting" de repositorios remotos.
- Muchos proyectos Open Source lo usan para "hostear" sus proyectos.



![Workflow](https://github.com/caedocha/git-tutorial/blob/master/images/workflow.png)

## Crear Un Repositorio

```ruby
  git init git-tutorial
```


## Clonar Un Repositorio De Github

```ruby
  git clone https://github.com/caedocha/git-tutorial.git
```


## Como Compartir Sus Cambios?

- Agregar los archivos modificados del "Working Directory" al "Index"
- Crear un "commmit" a partir de los cambios en el Index
- Subir el "commit" a Github

```ruby
  git add . # Agregar todos los archivos modificados
  -- o --
  git add test.rb # Agregar un archivo especifico

  git commit -m "Add test.rb"
  git push origin master
```


## Descargar Cambios

```ruby
  git pull origin master
```


## Ver Archivos Modificados

```ruby
  git status
```


## Ver Cambios En Archivos

```ruby
  git diff
```



![Stages](https://github.com/caedocha/git-tutorial/blob/master/images/stages.png)

## Branches

- Mecanismo para divergir del branch principal.
- El branch default es `master`
- Ideal para desarrollar features nuevos o probar soluciones sin afectar a los demas.



![Branches](https://github.com/caedocha/git-tutorial/blob/master/images/branches.png)

## Como Crear Un Branch Nuevo?

```ruby
  git checkout -b <nombre-de-branch-nuevo>
  git checkout -b "mi-nuevo-feature"
```


## Como Moverme Entre Branches?

```ruby
  git checkout <nombre-de-branch>
  git checkout master
```


## Merge Mis Cambios Al Branch Principal

- Moverme al branch al que le quiere "mergear" mi branch.
- Mergear mi branch al branch objetivo.

```ruby
  git checkout master
  git merge mi-nuevo-feature
```


## Recursos

- Git - The Simple Guide: http://rogerdudler.github.io/git-guide/
- Pro Git: https://git-scm.com/book/en/v2


## Agradecimientos

**Muchas gracias!**


