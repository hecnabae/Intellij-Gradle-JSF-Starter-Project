# README #

**JSF/Gradle Web Application built on IntelliJ IDEA**

This web app works on IntelliJ IDEA by using Gradle System DI and JSF Framework. It's a starter for those
who need to use IntelliJ IDEA as the development platform.

### How To Use? ###
Clone the project and run it on your favorite server. Add your dependencies under build.gradle file (just like Android).
In the case of you would like to use a library -jar- that doesn't exist in maven, just place it under 'libs' filder.
Gradle will automatically import it into the project.

    compile fileTree(dir: 'libs', include: ['*.jar'])
    
Place your Java files under 'main/java'. You can create packages as well.
    
### Persistency ###
You can do your persistent configuration under 'main/resources/base_conf'. If needed, you can add new folders of
configurations for different development environments. You can use gradle's profiling.

### Localization ###
Under 'main/resources/base_conf' you can add as many Bundle files as you wish. After creating new bundle files,
add the definitions under 'webapp/WEB-INF/faces-config'