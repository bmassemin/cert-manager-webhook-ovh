![OVH Webhook for Cert Manager](https://raw.githubusercontent.com/aureq/cert-manager-webhook-ovh/main/assets/images/cert-manager-webhook-ovh.svg "OVH Webhook for Cert Manager")

## Usage

[Helm](https://helm.sh) must be installed to use the charts.  Please refer to Helm's [documentation](https://helm.sh/docs) to get started.

Once Helm has been set up correctly, add the repo as follows:

    helm repo add cert-manager-webhook-ovh-charts https://aureq.github.io/cert-manager-webhook-ovh/

If you've' already added this repo earlier, run the command below to retrieve the latest versions of the packages.

    helm repo update

To search for all available charts in this repository, run the following command

    helm search repo cert-manager-webhook-ovh-charts

To install the cert-manager-webhook-ovh chart:

    helm upgrade --install --namespace cert-manager cm-webhook-ovh cert-manager-webhook-ovh-charts/cert-manager-webhook-ovh

To uninstall the chart:

    helm uninstall --namespace cert-manager cm-webhook-ovh