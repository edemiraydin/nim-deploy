# NIM on Azure Kubernetes Service (AKS)


To deploy NIM on AKS successfully, ensure you have the right GPU and driver version. The default GPU driver in Azure Kubernetes Services (AKS) is usually outdated for the latest NVIDIA software, and Microsoft does not yet have an official solution for this issue.

To resolve this, use the preview version of the CLI to create the AKS cluster. The Prerequisites section explains how to set up your local environment to enable AKS creation with the preview CLI.

After you are ready to create AKS, the next thing is to choose the right GPU instance.  Only L40S, A100, H100 GPU work for NIM but not all system configurations.  Create AKS section has more details about this.

## Prerequisites

Please follow [Pre-requirement instructions](./prerequisites/README.md) to get ready for AKS creation.

## Create AKS

Please follow [Create AKS instructions](./setup/README.md) to create AKS.

## Deploy NIM 
### Using Helm Chart

Please follow [Deploy NIM instructions](../../../helm/README.md) to deploy NIM.

### Using NIM Operator

Please follow [Deploy NIM Operator instructions](nim-operator-setup.md) to deploy NIM Operator.
