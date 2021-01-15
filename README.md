# GradleFlagProject
This project is to demonstrate Building Gradle modules based on Flag in a Multi Module project.
Medium article is progress..

## Gradle Module Build optimizations

Add below code with comments in your local.properties file and follow the instructions

```
# For faster build time you can set this flag to true.
# If True, build configuration will add modules listed under `localModules`
# as module dependency and will remove other modules to be added as AAR dependency
# if nothing is listed under localModules all modules will be removed and added as AAR
# dependency.
#
# Note: Ensure you run ./gradlew makeAARs task once before setting this variable to generate AAR files.
#
useLocalAAR=false

# add modules which is to be added as module dependency seperated by space
# for example :  localModules=:featureA :featureB :featureC
#
devModules=:scanandgo :featureA
```
