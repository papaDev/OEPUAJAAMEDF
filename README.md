# OEPUAJAAMEDF
Cours Organisez et packagez une application Java avec Apache Maven Exercice de Fin

# Commande pour créer le projet parent à l'aide de l'archétype maven-archetype-quickstart

mvn archetype:generate -DarchetypeGroupId=org.apache.maven.archetypes -DarchetypeArtifactId=maven-archetype-quickstart -DarchetypeVersion=1.1 -DgroupId=org.exercice.exo -DartifactId=ExerciceDeFin -Dversion=1.0-SNAPSHOT

Cette commande créer le projet parent "ExerciceDeFin" 

Entrez dans le projet créer avec la commancde suivante :

=> cd ExerciceDeFin

Editez le fichier pom.xml
	Modifiez le packaging du projet. Il faut utiliser le packaging pom au lieu de jar
	
# Créez ensuite tous les modules (sous-projets Maven) à l'aide d'archétypes
	=> ExerciceDeFin-batch (archétype maven-archetype-quickstart)
	Avec la commande suivante
	
	mvn -B archetype:generate \
	-DarchetypeGroupId=org.apache.maven.archetypes \
	-DarchetypeArtifactId=maven-archetype-quickstart \
	-DarchetypeVersion=1.1 \
	-DgroupId=org.exercice.exo \
	-DartifactId=ExerciceDeFin-batch \
	-Dpackage=org.exercice.exo.batch
	
	=> ExerciceDeFin-webapp (archétype maven-archetype-webapp)
	
    mvn -B archetype:generate \
    -DarchetypeGroupId=org.apache.maven.archetypes \
    -DarchetypeArtifactId=maven-archetype-webapp \
    -DgroupId=org.exercice.exo \
    -DartifactId=ExerciceDeFin-webapp \
    -Dpackage=org.exercice.exo.webapp
    
    => ExerciceDeFin-business (archétype maven-archetype-quickstart)
    
    mvn -B archetype:generate \
        -DarchetypeGroupId=org.apache.maven.archetypes \
        -DarchetypeArtifactId=maven-archetype-quickstart \
        -DarchetypeVersion=1.1 \
        -DgroupId=org.exercice.exo \
        -DartifactId=ExerciceDeFin-business \
        -Dpackage=org.exercice.exo.business
    
    => ExercieDeFin-consumer (archétype maven-archetype-quickstart)
    
    mvn -B archetype:generate \
        -DarchetypeGroupId=org.apache.maven.archetypes \
        -DarchetypeArtifactId=maven-archetype-quickstart \
        -DarchetypeVersion=1.1 \
        -DgroupId=org.exercice.exo \
        -DartifactId=ExerciceDeFin-consumer \
        -Dpackage=org.exercice.exo.consumer
    
    => ExerciceDeFin-model (archétype maven-archetype-quickstart)

    mvn -B archetype:generate \
        -DarchetypeGroupId=org.apache.maven.archetypes \
        -DarchetypeArtifactId=maven-archetype-quickstart \
        -DarchetypeVersion=1.1 \
        -DgroupId=org.exercice.exo \
        -DartifactId=ExerciceDeFin-model \
        -Dpackage=org.exercice.exo.model
    