---
permalink: /1.15/nogroup/v1/certificate/
---

# nogroup.v1.certificate

"A Certificate resource should be created to ensure an up to date and signed\nX.509 certificate is stored in the Kubernetes Secret resource named in `spec.secretName`.\n\n\nThe stored certificate will be renewed before it expires (as configured by `spec.renewBefore`)."

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
  * [`fn withOtherNames(otherNames)`](#fn-specwithothernames)
  * [`fn withOtherNamesMixin(otherNames)`](#fn-specwithothernamesmixin)
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
      * [`fn withAlias(alias)`](#fn-speckeystoresjkswithalias)
      * [`fn withCreate(create)`](#fn-speckeystoresjkswithcreate)
      * [`obj spec.keystores.jks.passwordSecretRef`](#obj-speckeystoresjkspasswordsecretref)
        * [`fn withKey(key)`](#fn-speckeystoresjkspasswordsecretrefwithkey)
        * [`fn withName(name)`](#fn-speckeystoresjkspasswordsecretrefwithname)
    * [`obj spec.keystores.pkcs12`](#obj-speckeystorespkcs12)
      * [`fn withCreate(create)`](#fn-speckeystorespkcs12withcreate)
      * [`fn withProfile(profile)`](#fn-speckeystorespkcs12withprofile)
      * [`obj spec.keystores.pkcs12.passwordSecretRef`](#obj-speckeystorespkcs12passwordsecretref)
        * [`fn withKey(key)`](#fn-speckeystorespkcs12passwordsecretrefwithkey)
        * [`fn withName(name)`](#fn-speckeystorespkcs12passwordsecretrefwithname)
  * [`obj spec.nameConstraints`](#obj-specnameconstraints)
    * [`fn withCritical(critical)`](#fn-specnameconstraintswithcritical)
    * [`obj spec.nameConstraints.excluded`](#obj-specnameconstraintsexcluded)
      * [`fn withDnsDomains(dnsDomains)`](#fn-specnameconstraintsexcludedwithdnsdomains)
      * [`fn withDnsDomainsMixin(dnsDomains)`](#fn-specnameconstraintsexcludedwithdnsdomainsmixin)
      * [`fn withEmailAddresses(emailAddresses)`](#fn-specnameconstraintsexcludedwithemailaddresses)
      * [`fn withEmailAddressesMixin(emailAddresses)`](#fn-specnameconstraintsexcludedwithemailaddressesmixin)
      * [`fn withIpRanges(ipRanges)`](#fn-specnameconstraintsexcludedwithipranges)
      * [`fn withIpRangesMixin(ipRanges)`](#fn-specnameconstraintsexcludedwithiprangesmixin)
      * [`fn withUriDomains(uriDomains)`](#fn-specnameconstraintsexcludedwithuridomains)
      * [`fn withUriDomainsMixin(uriDomains)`](#fn-specnameconstraintsexcludedwithuridomainsmixin)
    * [`obj spec.nameConstraints.permitted`](#obj-specnameconstraintspermitted)
      * [`fn withDnsDomains(dnsDomains)`](#fn-specnameconstraintspermittedwithdnsdomains)
      * [`fn withDnsDomainsMixin(dnsDomains)`](#fn-specnameconstraintspermittedwithdnsdomainsmixin)
      * [`fn withEmailAddresses(emailAddresses)`](#fn-specnameconstraintspermittedwithemailaddresses)
      * [`fn withEmailAddressesMixin(emailAddresses)`](#fn-specnameconstraintspermittedwithemailaddressesmixin)
      * [`fn withIpRanges(ipRanges)`](#fn-specnameconstraintspermittedwithipranges)
      * [`fn withIpRangesMixin(ipRanges)`](#fn-specnameconstraintspermittedwithiprangesmixin)
      * [`fn withUriDomains(uriDomains)`](#fn-specnameconstraintspermittedwithuridomains)
      * [`fn withUriDomainsMixin(uriDomains)`](#fn-specnameconstraintspermittedwithuridomainsmixin)
  * [`obj spec.otherNames`](#obj-specothernames)
    * [`fn withOid(oid)`](#fn-specothernameswithoid)
    * [`fn withUtf8Value(utf8Value)`](#fn-specothernameswithutf8value)
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

"Specification of the desired state of the Certificate resource.\nhttps://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#spec-and-status"

### fn spec.withAdditionalOutputFormats

```ts
withAdditionalOutputFormats(additionalOutputFormats)
```

"Defines extra output formats of the private key and signed certificate chain\nto be written to this Certificate's target Secret.\n\n\nThis is a Beta Feature enabled by default. It can be disabled with the\n`--feature-gates=AdditionalCertificateOutputFormats=false` option set on both\nthe controller and webhook components."

### fn spec.withAdditionalOutputFormatsMixin

```ts
withAdditionalOutputFormatsMixin(additionalOutputFormats)
```

"Defines extra output formats of the private key and signed certificate chain\nto be written to this Certificate's target Secret.\n\n\nThis is a Beta Feature enabled by default. It can be disabled with the\n`--feature-gates=AdditionalCertificateOutputFormats=false` option set on both\nthe controller and webhook components."

**Note:** This function appends passed data to existing values

### fn spec.withCommonName

```ts
withCommonName(commonName)
```

"Requested common name X509 certificate subject attribute.\nMore info: https://datatracker.ietf.org/doc/html/rfc5280#section-4.1.2.6\nNOTE: TLS clients will ignore this value when any subject alternative name is\nset (see https://tools.ietf.org/html/rfc6125#section-6.4.4).\n\n\nShould have a length of 64 characters or fewer to avoid generating invalid CSRs.\nCannot be set if the `literalSubject` field is set."

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

"Requested 'duration' (i.e. lifetime) of the Certificate. Note that the\nissuer may choose to ignore the requested duration, just like any other\nrequested attribute.\n\n\nIf unset, this defaults to 90 days.\nMinimum accepted duration is 1 hour.\nValue must be in units accepted by Go time.ParseDuration https://golang.org/pkg/time/#ParseDuration."

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

"Whether the KeyUsage and ExtKeyUsage extensions should be set in the encoded CSR.\n\n\nThis option defaults to true, and should only be disabled if the target\nissuer does not support CSRs with these X509 KeyUsage/ ExtKeyUsage extensions."

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

"Requested basic constraints isCA value.\nThe isCA value is used to set the `isCA` field on the created CertificateRequest\nresources. Note that the issuer may choose to ignore the requested isCA value, just\nlike any other requested attribute.\n\n\nIf true, this will automatically add the `cert sign` usage to the list\nof requested `usages`."

### fn spec.withLiteralSubject

```ts
withLiteralSubject(literalSubject)
```

"Requested X.509 certificate subject, represented using the LDAP \"String\nRepresentation of a Distinguished Name\" [1].\nImportant: the LDAP string format also specifies the order of the attributes\nin the subject, this is important when issuing certs for LDAP authentication.\nExample: `CN=foo,DC=corp,DC=example,DC=com`\nMore info [1]: https://datatracker.ietf.org/doc/html/rfc4514\nMore info: https://github.com/cert-manager/cert-manager/issues/3203\nMore info: https://github.com/cert-manager/cert-manager/issues/4424\n\n\nCannot be set if the `subject` or `commonName` field is set."

### fn spec.withOtherNames

```ts
withOtherNames(otherNames)
```

"`otherNames` is an escape hatch for SAN that allows any type. We currently restrict the support to string like otherNames, cf RFC 5280 p 37\nAny UTF8 String valued otherName can be passed with by setting the keys oid: x.x.x.x and UTF8Value: somevalue for `otherName`.\nMost commonly this would be UPN set with oid: 1.3.6.1.4.1.311.20.2.3\nYou should ensure that any OID passed is valid for the UTF8String type as we do not explicitly validate this."

### fn spec.withOtherNamesMixin

```ts
withOtherNamesMixin(otherNames)
```

"`otherNames` is an escape hatch for SAN that allows any type. We currently restrict the support to string like otherNames, cf RFC 5280 p 37\nAny UTF8 String valued otherName can be passed with by setting the keys oid: x.x.x.x and UTF8Value: somevalue for `otherName`.\nMost commonly this would be UPN set with oid: 1.3.6.1.4.1.311.20.2.3\nYou should ensure that any OID passed is valid for the UTF8String type as we do not explicitly validate this."

**Note:** This function appends passed data to existing values

### fn spec.withRenewBefore

```ts
withRenewBefore(renewBefore)
```

"How long before the currently issued certificate's expiry cert-manager should\nrenew the certificate. For example, if a certificate is valid for 60 minutes,\nand `renewBefore=10m`, cert-manager will begin to attempt to renew the certificate\n50 minutes after it was issued (i.e. when there are 10 minutes remaining until\nthe certificate is no longer valid).\n\n\nNOTE: The actual lifetime of the issued certificate is used to determine the\nrenewal time. If an issuer returns a certificate with a different lifetime than\nthe one requested, cert-manager will use the lifetime of the issued certificate.\n\n\nIf unset, this defaults to 1/3 of the issued certificate's lifetime.\nMinimum accepted value is 5 minutes.\nValue must be in units accepted by Go time.ParseDuration https://golang.org/pkg/time/#ParseDuration."

### fn spec.withRevisionHistoryLimit

```ts
withRevisionHistoryLimit(revisionHistoryLimit)
```

"The maximum number of CertificateRequest revisions that are maintained in\nthe Certificate's history. Each revision represents a single `CertificateRequest`\ncreated by this Certificate, either when it was created, renewed, or Spec\nwas changed. Revisions will be removed by oldest first if the number of\nrevisions exceeds this number.\n\n\nIf set, revisionHistoryLimit must be a value of `1` or greater.\nIf unset (`nil`), revisions will not be garbage collected.\nDefault value is `nil`."

### fn spec.withSecretName

```ts
withSecretName(secretName)
```

"Name of the Secret resource that will be automatically created and\nmanaged by this Certificate resource. It will be populated with a\nprivate key and certificate, signed by the denoted issuer. The Secret\nresource lives in the same namespace as the Certificate resource."

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

"Requested key usages and extended key usages.\nThese usages are used to set the `usages` field on the created CertificateRequest\nresources. If `encodeUsagesInRequest` is unset or set to `true`, the usages\nwill additionally be encoded in the `request` field which contains the CSR blob.\n\n\nIf unset, defaults to `digital signature` and `key encipherment`."

### fn spec.withUsagesMixin

```ts
withUsagesMixin(usages)
```

"Requested key usages and extended key usages.\nThese usages are used to set the `usages` field on the created CertificateRequest\nresources. If `encodeUsagesInRequest` is unset or set to `true`, the usages\nwill additionally be encoded in the `request` field which contains the CSR blob.\n\n\nIf unset, defaults to `digital signature` and `key encipherment`."

**Note:** This function appends passed data to existing values

## obj spec.additionalOutputFormats

"Defines extra output formats of the private key and signed certificate chain\nto be written to this Certificate's target Secret.\n\n\nThis is a Beta Feature enabled by default. It can be disabled with the\n`--feature-gates=AdditionalCertificateOutputFormats=false` option set on both\nthe controller and webhook components."

### fn spec.additionalOutputFormats.withType

```ts
withType(type)
```

"Type is the name of the format type that should be written to the\nCertificate's target Secret."

## obj spec.issuerRef

"Reference to the issuer responsible for issuing the certificate.\nIf the issuer is namespace-scoped, it must be in the same namespace\nas the Certificate. If the issuer is cluster-scoped, it can be used\nfrom any namespace.\n\n\nThe `name` field of the reference must always be specified."

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

"JKS configures options for storing a JKS keystore in the\n`spec.secretName` Secret resource."

### fn spec.keystores.jks.withAlias

```ts
withAlias(alias)
```

"Alias specifies the alias of the key in the keystore, required by the JKS format.\nIf not provided, the default alias `certificate` will be used."

### fn spec.keystores.jks.withCreate

```ts
withCreate(create)
```

"Create enables JKS keystore creation for the Certificate.\nIf true, a file named `keystore.jks` will be created in the target\nSecret resource, encrypted using the password stored in\n`passwordSecretRef`.\nThe keystore file will be updated immediately.\nIf the issuer provided a CA certificate, a file named `truststore.jks`\nwill also be created in the target Secret resource, encrypted using the\npassword stored in `passwordSecretRef`\ncontaining the issuing Certificate Authority"

## obj spec.keystores.jks.passwordSecretRef

"PasswordSecretRef is a reference to a key in a Secret resource\ncontaining the password used to encrypt the JKS keystore."

### fn spec.keystores.jks.passwordSecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used.\nSome instances of this field may be defaulted, in others it may be\nrequired."

### fn spec.keystores.jks.passwordSecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to.\nMore info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.keystores.pkcs12

"PKCS12 configures options for storing a PKCS12 keystore in the\n`spec.secretName` Secret resource."

### fn spec.keystores.pkcs12.withCreate

```ts
withCreate(create)
```

"Create enables PKCS12 keystore creation for the Certificate.\nIf true, a file named `keystore.p12` will be created in the target\nSecret resource, encrypted using the password stored in\n`passwordSecretRef`.\nThe keystore file will be updated immediately.\nIf the issuer provided a CA certificate, a file named `truststore.p12` will\nalso be created in the target Secret resource, encrypted using the\npassword stored in `passwordSecretRef` containing the issuing Certificate\nAuthority"

### fn spec.keystores.pkcs12.withProfile

```ts
withProfile(profile)
```

"Profile specifies the key and certificate encryption algorithms and the HMAC algorithm\nused to create the PKCS12 keystore. Default value is `LegacyRC2` for backward compatibility.\n\n\nIf provided, allowed values are:\n`LegacyRC2`: Deprecated. Not supported by default in OpenSSL 3 or Java 20.\n`LegacyDES`: Less secure algorithm. Use this option for maximal compatibility.\n`Modern2023`: Secure algorithm. Use this option in case you have to always use secure algorithms\n(eg. because of company policy). Please note that the security of the algorithm is not that important\nin reality, because the unencrypted certificate and private key are also stored in the Secret."

## obj spec.keystores.pkcs12.passwordSecretRef

"PasswordSecretRef is a reference to a key in a Secret resource\ncontaining the password used to encrypt the PKCS12 keystore."

### fn spec.keystores.pkcs12.passwordSecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used.\nSome instances of this field may be defaulted, in others it may be\nrequired."

### fn spec.keystores.pkcs12.passwordSecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to.\nMore info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.nameConstraints

"x.509 certificate NameConstraint extension which MUST NOT be used in a non-CA certificate.\nMore Info: https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.10\n\n\nThis is an Alpha Feature and is only enabled with the\n`--feature-gates=NameConstraints=true` option set on both\nthe controller and webhook components."

### fn spec.nameConstraints.withCritical

```ts
withCritical(critical)
```

"if true then the name constraints are marked critical."

## obj spec.nameConstraints.excluded

"Excluded contains the constraints which must be disallowed. Any name matching a\nrestriction in the excluded field is invalid regardless\nof information appearing in the permitted"

### fn spec.nameConstraints.excluded.withDnsDomains

```ts
withDnsDomains(dnsDomains)
```

"DNSDomains is a list of DNS domains that are permitted or excluded."

### fn spec.nameConstraints.excluded.withDnsDomainsMixin

```ts
withDnsDomainsMixin(dnsDomains)
```

"DNSDomains is a list of DNS domains that are permitted or excluded."

**Note:** This function appends passed data to existing values

### fn spec.nameConstraints.excluded.withEmailAddresses

```ts
withEmailAddresses(emailAddresses)
```

"EmailAddresses is a list of Email Addresses that are permitted or excluded."

### fn spec.nameConstraints.excluded.withEmailAddressesMixin

```ts
withEmailAddressesMixin(emailAddresses)
```

"EmailAddresses is a list of Email Addresses that are permitted or excluded."

**Note:** This function appends passed data to existing values

### fn spec.nameConstraints.excluded.withIpRanges

```ts
withIpRanges(ipRanges)
```

"IPRanges is a list of IP Ranges that are permitted or excluded.\nThis should be a valid CIDR notation."

### fn spec.nameConstraints.excluded.withIpRangesMixin

```ts
withIpRangesMixin(ipRanges)
```

"IPRanges is a list of IP Ranges that are permitted or excluded.\nThis should be a valid CIDR notation."

**Note:** This function appends passed data to existing values

### fn spec.nameConstraints.excluded.withUriDomains

```ts
withUriDomains(uriDomains)
```

"URIDomains is a list of URI domains that are permitted or excluded."

### fn spec.nameConstraints.excluded.withUriDomainsMixin

```ts
withUriDomainsMixin(uriDomains)
```

"URIDomains is a list of URI domains that are permitted or excluded."

**Note:** This function appends passed data to existing values

## obj spec.nameConstraints.permitted

"Permitted contains the constraints in which the names must be located."

### fn spec.nameConstraints.permitted.withDnsDomains

```ts
withDnsDomains(dnsDomains)
```

"DNSDomains is a list of DNS domains that are permitted or excluded."

### fn spec.nameConstraints.permitted.withDnsDomainsMixin

```ts
withDnsDomainsMixin(dnsDomains)
```

"DNSDomains is a list of DNS domains that are permitted or excluded."

**Note:** This function appends passed data to existing values

### fn spec.nameConstraints.permitted.withEmailAddresses

```ts
withEmailAddresses(emailAddresses)
```

"EmailAddresses is a list of Email Addresses that are permitted or excluded."

### fn spec.nameConstraints.permitted.withEmailAddressesMixin

```ts
withEmailAddressesMixin(emailAddresses)
```

"EmailAddresses is a list of Email Addresses that are permitted or excluded."

**Note:** This function appends passed data to existing values

### fn spec.nameConstraints.permitted.withIpRanges

```ts
withIpRanges(ipRanges)
```

"IPRanges is a list of IP Ranges that are permitted or excluded.\nThis should be a valid CIDR notation."

### fn spec.nameConstraints.permitted.withIpRangesMixin

```ts
withIpRangesMixin(ipRanges)
```

"IPRanges is a list of IP Ranges that are permitted or excluded.\nThis should be a valid CIDR notation."

**Note:** This function appends passed data to existing values

### fn spec.nameConstraints.permitted.withUriDomains

```ts
withUriDomains(uriDomains)
```

"URIDomains is a list of URI domains that are permitted or excluded."

### fn spec.nameConstraints.permitted.withUriDomainsMixin

```ts
withUriDomainsMixin(uriDomains)
```

"URIDomains is a list of URI domains that are permitted or excluded."

**Note:** This function appends passed data to existing values

## obj spec.otherNames

"`otherNames` is an escape hatch for SAN that allows any type. We currently restrict the support to string like otherNames, cf RFC 5280 p 37\nAny UTF8 String valued otherName can be passed with by setting the keys oid: x.x.x.x and UTF8Value: somevalue for `otherName`.\nMost commonly this would be UPN set with oid: 1.3.6.1.4.1.311.20.2.3\nYou should ensure that any OID passed is valid for the UTF8String type as we do not explicitly validate this."

### fn spec.otherNames.withOid

```ts
withOid(oid)
```

"OID is the object identifier for the otherName SAN.\nThe object identifier must be expressed as a dotted string, for\nexample, \"1.2.840.113556.1.4.221\"."

### fn spec.otherNames.withUtf8Value

```ts
withUtf8Value(utf8Value)
```

"utf8Value is the string value of the otherName SAN.\nThe utf8Value accepts any valid UTF8 string to set as value for the otherName SAN."

## obj spec.privateKey

"Private key options. These include the key algorithm and size, the used\nencoding and the rotation policy."

### fn spec.privateKey.withAlgorithm

```ts
withAlgorithm(algorithm)
```

"Algorithm is the private key algorithm of the corresponding private key\nfor this certificate.\n\n\nIf provided, allowed values are either `RSA`, `ECDSA` or `Ed25519`.\nIf `algorithm` is specified and `size` is not provided,\nkey size of 2048 will be used for `RSA` key algorithm and\nkey size of 256 will be used for `ECDSA` key algorithm.\nkey size is ignored when using the `Ed25519` key algorithm."

### fn spec.privateKey.withEncoding

```ts
withEncoding(encoding)
```

"The private key cryptography standards (PKCS) encoding for this\ncertificate's private key to be encoded in.\n\n\nIf provided, allowed values are `PKCS1` and `PKCS8` standing for PKCS#1\nand PKCS#8, respectively.\nDefaults to `PKCS1` if not specified."

### fn spec.privateKey.withRotationPolicy

```ts
withRotationPolicy(rotationPolicy)
```

"RotationPolicy controls how private keys should be regenerated when a\nre-issuance is being processed.\n\n\nIf set to `Never`, a private key will only be generated if one does not\nalready exist in the target `spec.secretName`. If one does exists but it\ndoes not have the correct algorithm or size, a warning will be raised\nto await user intervention.\nIf set to `Always`, a private key matching the specified requirements\nwill be generated whenever a re-issuance occurs.\nDefault is `Never` for backward compatibility."

### fn spec.privateKey.withSize

```ts
withSize(size)
```

"Size is the key bit size of the corresponding private key for this certificate.\n\n\nIf `algorithm` is set to `RSA`, valid values are `2048`, `4096` or `8192`,\nand will default to `2048` if not specified.\nIf `algorithm` is set to `ECDSA`, valid values are `256`, `384` or `521`,\nand will default to `256` if not specified.\nIf `algorithm` is set to `Ed25519`, Size is ignored.\nNo other values are allowed."

## obj spec.secretTemplate

"Defines annotations and labels to be copied to the Certificate's Secret.\nLabels and annotations on the Secret will be changed as they appear on the\nSecretTemplate when added or removed. SecretTemplate annotations are added\nin conjunction with, and cannot overwrite, the base set of annotations\ncert-manager sets on the Certificate's Secret."

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

"Requested set of X509 certificate subject attributes.\nMore info: https://datatracker.ietf.org/doc/html/rfc5280#section-4.1.2.6\n\n\nThe common name attribute is specified separately in the `commonName` field.\nCannot be set if the `literalSubject` field is set."

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