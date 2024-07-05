## Description

Here, In this template, we will deploy the application with the enabling of the tls for the https traffic using the manifest files in Kubernetes

---

#### Pre-requisite

* AZ Account
* Azure CLI

---

### Steps:-
1. Login into AZ account using `az login` or `az login --tenant <TENANT-ID>`
2. Login into the Azure using the Service Principal the Service Principal like `az service principal -u <client-id> -p <client-password> -t <tenant-ID>`.
3. Configure the tls secret by using these steps:

     a. Identities & Permissions: Assign necessary permissions to identities.

     b. Generate Certificates: Create public and private certificates.

     c. Connect AKS with Key Vault: Install Secrets Store CSI driver.

     d. Application Deployment: Deploy .NET app with Nginx sidecar.

     e. AGIC Installation: Enable AGIC and link to Application Gateway.

    f. Ingress Deployment: Upload certificates to Application Gateway and configure ingress.

4. Run the manifests files for your particular AKS and Application Gateway to enable the TLS end to end.

---
