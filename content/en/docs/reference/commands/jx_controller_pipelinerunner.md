---
date: 2019-09-23T21:39:11Z
title: "jx controller pipelinerunner"
slug: jx_controller_pipelinerunner
url: /commands/jx_controller_pipelinerunner/
---
## jx controller pipelinerunner

Runs the service to generate Tekton PipelineRun resources from source code webhooks such as from Prow

### Synopsis

Runs the service to generate Tekton resources from source code webhooks such as from Prow

```
jx controller pipelinerunner [flags]
```

### Examples

```
  # run the pipeline runner controller
  jx controller pipelinerunner
```

### Options

```
      --bind string                  The interface address to bind to (by default, will listen on all interfaces/addresses). (default "0.0.0.0")
  -h, --help                         help for pipelinerunner
      --meta-pipeline-image string   Specify the docker image to use if there is no image specified for a step.
      --no-git-init                  Disables checking we have setup git credentials on startup.
      --path string                  The path to listen on for requests to trigger a pipeline run. (default "/")
      --port int                     The TCP port to listen on. (default 8080)
      --semantic-release             Enable semantic releases
      --service-account string       The Kubernetes ServiceAccount to use to run the pipeline. (default "tekton-bot")
      --use-meta-pipeline            Uses the meta pipeline to create the pipeline. (default true)
```

### Options inherited from parent commands

```
  -b, --batch-mode   Runs in batch mode without prompting for user input (default true)
      --verbose      Enables verbose output
```

### SEE ALSO

* [jx controller](/commands/jx_controller/)	 - Runs a controller

###### Auto generated by spf13/cobra on 23-Sep-2019