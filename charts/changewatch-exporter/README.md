ChangeWatch Exporter Helm Chart
===============================

This is a Official Helm chart of [ChangeWatch Exporter](https://github.com/homagames/changewatch-exporter/). 


# Parameters

Parameter | Description | Default
--- | --- | ---
`image.repository` | Container repository | `ghcr.io/homagames/changewatch-exporter`
`image.pullPolicy` | Kubernetes pull policy of the image | `IfNotPresent`
`image.tag` | Kubernetes pull policy of the image | `.Chart.AppVersion`
`replicaCount` | Number of replicas of the deployment | `1`
`imagePullSecrets` |  | `[]`
`nameOverride` | | `""`
`podAnnotations` | Annotation to attach on the pod. Used to scrape prometheus metrics. | `<see values.yaml>`
`podSecurityContext.runAsNonRoot` | Set [Security Context](https://kubernetes.io/docs/tasks/configure-pod-container/security-context/) runAsNonRoot | `true`
`podSecurityContext.runAsUser` | Set [Security Context](https://kubernetes.io/docs/tasks/configure-pod-container/security-context/) runAsUser | `10001`
`securityContext.allowPrivilegeEscalation` | Set [Security Context](https://kubernetes.io/docs/tasks/configure-pod-container/security-context/) allowPrivilegeEscalation | `false`
`securityContext.capabilities.drop` | Set [Security Context](https://kubernetes.io/docs/tasks/configure-pod-container/security-context/) capabilities | `[ALL]`
`resources` | Set pod's resources | `{}`
`nodeSelector` | Set node selector | `{}`
`tolerations` | Set node toleration | `[]`
`affinity` | Set affinity | `{}`
`config` | Set affinity | `<see values.yaml>`

