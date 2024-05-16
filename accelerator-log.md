# Accelerator Log

## Options
```json
{
  "deploymentType" : "manifest",
  "message" : "World",
  "projectName" : "hello-world"
}
```
## Log
```
┏ engine (Chain)
┃  Info Running Chain(Exclude, GeneratorValidationTransform, UniquePath)
┃ ┏ engine.transformations[0] (Exclude)
┃ ┃  Info Will exclude [accelerator.yaml, accelerator.axl]
┃ ┃ Debug .gitignore didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug LICENSE didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug README.md didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug accelerator.yaml matched [accelerator.yaml, accelerator.axl] -> excluded
┃ ┃ Debug cloudfoundry/DEPLOYING.md didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug cloudfoundry/manifest.yml didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug mvnw didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug mvnw.cmd didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug pom.xml didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug src/main/java/com/example/hello/HelloWorldApplication.java didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug src/main/java/com/example/hello/HelloWorldController.java didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug src/main/resources/application.properties didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug src/test/java/com/example/hello/HelloWorldApplicationTests.java didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug tap/DEPLOYING.md didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┃ Debug tap/catalog-info.yaml didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┗ Debug tap/workload.yaml didn't match [accelerator.yaml, accelerator.axl] -> included
┃ ┏ ┏ engine.transformations[1].validated (Combo)
┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ engine.transformations[1].validated.delegate (Chain)
┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┏ engine.transformations[1].validated.delegate.transformations[0] (Merge)
┃ ┃ ┃ ┃  Info Running Merge(Combo, Combo, Combo, Combo, Combo, Combo, Combo)
┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.delegate.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ engine.transformations[1].validated.delegate.transformations[0].sources[0].delegate (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, Exclude)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.delegate.transformations[0].sources[0].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**]
┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug cloudfoundry/DEPLOYING.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug cloudfoundry/manifest.yml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/hello/HelloWorldApplication.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/hello/HelloWorldController.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/hello/HelloWorldApplicationTests.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug tap/DEPLOYING.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug tap/catalog-info.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┗ Debug tap/workload.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.delegate.transformations[0].sources[0].delegate.transformations[1] (Exclude)
┃ ┃ ┃ ┃ ┃ ┃  Info Will exclude [pom.xml, README.md, cloudfoundry/**, tap/**, .github/workflows/**]
┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [pom.xml, README.md, cloudfoundry/**, tap/**, .github/workflows/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [pom.xml, README.md, cloudfoundry/**, tap/**, .github/workflows/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [pom.xml, README.md, cloudfoundry/**, tap/**, .github/workflows/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [pom.xml, README.md, cloudfoundry/**, tap/**, .github/workflows/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [pom.xml, README.md, cloudfoundry/**, tap/**, .github/workflows/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug cloudfoundry/DEPLOYING.md matched [pom.xml, README.md, cloudfoundry/**, tap/**, .github/workflows/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug cloudfoundry/manifest.yml matched [pom.xml, README.md, cloudfoundry/**, tap/**, .github/workflows/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [pom.xml, README.md, cloudfoundry/**, tap/**, .github/workflows/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [pom.xml, README.md, cloudfoundry/**, tap/**, .github/workflows/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [pom.xml, README.md, cloudfoundry/**, tap/**, .github/workflows/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/hello/HelloWorldApplication.java didn't match [pom.xml, README.md, cloudfoundry/**, tap/**, .github/workflows/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/hello/HelloWorldController.java didn't match [pom.xml, README.md, cloudfoundry/**, tap/**, .github/workflows/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [pom.xml, README.md, cloudfoundry/**, tap/**, .github/workflows/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/hello/HelloWorldApplicationTests.java didn't match [pom.xml, README.md, cloudfoundry/**, tap/**, .github/workflows/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug tap/DEPLOYING.md matched [pom.xml, README.md, cloudfoundry/**, tap/**, .github/workflows/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug tap/catalog-info.yaml matched [pom.xml, README.md, cloudfoundry/**, tap/**, .github/workflows/**] -> excluded
┃ ┃ ┃ ┃ ┗ ┗ Debug tap/workload.yaml matched [pom.xml, README.md, cloudfoundry/**, tap/**, .github/workflows/**] -> excluded
┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.delegate.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ engine.transformations[1].validated.delegate.transformations[0].sources[1].delegate (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.delegate.transformations[0].sources[1].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃  Info Will include [pom.xml]
┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug cloudfoundry/DEPLOYING.md didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug cloudfoundry/manifest.yml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [pom.xml] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/hello/HelloWorldApplication.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/hello/HelloWorldController.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/hello/HelloWorldApplicationTests.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug tap/DEPLOYING.md didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug tap/catalog-info.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┗ Debug tap/workload.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.delegate.transformations[0].sources[1].delegate.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┗ ┗  Info Will replace [hello-world->hello-world]
┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.delegate.transformations[0].sources[2] (Combo)
┃ ┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'none') evaluated to false
┃ ┃ ┃ ┃ ┗ null ()
┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.delegate.transformations[0].sources[3] (Combo)
┃ ┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'manifest') evaluated to true
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ engine.transformations[1].validated.delegate.transformations[0].sources[3].delegate (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText, RewritePath)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.delegate.transformations[0].sources[3].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃  Info Will include [cloudfoundry/manifest.yml]
┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [cloudfoundry/manifest.yml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [cloudfoundry/manifest.yml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [cloudfoundry/manifest.yml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [cloudfoundry/manifest.yml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [cloudfoundry/manifest.yml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug cloudfoundry/DEPLOYING.md didn't match [cloudfoundry/manifest.yml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug cloudfoundry/manifest.yml matched [cloudfoundry/manifest.yml] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [cloudfoundry/manifest.yml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [cloudfoundry/manifest.yml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [cloudfoundry/manifest.yml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/hello/HelloWorldApplication.java didn't match [cloudfoundry/manifest.yml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/hello/HelloWorldController.java didn't match [cloudfoundry/manifest.yml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [cloudfoundry/manifest.yml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/hello/HelloWorldApplicationTests.java didn't match [cloudfoundry/manifest.yml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug tap/DEPLOYING.md didn't match [cloudfoundry/manifest.yml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug tap/catalog-info.yaml didn't match [cloudfoundry/manifest.yml] -> excluded
┃ ┃ ┃ ┃ ┃ ┗ Debug tap/workload.yaml didn't match [cloudfoundry/manifest.yml] -> excluded
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.delegate.transformations[0].sources[3].delegate.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [hello-world->hello-world, World->World]
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.delegate.transformations[0].sources[3].delegate.transformations[2] (RewritePath)
┃ ┃ ┃ ┃ ┗ ┗ Debug Path 'cloudfoundry/manifest.yml' matched '^(?<folder>.*/)?(?<filename>([^/]+?|)(?=(?<ext>\.[^/.]*)?)$)' with groups {ext=.yml, folder=cloudfoundry/, filename=manifest.yml, g0=cloudfoundry/manifest.yml, g1=cloudfoundry/, g2=manifest.yml, g3=manifest.yml, g4=.yml} and was rewritten to 'config/manifest.yml'
┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.delegate.transformations[0].sources[4] (Combo)
┃ ┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'workload') evaluated to false
┃ ┃ ┃ ┃ ┗ null ()
┃ ┃ ┃ ┃ ┏ engine.transformations[1].validated.delegate.transformations[0].sources[5] (Combo)
┃ ┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'workload') evaluated to false
┃ ┃ ┃ ┃ ┗ null ()
┃ ┃ ┃ ┃ ┏ README (Combo)
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ README.delegate (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┏ README.delegate.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(Combo, Combo, Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┏ README.delegate.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ ┃ README.delegate.transformations[0].sources[0].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ README.delegate.transformations[0].sources[0].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [README.md]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug cloudfoundry/DEPLOYING.md didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug cloudfoundry/manifest.yml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/hello/HelloWorldApplication.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/hello/HelloWorldController.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/hello/HelloWorldApplicationTests.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug tap/DEPLOYING.md didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug tap/catalog-info.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug tap/workload.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ README.delegate.transformations[0].sources[0].delegate.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗  Info Will replace [hello-world->hello-world]
┃ ┃ ┃ ┃ ┃ ┃ ┏ README.delegate.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'manifest') evaluated to true
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ ┃ README.delegate.transformations[0].sources[1].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText, RewritePath)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ README.delegate.transformations[0].sources[1].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [cloudfoundry/DEPLOYING.md]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [cloudfoundry/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.jar didn't match [cloudfoundry/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [cloudfoundry/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [cloudfoundry/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [cloudfoundry/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug cloudfoundry/DEPLOYING.md matched [cloudfoundry/DEPLOYING.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug cloudfoundry/manifest.yml didn't match [cloudfoundry/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [cloudfoundry/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [cloudfoundry/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [cloudfoundry/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/hello/HelloWorldApplication.java didn't match [cloudfoundry/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/hello/HelloWorldController.java didn't match [cloudfoundry/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [cloudfoundry/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/hello/HelloWorldApplicationTests.java didn't match [cloudfoundry/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug tap/DEPLOYING.md didn't match [cloudfoundry/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug tap/catalog-info.yaml didn't match [cloudfoundry/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug tap/workload.yaml didn't match [cloudfoundry/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ README.delegate.transformations[0].sources[1].delegate.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [hello-world->hello-world]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ README.delegate.transformations[0].sources[1].delegate.transformations[2] (RewritePath)
┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗ Debug Path 'cloudfoundry/DEPLOYING.md' matched '^(?<folder>.*/)?(?<filename>([^/]+?|)(?=(?<ext>\.[^/.]*)?)$)' with groups {ext=.md, folder=cloudfoundry/, filename=DEPLOYING.md, g0=cloudfoundry/DEPLOYING.md, g1=cloudfoundry/, g2=DEPLOYING.md, g3=DEPLOYING.md, g4=.md} and was rewritten to 'README.md'
┃ ┃ ┃ ┃ ┃ ┃ ┏ README.delegate.transformations[0].sources[2] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'workload') evaluated to false
┃ ┃ ┃ ┃ ┃ ┗ ┗ null ()
┃ ┃ ┃ ┃ ┃ ┏ README.delegate.transformations[1] (UniquePath)
┃ ┃ ┃ ┗ ┗ ┗ Debug Multiple representations for path 'README.md', will concatenate them together
┃ ┗ ┗ ╺ engine.transformations[1].validated.delegate.transformations[1] (UniquePath)
┗ ╺ engine.transformations[2] (UniquePath)
```
