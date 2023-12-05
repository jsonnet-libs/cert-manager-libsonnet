---
permalink: /1.13/nogroup/v1/certificate/
---

# nogroup.v1.certificate

"A Certificate resource should be created to ensure an up to date and signed X.509 certificate is stored in the Kubernetes Secret resource named in `spec.secretName`. \n The stored certificate will be renewed before it expires (as configured by `spec.renewBefore`)."

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
  * [`fn withName(name)`](#fn-metadatawithname)
  * [`fn withNamespace(namespace)`](#fn-metadatawithnamespace)
  * [`fn withOwnerReferences(ownerReferences)`](#fn-metadatawithownerreferences)
  * [`fn withOwnerReferencesMixin(ownerReferences)`](#fn-metadatawithownerreferencesmixin)
  * [`fn withResourceVersion(resourceVersion)`](#fn-metadatawithresourceversion)
  * [`fn withSelfLink(selfLink)`](#fn-metadatawithselflink)
  * [`fn withUid(uid)`](#fn-metadatawithuid)
* [`obj spec`](#obj-spec)
  * [`fn withAdditionalOutputFormats(additionalOutputFormats)`](#fn-specwithadditionaloutputformats)
  * [`fn withAdditionalOutputFormatsMixin(additionalOutputFormats)`](#fn-specwithadditionaloutputformatsmixin)
  * [`fn withCommonName(commonName)`](#fn-specwithcommonname)
  * [`fn withDnsNames(dnsNames)`](#fn-specwithdnsnames)
  * [`fn withDnsNamesMixin(dnsNames)`](#fn-specwithdnsnamesmixin)
  * [`fn withDuration(duration)`](#fn-specwithduration)
  * [`fn withEmailAddresses(emailAddresses)`](#fn-specwithemailaddresses)
  * [`fn withEmailAddressesMixin(emailAddresses)`](#fn-specwithemailaddressesmixin)
  * [`fn withEncodeUsagesInRequest(encodeUsagesInRequest)`](#fn-specwithencodeusagesinrequest)
  * [`fn withIpAddresses(ipAddresses)`](#fn-specwithipaddresses)
  * [`fn withIpAddressesMixin(ipAddresses)`](#fn-specwithipaddressesmixin)
  * [`fn withIsCA(isCA)`](#fn-specwithisca)
  * [`fn withLiteralSubject(literalSubject)`](#fn-specwithliteralsubject)
  * [`fn withRenewBefore(renewBefore)`](#fn-specwithrenewbefore)
  * [`fn withRevisionHistoryLimit(revisionHistoryLimit)`](#fn-specwithrevisionhistorylimit)
  * [`fn withSecretName(secretName)`](#fn-specwithsecretname)
  * [`fn withUris(uris)`](#fn-specwithuris)
  * [`fn withUrisMixin(uris)`](#fn-specwithurismixin)
  * [`fn withUsages(usages)`](#fn-specwithusages)
  * [`fn withUsagesMixin(usages)`](#fn-specwithusagesmixin)
  * [`obj spec.additionalOutputFormats`](#obj-specadditionaloutputformats)
    * [`fn withType(type)`](#fn-specadditionaloutputformatswithtype)
  * [`obj spec.issuerRef`](#obj-specissuerref)
    * [`fn withGroup(group)`](#fn-specissuerrefwithgroup)
    * [`fn withKind(kind)`](#fn-specissuerrefwithkind)
    * [`fn withName(name)`](#fn-specissuerrefwithname)
  * [`obj spec.keystores`](#obj-speckeystores)
    * [`obj spec.keystores.jks`](#obj-speckeystoresjks)
      * [`fn withCreate(create)`](#fn-speckeystoresjkswithcreate)
      * [`obj spec.keystores.jks.passwordSecretRef`](#obj-speckeystoresjkspasswordsecretref)
        * [`fn withKey(key)`](#fn-speckeystoresjkspasswordsecretrefwithkey)
        * [`fn withName(name)`](#fn-speckeystoresjkspasswordsecretrefwithname)
    * [`obj spec.keystores.pkcs12`](#obj-speckeystorespkcs12)
      * [`fn withCreate(create)`](#fn-speckeystorespkcs12withcreate)
      * [`obj spec.keystores.pkcs12.passwordSecretRef`](#obj-speckeystorespkcs12passwordsecretref)
        * [`fn withKey(key)`](#fn-speckeystorespkcs12passwordsecretrefwithkey)
        * [`fn withName(name)`](#fn-speckeystorespkcs12passwordsecretrefwithname)
  * [`obj spec.privateKey`](#obj-specprivatekey)
    * [`fn withAlgorithm(algorithm)`](#fn-specprivatekeywithalgorithm)
    * [`fn withEncoding(encoding)`](#fn-specprivatekeywithencoding)
    * [`fn withRotationPolicy(rotationPolicy)`](#fn-specprivatekeywithrotationpolicy)
    * [`fn withSize(size)`](#fn-specprivatekeywithsize)
  * [`obj spec.secretTemplate`](#obj-specsecrettemplate)
    * [`fn withAnnotations(annotations)`](#fn-specsecrettemplatewithannotations)
    * [`fn withAnnotationsMixin(annotations)`](#fn-specsecrettemplatewithannotationsmixin)
    * [`fn withLabels(labels)`](#fn-specsecrettemplatewithlabels)
    * [`fn withLabelsMixin(labels)`](#fn-specsecrettemplatewithlabelsmixin)
  * [`obj spec.subject`](#obj-specsubject)
    * [`fn withCountries(countries)`](#fn-specsubjectwithcountries)
    * [`fn withCountriesMixin(countries)`](#fn-specsubjectwithcountriesmixin)
    * [`fn withLocalities(localities)`](#fn-specsubjectwithlocalities)
    * [`fn withLocalitiesMixin(localities)`](#fn-specsubjectwithlocalitiesmixin)
    * [`fn withOrganizationalUnits(organizationalUnits)`](#fn-specsubjectwithorganizationalunits)
    * [`fn withOrganizationalUnitsMixin(organizationalUnits)`](#fn-specsubjectwithorganizationalunitsmixin)
    * [`fn withOrganizations(organizations)`](#fn-specsubjectwithorganizations)
    * [`fn withOrganizationsMixin(organizations)`](#fn-specsubjectwithorganizationsmixin)
    * [`fn withPostalCodes(postalCodes)`](#fn-specsubjectwithpostalcodes)
    * [`fn withPostalCodesMixin(postalCodes)`](#fn-specsubjectwithpostalcodesmixin)
    * [`fn withProvinces(provinces)`](#fn-specsubjectwithprovinces)
    * [`fn withProvincesMixin(provinces)`](#fn-specsubjectwithprovincesmixin)
    * [`fn withSerialNumber(serialNumber)`](#fn-specsubjectwithserialnumber)
    * [`fn withStreetAddresses(streetAddresses)`](#fn-specsubjectwithstreetaddresses)
    * [`fn withStreetAddressesMixin(streetAddresses)`](#fn-specsubjectwithstreetaddressesmixin)

## Fields

### fn new

```ts
new(name)
```

new returns an instance of Certificate

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

"Specification of the desired state of the Certificate resource. https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#spec-and-status"

### fn spec.withAdditionalOutputFormats

```ts
withAdditionalOutputFormats(additionalOutputFormats)
```

"Defines extra output formats of the private key and signed certificate chain to be written to this Certificate's target Secret. \n This is an Alpha Feature and is only enabled with the `--feature-gates=AdditionalCertificateOutputFormats=true` option set on both the controller and webhook components."

### fn spec.withAdditionalOutputFormatsMixin

```ts
withAdditionalOutputFormatsMixin(additionalOutputFormats)
```

"Defines extra output formats of the private key and signed certificate chain to be written to this Certificate's target Secret. \n This is an Alpha Feature and is only enabled with the `--feature-gates=AdditionalCertificateOutputFormats=true` option set on both the controller and webhook components."

**Note:** This function appends passed data to existing values

### fn spec.withCommonName

```ts
withCommonName(commonName)
```

"Requested common name X509 certificate subject attribute. More info: https://datatracker.ietf.org/doc/html/rfc5280#section-4.1.2.6 NOTE: TLS clients will ignore this value when any subject alternative name is set (see https://tools.ietf.org/html/rfc6125#section-6.4.4). \n Should have a length of 64 characters or fewer to avoid generating invalid CSRs. Cannot be set if the `literalSubject` field is set."

### fn spec.withDnsNames

```ts
withDnsNames(dnsNames)
```

"Requested DNS subject alternative names."

### fn spec.withDnsNamesMixin

```ts
withDnsNamesMixin(dnsNames)
```

"Requested DNS subject alternative names."

**Note:** This function appends passed data to existing values

### fn spec.withDuration

```ts
withDuration(duration)
```

"Requested 'duration' (i.e. lifetime) of the Certificate. Note that the issuer may choose to ignore the requested duration, just like any other requested attribute. \n If unset, this defaults to 90 days. Minimum accepted duration is 1 hour. Value must be in units accepted by Go time.ParseDuration https://golang.org/pkg/time/#ParseDuration."

### fn spec.withEmailAddresses

```ts
withEmailAddresses(emailAddresses)
```

"Requested email subject alternative names."

### fn spec.withEmailAddressesMixin

```ts
withEmailAddressesMixin(emailAddresses)
```

"Requested email subject alternative names."

**Note:** This function appends passed data to existing values

### fn spec.withEncodeUsagesInRequest

```ts
withEncodeUsagesInRequest(encodeUsagesInRequest)
```

"Whether the KeyUsage and ExtKeyUsage extensions should be set in the encoded CSR. \n This option defaults to true, and should only be disabled if the target issuer does not support CSRs with these X509 KeyUsage/ ExtKeyUsage extensions."

### fn spec.withIpAddresses

```ts
withIpAddresses(ipAddresses)
```

"Requested IP address subject alternative names."

### fn spec.withIpAddressesMixin

```ts
withIpAddressesMixin(ipAddresses)
```

"Requested IP address subject alternative names."

**Note:** This function appends passed data to existing values

### fn spec.withIsCA

```ts
withIsCA(isCA)
```

"Requested basic constraints isCA value. The isCA value is used to set the `isCA` field on the created CertificateRequest resources. Note that the issuer may choose to ignore the requested isCA value, just like any other requested attribute. \n If true, this will automatically add the `cert sign` usage to the list of requested `usages`."

### fn spec.withLiteralSubject

```ts
withLiteralSubject(literalSubject)
```

"Requested X.509 certificate subject, represented using the LDAP \"String Representation of a Distinguished Name\" [1]. Important: the LDAP string format also specifies the order of the attributes in the subject, this is important when issuing certs for LDAP authentication. Example: `CN=foo,DC=corp,DC=example,DC=com` More info [1]: https://datatracker.ietf.org/doc/html/rfc4514 More info: https://github.com/cert-manager/cert-manager/issues/3203 More info: https://github.com/cert-manager/cert-manager/issues/4424 \n Cannot be set if the `subject` or `commonName` field is set. This is an Alpha Feature and is only enabled with the `--feature-gates=LiteralCertificateSubject=true` option set on both the controller and webhook components."

### fn spec.withRenewBefore

```ts
withRenewBefore(renewBefore)
```

"How long before the currently issued certificate's expiry cert-manager should renew the certificate. For example, if a certificate is valid for 60 minutes, and `renewBefore=10m`, cert-manager will begin to attempt to renew the certificate 50 minutes after it was issued (i.e. when there are 10 minutes remaining until the certificate is no longer valid). \n NOTE: The actual lifetime of the issued certificate is used to determine the renewal time. If an issuer returns a certificate with a different lifetime than the one requested, cert-manager will use the lifetime of the issued certificate. \n If unset, this defaults to 1/3 of the issued certificate's lifetime. Minimum accepted value is 5 minutes. Value must be in units accepted by Go time.ParseDuration https://golang.org/pkg/time/#ParseDuration."

### fn spec.withRevisionHistoryLimit

```ts
withRevisionHistoryLimit(revisionHistoryLimit)
```

"The maximum number of CertificateRequest revisions that are maintained in the Certificate's history. Each revision represents a single `CertificateRequest` created by this Certificate, either when it was created, renewed, or Spec was changed. Revisions will be removed by oldest first if the number of revisions exceeds this number. \n If set, revisionHistoryLimit must be a value of `1` or greater. If unset (`nil`), revisions will not be garbage collected. Default value is `nil`."

### fn spec.withSecretName

```ts
withSecretName(secretName)
```

"Name of the Secret resource that will be automatically created and managed by this Certificate resource. It will be populated with a private key and certificate, signed by the denoted issuer. The Secret resource lives in the same namespace as the Certificate resource."

### fn spec.withUris

```ts
withUris(uris)
```

"Requested URI subject alternative names."

### fn spec.withUrisMixin

```ts
withUrisMixin(uris)
```

"Requested URI subject alternative names."

**Note:** This function appends passed data to existing values

### fn spec.withUsages

```ts
withUsages(usages)
```

"Requested key usages and extended key usages. These usages are used to set the `usages` field on the created CertificateRequest resources. If `encodeUsagesInRequest` is unset or set to `true`, the usages will additionally be encoded in the `request` field which contains the CSR blob. \n If unset, defaults to `digital signature` and `key encipherment`."

### fn spec.withUsagesMixin

```ts
withUsagesMixin(usages)
```

"Requested key usages and extended key usages. These usages are used to set the `usages` field on the created CertificateRequest resources. If `encodeUsagesInRequest` is unset or set to `true`, the usages will additionally be encoded in the `request` field which contains the CSR blob. \n If unset, defaults to `digital signature` and `key encipherment`."

**Note:** This function appends passed data to existing values

## obj spec.additionalOutputFormats

"Defines extra output formats of the private key and signed certificate chain to be written to this Certificate's target Secret. \n This is an Alpha Feature and is only enabled with the `--feature-gates=AdditionalCertificateOutputFormats=true` option set on both the controller and webhook components."

### fn spec.additionalOutputFormats.withType

```ts
withType(type)
```

"Type is the name of the format type that should be written to the Certificate's target Secret."

## obj spec.issuerRef

"Reference to the issuer responsible for issuing the certificate. If the issuer is namespace-scoped, it must be in the same namespace as the Certificate. If the issuer is cluster-scoped, it can be used from any namespace. \n The `name` field of the reference must always be specified."

### fn spec.issuerRef.withGroup

```ts
withGroup(group)
```

"Group of the resource being referred to."

### fn spec.issuerRef.withKind

```ts
withKind(kind)
```

"Kind of the resource being referred to."

### fn spec.issuerRef.withName

```ts
withName(name)
```

"Name of the resource being referred to."

## obj spec.keystores

"Additional keystore output formats to be stored in the Certificate's Secret."

## obj spec.keystores.jks

"JKS configures options for storing a JKS keystore in the `spec.secretName` Secret resource."

### fn spec.keystores.jks.withCreate

```ts
withCreate(create)
```

"Create enables JKS keystore creation for the Certificate. If true, a file named `keystore.jks` will be created in the target Secret resource, encrypted using the password stored in `passwordSecretRef`. The keystore file will be updated immediately. If the issuer provided a CA certificate, a file named `truststore.jks` will also be created in the target Secret resource, encrypted using the password stored in `passwordSecretRef` containing the issuing Certificate Authority"

## obj spec.keystores.jks.passwordSecretRef

"PasswordSecretRef is a reference to a key in a Secret resource containing the password used to encrypt the JKS keystore."

### fn spec.keystores.jks.passwordSecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used. Some instances of this field may be defaulted, in others it may be required."

### fn spec.keystores.jks.passwordSecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.keystores.pkcs12

"PKCS12 configures options for storing a PKCS12 keystore in the `spec.secretName` Secret resource."

### fn spec.keystores.pkcs12.withCreate

```ts
withCreate(create)
```

"Create enables PKCS12 keystore creation for the Certificate. If true, a file named `keystore.p12` will be created in the target Secret resource, encrypted using the password stored in `passwordSecretRef`. The keystore file will be updated immediately. If the issuer provided a CA certificate, a file named `truststore.p12` will also be created in the target Secret resource, encrypted using the password stored in `passwordSecretRef` containing the issuing Certificate Authority"

## obj spec.keystores.pkcs12.passwordSecretRef

"PasswordSecretRef is a reference to a key in a Secret resource containing the password used to encrypt the PKCS12 keystore."

### fn spec.keystores.pkcs12.passwordSecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used. Some instances of this field may be defaulted, in others it may be required."

### fn spec.keystores.pkcs12.passwordSecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.privateKey

"Private key options. These include the key algorithm and size, the used encoding and the rotation policy."

### fn spec.privateKey.withAlgorithm

```ts
withAlgorithm(algorithm)
```

"Algorithm is the private key algorithm of the corresponding private key for this certificate. \n If provided, allowed values are either `RSA`, `ECDSA` or `Ed25519`. If `algorithm` is specified and `size` is not provided, key size of 2048 will be used for `RSA` key algorithm and key size of 256 will be used for `ECDSA` key algorithm. key size is ignored when using the `Ed25519` key algorithm."

### fn spec.privateKey.withEncoding

```ts
withEncoding(encoding)
```

"The private key cryptography standards (PKCS) encoding for this certificate's private key to be encoded in. \n If provided, allowed values are `PKCS1` and `PKCS8` standing for PKCS#1 and PKCS#8, respectively. Defaults to `PKCS1` if not specified."

### fn spec.privateKey.withRotationPolicy

```ts
withRotationPolicy(rotationPolicy)
```

"RotationPolicy controls how private keys should be regenerated when a re-issuance is being processed. \n If set to `Never`, a private key will only be generated if one does not already exist in the target `spec.secretName`. If one does exists but it does not have the correct algorithm or size, a warning will be raised to await user intervention. If set to `Always`, a private key matching the specified requirements will be generated whenever a re-issuance occurs. Default is `Never` for backward compatibility."

### fn spec.privateKey.withSize

```ts
withSize(size)
```

"Size is the key bit size of the corresponding private key for this certificate. \n If `algorithm` is set to `RSA`, valid values are `2048`, `4096` or `8192`, and will default to `2048` if not specified. If `algorithm` is set to `ECDSA`, valid values are `256`, `384` or `521`, and will default to `256` if not specified. If `algorithm` is set to `Ed25519`, Size is ignored. No other values are allowed."

## obj spec.secretTemplate

"Defines annotations and labels to be copied to the Certificate's Secret. Labels and annotations on the Secret will be changed as they appear on the SecretTemplate when added or removed. SecretTemplate annotations are added in conjunction with, and cannot overwrite, the base set of annotations cert-manager sets on the Certificate's Secret."

### fn spec.secretTemplate.withAnnotations

```ts
withAnnotations(annotations)
```

"Annotations is a key value map to be copied to the target Kubernetes Secret."

### fn spec.secretTemplate.withAnnotationsMixin

```ts
withAnnotationsMixin(annotations)
```

"Annotations is a key value map to be copied to the target Kubernetes Secret."

**Note:** This function appends passed data to existing values

### fn spec.secretTemplate.withLabels

```ts
withLabels(labels)
```

"Labels is a key value map to be copied to the target Kubernetes Secret."

### fn spec.secretTemplate.withLabelsMixin

```ts
withLabelsMixin(labels)
```

"Labels is a key value map to be copied to the target Kubernetes Secret."

**Note:** This function appends passed data to existing values

## obj spec.subject

"Requested set of X509 certificate subject attributes. More info: https://datatracker.ietf.org/doc/html/rfc5280#section-4.1.2.6 \n The common name attribute is specified separately in the `commonName` field. Cannot be set if the `literalSubject` field is set."

### fn spec.subject.withCountries

```ts
withCountries(countries)
```

"Countries to be used on the Certificate."

### fn spec.subject.withCountriesMixin

```ts
withCountriesMixin(countries)
```

"Countries to be used on the Certificate."

**Note:** This function appends passed data to existing values

### fn spec.subject.withLocalities

```ts
withLocalities(localities)
```

"Cities to be used on the Certificate."

### fn spec.subject.withLocalitiesMixin

```ts
withLocalitiesMixin(localities)
```

"Cities to be used on the Certificate."

**Note:** This function appends passed data to existing values

### fn spec.subject.withOrganizationalUnits

```ts
withOrganizationalUnits(organizationalUnits)
```

"Organizational Units to be used on the Certificate."

### fn spec.subject.withOrganizationalUnitsMixin

```ts
withOrganizationalUnitsMixin(organizationalUnits)
```

"Organizational Units to be used on the Certificate."

**Note:** This function appends passed data to existing values

### fn spec.subject.withOrganizations

```ts
withOrganizations(organizations)
```

"Organizations to be used on the Certificate."

### fn spec.subject.withOrganizationsMixin

```ts
withOrganizationsMixin(organizations)
```

"Organizations to be used on the Certificate."

**Note:** This function appends passed data to existing values

### fn spec.subject.withPostalCodes

```ts
withPostalCodes(postalCodes)
```

"Postal codes to be used on the Certificate."

### fn spec.subject.withPostalCodesMixin

```ts
withPostalCodesMixin(postalCodes)
```

"Postal codes to be used on the Certificate."

**Note:** This function appends passed data to existing values

### fn spec.subject.withProvinces

```ts
withProvinces(provinces)
```

"State/Provinces to be used on the Certificate."

### fn spec.subject.withProvincesMixin

```ts
withProvincesMixin(provinces)
```

"State/Provinces to be used on the Certificate."

**Note:** This function appends passed data to existing values

### fn spec.subject.withSerialNumber

```ts
withSerialNumber(serialNumber)
```

"Serial number to be used on the Certificate."

### fn spec.subject.withStreetAddresses

```ts
withStreetAddresses(streetAddresses)
```

"Street addresses to be used on the Certificate."

### fn spec.subject.withStreetAddressesMixin

```ts
withStreetAddressesMixin(streetAddresses)
```

"Street addresses to be used on the Certificate."

**Note:** This function appends passed data to existing values