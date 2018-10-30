# mvnrepository
Myself maven repository

Usage

pom.xml:

    <repositories>
        <repository>
            <id>xwc1125-mvnrepository</id>
            <name>xwc1125-mvnrepository</name>
            <url>https://raw.githubusercontent.com/xwc1125/mvnrepository/master/repository</url>
        </repository>
    </repositories>

## Install jar to  repository
        for example:
        
        mvn install:install-file -Dfile=/Users/xwc1125/Downloads/libs/slf4j-api-1.6.6.jar -DgroupId=com.xwc1125.log -DartifactId=slf4j-api -Dversion=1.6.6 -Dpackaging=jar -DgeneratePom=true -DcreateChecksum=true
        
        or
        
        mvn install:install-file -Dfile=/Downloads/libs/slf4j-api-1.6.6.jar -DgroupId=com.xwc1125.log -DartifactId=slf4j-api -Dversion=1.6.6 -Dpackaging=jar -DgeneratePom=true -DlocalRepositoryPath=/Users/xwc1125/Workspaces/Git/xwc1125/mvnrepository/repository -DcreateChecksum=true
        

## Update the maven-repo
        git push to the Github