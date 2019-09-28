## Maven Command to install odm jar in local m2 repo

### Inorder to install jar/rar file into .m2 repo in our local.

Here are example commands we can used. 
'mvn install:install-file -Dpackaging=jar -DgroupId=com.ilog.jrules -DartifactId=asm -Dversion=5.2 -Dfile=C:\new_jars\jrules\asm-5.2.jar'
`mvn install:install-file -Dpackaging=jar -DgroupId=com.ilog.jrules -DartifactId=asm-commons -Dversion=5.2 -Dfile=C:\new_jars\jrules\asm-commons-5.2.jar`
mvn install:install-file -Dpackaging=jar -DgroupId=com.ilog.jrules -DartifactId=asm-tree -Dversion=5.2 -Dfile=C:\new_jars\jrules\asm-tree-5.2.jar
mvn install:install-file -Dpackaging=jar -DgroupId=com.ilog.jrules -DartifactId=jrules-engine -Dversion=8.9.2.1 -Dfile=C:\new_jars\jrules\jrules-engine-8.9.2.1.jar
mvn install:install-file -Dpackaging=jar -DgroupId=com.ilog.executionserver -DartifactId=jrules-res-session-java -Dversion=8.9.2.1 -Dfile=C:\new_jars\executionserver\jrules-res-session-java-8.9.2.1.jar
mvn install:install-file -Dpackaging=jar -DgroupId=com.ilog.executionserver -DartifactId=jrules-res-tools -Dversion=8.9.2.1 -Dfile=C:\new_jars\executionserver\jrules-res-tools-8.9.2.1.jar
mvn install:install-file -Dpackaging=rar -DgroupId=com.ilog.executionserver -DartifactId=jrules-res-xu-WAS85 -Dversion=8.9.2.1 -Dfile=C:\new_jars\executionserver\jrules-res-xu-WAS85-8.9.2.1.rar


Below is one of the example I ran to install jrules-res-xu-WAS85 jar in my local .m2 repo.

C:\>mvn install:install-file -Dpackaging=rar -DgroupId=com.ilog.executionserver -DartifactId=jrules-res-xu-WAS85 -Dversion=8.9.2.1_B -Dfile=C:\new_jars\rules\jrules-res-xu-WAS85-8.9.2.1_B.rar
[INFO] Scanning for projects...
[INFO]
[INFO] ------------------------------------------------------------------------
[INFO] Building Maven Stub Project (No POM) 1
[INFO] ------------------------------------------------------------------------
[INFO]
[INFO] --- maven-install-plugin:2.4:install-file (default-cli) @ standalone-pom ---
[INFO] Installing C:\new_jars\rules\jrules-res-xu-WAS85-8.9.2.1_B.rar to C:\Users\i327675\.m2\repository\com\ilog\executionserver\jrules-res-xu-WAS85\8.9.2.1_B\jrules-res-xu-WAS85-8.9.2.1_B.rar
[INFO] Installing C:\Users\<id>\AppData\Local\Temp\mvninstall687550819361853982.pom to C:\Users\i327675\.m2\repository\com\ilog\executionserver\jrules-res-xu-WAS85\8.9.2.1_B\jrules-res-xu-WAS85-8.9.2.1_B.pom
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time: 0.954 s
[INFO] Finished at: 2019-08-22T23:00:26-05:00
[INFO] Final Memory: 6M/245M
[INFO] ------------------------------------------------------------------------
C:\>

