- Introduce links within the observations, etc.
- Add routine steps to work with templates, stacks, and version control
- Change templates to use fine-grained privileges
- Steps for each kata
- Rename mapping
- Add `NoEcho` to `GithubAccessToken`
- Find the right imagery to communicate the concepts
    - hot-water tap on water dispenser to illustrate capabilities
    - add cricket quiz
- add .json version of templates
- Updates to `Description` in the template are not considered as updates to the stack
- Create survey for feedback from participants
- Add a style guide
- Add suggested exercises
- Demonstrate Jenkins version

    - If the pipeline is not provisioned successfully, you may need to delete and re-create the stack for the pipeline
    - The stack for the pipeline will fail to delete the "ArtifactStoreBucket", if the Source action ran successfully and copied any files into the bucket. If this is the case, delete the S3 bucket directly, and re-attempt deleting the stack for the pipeline.
- Introduce a `DeletionPolicy` attribute of `Retain` on the `ArtifactStoreBucket` and update the stack
