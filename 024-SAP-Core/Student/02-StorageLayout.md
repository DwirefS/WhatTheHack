# Challenge 2: Storage Design - build storage layout for the SAP Deployment

[< Previous Challenge](./01-containers.md) - **[Home](../README.md)** - [Next Challenge >](./03-k8sintro.md)

## Introduction

In previous challenge we picked Azure VM sku's for running SAP HANA, the CPU and Memory requirments have been allocated, but where do the binaries reside and what about persistence area for data, logs and what about database backups? 

## Description

In this challenge we will be creating and setting up a new, private, Azure Container Registry. This will be the new home of the containers we just created. We will see later on how Kubernetes will pull our images from this registry.

- Deploy an Azure Container Registry (ACR)
- Ensure your ACR has proper permissions and credentials set up
- Login to your ACR
- Push your Docker container images to the ACR
- List all images in your ACR

## Success Criteria

1. You have designed the filesystem layout.
2. You have identified the storage containers and data disk sku's.



RK - notes

• Design storage layout for HANA scale-up system

Hint: Follow SAP TDI guidelines


Different Storage types for HANA on Azure: 

		○ Azure premium SSD or premium storage
		○ Ultra disk
		○ Azure NetApp Files
		○ Filesystem types

