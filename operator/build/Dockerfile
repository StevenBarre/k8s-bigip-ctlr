FROM quay.io/operator-framework/helm-operator:latest

### Required OpenShift Labels
LABEL name="F5 BIG-IP Controller Operator" \
      vendor="F5 Networks Inc" \
      version="v1.8.0" \
      release="1" \
      summary="F5 BIG-IP Controller Operator" \
      description="This operator will deploy F5 BIG-IP Controller for Kubernetes and OpenShift into the cluster."

# Required Licenses
COPY operator/licenses /licenses

COPY operator/watches.yaml ${HOME}/watches.yaml
COPY ./helm-charts/f5-bigip-ctlr ${HOME}/helm-charts/f5-bigip-ctlr
