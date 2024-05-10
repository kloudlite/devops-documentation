# Basic Concepts

Kloudlite makes application deployment and management straightforward by organizing resources efficiently. This guide introduces the core concepts of Kloudlite, designed to equip developers with a comprehensive toolkit.

### Kloudlite Project

A **Kloudlite Project** is where your application's environments and managed services live. It's the main organizational structure in Kloudlite, containing everything your applications need to run smoothly.

Read more about project below:

[setup-first-project.md](getting-started/setup-first-project.md "mention")

### Managed Services

**Managed Services** are key services that your application relies on to function. Kloudlite simplifies the process of setting up, managing, and maintaining these services, including:

* **MongoDB** (available in both Cluster and Standalone modes)
* **MySQL** (available in both Cluster and Standalone modes)
* **Redis** (available in both Cluster and Standalone modes)

These services are managed by Kloudlite to free you from manual setup and maintenance, ensuring your applications have the support they need. We're always working to add more services.

Read more about managed services below:

[create-managed-service.md](getting-started/create-managed-service.md "mention")

### Environment

An **Environment** in a Kloudlite Project includes your applications, configurations, secrets, managed resources, and routing. Environments are designed to be stateless, making it easy to replicate or remove them, which supports flexible and scalable application development.

Read more about environment below:

[create-environment.md](getting-started/create-environment.md "mention")

### Kloudlite Application

A **Kloudlite Application** is a Kubernetes resource tailored for managing your application's deployment, service, autoscaling, and monitoring, ensuring efficient and scalable management of your workloads.

Read more about application below:

[create-app.md](getting-started/create-app.md "mention")

### Router & Routes

**Router & Routes** manage how external traffic reaches your applications, controlling the entry points and communication pathways to your services.

Read more about router and route below:

[create-router-and-route.md](getting-started/create-router-and-route.md "mention")

### Managed Resources

**Managed Resources** are connections to Managed Services like a MySQL database or a Kafka topic. They facilitate the use of managed services in your environments without maintaining any state themselves.

Read more about managed resource below:

[create-managed-resource.md](getting-started/create-managed-resource.md "mention")



## Image Pull Secrets

The "Image Pull Secrets" feature allows users to securely pull private container images from external container registries during Kubernetes deployments. This feature is essential for users who store their container images in private repositories that require authentication.

[image-pull-secrets.md](getting-started/image-pull-secrets.md "mention")
