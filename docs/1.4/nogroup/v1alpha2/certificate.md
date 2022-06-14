---
permalink: /1.4/nogroup/v1alpha2/certificate/
---

# nogroup.v1alpha2.certificate

"A Certificate resource should be created to ensure an up to date and signed x509 certificate is stored in the Kubernetes Secret resource named in `spec.secretName`. \n The stored certificate will be renewed before it expires (as configured by `spec.renewBefore`)."

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
  * [`fn withCommonName(commonName)`](#fn-specwithcommonname)
  * [`fn withDnsNames(dnsNames)`](#fn-specwithdnsnames)
  * [`fn withDnsNamesMixin(dnsNames)`](#fn-specwithdnsnamesmixin)
  * [`fn withDuration(duration)`](#fn-specwithduration)
  * [`fn withEmailSANs(emailSANs)`](#fn-specwithemailsans)
  * [`fn withEmailSANsMixin(emailSANs)`](#fn-specwithemailsansmixin)
  * [`fn withEncodeUsagesInRequest(encodeUsagesInRequest)`](#fn-specwithencodeusagesinrequest)
  * [`fn withIpAddresses(ipAddresses)`](#fn-specwithipaddresses)
  * [`fn withIpAddressesMixin(ipAddresses)`](#fn-specwithipaddressesmixin)
  * [`fn withIsCA(isCA)`](#fn-specwithisca)
  * [`fn withKeyAlgorithm(keyAlgorithm)`](#fn-specwithkeyalgorithm)
  * [`fn withKeyEncoding(keyEncoding)`](#fn-specwithkeyencoding)
  * [`fn withKeySize(keySize)`](#fn-specwithkeysize)
  * [`fn withOrganization(organization)`](#fn-specwithorganization)
  * [`fn withOrganizationMixin(organization)`](#fn-specwithorganizationmixin)
  * [`fn withRenewBefore(renewBefore)`](#fn-specwithrenewbefore)
  * [`fn withRevisionHistoryLimit(revisionHistoryLimit)`](#fn-specwithrevisionhistorylimit)
  * [`fn withSecretName(secretName)`](#fn-specwithsecretname)
  * [`fn withUriSANs(uriSANs)`](#fn-specwithurisans)
  * [`fn withUriSANsMixin(uriSANs)`](#fn-specwithurisansmixin)
  * [`fn withUsages(usages)`](#fn-specwithusages)
  * [`fn withUsagesMixin(usages)`](#fn-specwithusagesmixin)
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
    * [`fn withRotationPolicy(rotationPolicy)`](#fn-specprivatekeywithrotationpolicy)
  * [`obj spec.subject`](#obj-specsubject)
    * [`fn withCountries(countries)`](#fn-specsubjectwithcountries)
    * [`fn withCountriesMixin(countries)`](#fn-specsubjectwithcountriesmixin)
    * [`fn withLocalities(localities)`](#fn-specsubjectwithlocalities)
    * [`fn withLocalitiesMixin(localities)`](#fn-specsubjectwithlocalitiesmixin)
    * [`fn withOrganizationalUnits(organizationalUnits)`](#fn-specsubjectwithorganizationalunits)
    * [`fn withOrganizationalUnitsMixin(organizationalUnits)`](#fn-specsubjectwithorganizationalunitsmixin)
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

"Desired state of the Certificate resource."

### fn spec.withCommonName

```ts
withCommonName(commonName)
```

"CommonName is a common name to be used on the Certificate. The CommonName should have a length of 64 characters or fewer to avoid generating invalid CSRs. This value is ignored by TLS clients when any subject alt name is set. This is x509 behaviour: https://tools.ietf.org/html/rfc6125#section-6.4.4"

### fn spec.withDnsNames

```ts
withDnsNames(dnsNames)
```

"DNSNames is a list of DNS subjectAltNames to be set on the Certificate."

### fn spec.withDnsNamesMixin

```ts
withDnsNamesMixin(dnsNames)
```

"DNSNames is a list of DNS subjectAltNames to be set on the Certificate."

**Note:** This function appends passed data to existing values

### fn spec.withDuration

```ts
withDuration(duration)
```

"The requested 'duration' (i.e. lifetime) of the Certificate. This option may be ignored/overridden by some issuer types. If unset this defaults to 90 days. Certificate will be renewed either 2/3 through its duration or `renewBefore` period before its expiry, whichever is later. Minimum accepted duration is 1 hour. Value must be in units accepted by Go time.ParseDuration https://golang.org/pkg/time/#ParseDuration"

### fn spec.withEmailSANs

```ts
withEmailSANs(emailSANs)
```

"EmailSANs is a list of email subjectAltNames to be set on the Certificate."

### fn spec.withEmailSANsMixin

```ts
withEmailSANsMixin(emailSANs)
```

"EmailSANs is a list of email subjectAltNames to be set on the Certificate."

**Note:** This function appends passed data to existing values

### fn spec.withEncodeUsagesInRequest

```ts
withEncodeUsagesInRequest(encodeUsagesInRequest)
```

"EncodeUsagesInRequest controls whether key usages should be present in the CertificateRequest"

### fn spec.withIpAddresses

```ts
withIpAddresses(ipAddresses)
```

"IPAddresses is a list of IP address subjectAltNames to be set on the Certificate."

### fn spec.withIpAddressesMixin

```ts
withIpAddressesMixin(ipAddresses)
```

"IPAddresses is a list of IP address subjectAltNames to be set on the Certificate."

**Note:** This function appends passed data to existing values

### fn spec.withIsCA

```ts
withIsCA(isCA)
```

"IsCA will mark this Certificate as valid for certificate signing. This will automatically add the `cert sign` usage to the list of `usages`."

### fn spec.withKeyAlgorithm

```ts
withKeyAlgorithm(keyAlgorithm)
```

"KeyAlgorithm is the private key algorithm of the corresponding private key for this certificate. If provided, allowed values are either `rsa` or `ecdsa` If `keyAlgorithm` is specified and `keySize` is not provided, key size of 256 will be used for `ecdsa` key algorithm and key size of 2048 will be used for `rsa` key algorithm."

### fn spec.withKeyEncoding

```ts
withKeyEncoding(keyEncoding)
```

"KeyEncoding is the private key cryptography standards (PKCS) for this certificate's private key to be encoded in. If provided, allowed values are `pkcs1` and `pkcs8` standing for PKCS#1 and PKCS#8, respectively. If KeyEncoding is not specified, then `pkcs1` will be used by default."

### fn spec.withKeySize

```ts
withKeySize(keySize)
```

"KeySize is the key bit size of the corresponding private key for this certificate. If `keyAlgorithm` is set to `rsa`, valid values are `2048`, `4096` or `8192`, and will default to `2048` if not specified. If `keyAlgorithm` is set to `ecdsa`, valid values are `256`, `384` or `521`, and will default to `256` if not specified. No other values are allowed."

### fn spec.withOrganization

```ts
withOrganization(organization)
```

"Organization is a list of organizations to be used on the Certificate."

### fn spec.withOrganizationMixin

```ts
withOrganizationMixin(organization)
```

"Organization is a list of organizations to be used on the Certificate."

**Note:** This function appends passed data to existing values

### fn spec.withRenewBefore

```ts
withRenewBefore(renewBefore)
```

"How long before the currently issued certificate's expiry cert-manager should renew the certificate. The default is 2/3 of the issued certificate's duration. Minimum accepted value is 5 minutes. Value must be in units accepted by Go time.ParseDuration https://golang.org/pkg/time/#ParseDuration"

### fn spec.withRevisionHistoryLimit

```ts
withRevisionHistoryLimit(revisionHistoryLimit)
```

"revisionHistoryLimit is the maximum number of CertificateRequest revisions that are maintained in the Certificate's history. Each revision represents a single `CertificateRequest` created by this Certificate, either when it was created, renewed, or Spec was changed. Revisions will be removed by oldest first if the number of revisions exceeds this number. If set, revisionHistoryLimit must be a value of `1` or greater. If unset (`nil`), revisions will not be garbage collected. Default value is `nil`."

### fn spec.withSecretName

```ts
withSecretName(secretName)
```

"SecretName is the name of the secret resource that will be automatically created and managed by this Certificate resource. It will be populated with a private key and certificate, signed by the denoted issuer."

### fn spec.withUriSANs

```ts
withUriSANs(uriSANs)
```

"URISANs is a list of URI subjectAltNames to be set on the Certificate."

### fn spec.withUriSANsMixin

```ts
withUriSANsMixin(uriSANs)
```

"URISANs is a list of URI subjectAltNames to be set on the Certificate."

**Note:** This function appends passed data to existing values

### fn spec.withUsages

```ts
withUsages(usages)
```

"Usages is the set of x509 usages that are requested for the certificate. Defaults to `digital signature` and `key encipherment` if not specified."

### fn spec.withUsagesMixin

```ts
withUsagesMixin(usages)
```

"Usages is the set of x509 usages that are requested for the certificate. Defaults to `digital signature` and `key encipherment` if not specified."

**Note:** This function appends passed data to existing values

## obj spec.issuerRef

"IssuerRef is a reference to the issuer for this certificate. If the `kind` field is not set, or set to `Issuer`, an Issuer resource with the given name in the same namespace as the Certificate will be used. If the `kind` field is set to `ClusterIssuer`, a ClusterIssuer with the provided name will be used. The `name` field in this stanza is required at all times."

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

"Keystores configures additional keystore output formats stored in the `secretName` Secret resource."

## obj spec.keystores.jks

"JKS configures options for storing a JKS keystore in the `spec.secretName` Secret resource."

### fn spec.keystores.jks.withCreate

```ts
withCreate(create)
```

"Create enables JKS keystore creation for the Certificate. If true, a file named `keystore.jks` will be created in the target Secret resource, encrypted using the password stored in `passwordSecretRef`. The keystore file will only be updated upon re-issuance."

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

"Create enables PKCS12 keystore creation for the Certificate. If true, a file named `keystore.p12` will be created in the target Secret resource, encrypted using the password stored in `passwordSecretRef`. The keystore file will only be updated upon re-issuance."

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

"Options to control private keys used for the Certificate."

### fn spec.privateKey.withRotationPolicy

```ts
withRotationPolicy(rotationPolicy)
```

"RotationPolicy controls how private keys should be regenerated when a re-issuance is being processed. If set to Never, a private key will only be generated if one does not already exist in the target `spec.secretName`. If one does exists but it does not have the correct algorithm or size, a warning will be raised to await user intervention. If set to Always, a private key matching the specified requirements will be generated whenever a re-issuance occurs. Default is 'Never' for backward compatibility."

## obj spec.subject

"Full X509 name specification (https://golang.org/pkg/crypto/x509/pkix/#Name)."

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