# Template pour un projet Java
Ce projet propose un modèle pour démarrer des projets Java.
Son usage nécessite bien sûr l'installation préalable du [JDK](https://adoptopenjdk.net/).

## Compiler le projet
Le projet se compile en utilisant [gradle](https://gradle.org/) et plus précisément le plugin [gradle wrapper](https://docs.gradle.org/current/userguide/gradle_wrapper.html).

Sous Linux
```bash
> ./gradlew build
```

Sous Windows
```
> gradlew.bat build
```

## Éxécuter l'application
L'exécution utilise le plugin Gradle [Application](https://docs.gradle.org/current/userguide/application_plugin.html).

```bash
$ ./gradlew run
```

Des archives zip ou tar se trouvant dans le répertoire ``build/distributions``.

## Créer un projet à partir du template
1. Changer le nom du projet dans
    * ``settings.gradle.kts``
    * ``build.gradle.kts`` (nom du package de la classe principale)
    * ``src/main/java/fr/uvsq/poo/tpljava`` (nom du package)
    * ``src/main/java/fr/uvsq/poo/tpljava/Application.java`` (nom du package)
    * ``src/test/java/fr/uvsq/poo/tpljava`` (nom du package)
    * ``src/test/java/fr/uvsq/poo/tpljava/ApplicationTest.java`` (nom du package)
1. Modifier le README.md

## Mettre à jour la version de Gradle
Pour déterminer la version de Gradle actuellement utilisée dans le projet :
```
> ./gradlew help
```

Pour mettre à jour la version de Gradle vers la version 6.5 :
```
> ./gradlew wrapper --gradle-version 6.5
```
