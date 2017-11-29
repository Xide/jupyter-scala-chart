# Jupyter Scala notebook Helm chart

This project let you deploy the [jupyter scala](https://github.com/jupyter-scala/jupyter-scala) notebook using
[this](https://hub.docker.com/r/dockoey/jupyter-scala/) Docker image on Kubernetes using Helm chart.

## Configuration

You can tweak the `values.yaml` as needed, main variables are:

| variable                 | Usage                                                                                                                                                      |
| ------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| .Values.persistantVolume | You can enable or disable persistant storage for your notebook, change the claim size or storage class to use                                              |
| .Values.ingress          | If the notebook have to be avaliable outside the cluster, you can configure an host (that route to the cluster) to forward request to the notebook service |
| .Values.notebookPassword | The password asked by jupyter when logging on a notebook, empty by default                                                                                                                                                           |
