This is a temporary public synchronization of our internal maven repository, to be used with Gemserk projects until all required dependencies are in maven central.

In order to use a Gemserk project as a dependency you have to add to your settings.xml the next configuration:
```
   <profiles>
       <profile>
           <id>gemserk-maven-repo</id>
           <repositories>
               <repository>
                   <id>googlecode.gemserk.releases</id>
                   <url>http://gemserk-maven-repo.googlecode.com/svn/maven/releases/</url>
               </repository>
               <repository>
                   <id>googlecode.gemserk.snapshots</id>
                   <url>http://gemserk-maven-repo.googlecode.com/svn/maven/snapshots/</url>
               </repository>
               <repository>
                   <id>googlecode.gemserk.thirdparty</id>
                   <url>http://gemserk-maven-repo.googlecode.com/svn/maven/thirdparty/</url>
               </repository>
               <repository>
                   <id>maven2-repository.dev.java.net</id>
                   <url>http://download.java.net/maven/2/</url>
               </repository>
           </repositories>
       </profile>
   </profiles>
  <activeProfiles>
    <activeProfile>gemserk-maven-repo</activeProfile>
  </activeProfiles>
```