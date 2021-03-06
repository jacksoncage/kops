## KubeAPIServerConfig v1alpha2 kops

Group        | Version     | Kind
------------ | ---------- | -----------
kops | v1alpha2 | KubeAPIServerConfig



KubeAPIServerConfig defines the configuration for the kube api

<aside class="notice">
Appears In:

<ul> 
<li><a href="#clusterspec-v1alpha2-kops">ClusterSpec kops/v1alpha2</a></li>
</ul></aside>

Field        | Description
------------ | -----------
address <br /> *string*    | Address is the binding address for the kube api
admissionControl <br /> *string array*    | AdmissionControl is a list of admission controllers to user
allowPrivileged <br /> *boolean*    | AllowPrivileged indicates if we can run privileged containers
anonymousAuth <br /> *boolean*    | AnonymousAuth indicates if anonymous authentication is permitted
apiServerCount <br /> *integer*    | APIServerCount is the number of api servers
auditLogMaxAge <br /> *integer*    | The maximum number of days to retain old audit log files based on the timestamp encoded in their filename.
auditLogMaxBackups <br /> *integer*    | The maximum number of old audit log files to retain.
auditLogMaxSize <br /> *integer*    | The maximum size in megabytes of the audit log file before it gets rotated. Defaults to 100MB.
auditLogPath <br /> *string*    | If set, all requests coming to the apiserver will be logged to this file.
authenticationTokenWebhookCacheTtl <br /> *[Duration](#duration-v1-meta)*    | The duration to cache responses from the webhook token authenticator. Default is 2m. (default 2m0s)
authenticationTokenWebhookConfigFile <br /> *string*    | File with webhook configuration for token authentication in kubeconfig format. The API server will query the remote service to determine authentication for bearer tokens.
authorizationMode <br /> *string*    | AuthorizationMode is the authorization mode the kubeapi is running in
authorizationRbacSuperUser <br /> *string*    | AuthorizationRBACSuperUser is the name of the superuser for default rbac
basicAuthFile <br /> *string*    | 
clientCAFile <br /> *string*    | 
cloudProvider <br /> *string*    | CloudProvider is the name of the cloudProvider we are using, aws, gce etcd
etcdCaFile <br /> *string*    | EtcdCAFile is the path to a ca certificate
etcdCertFile <br /> *string*    | EtcdCertFile is the path to a certificate
etcdKeyFile <br /> *string*    | EtcdKeyFile is the path to a orivate key
etcdServers <br /> *string array*    | EtcdServers is a list of the etcd service to connect
etcdServersOverrides <br /> *string array*    | EtcdServersOverrides is per-resource etcd servers overrides, comma separated. The individual override format: group/resource#servers, where servers are http://ip:port, semicolon separated
experimentalEncryptionProviderConfig <br /> *string*    | ExperimentalEncryptionProviderConfig enables encryption at rest for secrets.
image <br /> *string*    | Image is the docker container used
insecurePort <br /> *integer*    | InsecurePort is the port the insecure api runs
kubeletClientCertificate <br /> *string*    | KubeletClientCertificate is the path of a certificate for secure communication between api and kubelet
kubeletClientKey <br /> *string*    | KubeletClientKey is the path of a private to secure communication between api and kubelet
kubeletPreferredAddressTypes <br /> *string array*    | KubeletPreferredAddressTypes is a list of the preferred NodeAddressTypes to use for kubelet connections
logLevel <br /> *integer*    | LogLevel is the logging level of the api
oidcCAFile <br /> *string*    | If set, the OpenID server's certificate will be verified by one of the authorities in the oidc-ca-file
oidcClientID <br /> *string*    | The client ID for the OpenID Connect client, must be set if oidc-issuer-url is set.
oidcGroupsClaim <br /> *string*    | If provided, the name of a custom OpenID Connect claim for specifying user groups. The claim value is expected to be a string or array of strings.
oidcIssuerURL <br /> *string*    | The URL of the OpenID issuer, only HTTPS scheme will be accepted. If set, it will be used to verify the OIDC JSON Web Token (JWT).
oidcUsernameClaim <br /> *string*    | The OpenID claim to use as the user name. Note that claims other than the default ('sub') is not guaranteed to be unique and immutable.
proxyClientCertFile <br /> *string*    | The apiserver's client certificate used for outbound requests.
proxyClientKeyFile <br /> *string*    | The apiserver's client key used for outbound requests.
runtimeConfig <br /> *object*    | RuntimeConfig is a series of keys/values are parsed into the `--runtime-config` parameters
securePort <br /> *integer*    | SecurePort is the port the kube runs on
serviceClusterIPRange <br /> *string*    | ServiceClusterIPRange is the service address range
serviceNodePortRange <br /> *string*    | Passed as --service-node-port-range to kube-apiserver. Expects 'startPort-endPort' format. Eg. 30000-33000
storageBackend <br /> *string*    | StorageBackend is the backend storage
tlsCertFile <br /> *string*    | 
tlsPrivateKeyFile <br /> *string*    | 
tokenAuthFile <br /> *string*    | 

