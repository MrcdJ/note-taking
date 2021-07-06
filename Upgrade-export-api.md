# Upgrade export-api

In pom.xml, check all dependencies.

## To clean later?

logstash



## What can we clean?

mockito & junit verifier qu'on a bien start-test


Avoir seulement des spring-boot-start-... pour plus propre
On peut faire des excludes d'imports faits par un starter.

ex:

<dependency>
      <groupId>org.springframework.boot</groupId>
      <artifactId>spring-boot-starter-web</artifactId>
      <exclusions>
        <exclusion>
          <!-- this dependency has be relocated to the group id -->
          <!-- org.hibernate.validator -->
          <!-- thus, avoid to include two times the hibernate-validator artifact -->
          <groupId>org.hibernate</groupId>
          <artifactId>hibernate-validator</artifactId>
        </exclusion>
      </exclusions>
    </dependency>





Voir avec Nidhal pour tests d'exploration export-api