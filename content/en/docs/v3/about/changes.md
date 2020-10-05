---
title: Changes
linktitle: Changes
description: The change log for Jenkins X 3.x
weight: 55
---

You may also find the [Roadmap](/community/roadmap/) and [Maturity Matrix](/docs/v3/about/maturity-matrix/) documents useful:


## Changes 

* We now have [Tekton Catalog integration](/docs/v3/guides/pipeline-catalog/) so that you can:
  * easily [edit any pipeline in any git repository](/docs/v3/guides/pipeline-catalog/#editing-pipelines) by just modifying the `PipelineRun` files in your `.ligthhouse/jenkins-x` folder
  * [add new pipelines to any git repository](/docs/v3/guides/pipeline-catalog/#add-new-pipelines) to reuse any `PipelineRun` files you find from places like the [tekton catalog](https://github.com/tektoncd/catalog) into your repositories

* We have migrated most of the [Jenkins X Plugins](https://github.com/jenkins-x/jx-cli#plugins) over to the new client-go 1.19.x version now which is a fairly major change due to the API changes in client-go. So we've moved many of the [libraries](https://github.com/jenkins-x/jx-cli#libraries) over to use `v3` instead such as using libraries like [jx-api](https://github.com/jenkins-x/jx-api) or [jx-helpers](https://github.com/jenkins-x/jx-helpers)
  * if you were planning on submitting a Pull Request on any plugin please make sure you rebase before submitting a Pull Request. Also upgrade to go `1.15.2` ASAP 
  
* New [Maturity Matrix](/docs/v3/about/maturity-matrix/) published! You can now view at a glance the different capabilities across clouds and infrastructure. Many thanks [Nitin](https://github.com/borntorock) for all your hard work