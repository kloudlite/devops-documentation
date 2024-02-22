# Basic Concepts

Kloudlite simplifies application deployment and management by organizing resources into a coherent structure. Here's an overview of the fundamental concepts within Kloudlite, designed to provide a comprehensive toolkit for your development needs.

## Kloudlite Project

A **Kloudlite Project** acts as a container for your Environments and Managed Services. It's the primary organizational unit within Kloudlite, encapsulating all the resources needed for your applications to run efficiently.

{% content-ref url="getting-started/setup-first-project.md" %}
[setup-first-project.md](getting-started/setup-first-project.md)
{% endcontent-ref %}

## Managed Service

**Managed Services** are stateful backing services crucial for application functionality. Kloudlite facilitates the deployment, management, and maintenance of these services, including:

* **MongoDB** (Cluster and Standalone)
* **MySQL** (Cluster and Standalone)
* **Redis** (Cluster and Standalone)

These managed services eliminate the need for manual setup and maintenance, ensuring your applications are supported by reliable backing services. We plan to broaden our range of managed services in future releases.

{% content-ref url="getting-started/create-managed-service.md" %}
[create-managed-service.md](getting-started/create-managed-service.md)
{% endcontent-ref %}

## Environment

An **Environment** within a Kloudlite Project encapsulates apps, configs, secrets, managed resources, and routers. Environments, being stateless, can be cloned and discarded with ease, offering flexibility and scalability for your application development lifecycle.

{% content-ref url="getting-started/create-environment.md" %}
[create-environment.md](getting-started/create-environment.md)
{% endcontent-ref %}

## Kloudlite Application

A **Kloudlite Application** is a Kubernetes resource designed for managing the deployment, service, autoscaling, and monitoring of your applications. It ensures your workloads are efficiently managed and scalable.

{% content-ref url="getting-started/create-app.md" %}
[create-app.md](getting-started/create-app.md)
{% endcontent-ref %}

## Router & Routes

**Router & Routes** handle the ingress for your workloads, managing how external traffic is directed to your applications. This system allows you to control access points and pathways for communication with your services.

{% content-ref url="getting-started/create-router-and-route.md" %}
[create-router-and-route.md](getting-started/create-router-and-route.md)
{% endcontent-ref %}

## Managed Resources

**Managed Resources** are stateless entities that define a relationship with a Managed Service. For instance, a Database in MySQL or a Topic in Kafka Managed Service. They represent the connection and utilization of managed services without maintaining the state within the environment.

{% content-ref url="getting-started/create-managed-resource.md" %}
[create-managed-resource.md](getting-started/create-managed-resource.md)
{% endcontent-ref %}



##
