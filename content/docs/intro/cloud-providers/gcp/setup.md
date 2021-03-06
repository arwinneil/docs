---
title: Google Cloud Platform (GCP) Setup
meta_desc: This page provides an overview on how to setup the Google Cloud
           Platform Provider with Pulumi.
aliases: ["/docs/reference/clouds/gcp/setup/"]
---

[Pulumi Google Cloud Platform Provider]: {{< relref "./" >}}

The [Pulumi Google Cloud Platform Provider] needs to be configured with Google credentials
before it can be used to create resources.

When developing locally, we recommend that you use `gcloud login` to configure your account credentials. First, install the [Google Cloud SDK](https://cloud.google.com/sdk/install), which includes the `gcloud` command line tool. Then, execute the following:

```bash
$ gcloud auth login
$ gcloud config set project <YOUR_GCP_PROJECT_HERE>
$ gcloud auth application-default login
```

If you are using Pulumi in an non-interactive setting (such as a CI/CD system) you will need to [configure and use a service account]({{< relref "service-account" >}}) instead.

## Optional Settings

The Pulumi Google Cloud Platform Provider accepts these environment variables
to further configure the provider:

* `GOOGLE_PROJECT` - The default project for new resources, if one is not specified
when creating a resource
* `GOOGLE_REGION` - The default region for new resources, if one is not specified
when creating a resource
* `GOOGLE_ZONE` - The default zone for new resources, if one is not specified when
creating a resource.

If these values are not provided, some resources may require you to provide these
values as `project`, `region`, or `zone` properties.  You may also set these values per project using `pulumi config`:

```bash
$ pulumi config set gcp:project <your-project-here>
$ pulumi config set gcp:region <your-region-here>
$ pulumi config set gcp:zone <your-zone-here>
```
