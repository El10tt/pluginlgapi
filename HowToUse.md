# How to use

Une API pour intéragir avec le plugin de LG UHC By Ph1Lou

## Getting Started

Cette API a pour but d'être intégré dans un plugin tournant dans la même jvm que le plugin lg uhc. Cette API permet d'intéragir avec le plugin.

### Prerequisites
Vous aurez besoin du plugin lg uhc en version snapshot 1.15 dernière version en cours. Cette version est disponible sur mon discord en demandant le rôle Snapshot viewer.

### Installing
Pour installer cette API dans votre projet avec maven, nous allons utiliser le site [JitPack.io](https://jitpack.io "JitPack.io").

#### Maven
##### Repository
Dans votre fichier *pom.xml*, allez dans la section *repositories* et ajoutez:
```xml
<repository>
            <id>jitpack.io</id>
            <url>https://jitpack.io</url>
</repository>
```

##### Dependency
Dans votre fichier *pom.xml*, allez dans la section *dependencies* et ajoutez:
```xml
<dependency>
            <groupId>io.github.ph1lou</groupId>
            <artifactId>pluginlgapi</artifactId>
            <version>1.0-SNAPSHOT</version>
</dependency>
```

##### Download
Après ceci, mettez à jour les dépendances Maven.
Cette manipulation dépend de votre IDE. Sur Intellij IDEA, un logo Maven avec une flêche apparaîtra, cliquez dessus.

#### Gradle
##### Repository
Ajoutez-le dans votre fichier *build.gradle*  à la fin de la section *repositories* comme ceci:
```
allprojects {
	repositories {
		...
		maven { url 'https://jitpack.io' }
	}
}
```

##### Dependency
Ajoutez la dépendance dans votre fichier *build.gradle*.
```
dependencies {
	        implementation 'com.github.Ph1Lou:pluginlgapi:1.0-SNAPSHOT'
}
```
#### Without Maven or Gradle
Téléchargez et compilez le projet, ajoutez le tel Spigot à votre projet.

### Initialization
```java
GetWereWolfAPI ww = (GetWereWolfAPI) Bukkit.getPluginManager().getPlugin("pluginLG");
```
Puis :
```java
WerewolfApi werewolfAPI = ww.getWereWolfAPI();
```

### Usage
// Comming Soon
