
# ai-ml-workshop-operator

This operator deploys machine learning workflows notebooks: https://github.com/willb/openshift-ml-workflows-workshop

**Requirements:**
- Openshift CLI

Run the following commands to deploy the operator and custom resource:

      oc create -f deploy/crds/charts.helm.k8s.io_aimlworkshopcharts_crd.yaml
      oc create -f deploy/service_account.yaml
      oc create -f deploy/role.yaml
      oc create -f deploy/role_binding.yaml
      oc create -f deploy/operator.yaml
      oc create -f deploy/crds/charts.helm.k8s.io_v1alpha1_aimlworkshopchart_cr.yaml

**To get route URL:**

    oc get route

Log in to Jupyter console with password "developer"

