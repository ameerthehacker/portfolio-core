![demo](~architecture.png)

## What is it <i class="far fa-question-circle"></i> 

I was given the responsibility to morderize a legacy **.NET app** running in Azure App Servies by migrating it to **.NET Core** and **Containers** within just 2 weeks. I went above and beyond to meet the deadline and rewamped its entire architecture to microservices based by embracing the usage of .NET Core, Docker and Kubernetes during the process. I took up an additional task to build a robust and higly reliable CI/CD pipeline using **Azure DevOps** which would really empowered faster deliverables in the future. By following some best practices I was able to reduce the total resource utilization cost by 10%. I designed the entire migration plan which made the platform migration very seamless with 0 downtime without the clients even noticing.
I was highly appreciated for meeting the deadline while maintaining high quality deliverables.

## Services <i class="fas fa-cogs"></i>

### UI

The UI is built with **Angular 7**, it is served from the near by **Azure CDN** node to the user.

### Mobile App

The Mobile App is built with Xamarin and it can be used to submit certain reports

### Email Sender

It is a .NET Core service which is responsible for sending mails for queued messages in **Azure Service Bus**

### Web API

It is a ASP.NET Core based Web REST API application. The Web API communicates with the **Email Sender** service through the Azure Service Bus if it wants to send any emails

### Finance Notifications

It is a .NET Core cron job service which is responsible for sending monthly emails by communicating with the **Email Sender** service through the Azure Service Bus

## Tech Stack <i class="fas fa-layer-group"></i>

<i class="fab fas fa-dharmachakra kube"></i> Kubernetes

<i class="fab fa-docker docker"></i> Docker

<i class="fab fa-angular angular"></i> Angular

<i class="fas fa-server"></i> .NET Core

<i class="fas fa-server"></i> ASP.NET Core

## Live Demo <i class="fas fa-laptop-code"></i>

You can access the production site from <a target="_blank" rel="noopener noreferrer" href="https://portal.mychoicesfoundation.in/">here</a>