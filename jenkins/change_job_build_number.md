# Change job build number

If you have access to the script console (Manage Jenkins -> Script Console), then you can do this following:

```groovy
Jenkins.instance.getItemByFullName("PipelineName/BranchName").updateNextBuildNumber(45)
```

The value can be verified without building using:

```groovy
Jenkins.instance.getItemByFullName("PipelineName/BranchName").getNextBuildNumber()
```
