# MSBuild Arguments #
These arguments will cause MSBuild to create a WebDeploy package for easier
deployment to IIS and the cloud. Copy and paste them into the Build Solution
task's MSBuild Arguments field.

```
/p:DeployOnBuild=true /p:WebPublishMethod=Package /p:PackageAsSingleFile=true 
/p:SkipInvalidConfigurations=true /p:PackageLocation="$(build.artifactstagingdirectory)\\"
```