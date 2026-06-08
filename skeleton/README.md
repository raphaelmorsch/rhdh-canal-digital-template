# ${{ values.componentId }} GitOps onboarding

Este repositório foi criado por um Golden Template do Red Hat Developer Hub.

Ele não substitui o repositório de código fonte. Ele adiciona a camada de plataforma:

- Registro no Software Catalog
- Manifests OpenShift / Serverless
- Pipeline Tekton de build
- Estrutura GitOps para Argo CD

## Código fonte

`${{ values.sourceRepoUrl }}`

Branch: `${{ values.sourceBranch }}`

## Aplicar no OpenShift

```bash
oc apply -k gitops/overlays/dev
oc apply -f pipelines/build-pipeline.yaml
```
