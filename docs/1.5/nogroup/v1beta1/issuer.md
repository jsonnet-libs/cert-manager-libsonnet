---
permalink: /1.5/nogroup/v1beta1/issuer/
---

# nogroup.v1beta1.issuer

"An Issuer represents a certificate issuing authority which can be referenced as part of `issuerRef` fields. It is scoped to a single namespace and can therefore only be referenced by resources within the same namespace."

## Index

* [`fn new(name)`](#fn-new)
* [`obj metadata`](#obj-metadata)
  * [`fn withAnnotations(annotations)`](#fn-metadatawithannotations)
  * [`fn withAnnotationsMixin(annotations)`](#fn-metadatawithannotationsmixin)
  * [`fn withClusterName(clusterName)`](#fn-metadatawithclustername)
  * [`fn withCreationTimestamp(creationTimestamp)`](#fn-metadatawithcreationtimestamp)
  * [`fn withDeletionGracePeriodSeconds(deletionGracePeriodSeconds)`](#fn-metadatawithdeletiongraceperiodseconds)
  * [`fn withDeletionTimestamp(deletionTimestamp)`](#fn-metadatawithdeletiontimestamp)
  * [`fn withFinalizers(finalizers)`](#fn-metadatawithfinalizers)
  * [`fn withFinalizersMixin(finalizers)`](#fn-metadatawithfinalizersmixin)
  * [`fn withGenerateName(generateName)`](#fn-metadatawithgeneratename)
  * [`fn withGeneration(generation)`](#fn-metadatawithgeneration)
  * [`fn withLabels(labels)`](#fn-metadatawithlabels)
  * [`fn withLabelsMixin(labels)`](#fn-metadatawithlabelsmixin)
  * [`fn withManagedFields(managedFields)`](#fn-metadatawithmanagedfields)
  * [`fn withManagedFieldsMixin(managedFields)`](#fn-metadatawithmanagedfieldsmixin)
  * [`fn withName(name)`](#fn-metadatawithname)
  * [`fn withNamespace(namespace)`](#fn-metadatawithnamespace)
  * [`fn withOwnerReferences(ownerReferences)`](#fn-metadatawithownerreferences)
  * [`fn withOwnerReferencesMixin(ownerReferences)`](#fn-metadatawithownerreferencesmixin)
  * [`fn withResourceVersion(resourceVersion)`](#fn-metadatawithresourceversion)
  * [`fn withSelfLink(selfLink)`](#fn-metadatawithselflink)
  * [`fn withUid(uid)`](#fn-metadatawithuid)
* [`obj spec`](#obj-spec)
  * [`obj spec.acme`](#obj-specacme)
    * [`fn withDisableAccountKeyGeneration(disableAccountKeyGeneration)`](#fn-specacmewithdisableaccountkeygeneration)
    * [`fn withEmail(email)`](#fn-specacmewithemail)
    * [`fn withEnableDurationFeature(enableDurationFeature)`](#fn-specacmewithenabledurationfeature)
    * [`fn withPreferredChain(preferredChain)`](#fn-specacmewithpreferredchain)
    * [`fn withServer(server)`](#fn-specacmewithserver)
    * [`fn withSkipTLSVerify(skipTLSVerify)`](#fn-specacmewithskiptlsverify)
    * [`fn withSolvers(solvers)`](#fn-specacmewithsolvers)
    * [`fn withSolversMixin(solvers)`](#fn-specacmewithsolversmixin)
    * [`obj spec.acme.externalAccountBinding`](#obj-specacmeexternalaccountbinding)
      * [`fn withKeyAlgorithm(keyAlgorithm)`](#fn-specacmeexternalaccountbindingwithkeyalgorithm)
      * [`fn withKeyID(keyID)`](#fn-specacmeexternalaccountbindingwithkeyid)
      * [`obj spec.acme.externalAccountBinding.keySecretRef`](#obj-specacmeexternalaccountbindingkeysecretref)
        * [`fn withKey(key)`](#fn-specacmeexternalaccountbindingkeysecretrefwithkey)
        * [`fn withName(name)`](#fn-specacmeexternalaccountbindingkeysecretrefwithname)
    * [`obj spec.acme.privateKeySecretRef`](#obj-specacmeprivatekeysecretref)
      * [`fn withKey(key)`](#fn-specacmeprivatekeysecretrefwithkey)
      * [`fn withName(name)`](#fn-specacmeprivatekeysecretrefwithname)
  * [`obj spec.ca`](#obj-specca)
    * [`fn withCrlDistributionPoints(crlDistributionPoints)`](#fn-speccawithcrldistributionpoints)
    * [`fn withCrlDistributionPointsMixin(crlDistributionPoints)`](#fn-speccawithcrldistributionpointsmixin)
    * [`fn withOcspServers(ocspServers)`](#fn-speccawithocspservers)
    * [`fn withOcspServersMixin(ocspServers)`](#fn-speccawithocspserversmixin)
    * [`fn withSecretName(secretName)`](#fn-speccawithsecretname)
  * [`obj spec.selfSigned`](#obj-specselfsigned)
    * [`fn withCrlDistributionPoints(crlDistributionPoints)`](#fn-specselfsignedwithcrldistributionpoints)
    * [`fn withCrlDistributionPointsMixin(crlDistributionPoints)`](#fn-specselfsignedwithcrldistributionpointsmixin)
  * [`obj spec.vault`](#obj-specvault)
    * [`fn withCaBundle(caBundle)`](#fn-specvaultwithcabundle)
    * [`fn withNamespace(namespace)`](#fn-specvaultwithnamespace)
    * [`fn withPath(path)`](#fn-specvaultwithpath)
    * [`fn withServer(server)`](#fn-specvaultwithserver)
    * [`obj spec.vault.auth`](#obj-specvaultauth)
      * [`obj spec.vault.auth.appRole`](#obj-specvaultauthapprole)
        * [`fn withPath(path)`](#fn-specvaultauthapprolewithpath)
        * [`fn withRoleId(roleId)`](#fn-specvaultauthapprolewithroleid)
        * [`obj spec.vault.auth.appRole.secretRef`](#obj-specvaultauthapprolesecretref)
          * [`fn withKey(key)`](#fn-specvaultauthapprolesecretrefwithkey)
          * [`fn withName(name)`](#fn-specvaultauthapprolesecretrefwithname)
      * [`obj spec.vault.auth.kubernetes`](#obj-specvaultauthkubernetes)
        * [`fn withMountPath(mountPath)`](#fn-specvaultauthkuberneteswithmountpath)
        * [`fn withRole(role)`](#fn-specvaultauthkuberneteswithrole)
        * [`obj spec.vault.auth.kubernetes.secretRef`](#obj-specvaultauthkubernetessecretref)
          * [`fn withKey(key)`](#fn-specvaultauthkubernetessecretrefwithkey)
          * [`fn withName(name)`](#fn-specvaultauthkubernetessecretrefwithname)
      * [`obj spec.vault.auth.tokenSecretRef`](#obj-specvaultauthtokensecretref)
        * [`fn withKey(key)`](#fn-specvaultauthtokensecretrefwithkey)
        * [`fn withName(name)`](#fn-specvaultauthtokensecretrefwithname)
  * [`obj spec.venafi`](#obj-specvenafi)
    * [`fn withZone(zone)`](#fn-specvenafiwithzone)
    * [`obj spec.venafi.cloud`](#obj-specvenaficloud)
      * [`fn withUrl(url)`](#fn-specvenaficloudwithurl)
      * [`obj spec.venafi.cloud.apiTokenSecretRef`](#obj-specvenaficloudapitokensecretref)
        * [`fn withKey(key)`](#fn-specvenaficloudapitokensecretrefwithkey)
        * [`fn withName(name)`](#fn-specvenaficloudapitokensecretrefwithname)
    * [`obj spec.venafi.tpp`](#obj-specvenafitpp)
      * [`fn withCaBundle(caBundle)`](#fn-specvenafitppwithcabundle)
      * [`fn withUrl(url)`](#fn-specvenafitppwithurl)
      * [`obj spec.venafi.tpp.credentialsRef`](#obj-specvenafitppcredentialsref)
        * [`fn withName(name)`](#fn-specvenafitppcredentialsrefwithname)

## Fields

### fn new

```ts
new(name)
```

new returns an instance of Issuer

## obj metadata

"ObjectMeta is metadata that all persisted resources must have, which includes all objects users must create."

### fn metadata.withAnnotations

```ts
withAnnotations(annotations)
```

"Annotations is an unstructured key value map stored with a resource that may be set by external tools to store and retrieve arbitrary metadata. They are not queryable and should be preserved when modifying objects. More info: http://kubernetes.io/docs/user-guide/annotations"

### fn metadata.withAnnotationsMixin

```ts
withAnnotationsMixin(annotations)
```

"Annotations is an unstructured key value map stored with a resource that may be set by external tools to store and retrieve arbitrary metadata. They are not queryable and should be preserved when modifying objects. More info: http://kubernetes.io/docs/user-guide/annotations"

**Note:** This function appends passed data to existing values

### fn metadata.withClusterName

```ts
withClusterName(clusterName)
```

"The name of the cluster which the object belongs to. This is used to distinguish resources with same name and namespace in different clusters. This field is not set anywhere right now and apiserver is going to ignore it if set in create or update request."

### fn metadata.withCreationTimestamp

```ts
withCreationTimestamp(creationTimestamp)
```

"Time is a wrapper around time.Time which supports correct marshaling to YAML and JSON.  Wrappers are provided for many of the factory methods that the time package offers."

### fn metadata.withDeletionGracePeriodSeconds

```ts
withDeletionGracePeriodSeconds(deletionGracePeriodSeconds)
```

"Number of seconds allowed for this object to gracefully terminate before it will be removed from the system. Only set when deletionTimestamp is also set. May only be shortened. Read-only."

### fn metadata.withDeletionTimestamp

```ts
withDeletionTimestamp(deletionTimestamp)
```

"Time is a wrapper around time.Time which supports correct marshaling to YAML and JSON.  Wrappers are provided for many of the factory methods that the time package offers."

### fn metadata.withFinalizers

```ts
withFinalizers(finalizers)
```

"Must be empty before the object is deleted from the registry. Each entry is an identifier for the responsible component that will remove the entry from the list. If the deletionTimestamp of the object is non-nil, entries in this list can only be removed. Finalizers may be processed and removed in any order.  Order is NOT enforced because it introduces significant risk of stuck finalizers. finalizers is a shared field, any actor with permission can reorder it. If the finalizer list is processed in order, then this can lead to a situation in which the component responsible for the first finalizer in the list is waiting for a signal (field value, external system, or other) produced by a component responsible for a finalizer later in the list, resulting in a deadlock. Without enforced ordering finalizers are free to order amongst themselves and are not vulnerable to ordering changes in the list."

### fn metadata.withFinalizersMixin

```ts
withFinalizersMixin(finalizers)
```

"Must be empty before the object is deleted from the registry. Each entry is an identifier for the responsible component that will remove the entry from the list. If the deletionTimestamp of the object is non-nil, entries in this list can only be removed. Finalizers may be processed and removed in any order.  Order is NOT enforced because it introduces significant risk of stuck finalizers. finalizers is a shared field, any actor with permission can reorder it. If the finalizer list is processed in order, then this can lead to a situation in which the component responsible for the first finalizer in the list is waiting for a signal (field value, external system, or other) produced by a component responsible for a finalizer later in the list, resulting in a deadlock. Without enforced ordering finalizers are free to order amongst themselves and are not vulnerable to ordering changes in the list."

**Note:** This function appends passed data to existing values

### fn metadata.withGenerateName

```ts
withGenerateName(generateName)
```

"GenerateName is an optional prefix, used by the server, to generate a unique name ONLY IF the Name field has not been provided. If this field is used, the name returned to the client will be different than the name passed. This value will also be combined with a unique suffix. The provided value has the same validation rules as the Name field, and may be truncated by the length of the suffix required to make the value unique on the server.\n\nIf this field is specified and the generated name exists, the server will NOT return a 409 - instead, it will either return 201 Created or 500 with Reason ServerTimeout indicating a unique name could not be found in the time allotted, and the client should retry (optionally after the time indicated in the Retry-After header).\n\nApplied only if Name is not specified. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#idempotency"

### fn metadata.withGeneration

```ts
withGeneration(generation)
```

"A sequence number representing a specific generation of the desired state. Populated by the system. Read-only."

### fn metadata.withLabels

```ts
withLabels(labels)
```

"Map of string keys and values that can be used to organize and categorize (scope and select) objects. May match selectors of replication controllers and services. More info: http://kubernetes.io/docs/user-guide/labels"

### fn metadata.withLabelsMixin

```ts
withLabelsMixin(labels)
```

"Map of string keys and values that can be used to organize and categorize (scope and select) objects. May match selectors of replication controllers and services. More info: http://kubernetes.io/docs/user-guide/labels"

**Note:** This function appends passed data to existing values

### fn metadata.withManagedFields

```ts
withManagedFields(managedFields)
```

"ManagedFields maps workflow-id and version to the set of fields that are managed by that workflow. This is mostly for internal housekeeping, and users typically shouldn't need to set or understand this field. A workflow can be the user's name, a controller's name, or the name of a specific apply path like \"ci-cd\". The set of fields is always in the version that the workflow used when modifying the object."

### fn metadata.withManagedFieldsMixin

```ts
withManagedFieldsMixin(managedFields)
```

"ManagedFields maps workflow-id and version to the set of fields that are managed by that workflow. This is mostly for internal housekeeping, and users typically shouldn't need to set or understand this field. A workflow can be the user's name, a controller's name, or the name of a specific apply path like \"ci-cd\". The set of fields is always in the version that the workflow used when modifying the object."

**Note:** This function appends passed data to existing values

### fn metadata.withName

```ts
withName(name)
```

"Name must be unique within a namespace. Is required when creating resources, although some resources may allow a client to request the generation of an appropriate name automatically. Name is primarily intended for creation idempotence and configuration definition. Cannot be updated. More info: http://kubernetes.io/docs/user-guide/identifiers#names"

### fn metadata.withNamespace

```ts
withNamespace(namespace)
```

"Namespace defines the space within which each name must be unique. An empty namespace is equivalent to the \"default\" namespace, but \"default\" is the canonical representation. Not all objects are required to be scoped to a namespace - the value of this field for those objects will be empty.\n\nMust be a DNS_LABEL. Cannot be updated. More info: http://kubernetes.io/docs/user-guide/namespaces"

### fn metadata.withOwnerReferences

```ts
withOwnerReferences(ownerReferences)
```

"List of objects depended by this object. If ALL objects in the list have been deleted, this object will be garbage collected. If this object is managed by a controller, then an entry in this list will point to this controller, with the controller field set to true. There cannot be more than one managing controller."

### fn metadata.withOwnerReferencesMixin

```ts
withOwnerReferencesMixin(ownerReferences)
```

"List of objects depended by this object. If ALL objects in the list have been deleted, this object will be garbage collected. If this object is managed by a controller, then an entry in this list will point to this controller, with the controller field set to true. There cannot be more than one managing controller."

**Note:** This function appends passed data to existing values

### fn metadata.withResourceVersion

```ts
withResourceVersion(resourceVersion)
```

"An opaque value that represents the internal version of this object that can be used by clients to determine when objects have changed. May be used for optimistic concurrency, change detection, and the watch operation on a resource or set of resources. Clients must treat these values as opaque and passed unmodified back to the server. They may only be valid for a particular resource or set of resources.\n\nPopulated by the system. Read-only. Value must be treated as opaque by clients and . More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#concurrency-control-and-consistency"

### fn metadata.withSelfLink

```ts
withSelfLink(selfLink)
```

"SelfLink is a URL representing this object. Populated by the system. Read-only.\n\nDEPRECATED Kubernetes will stop propagating this field in 1.20 release and the field is planned to be removed in 1.21 release."

### fn metadata.withUid

```ts
withUid(uid)
```

"UID is the unique in time and space value for this object. It is typically generated by the server on successful creation of a resource and is not allowed to change on PUT operations.\n\nPopulated by the system. Read-only. More info: http://kubernetes.io/docs/user-guide/identifiers#uids"

## obj spec

"Desired state of the Issuer resource."

## obj spec.acme

"ACME configures this issuer to communicate with a RFC8555 (ACME) server to obtain signed x509 certificates."

### fn spec.acme.withDisableAccountKeyGeneration

```ts
withDisableAccountKeyGeneration(disableAccountKeyGeneration)
```

"Enables or disables generating a new ACME account key. If true, the Issuer resource will *not* request a new account but will expect the account key to be supplied via an existing secret. If false, the cert-manager system will generate a new ACME account key for the Issuer. Defaults to false."

### fn spec.acme.withEmail

```ts
withEmail(email)
```

"Email is the email address to be associated with the ACME account. This field is optional, but it is strongly recommended to be set. It will be used to contact you in case of issues with your account or certificates, including expiry notification emails. This field may be updated after the account is initially registered."

### fn spec.acme.withEnableDurationFeature

```ts
withEnableDurationFeature(enableDurationFeature)
```

"Enables requesting a Not After date on certificates that matches the duration of the certificate. This is not supported by all ACME servers like Let's Encrypt. If set to true when the ACME server does not support it it will create an error on the Order. Defaults to false."

### fn spec.acme.withPreferredChain

```ts
withPreferredChain(preferredChain)
```

"PreferredChain is the chain to use if the ACME server outputs multiple. PreferredChain is no guarantee that this one gets delivered by the ACME endpoint. For example, for Let's Encrypt's DST crosssign you would use: \"DST Root CA X3\" or \"ISRG Root X1\" for the newer Let's Encrypt root CA. This value picks the first certificate bundle in the ACME alternative chains that has a certificate with this value as its issuer's CN"

### fn spec.acme.withServer

```ts
withServer(server)
```

"Server is the URL used to access the ACME server's 'directory' endpoint. For example, for Let's Encrypt's staging endpoint, you would use: \"https://acme-staging-v02.api.letsencrypt.org/directory\". Only ACME v2 endpoints (i.e. RFC 8555) are supported."

### fn spec.acme.withSkipTLSVerify

```ts
withSkipTLSVerify(skipTLSVerify)
```

"Enables or disables validation of the ACME server TLS certificate. If true, requests to the ACME server will not have their TLS certificate validated (i.e. insecure connections will be allowed). Only enable this option in development environments. The cert-manager system installed roots will be used to verify connections to the ACME server if this is false. Defaults to false."

### fn spec.acme.withSolvers

```ts
withSolvers(solvers)
```

"Solvers is a list of challenge solvers that will be used to solve ACME challenges for the matching domains. Solver configurations must be provided in order to obtain certificates from an ACME server. For more information, see: https://cert-manager.io/docs/configuration/acme/"

### fn spec.acme.withSolversMixin

```ts
withSolversMixin(solvers)
```

"Solvers is a list of challenge solvers that will be used to solve ACME challenges for the matching domains. Solver configurations must be provided in order to obtain certificates from an ACME server. For more information, see: https://cert-manager.io/docs/configuration/acme/"

**Note:** This function appends passed data to existing values

## obj spec.acme.externalAccountBinding

"ExternalAccountBinding is a reference to a CA external account of the ACME server. If set, upon registration cert-manager will attempt to associate the given external account credentials with the registered ACME account."

### fn spec.acme.externalAccountBinding.withKeyAlgorithm

```ts
withKeyAlgorithm(keyAlgorithm)
```

"Deprecated: keyAlgorithm field exists for historical compatibility reasons and should not be used. The algorithm is now hardcoded to HS256 in golang/x/crypto/acme."

### fn spec.acme.externalAccountBinding.withKeyID

```ts
withKeyID(keyID)
```

"keyID is the ID of the CA key that the External Account is bound to."

## obj spec.acme.externalAccountBinding.keySecretRef

"keySecretRef is a Secret Key Selector referencing a data item in a Kubernetes Secret which holds the symmetric MAC key of the External Account Binding. The `key` is the index string that is paired with the key data in the Secret and should not be confused with the key data itself, or indeed with the External Account Binding keyID above. The secret key stored in the Secret **must** be un-padded, base64 URL encoded data."

### fn spec.acme.externalAccountBinding.keySecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used. Some instances of this field may be defaulted, in others it may be required."

### fn spec.acme.externalAccountBinding.keySecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.acme.privateKeySecretRef

"PrivateKey is the name of a Kubernetes Secret resource that will be used to store the automatically generated ACME account private key. Optionally, a `key` may be specified to select a specific entry within the named Secret resource. If `key` is not specified, a default of `tls.key` will be used."

### fn spec.acme.privateKeySecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used. Some instances of this field may be defaulted, in others it may be required."

### fn spec.acme.privateKeySecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.ca

"CA configures this issuer to sign certificates using a signing CA keypair stored in a Secret resource. This is used to build internal PKIs that are managed by cert-manager."

### fn spec.ca.withCrlDistributionPoints

```ts
withCrlDistributionPoints(crlDistributionPoints)
```

"The CRL distribution points is an X.509 v3 certificate extension which identifies the location of the CRL from which the revocation of this certificate can be checked. If not set, certificates will be issued without distribution points set."

### fn spec.ca.withCrlDistributionPointsMixin

```ts
withCrlDistributionPointsMixin(crlDistributionPoints)
```

"The CRL distribution points is an X.509 v3 certificate extension which identifies the location of the CRL from which the revocation of this certificate can be checked. If not set, certificates will be issued without distribution points set."

**Note:** This function appends passed data to existing values

### fn spec.ca.withOcspServers

```ts
withOcspServers(ocspServers)
```

"The OCSP server list is an X.509 v3 extension that defines a list of URLs of OCSP responders. The OCSP responders can be queried for the revocation status of an issued certificate. If not set, the certificate will be issued with no OCSP servers set. For example, an OCSP server URL could be \"http://ocsp.int-x3.letsencrypt.org\"."

### fn spec.ca.withOcspServersMixin

```ts
withOcspServersMixin(ocspServers)
```

"The OCSP server list is an X.509 v3 extension that defines a list of URLs of OCSP responders. The OCSP responders can be queried for the revocation status of an issued certificate. If not set, the certificate will be issued with no OCSP servers set. For example, an OCSP server URL could be \"http://ocsp.int-x3.letsencrypt.org\"."

**Note:** This function appends passed data to existing values

### fn spec.ca.withSecretName

```ts
withSecretName(secretName)
```

"SecretName is the name of the secret used to sign Certificates issued by this Issuer."

## obj spec.selfSigned

"SelfSigned configures this issuer to 'self sign' certificates using the private key used to create the CertificateRequest object."

### fn spec.selfSigned.withCrlDistributionPoints

```ts
withCrlDistributionPoints(crlDistributionPoints)
```

"The CRL distribution points is an X.509 v3 certificate extension which identifies the location of the CRL from which the revocation of this certificate can be checked. If not set certificate will be issued without CDP. Values are strings."

### fn spec.selfSigned.withCrlDistributionPointsMixin

```ts
withCrlDistributionPointsMixin(crlDistributionPoints)
```

"The CRL distribution points is an X.509 v3 certificate extension which identifies the location of the CRL from which the revocation of this certificate can be checked. If not set certificate will be issued without CDP. Values are strings."

**Note:** This function appends passed data to existing values

## obj spec.vault

"Vault configures this issuer to sign certificates using a HashiCorp Vault PKI backend."

### fn spec.vault.withCaBundle

```ts
withCaBundle(caBundle)
```

"PEM-encoded CA bundle (base64-encoded) used to validate Vault server certificate. Only used if the Server URL is using HTTPS protocol. This parameter is ignored for plain HTTP protocol connection. If not set the system root certificates are used to validate the TLS connection."

### fn spec.vault.withNamespace

```ts
withNamespace(namespace)
```

"Name of the vault namespace. Namespaces is a set of features within Vault Enterprise that allows Vault environments to support Secure Multi-tenancy. e.g: \"ns1\" More about namespaces can be found here https://www.vaultproject.io/docs/enterprise/namespaces"

### fn spec.vault.withPath

```ts
withPath(path)
```

"Path is the mount path of the Vault PKI backend's `sign` endpoint, e.g: \"my_pki_mount/sign/my-role-name\"."

### fn spec.vault.withServer

```ts
withServer(server)
```

"Server is the connection address for the Vault server, e.g: \"https://vault.example.com:8200\"."

## obj spec.vault.auth

"Auth configures how cert-manager authenticates with the Vault server."

## obj spec.vault.auth.appRole

"AppRole authenticates with Vault using the App Role auth mechanism, with the role and secret stored in a Kubernetes Secret resource."

### fn spec.vault.auth.appRole.withPath

```ts
withPath(path)
```

"Path where the App Role authentication backend is mounted in Vault, e.g: \"approle\

### fn spec.vault.auth.appRole.withRoleId

```ts
withRoleId(roleId)
```

"RoleID configured in the App Role authentication backend when setting up the authentication backend in Vault."

## obj spec.vault.auth.appRole.secretRef

"Reference to a key in a Secret that contains the App Role secret used to authenticate with Vault. The `key` field must be specified and denotes which entry within the Secret resource is used as the app role secret."

### fn spec.vault.auth.appRole.secretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used. Some instances of this field may be defaulted, in others it may be required."

### fn spec.vault.auth.appRole.secretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.vault.auth.kubernetes

"Kubernetes authenticates with Vault by passing the ServiceAccount token stored in the named Secret resource to the Vault server."

### fn spec.vault.auth.kubernetes.withMountPath

```ts
withMountPath(mountPath)
```

"The Vault mountPath here is the mount path to use when authenticating with Vault. For example, setting a value to `/v1/auth/foo`, will use the path `/v1/auth/foo/login` to authenticate with Vault. If unspecified, the default value \"/v1/auth/kubernetes\" will be used."

### fn spec.vault.auth.kubernetes.withRole

```ts
withRole(role)
```

"A required field containing the Vault Role to assume. A Role binds a Kubernetes ServiceAccount with a set of Vault policies."

## obj spec.vault.auth.kubernetes.secretRef

"The required Secret field containing a Kubernetes ServiceAccount JWT used for authenticating with Vault. Use of 'ambient credentials' is not supported."

### fn spec.vault.auth.kubernetes.secretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used. Some instances of this field may be defaulted, in others it may be required."

### fn spec.vault.auth.kubernetes.secretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.vault.auth.tokenSecretRef

"TokenSecretRef authenticates with Vault by presenting a token."

### fn spec.vault.auth.tokenSecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used. Some instances of this field may be defaulted, in others it may be required."

### fn spec.vault.auth.tokenSecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.venafi

"Venafi configures this issuer to sign certificates using a Venafi TPP or Venafi Cloud policy zone."

### fn spec.venafi.withZone

```ts
withZone(zone)
```

"Zone is the Venafi Policy Zone to use for this issuer. All requests made to the Venafi platform will be restricted by the named zone policy. This field is required."

## obj spec.venafi.cloud

"Cloud specifies the Venafi cloud configuration settings. Only one of TPP or Cloud may be specified."

### fn spec.venafi.cloud.withUrl

```ts
withUrl(url)
```

"URL is the base URL for Venafi Cloud. Defaults to \"https://api.venafi.cloud/v1\"."

## obj spec.venafi.cloud.apiTokenSecretRef

"APITokenSecretRef is a secret key selector for the Venafi Cloud API token."

### fn spec.venafi.cloud.apiTokenSecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used. Some instances of this field may be defaulted, in others it may be required."

### fn spec.venafi.cloud.apiTokenSecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.venafi.tpp

"TPP specifies Trust Protection Platform configuration settings. Only one of TPP or Cloud may be specified."

### fn spec.venafi.tpp.withCaBundle

```ts
withCaBundle(caBundle)
```

"CABundle is a PEM encoded TLS certificate to use to verify connections to the TPP instance. If specified, system roots will not be used and the issuing CA for the TPP instance must be verifiable using the provided root. If not specified, the connection will be verified using the cert-manager system root certificates."

### fn spec.venafi.tpp.withUrl

```ts
withUrl(url)
```

"URL is the base URL for the vedsdk endpoint of the Venafi TPP instance, for example: \"https://tpp.example.com/vedsdk\"."

## obj spec.venafi.tpp.credentialsRef

"CredentialsRef is a reference to a Secret containing the username and password for the TPP server. The secret must contain two keys, 'username' and 'password'."

### fn spec.venafi.tpp.credentialsRef.withName

```ts
withName(name)
```

"Name of the resource being referred to. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"