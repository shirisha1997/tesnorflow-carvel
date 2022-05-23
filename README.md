# TensorFlow ResNet

TensorFlow ResNet is a client utility for use with TensorFlow Serving and ResNet models.

## TensorFlow parameters

|Parameter|Description|Type|Default|
|---------|-----------|----|-------|
|server.image.pullPolicy|TensorFlow Serving image pull policy|string|IfNotPresent|
|containerPorts.server|Tensorflow server port|integer|8500|
|containerPorts.restApi|TensorFlow Serving Rest API Port|integer|8501|
|replicaCount|Number of replicas|integer|1|
|podSecurityContext.enabled|Enabled pod Security Context|string|TRUE|
|podSecurityContext.fsGroup|Set pod Security Context fsGroup|integer|1001|
|containerSecurityContext.enabled|Enabled container Security Context|string|TRUE|
|containerSecurityContext.runAsUser|Set container Security Context runAsUser|integer|1001|
|containerSecurityContext.runAsNonRoot|Set container Security Context runAsNonRoot|string|TRUE|
|startupProbe.enabled|Enable startupProbe|string|FALSE|
|startupProbe.initialDelaySeconds|Initial delay seconds for startupProbe|integer|30|
|startupProbe.periodSeconds|Period seconds for startupProbe|integer|5|
|startupProbe.timeoutSeconds|Timeout seconds for startupProbe|integer|5|
|startupProbe.failureThreshold|Failure threshold for startupProbe|integer|6|
|startupProbe.successThreshold|Success threshold for startupProbe|integer|1|
|livenessProbe.initialDelaySeconds|Initial delay seconds for livenessProbe|integer|30|
|livenessProbe.periodSeconds|Period seconds for livenessProbe|integer|5|
|livenessProbe.timeoutSeconds|Timeout seconds for livenessProbe|integer|5|
|livenessProbe.failureThreshold|Failure threshold for livenessProbe|integer|6|
|livenessProbe.successThreshold|Success threshold for livenessProbe|integer|1|
|readinessProbe.initialDelaySeconds|Initial delay seconds for readinessProbe|integer|15|
|readinessProbe.periodSeconds|Period seconds for readinessProbe|integer|5|
|readinessProbe.timeoutSeconds|Timeout seconds for readinessProbe|integer|5|
|readinessProbe.failureThreshold|Failure threshold for readinessProbe|integer|6|
|readinessProbe.successThreshold|Success threshold for readinessProbe|integer|1|
|service.type|Kubernetes Service type|string|LoadBalancer|
|service.ports.server|TensorFlow Serving server port|integer|8500|
|service.ports.restApi|TensorFlow Serving Rest API port|integer|8501|
