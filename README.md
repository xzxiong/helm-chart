# helm-charts

more details on https://helm.sh/zh/docs/howto/chart_releaser_action/


## Usage

[Helm](https://helm.sh) must be installed to use the charts.  Please refer to
Helm's [documentation](https://helm.sh/docs) to get started.

Once Helm has been set up correctly, add the repo as follows:

    helm repo add <alias> https://xzxiong.github.io/helm-charts

If you had already added this repo earlier, run `helm repo update` to retrieve
the latest versions of the packages.  You can then run `helm search repo
<alias>` to see the charts.

To install the <chart-name> chart:

    helm install my-<chart-name> <alias>/<chart-name>

To show the <chart-name> chart version:

    helm search repo my-<chart-name> <alias>/<chart-name> --versions --devel

To uninstall the chart:

    helm delete my-<chart-name>
