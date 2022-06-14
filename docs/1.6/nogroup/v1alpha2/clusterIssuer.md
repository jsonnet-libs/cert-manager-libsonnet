---
permalink: /1.6/nogroup/v1alpha2/clusterIssuer/
---

# nogroup.v1alpha2.clusterIssuer

"A ClusterIssuer represents a certificate issuing authority which can be referenced as part of `issuerRef` fields. It is similar to an Issuer, however it is cluster-scoped and therefore can be referenced by resources that exist in *any* namespace, not just the same namespace as the referent."

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
    * [`obj spec.acme.solvers`](#obj-specacmesolvers)
      * [`obj spec.acme.solvers.dns01`](#obj-specacmesolversdns01)
        * [`fn withCnameStrategy(cnameStrategy)`](#fn-specacmesolversdns01withcnamestrategy)
        * [`obj spec.acme.solvers.dns01.acmedns`](#obj-specacmesolversdns01acmedns)
          * [`fn withHost(host)`](#fn-specacmesolversdns01acmednswithhost)
          * [`obj spec.acme.solvers.dns01.acmedns.accountSecretRef`](#obj-specacmesolversdns01acmednsaccountsecretref)
            * [`fn withKey(key)`](#fn-specacmesolversdns01acmednsaccountsecretrefwithkey)
            * [`fn withName(name)`](#fn-specacmesolversdns01acmednsaccountsecretrefwithname)
        * [`obj spec.acme.solvers.dns01.akamai`](#obj-specacmesolversdns01akamai)
          * [`fn withServiceConsumerDomain(serviceConsumerDomain)`](#fn-specacmesolversdns01akamaiwithserviceconsumerdomain)
          * [`obj spec.acme.solvers.dns01.akamai.accessTokenSecretRef`](#obj-specacmesolversdns01akamaiaccesstokensecretref)
            * [`fn withKey(key)`](#fn-specacmesolversdns01akamaiaccesstokensecretrefwithkey)
            * [`fn withName(name)`](#fn-specacmesolversdns01akamaiaccesstokensecretrefwithname)
          * [`obj spec.acme.solvers.dns01.akamai.clientSecretSecretRef`](#obj-specacmesolversdns01akamaiclientsecretsecretref)
            * [`fn withKey(key)`](#fn-specacmesolversdns01akamaiclientsecretsecretrefwithkey)
            * [`fn withName(name)`](#fn-specacmesolversdns01akamaiclientsecretsecretrefwithname)
          * [`obj spec.acme.solvers.dns01.akamai.clientTokenSecretRef`](#obj-specacmesolversdns01akamaiclienttokensecretref)
            * [`fn withKey(key)`](#fn-specacmesolversdns01akamaiclienttokensecretrefwithkey)
            * [`fn withName(name)`](#fn-specacmesolversdns01akamaiclienttokensecretrefwithname)
        * [`obj spec.acme.solvers.dns01.azuredns`](#obj-specacmesolversdns01azuredns)
          * [`fn withClientID(clientID)`](#fn-specacmesolversdns01azurednswithclientid)
          * [`fn withEnvironment(environment)`](#fn-specacmesolversdns01azurednswithenvironment)
          * [`fn withHostedZoneName(hostedZoneName)`](#fn-specacmesolversdns01azurednswithhostedzonename)
          * [`fn withResourceGroupName(resourceGroupName)`](#fn-specacmesolversdns01azurednswithresourcegroupname)
          * [`fn withSubscriptionID(subscriptionID)`](#fn-specacmesolversdns01azurednswithsubscriptionid)
          * [`fn withTenantID(tenantID)`](#fn-specacmesolversdns01azurednswithtenantid)
          * [`obj spec.acme.solvers.dns01.azuredns.clientSecretSecretRef`](#obj-specacmesolversdns01azurednsclientsecretsecretref)
            * [`fn withKey(key)`](#fn-specacmesolversdns01azurednsclientsecretsecretrefwithkey)
            * [`fn withName(name)`](#fn-specacmesolversdns01azurednsclientsecretsecretrefwithname)
          * [`obj spec.acme.solvers.dns01.azuredns.managedIdentity`](#obj-specacmesolversdns01azurednsmanagedidentity)
            * [`fn withClientID(clientID)`](#fn-specacmesolversdns01azurednsmanagedidentitywithclientid)
            * [`fn withResourceID(resourceID)`](#fn-specacmesolversdns01azurednsmanagedidentitywithresourceid)
        * [`obj spec.acme.solvers.dns01.clouddns`](#obj-specacmesolversdns01clouddns)
          * [`fn withHostedZoneName(hostedZoneName)`](#fn-specacmesolversdns01clouddnswithhostedzonename)
          * [`fn withProject(project)`](#fn-specacmesolversdns01clouddnswithproject)
          * [`obj spec.acme.solvers.dns01.clouddns.serviceAccountSecretRef`](#obj-specacmesolversdns01clouddnsserviceaccountsecretref)
            * [`fn withKey(key)`](#fn-specacmesolversdns01clouddnsserviceaccountsecretrefwithkey)
            * [`fn withName(name)`](#fn-specacmesolversdns01clouddnsserviceaccountsecretrefwithname)
        * [`obj spec.acme.solvers.dns01.cloudflare`](#obj-specacmesolversdns01cloudflare)
          * [`fn withEmail(email)`](#fn-specacmesolversdns01cloudflarewithemail)
          * [`obj spec.acme.solvers.dns01.cloudflare.apiKeySecretRef`](#obj-specacmesolversdns01cloudflareapikeysecretref)
            * [`fn withKey(key)`](#fn-specacmesolversdns01cloudflareapikeysecretrefwithkey)
            * [`fn withName(name)`](#fn-specacmesolversdns01cloudflareapikeysecretrefwithname)
          * [`obj spec.acme.solvers.dns01.cloudflare.apiTokenSecretRef`](#obj-specacmesolversdns01cloudflareapitokensecretref)
            * [`fn withKey(key)`](#fn-specacmesolversdns01cloudflareapitokensecretrefwithkey)
            * [`fn withName(name)`](#fn-specacmesolversdns01cloudflareapitokensecretrefwithname)
        * [`obj spec.acme.solvers.dns01.digitalocean`](#obj-specacmesolversdns01digitalocean)
          * [`obj spec.acme.solvers.dns01.digitalocean.tokenSecretRef`](#obj-specacmesolversdns01digitaloceantokensecretref)
            * [`fn withKey(key)`](#fn-specacmesolversdns01digitaloceantokensecretrefwithkey)
            * [`fn withName(name)`](#fn-specacmesolversdns01digitaloceantokensecretrefwithname)
        * [`obj spec.acme.solvers.dns01.rfc2136`](#obj-specacmesolversdns01rfc2136)
          * [`fn withNameserver(nameserver)`](#fn-specacmesolversdns01rfc2136withnameserver)
          * [`fn withTsigAlgorithm(tsigAlgorithm)`](#fn-specacmesolversdns01rfc2136withtsigalgorithm)
          * [`fn withTsigKeyName(tsigKeyName)`](#fn-specacmesolversdns01rfc2136withtsigkeyname)
          * [`obj spec.acme.solvers.dns01.rfc2136.tsigSecretSecretRef`](#obj-specacmesolversdns01rfc2136tsigsecretsecretref)
            * [`fn withKey(key)`](#fn-specacmesolversdns01rfc2136tsigsecretsecretrefwithkey)
            * [`fn withName(name)`](#fn-specacmesolversdns01rfc2136tsigsecretsecretrefwithname)
        * [`obj spec.acme.solvers.dns01.route53`](#obj-specacmesolversdns01route53)
          * [`fn withAccessKeyID(accessKeyID)`](#fn-specacmesolversdns01route53withaccesskeyid)
          * [`fn withHostedZoneID(hostedZoneID)`](#fn-specacmesolversdns01route53withhostedzoneid)
          * [`fn withRegion(region)`](#fn-specacmesolversdns01route53withregion)
          * [`fn withRole(role)`](#fn-specacmesolversdns01route53withrole)
          * [`obj spec.acme.solvers.dns01.route53.secretAccessKeySecretRef`](#obj-specacmesolversdns01route53secretaccesskeysecretref)
            * [`fn withKey(key)`](#fn-specacmesolversdns01route53secretaccesskeysecretrefwithkey)
            * [`fn withName(name)`](#fn-specacmesolversdns01route53secretaccesskeysecretrefwithname)
        * [`obj spec.acme.solvers.dns01.webhook`](#obj-specacmesolversdns01webhook)
          * [`fn withConfig(config)`](#fn-specacmesolversdns01webhookwithconfig)
          * [`fn withGroupName(groupName)`](#fn-specacmesolversdns01webhookwithgroupname)
          * [`fn withSolverName(solverName)`](#fn-specacmesolversdns01webhookwithsolvername)
      * [`obj spec.acme.solvers.http01`](#obj-specacmesolvershttp01)
        * [`obj spec.acme.solvers.http01.gatewayHTTPRoute`](#obj-specacmesolvershttp01gatewayhttproute)
          * [`fn withLabels(labels)`](#fn-specacmesolvershttp01gatewayhttproutewithlabels)
          * [`fn withLabelsMixin(labels)`](#fn-specacmesolvershttp01gatewayhttproutewithlabelsmixin)
          * [`fn withServiceType(serviceType)`](#fn-specacmesolvershttp01gatewayhttproutewithservicetype)
        * [`obj spec.acme.solvers.http01.ingress`](#obj-specacmesolvershttp01ingress)
          * [`fn withClass(class)`](#fn-specacmesolvershttp01ingresswithclass)
          * [`fn withName(name)`](#fn-specacmesolvershttp01ingresswithname)
          * [`fn withServiceType(serviceType)`](#fn-specacmesolvershttp01ingresswithservicetype)
          * [`obj spec.acme.solvers.http01.ingress.ingressTemplate`](#obj-specacmesolvershttp01ingressingresstemplate)
            * [`obj spec.acme.solvers.http01.ingress.ingressTemplate.metadata`](#obj-specacmesolvershttp01ingressingresstemplatemetadata)
              * [`fn withAnnotations(annotations)`](#fn-specacmesolvershttp01ingressingresstemplatemetadatawithannotations)
              * [`fn withAnnotationsMixin(annotations)`](#fn-specacmesolvershttp01ingressingresstemplatemetadatawithannotationsmixin)
              * [`fn withLabels(labels)`](#fn-specacmesolvershttp01ingressingresstemplatemetadatawithlabels)
              * [`fn withLabelsMixin(labels)`](#fn-specacmesolvershttp01ingressingresstemplatemetadatawithlabelsmixin)
          * [`obj spec.acme.solvers.http01.ingress.podTemplate`](#obj-specacmesolvershttp01ingresspodtemplate)
            * [`obj spec.acme.solvers.http01.ingress.podTemplate.metadata`](#obj-specacmesolvershttp01ingresspodtemplatemetadata)
              * [`fn withAnnotations(annotations)`](#fn-specacmesolvershttp01ingresspodtemplatemetadatawithannotations)
              * [`fn withAnnotationsMixin(annotations)`](#fn-specacmesolvershttp01ingresspodtemplatemetadatawithannotationsmixin)
              * [`fn withLabels(labels)`](#fn-specacmesolvershttp01ingresspodtemplatemetadatawithlabels)
              * [`fn withLabelsMixin(labels)`](#fn-specacmesolvershttp01ingresspodtemplatemetadatawithlabelsmixin)
            * [`obj spec.acme.solvers.http01.ingress.podTemplate.spec`](#obj-specacmesolvershttp01ingresspodtemplatespec)
              * [`fn withNodeSelector(nodeSelector)`](#fn-specacmesolvershttp01ingresspodtemplatespecwithnodeselector)
              * [`fn withNodeSelectorMixin(nodeSelector)`](#fn-specacmesolvershttp01ingresspodtemplatespecwithnodeselectormixin)
              * [`fn withPriorityClassName(priorityClassName)`](#fn-specacmesolvershttp01ingresspodtemplatespecwithpriorityclassname)
              * [`fn withServiceAccountName(serviceAccountName)`](#fn-specacmesolvershttp01ingresspodtemplatespecwithserviceaccountname)
              * [`fn withTolerations(tolerations)`](#fn-specacmesolvershttp01ingresspodtemplatespecwithtolerations)
              * [`fn withTolerationsMixin(tolerations)`](#fn-specacmesolvershttp01ingresspodtemplatespecwithtolerationsmixin)
              * [`obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity`](#obj-specacmesolvershttp01ingresspodtemplatespecaffinity)
                * [`obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity`](#obj-specacmesolvershttp01ingresspodtemplatespecaffinitynodeaffinity)
                  * [`fn withPreferredDuringSchedulingIgnoredDuringExecution(preferredDuringSchedulingIgnoredDuringExecution)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitynodeaffinitywithpreferredduringschedulingignoredduringexecution)
                  * [`fn withPreferredDuringSchedulingIgnoredDuringExecutionMixin(preferredDuringSchedulingIgnoredDuringExecution)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitynodeaffinitywithpreferredduringschedulingignoredduringexecutionmixin)
                  * [`obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution`](#obj-specacmesolvershttp01ingresspodtemplatespecaffinitynodeaffinitypreferredduringschedulingignoredduringexecution)
                    * [`fn withWeight(weight)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitynodeaffinitypreferredduringschedulingignoredduringexecutionwithweight)
                    * [`obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution.preference`](#obj-specacmesolvershttp01ingresspodtemplatespecaffinitynodeaffinitypreferredduringschedulingignoredduringexecutionpreference)
                      * [`fn withMatchExpressions(matchExpressions)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitynodeaffinitypreferredduringschedulingignoredduringexecutionpreferencewithmatchexpressions)
                      * [`fn withMatchExpressionsMixin(matchExpressions)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitynodeaffinitypreferredduringschedulingignoredduringexecutionpreferencewithmatchexpressionsmixin)
                      * [`fn withMatchFields(matchFields)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitynodeaffinitypreferredduringschedulingignoredduringexecutionpreferencewithmatchfields)
                      * [`fn withMatchFieldsMixin(matchFields)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitynodeaffinitypreferredduringschedulingignoredduringexecutionpreferencewithmatchfieldsmixin)
                      * [`obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution.preference.matchExpressions`](#obj-specacmesolvershttp01ingresspodtemplatespecaffinitynodeaffinitypreferredduringschedulingignoredduringexecutionpreferencematchexpressions)
                        * [`fn withKey(key)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitynodeaffinitypreferredduringschedulingignoredduringexecutionpreferencematchexpressionswithkey)
                        * [`fn withOperator(operator)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitynodeaffinitypreferredduringschedulingignoredduringexecutionpreferencematchexpressionswithoperator)
                        * [`fn withValues(values)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitynodeaffinitypreferredduringschedulingignoredduringexecutionpreferencematchexpressionswithvalues)
                        * [`fn withValuesMixin(values)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitynodeaffinitypreferredduringschedulingignoredduringexecutionpreferencematchexpressionswithvaluesmixin)
                      * [`obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution.preference.matchFields`](#obj-specacmesolvershttp01ingresspodtemplatespecaffinitynodeaffinitypreferredduringschedulingignoredduringexecutionpreferencematchfields)
                        * [`fn withKey(key)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitynodeaffinitypreferredduringschedulingignoredduringexecutionpreferencematchfieldswithkey)
                        * [`fn withOperator(operator)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitynodeaffinitypreferredduringschedulingignoredduringexecutionpreferencematchfieldswithoperator)
                        * [`fn withValues(values)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitynodeaffinitypreferredduringschedulingignoredduringexecutionpreferencematchfieldswithvalues)
                        * [`fn withValuesMixin(values)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitynodeaffinitypreferredduringschedulingignoredduringexecutionpreferencematchfieldswithvaluesmixin)
                  * [`obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution`](#obj-specacmesolvershttp01ingresspodtemplatespecaffinitynodeaffinityrequiredduringschedulingignoredduringexecution)
                    * [`fn withNodeSelectorTerms(nodeSelectorTerms)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitynodeaffinityrequiredduringschedulingignoredduringexecutionwithnodeselectorterms)
                    * [`fn withNodeSelectorTermsMixin(nodeSelectorTerms)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitynodeaffinityrequiredduringschedulingignoredduringexecutionwithnodeselectortermsmixin)
                    * [`obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.nodeSelectorTerms`](#obj-specacmesolvershttp01ingresspodtemplatespecaffinitynodeaffinityrequiredduringschedulingignoredduringexecutionnodeselectorterms)
                      * [`fn withMatchExpressions(matchExpressions)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitynodeaffinityrequiredduringschedulingignoredduringexecutionnodeselectortermswithmatchexpressions)
                      * [`fn withMatchExpressionsMixin(matchExpressions)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitynodeaffinityrequiredduringschedulingignoredduringexecutionnodeselectortermswithmatchexpressionsmixin)
                      * [`fn withMatchFields(matchFields)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitynodeaffinityrequiredduringschedulingignoredduringexecutionnodeselectortermswithmatchfields)
                      * [`fn withMatchFieldsMixin(matchFields)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitynodeaffinityrequiredduringschedulingignoredduringexecutionnodeselectortermswithmatchfieldsmixin)
                      * [`obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.nodeSelectorTerms.matchExpressions`](#obj-specacmesolvershttp01ingresspodtemplatespecaffinitynodeaffinityrequiredduringschedulingignoredduringexecutionnodeselectortermsmatchexpressions)
                        * [`fn withKey(key)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitynodeaffinityrequiredduringschedulingignoredduringexecutionnodeselectortermsmatchexpressionswithkey)
                        * [`fn withOperator(operator)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitynodeaffinityrequiredduringschedulingignoredduringexecutionnodeselectortermsmatchexpressionswithoperator)
                        * [`fn withValues(values)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitynodeaffinityrequiredduringschedulingignoredduringexecutionnodeselectortermsmatchexpressionswithvalues)
                        * [`fn withValuesMixin(values)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitynodeaffinityrequiredduringschedulingignoredduringexecutionnodeselectortermsmatchexpressionswithvaluesmixin)
                      * [`obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.nodeSelectorTerms.matchFields`](#obj-specacmesolvershttp01ingresspodtemplatespecaffinitynodeaffinityrequiredduringschedulingignoredduringexecutionnodeselectortermsmatchfields)
                        * [`fn withKey(key)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitynodeaffinityrequiredduringschedulingignoredduringexecutionnodeselectortermsmatchfieldswithkey)
                        * [`fn withOperator(operator)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitynodeaffinityrequiredduringschedulingignoredduringexecutionnodeselectortermsmatchfieldswithoperator)
                        * [`fn withValues(values)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitynodeaffinityrequiredduringschedulingignoredduringexecutionnodeselectortermsmatchfieldswithvalues)
                        * [`fn withValuesMixin(values)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitynodeaffinityrequiredduringschedulingignoredduringexecutionnodeselectortermsmatchfieldswithvaluesmixin)
                * [`obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity`](#obj-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinity)
                  * [`fn withPreferredDuringSchedulingIgnoredDuringExecution(preferredDuringSchedulingIgnoredDuringExecution)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinitywithpreferredduringschedulingignoredduringexecution)
                  * [`fn withPreferredDuringSchedulingIgnoredDuringExecutionMixin(preferredDuringSchedulingIgnoredDuringExecution)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinitywithpreferredduringschedulingignoredduringexecutionmixin)
                  * [`fn withRequiredDuringSchedulingIgnoredDuringExecution(requiredDuringSchedulingIgnoredDuringExecution)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinitywithrequiredduringschedulingignoredduringexecution)
                  * [`fn withRequiredDuringSchedulingIgnoredDuringExecutionMixin(requiredDuringSchedulingIgnoredDuringExecution)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinitywithrequiredduringschedulingignoredduringexecutionmixin)
                  * [`obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution`](#obj-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecution)
                    * [`fn withWeight(weight)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionwithweight)
                    * [`obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm`](#obj-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinityterm)
                      * [`fn withNamespaces(namespaces)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermwithnamespaces)
                      * [`fn withNamespacesMixin(namespaces)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermwithnamespacesmixin)
                      * [`fn withTopologyKey(topologyKey)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermwithtopologykey)
                      * [`obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector`](#obj-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermlabelselector)
                        * [`fn withMatchExpressions(matchExpressions)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermlabelselectorwithmatchexpressions)
                        * [`fn withMatchExpressionsMixin(matchExpressions)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermlabelselectorwithmatchexpressionsmixin)
                        * [`fn withMatchLabels(matchLabels)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermlabelselectorwithmatchlabels)
                        * [`fn withMatchLabelsMixin(matchLabels)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermlabelselectorwithmatchlabelsmixin)
                        * [`obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.matchExpressions`](#obj-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermlabelselectormatchexpressions)
                          * [`fn withKey(key)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermlabelselectormatchexpressionswithkey)
                          * [`fn withOperator(operator)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermlabelselectormatchexpressionswithoperator)
                          * [`fn withValues(values)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermlabelselectormatchexpressionswithvalues)
                          * [`fn withValuesMixin(values)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermlabelselectormatchexpressionswithvaluesmixin)
                      * [`obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector`](#obj-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermnamespaceselector)
                        * [`fn withMatchExpressions(matchExpressions)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermnamespaceselectorwithmatchexpressions)
                        * [`fn withMatchExpressionsMixin(matchExpressions)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermnamespaceselectorwithmatchexpressionsmixin)
                        * [`fn withMatchLabels(matchLabels)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermnamespaceselectorwithmatchlabels)
                        * [`fn withMatchLabelsMixin(matchLabels)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermnamespaceselectorwithmatchlabelsmixin)
                        * [`obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.matchExpressions`](#obj-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermnamespaceselectormatchexpressions)
                          * [`fn withKey(key)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermnamespaceselectormatchexpressionswithkey)
                          * [`fn withOperator(operator)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermnamespaceselectormatchexpressionswithoperator)
                          * [`fn withValues(values)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermnamespaceselectormatchexpressionswithvalues)
                          * [`fn withValuesMixin(values)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermnamespaceselectormatchexpressionswithvaluesmixin)
                  * [`obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution`](#obj-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecution)
                    * [`fn withNamespaces(namespaces)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionwithnamespaces)
                    * [`fn withNamespacesMixin(namespaces)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionwithnamespacesmixin)
                    * [`fn withTopologyKey(topologyKey)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionwithtopologykey)
                    * [`obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector`](#obj-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionlabelselector)
                      * [`fn withMatchExpressions(matchExpressions)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionlabelselectorwithmatchexpressions)
                      * [`fn withMatchExpressionsMixin(matchExpressions)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionlabelselectorwithmatchexpressionsmixin)
                      * [`fn withMatchLabels(matchLabels)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionlabelselectorwithmatchlabels)
                      * [`fn withMatchLabelsMixin(matchLabels)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionlabelselectorwithmatchlabelsmixin)
                      * [`obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.matchExpressions`](#obj-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionlabelselectormatchexpressions)
                        * [`fn withKey(key)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionlabelselectormatchexpressionswithkey)
                        * [`fn withOperator(operator)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionlabelselectormatchexpressionswithoperator)
                        * [`fn withValues(values)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionlabelselectormatchexpressionswithvalues)
                        * [`fn withValuesMixin(values)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionlabelselectormatchexpressionswithvaluesmixin)
                    * [`obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector`](#obj-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionnamespaceselector)
                      * [`fn withMatchExpressions(matchExpressions)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionnamespaceselectorwithmatchexpressions)
                      * [`fn withMatchExpressionsMixin(matchExpressions)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionnamespaceselectorwithmatchexpressionsmixin)
                      * [`fn withMatchLabels(matchLabels)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionnamespaceselectorwithmatchlabels)
                      * [`fn withMatchLabelsMixin(matchLabels)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionnamespaceselectorwithmatchlabelsmixin)
                      * [`obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.matchExpressions`](#obj-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionnamespaceselectormatchexpressions)
                        * [`fn withKey(key)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionnamespaceselectormatchexpressionswithkey)
                        * [`fn withOperator(operator)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionnamespaceselectormatchexpressionswithoperator)
                        * [`fn withValues(values)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionnamespaceselectormatchexpressionswithvalues)
                        * [`fn withValuesMixin(values)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionnamespaceselectormatchexpressionswithvaluesmixin)
                * [`obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity`](#obj-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinity)
                  * [`fn withPreferredDuringSchedulingIgnoredDuringExecution(preferredDuringSchedulingIgnoredDuringExecution)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinitywithpreferredduringschedulingignoredduringexecution)
                  * [`fn withPreferredDuringSchedulingIgnoredDuringExecutionMixin(preferredDuringSchedulingIgnoredDuringExecution)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinitywithpreferredduringschedulingignoredduringexecutionmixin)
                  * [`fn withRequiredDuringSchedulingIgnoredDuringExecution(requiredDuringSchedulingIgnoredDuringExecution)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinitywithrequiredduringschedulingignoredduringexecution)
                  * [`fn withRequiredDuringSchedulingIgnoredDuringExecutionMixin(requiredDuringSchedulingIgnoredDuringExecution)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinitywithrequiredduringschedulingignoredduringexecutionmixin)
                  * [`obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution`](#obj-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecution)
                    * [`fn withWeight(weight)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionwithweight)
                    * [`obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm`](#obj-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinityterm)
                      * [`fn withNamespaces(namespaces)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermwithnamespaces)
                      * [`fn withNamespacesMixin(namespaces)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermwithnamespacesmixin)
                      * [`fn withTopologyKey(topologyKey)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermwithtopologykey)
                      * [`obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector`](#obj-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermlabelselector)
                        * [`fn withMatchExpressions(matchExpressions)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermlabelselectorwithmatchexpressions)
                        * [`fn withMatchExpressionsMixin(matchExpressions)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermlabelselectorwithmatchexpressionsmixin)
                        * [`fn withMatchLabels(matchLabels)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermlabelselectorwithmatchlabels)
                        * [`fn withMatchLabelsMixin(matchLabels)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermlabelselectorwithmatchlabelsmixin)
                        * [`obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.matchExpressions`](#obj-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermlabelselectormatchexpressions)
                          * [`fn withKey(key)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermlabelselectormatchexpressionswithkey)
                          * [`fn withOperator(operator)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermlabelselectormatchexpressionswithoperator)
                          * [`fn withValues(values)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermlabelselectormatchexpressionswithvalues)
                          * [`fn withValuesMixin(values)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermlabelselectormatchexpressionswithvaluesmixin)
                      * [`obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector`](#obj-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermnamespaceselector)
                        * [`fn withMatchExpressions(matchExpressions)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermnamespaceselectorwithmatchexpressions)
                        * [`fn withMatchExpressionsMixin(matchExpressions)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermnamespaceselectorwithmatchexpressionsmixin)
                        * [`fn withMatchLabels(matchLabels)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermnamespaceselectorwithmatchlabels)
                        * [`fn withMatchLabelsMixin(matchLabels)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermnamespaceselectorwithmatchlabelsmixin)
                        * [`obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.matchExpressions`](#obj-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermnamespaceselectormatchexpressions)
                          * [`fn withKey(key)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermnamespaceselectormatchexpressionswithkey)
                          * [`fn withOperator(operator)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermnamespaceselectormatchexpressionswithoperator)
                          * [`fn withValues(values)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermnamespaceselectormatchexpressionswithvalues)
                          * [`fn withValuesMixin(values)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermnamespaceselectormatchexpressionswithvaluesmixin)
                  * [`obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution`](#obj-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecution)
                    * [`fn withNamespaces(namespaces)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionwithnamespaces)
                    * [`fn withNamespacesMixin(namespaces)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionwithnamespacesmixin)
                    * [`fn withTopologyKey(topologyKey)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionwithtopologykey)
                    * [`obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector`](#obj-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionlabelselector)
                      * [`fn withMatchExpressions(matchExpressions)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionlabelselectorwithmatchexpressions)
                      * [`fn withMatchExpressionsMixin(matchExpressions)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionlabelselectorwithmatchexpressionsmixin)
                      * [`fn withMatchLabels(matchLabels)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionlabelselectorwithmatchlabels)
                      * [`fn withMatchLabelsMixin(matchLabels)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionlabelselectorwithmatchlabelsmixin)
                      * [`obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.matchExpressions`](#obj-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionlabelselectormatchexpressions)
                        * [`fn withKey(key)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionlabelselectormatchexpressionswithkey)
                        * [`fn withOperator(operator)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionlabelselectormatchexpressionswithoperator)
                        * [`fn withValues(values)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionlabelselectormatchexpressionswithvalues)
                        * [`fn withValuesMixin(values)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionlabelselectormatchexpressionswithvaluesmixin)
                    * [`obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector`](#obj-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionnamespaceselector)
                      * [`fn withMatchExpressions(matchExpressions)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionnamespaceselectorwithmatchexpressions)
                      * [`fn withMatchExpressionsMixin(matchExpressions)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionnamespaceselectorwithmatchexpressionsmixin)
                      * [`fn withMatchLabels(matchLabels)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionnamespaceselectorwithmatchlabels)
                      * [`fn withMatchLabelsMixin(matchLabels)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionnamespaceselectorwithmatchlabelsmixin)
                      * [`obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.matchExpressions`](#obj-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionnamespaceselectormatchexpressions)
                        * [`fn withKey(key)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionnamespaceselectormatchexpressionswithkey)
                        * [`fn withOperator(operator)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionnamespaceselectormatchexpressionswithoperator)
                        * [`fn withValues(values)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionnamespaceselectormatchexpressionswithvalues)
                        * [`fn withValuesMixin(values)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionnamespaceselectormatchexpressionswithvaluesmixin)
              * [`obj spec.acme.solvers.http01.ingress.podTemplate.spec.tolerations`](#obj-specacmesolvershttp01ingresspodtemplatespectolerations)
                * [`fn withEffect(effect)`](#fn-specacmesolvershttp01ingresspodtemplatespectolerationswitheffect)
                * [`fn withKey(key)`](#fn-specacmesolvershttp01ingresspodtemplatespectolerationswithkey)
                * [`fn withOperator(operator)`](#fn-specacmesolvershttp01ingresspodtemplatespectolerationswithoperator)
                * [`fn withTolerationSeconds(tolerationSeconds)`](#fn-specacmesolvershttp01ingresspodtemplatespectolerationswithtolerationseconds)
                * [`fn withValue(value)`](#fn-specacmesolvershttp01ingresspodtemplatespectolerationswithvalue)
      * [`obj spec.acme.solvers.selector`](#obj-specacmesolversselector)
        * [`fn withDnsNames(dnsNames)`](#fn-specacmesolversselectorwithdnsnames)
        * [`fn withDnsNamesMixin(dnsNames)`](#fn-specacmesolversselectorwithdnsnamesmixin)
        * [`fn withDnsZones(dnsZones)`](#fn-specacmesolversselectorwithdnszones)
        * [`fn withDnsZonesMixin(dnsZones)`](#fn-specacmesolversselectorwithdnszonesmixin)
        * [`fn withMatchLabels(matchLabels)`](#fn-specacmesolversselectorwithmatchlabels)
        * [`fn withMatchLabelsMixin(matchLabels)`](#fn-specacmesolversselectorwithmatchlabelsmixin)
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

new returns an instance of ClusterIssuer

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

"Desired state of the ClusterIssuer resource."

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

## obj spec.acme.solvers

"Solvers is a list of challenge solvers that will be used to solve ACME challenges for the matching domains. Solver configurations must be provided in order to obtain certificates from an ACME server. For more information, see: https://cert-manager.io/docs/configuration/acme/"

## obj spec.acme.solvers.dns01

"Configures cert-manager to attempt to complete authorizations by performing the DNS01 challenge flow."

### fn spec.acme.solvers.dns01.withCnameStrategy

```ts
withCnameStrategy(cnameStrategy)
```

"CNAMEStrategy configures how the DNS01 provider should handle CNAME records when found in DNS zones."

## obj spec.acme.solvers.dns01.acmedns

"Use the 'ACME DNS' (https://github.com/joohoi/acme-dns) API to manage DNS01 challenge records."

### fn spec.acme.solvers.dns01.acmedns.withHost

```ts
withHost(host)
```



## obj spec.acme.solvers.dns01.acmedns.accountSecretRef

"A reference to a specific 'key' within a Secret resource. In some instances, `key` is a required field."

### fn spec.acme.solvers.dns01.acmedns.accountSecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used. Some instances of this field may be defaulted, in others it may be required."

### fn spec.acme.solvers.dns01.acmedns.accountSecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.acme.solvers.dns01.akamai

"Use the Akamai DNS zone management API to manage DNS01 challenge records."

### fn spec.acme.solvers.dns01.akamai.withServiceConsumerDomain

```ts
withServiceConsumerDomain(serviceConsumerDomain)
```



## obj spec.acme.solvers.dns01.akamai.accessTokenSecretRef

"A reference to a specific 'key' within a Secret resource. In some instances, `key` is a required field."

### fn spec.acme.solvers.dns01.akamai.accessTokenSecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used. Some instances of this field may be defaulted, in others it may be required."

### fn spec.acme.solvers.dns01.akamai.accessTokenSecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.acme.solvers.dns01.akamai.clientSecretSecretRef

"A reference to a specific 'key' within a Secret resource. In some instances, `key` is a required field."

### fn spec.acme.solvers.dns01.akamai.clientSecretSecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used. Some instances of this field may be defaulted, in others it may be required."

### fn spec.acme.solvers.dns01.akamai.clientSecretSecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.acme.solvers.dns01.akamai.clientTokenSecretRef

"A reference to a specific 'key' within a Secret resource. In some instances, `key` is a required field."

### fn spec.acme.solvers.dns01.akamai.clientTokenSecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used. Some instances of this field may be defaulted, in others it may be required."

### fn spec.acme.solvers.dns01.akamai.clientTokenSecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.acme.solvers.dns01.azuredns

"Use the Microsoft Azure DNS API to manage DNS01 challenge records."

### fn spec.acme.solvers.dns01.azuredns.withClientID

```ts
withClientID(clientID)
```

"if both this and ClientSecret are left unset MSI will be used"

### fn spec.acme.solvers.dns01.azuredns.withEnvironment

```ts
withEnvironment(environment)
```

"name of the Azure environment (default AzurePublicCloud)"

### fn spec.acme.solvers.dns01.azuredns.withHostedZoneName

```ts
withHostedZoneName(hostedZoneName)
```

"name of the DNS zone that should be used"

### fn spec.acme.solvers.dns01.azuredns.withResourceGroupName

```ts
withResourceGroupName(resourceGroupName)
```

"resource group the DNS zone is located in"

### fn spec.acme.solvers.dns01.azuredns.withSubscriptionID

```ts
withSubscriptionID(subscriptionID)
```

"ID of the Azure subscription"

### fn spec.acme.solvers.dns01.azuredns.withTenantID

```ts
withTenantID(tenantID)
```

"when specifying ClientID and ClientSecret then this field is also needed"

## obj spec.acme.solvers.dns01.azuredns.clientSecretSecretRef

"if both this and ClientID are left unset MSI will be used"

### fn spec.acme.solvers.dns01.azuredns.clientSecretSecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used. Some instances of this field may be defaulted, in others it may be required."

### fn spec.acme.solvers.dns01.azuredns.clientSecretSecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.acme.solvers.dns01.azuredns.managedIdentity

"managed identity configuration, can not be used at the same time as clientID, clientSecretSecretRef or tenantID"

### fn spec.acme.solvers.dns01.azuredns.managedIdentity.withClientID

```ts
withClientID(clientID)
```

"client ID of the managed identity, can not be used at the same time as resourceID"

### fn spec.acme.solvers.dns01.azuredns.managedIdentity.withResourceID

```ts
withResourceID(resourceID)
```

"resource ID of the managed identity, can not be used at the same time as clientID"

## obj spec.acme.solvers.dns01.clouddns

"Use the Google Cloud DNS API to manage DNS01 challenge records."

### fn spec.acme.solvers.dns01.clouddns.withHostedZoneName

```ts
withHostedZoneName(hostedZoneName)
```

"HostedZoneName is an optional field that tells cert-manager in which Cloud DNS zone the challenge record has to be created. If left empty cert-manager will automatically choose a zone."

### fn spec.acme.solvers.dns01.clouddns.withProject

```ts
withProject(project)
```



## obj spec.acme.solvers.dns01.clouddns.serviceAccountSecretRef

"A reference to a specific 'key' within a Secret resource. In some instances, `key` is a required field."

### fn spec.acme.solvers.dns01.clouddns.serviceAccountSecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used. Some instances of this field may be defaulted, in others it may be required."

### fn spec.acme.solvers.dns01.clouddns.serviceAccountSecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.acme.solvers.dns01.cloudflare

"Use the Cloudflare API to manage DNS01 challenge records."

### fn spec.acme.solvers.dns01.cloudflare.withEmail

```ts
withEmail(email)
```

"Email of the account, only required when using API key based authentication."

## obj spec.acme.solvers.dns01.cloudflare.apiKeySecretRef

"API key to use to authenticate with Cloudflare. Note: using an API token to authenticate is now the recommended method as it allows greater control of permissions."

### fn spec.acme.solvers.dns01.cloudflare.apiKeySecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used. Some instances of this field may be defaulted, in others it may be required."

### fn spec.acme.solvers.dns01.cloudflare.apiKeySecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.acme.solvers.dns01.cloudflare.apiTokenSecretRef

"API token used to authenticate with Cloudflare."

### fn spec.acme.solvers.dns01.cloudflare.apiTokenSecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used. Some instances of this field may be defaulted, in others it may be required."

### fn spec.acme.solvers.dns01.cloudflare.apiTokenSecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.acme.solvers.dns01.digitalocean

"Use the DigitalOcean DNS API to manage DNS01 challenge records."

## obj spec.acme.solvers.dns01.digitalocean.tokenSecretRef

"A reference to a specific 'key' within a Secret resource. In some instances, `key` is a required field."

### fn spec.acme.solvers.dns01.digitalocean.tokenSecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used. Some instances of this field may be defaulted, in others it may be required."

### fn spec.acme.solvers.dns01.digitalocean.tokenSecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.acme.solvers.dns01.rfc2136

"Use RFC2136 (\"Dynamic Updates in the Domain Name System\") (https://datatracker.ietf.org/doc/rfc2136/) to manage DNS01 challenge records."

### fn spec.acme.solvers.dns01.rfc2136.withNameserver

```ts
withNameserver(nameserver)
```

"The IP address or hostname of an authoritative DNS server supporting RFC2136 in the form host:port. If the host is an IPv6 address it must be enclosed in square brackets (e.g [2001:db8::1])\u00a0; port is optional. This field is required."

### fn spec.acme.solvers.dns01.rfc2136.withTsigAlgorithm

```ts
withTsigAlgorithm(tsigAlgorithm)
```

"The TSIG Algorithm configured in the DNS supporting RFC2136. Used only when ``tsigSecretSecretRef`` and ``tsigKeyName`` are defined. Supported values are (case-insensitive): ``HMACMD5`` (default), ``HMACSHA1``, ``HMACSHA256`` or ``HMACSHA512``."

### fn spec.acme.solvers.dns01.rfc2136.withTsigKeyName

```ts
withTsigKeyName(tsigKeyName)
```

"The TSIG Key name configured in the DNS. If ``tsigSecretSecretRef`` is defined, this field is required."

## obj spec.acme.solvers.dns01.rfc2136.tsigSecretSecretRef

"The name of the secret containing the TSIG value. If ``tsigKeyName`` is defined, this field is required."

### fn spec.acme.solvers.dns01.rfc2136.tsigSecretSecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used. Some instances of this field may be defaulted, in others it may be required."

### fn spec.acme.solvers.dns01.rfc2136.tsigSecretSecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.acme.solvers.dns01.route53

"Use the AWS Route53 API to manage DNS01 challenge records."

### fn spec.acme.solvers.dns01.route53.withAccessKeyID

```ts
withAccessKeyID(accessKeyID)
```

"The AccessKeyID is used for authentication. If not set we fall-back to using env vars, shared credentials file or AWS Instance metadata see: https://docs.aws.amazon.com/sdk-for-go/v1/developer-guide/configuring-sdk.html#specifying-credentials"

### fn spec.acme.solvers.dns01.route53.withHostedZoneID

```ts
withHostedZoneID(hostedZoneID)
```

"If set, the provider will manage only this zone in Route53 and will not do an lookup using the route53:ListHostedZonesByName api call."

### fn spec.acme.solvers.dns01.route53.withRegion

```ts
withRegion(region)
```

"Always set the region when using AccessKeyID and SecretAccessKey"

### fn spec.acme.solvers.dns01.route53.withRole

```ts
withRole(role)
```

"Role is a Role ARN which the Route53 provider will assume using either the explicit credentials AccessKeyID/SecretAccessKey or the inferred credentials from environment variables, shared credentials file or AWS Instance metadata"

## obj spec.acme.solvers.dns01.route53.secretAccessKeySecretRef

"The SecretAccessKey is used for authentication. If not set we fall-back to using env vars, shared credentials file or AWS Instance metadata https://docs.aws.amazon.com/sdk-for-go/v1/developer-guide/configuring-sdk.html#specifying-credentials"

### fn spec.acme.solvers.dns01.route53.secretAccessKeySecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used. Some instances of this field may be defaulted, in others it may be required."

### fn spec.acme.solvers.dns01.route53.secretAccessKeySecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.acme.solvers.dns01.webhook

"Configure an external webhook based DNS01 challenge solver to manage DNS01 challenge records."

### fn spec.acme.solvers.dns01.webhook.withConfig

```ts
withConfig(config)
```

"Additional configuration that should be passed to the webhook apiserver when challenges are processed. This can contain arbitrary JSON data. Secret values should not be specified in this stanza. If secret values are needed (e.g. credentials for a DNS service), you should use a SecretKeySelector to reference a Secret resource. For details on the schema of this field, consult the webhook provider implementation's documentation."

### fn spec.acme.solvers.dns01.webhook.withGroupName

```ts
withGroupName(groupName)
```

"The API group name that should be used when POSTing ChallengePayload resources to the webhook apiserver. This should be the same as the GroupName specified in the webhook provider implementation."

### fn spec.acme.solvers.dns01.webhook.withSolverName

```ts
withSolverName(solverName)
```

"The name of the solver to use, as defined in the webhook provider implementation. This will typically be the name of the provider, e.g. 'cloudflare'."

## obj spec.acme.solvers.http01

"Configures cert-manager to attempt to complete authorizations by performing the HTTP01 challenge flow. It is not possible to obtain certificates for wildcard domain names (e.g. `*.example.com`) using the HTTP01 challenge mechanism."

## obj spec.acme.solvers.http01.gatewayHTTPRoute

"The Gateway API is a sig-network community API that models service networking in Kubernetes (https://gateway-api.sigs.k8s.io/). The Gateway solver will create HTTPRoutes with the specified labels in the same namespace as the challenge. This solver is experimental, and fields / behaviour may change in the future."

### fn spec.acme.solvers.http01.gatewayHTTPRoute.withLabels

```ts
withLabels(labels)
```

"The labels that cert-manager will use when creating the temporary HTTPRoute needed for solving the HTTP-01 challenge. These labels must match the label selector of at least one Gateway."

### fn spec.acme.solvers.http01.gatewayHTTPRoute.withLabelsMixin

```ts
withLabelsMixin(labels)
```

"The labels that cert-manager will use when creating the temporary HTTPRoute needed for solving the HTTP-01 challenge. These labels must match the label selector of at least one Gateway."

**Note:** This function appends passed data to existing values

### fn spec.acme.solvers.http01.gatewayHTTPRoute.withServiceType

```ts
withServiceType(serviceType)
```

"Optional service type for Kubernetes solver service. Supported values are NodePort or ClusterIP. If unset, defaults to NodePort."

## obj spec.acme.solvers.http01.ingress

"The ingress based HTTP01 challenge solver will solve challenges by creating or modifying Ingress resources in order to route requests for '/.well-known/acme-challenge/XYZ' to 'challenge solver' pods that are provisioned by cert-manager for each Challenge to be completed."

### fn spec.acme.solvers.http01.ingress.withClass

```ts
withClass(class)
```

"The ingress class to use when creating Ingress resources to solve ACME challenges that use this challenge solver. Only one of 'class' or 'name' may be specified."

### fn spec.acme.solvers.http01.ingress.withName

```ts
withName(name)
```

"The name of the ingress resource that should have ACME challenge solving routes inserted into it in order to solve HTTP01 challenges. This is typically used in conjunction with ingress controllers like ingress-gce, which maintains a 1:1 mapping between external IPs and ingress resources."

### fn spec.acme.solvers.http01.ingress.withServiceType

```ts
withServiceType(serviceType)
```

"Optional service type for Kubernetes solver service. Supported values are NodePort or ClusterIP. If unset, defaults to NodePort."

## obj spec.acme.solvers.http01.ingress.ingressTemplate

"Optional ingress template used to configure the ACME challenge solver ingress used for HTTP01 challenges"

## obj spec.acme.solvers.http01.ingress.ingressTemplate.metadata

"ObjectMeta overrides for the ingress used to solve HTTP01 challenges. Only the 'labels' and 'annotations' fields may be set. If labels or annotations overlap with in-built values, the values here will override the in-built values."

### fn spec.acme.solvers.http01.ingress.ingressTemplate.metadata.withAnnotations

```ts
withAnnotations(annotations)
```

"Annotations that should be added to the created ACME HTTP01 solver ingress."

### fn spec.acme.solvers.http01.ingress.ingressTemplate.metadata.withAnnotationsMixin

```ts
withAnnotationsMixin(annotations)
```

"Annotations that should be added to the created ACME HTTP01 solver ingress."

**Note:** This function appends passed data to existing values

### fn spec.acme.solvers.http01.ingress.ingressTemplate.metadata.withLabels

```ts
withLabels(labels)
```

"Labels that should be added to the created ACME HTTP01 solver ingress."

### fn spec.acme.solvers.http01.ingress.ingressTemplate.metadata.withLabelsMixin

```ts
withLabelsMixin(labels)
```

"Labels that should be added to the created ACME HTTP01 solver ingress."

**Note:** This function appends passed data to existing values

## obj spec.acme.solvers.http01.ingress.podTemplate

"Optional pod template used to configure the ACME challenge solver pods used for HTTP01 challenges."

## obj spec.acme.solvers.http01.ingress.podTemplate.metadata

"ObjectMeta overrides for the pod used to solve HTTP01 challenges. Only the 'labels' and 'annotations' fields may be set. If labels or annotations overlap with in-built values, the values here will override the in-built values."

### fn spec.acme.solvers.http01.ingress.podTemplate.metadata.withAnnotations

```ts
withAnnotations(annotations)
```

"Annotations that should be added to the create ACME HTTP01 solver pods."

### fn spec.acme.solvers.http01.ingress.podTemplate.metadata.withAnnotationsMixin

```ts
withAnnotationsMixin(annotations)
```

"Annotations that should be added to the create ACME HTTP01 solver pods."

**Note:** This function appends passed data to existing values

### fn spec.acme.solvers.http01.ingress.podTemplate.metadata.withLabels

```ts
withLabels(labels)
```

"Labels that should be added to the created ACME HTTP01 solver pods."

### fn spec.acme.solvers.http01.ingress.podTemplate.metadata.withLabelsMixin

```ts
withLabelsMixin(labels)
```

"Labels that should be added to the created ACME HTTP01 solver pods."

**Note:** This function appends passed data to existing values

## obj spec.acme.solvers.http01.ingress.podTemplate.spec

"PodSpec defines overrides for the HTTP01 challenge solver pod. Only the 'priorityClassName', 'nodeSelector', 'affinity', 'serviceAccountName' and 'tolerations' fields are supported currently. All other fields will be ignored."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.withNodeSelector

```ts
withNodeSelector(nodeSelector)
```

"NodeSelector is a selector which must be true for the pod to fit on a node. Selector which must match a node's labels for the pod to be scheduled on that node. More info: https://kubernetes.io/docs/concepts/configuration/assign-pod-node/"

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.withNodeSelectorMixin

```ts
withNodeSelectorMixin(nodeSelector)
```

"NodeSelector is a selector which must be true for the pod to fit on a node. Selector which must match a node's labels for the pod to be scheduled on that node. More info: https://kubernetes.io/docs/concepts/configuration/assign-pod-node/"

**Note:** This function appends passed data to existing values

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.withPriorityClassName

```ts
withPriorityClassName(priorityClassName)
```

"If specified, the pod's priorityClassName."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.withServiceAccountName

```ts
withServiceAccountName(serviceAccountName)
```

"If specified, the pod's service account"

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.withTolerations

```ts
withTolerations(tolerations)
```

"If specified, the pod's tolerations."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.withTolerationsMixin

```ts
withTolerationsMixin(tolerations)
```

"If specified, the pod's tolerations."

**Note:** This function appends passed data to existing values

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity

"If specified, the pod's scheduling constraints"

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity

"Describes node affinity scheduling rules for the pod."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.withPreferredDuringSchedulingIgnoredDuringExecution

```ts
withPreferredDuringSchedulingIgnoredDuringExecution(preferredDuringSchedulingIgnoredDuringExecution)
```

"The scheduler will prefer to schedule pods to nodes that satisfy the affinity expressions specified by this field, but it may choose a node that violates one or more of the expressions. The node that is most preferred is the one with the greatest sum of weights, i.e. for each node that meets all of the scheduling requirements (resource request, requiredDuringScheduling affinity expressions, etc.), compute a sum by iterating through the elements of this field and adding \"weight\" to the sum if the node matches the corresponding matchExpressions; the node(s) with the highest sum are the most preferred."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.withPreferredDuringSchedulingIgnoredDuringExecutionMixin

```ts
withPreferredDuringSchedulingIgnoredDuringExecutionMixin(preferredDuringSchedulingIgnoredDuringExecution)
```

"The scheduler will prefer to schedule pods to nodes that satisfy the affinity expressions specified by this field, but it may choose a node that violates one or more of the expressions. The node that is most preferred is the one with the greatest sum of weights, i.e. for each node that meets all of the scheduling requirements (resource request, requiredDuringScheduling affinity expressions, etc.), compute a sum by iterating through the elements of this field and adding \"weight\" to the sum if the node matches the corresponding matchExpressions; the node(s) with the highest sum are the most preferred."

**Note:** This function appends passed data to existing values

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution

"The scheduler will prefer to schedule pods to nodes that satisfy the affinity expressions specified by this field, but it may choose a node that violates one or more of the expressions. The node that is most preferred is the one with the greatest sum of weights, i.e. for each node that meets all of the scheduling requirements (resource request, requiredDuringScheduling affinity expressions, etc.), compute a sum by iterating through the elements of this field and adding \"weight\" to the sum if the node matches the corresponding matchExpressions; the node(s) with the highest sum are the most preferred."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution.withWeight

```ts
withWeight(weight)
```

"Weight associated with matching the corresponding nodeSelectorTerm, in the range 1-100."

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution.preference

"A node selector term, associated with the corresponding weight."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution.preference.withMatchExpressions

```ts
withMatchExpressions(matchExpressions)
```

"A list of node selector requirements by node's labels."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution.preference.withMatchExpressionsMixin

```ts
withMatchExpressionsMixin(matchExpressions)
```

"A list of node selector requirements by node's labels."

**Note:** This function appends passed data to existing values

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution.preference.withMatchFields

```ts
withMatchFields(matchFields)
```

"A list of node selector requirements by node's fields."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution.preference.withMatchFieldsMixin

```ts
withMatchFieldsMixin(matchFields)
```

"A list of node selector requirements by node's fields."

**Note:** This function appends passed data to existing values

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution.preference.matchExpressions

"A list of node selector requirements by node's labels."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution.preference.matchExpressions.withKey

```ts
withKey(key)
```

"The label key that the selector applies to."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution.preference.matchExpressions.withOperator

```ts
withOperator(operator)
```

"Represents a key's relationship to a set of values. Valid operators are In, NotIn, Exists, DoesNotExist. Gt, and Lt."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution.preference.matchExpressions.withValues

```ts
withValues(values)
```

"An array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. If the operator is Gt or Lt, the values array must have a single element, which will be interpreted as an integer. This array is replaced during a strategic merge patch."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution.preference.matchExpressions.withValuesMixin

```ts
withValuesMixin(values)
```

"An array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. If the operator is Gt or Lt, the values array must have a single element, which will be interpreted as an integer. This array is replaced during a strategic merge patch."

**Note:** This function appends passed data to existing values

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution.preference.matchFields

"A list of node selector requirements by node's fields."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution.preference.matchFields.withKey

```ts
withKey(key)
```

"The label key that the selector applies to."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution.preference.matchFields.withOperator

```ts
withOperator(operator)
```

"Represents a key's relationship to a set of values. Valid operators are In, NotIn, Exists, DoesNotExist. Gt, and Lt."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution.preference.matchFields.withValues

```ts
withValues(values)
```

"An array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. If the operator is Gt or Lt, the values array must have a single element, which will be interpreted as an integer. This array is replaced during a strategic merge patch."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution.preference.matchFields.withValuesMixin

```ts
withValuesMixin(values)
```

"An array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. If the operator is Gt or Lt, the values array must have a single element, which will be interpreted as an integer. This array is replaced during a strategic merge patch."

**Note:** This function appends passed data to existing values

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution

"If the affinity requirements specified by this field are not met at scheduling time, the pod will not be scheduled onto the node. If the affinity requirements specified by this field cease to be met at some point during pod execution (e.g. due to an update), the system may or may not try to eventually evict the pod from its node."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.withNodeSelectorTerms

```ts
withNodeSelectorTerms(nodeSelectorTerms)
```

"Required. A list of node selector terms. The terms are ORed."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.withNodeSelectorTermsMixin

```ts
withNodeSelectorTermsMixin(nodeSelectorTerms)
```

"Required. A list of node selector terms. The terms are ORed."

**Note:** This function appends passed data to existing values

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.nodeSelectorTerms

"Required. A list of node selector terms. The terms are ORed."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.nodeSelectorTerms.withMatchExpressions

```ts
withMatchExpressions(matchExpressions)
```

"A list of node selector requirements by node's labels."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.nodeSelectorTerms.withMatchExpressionsMixin

```ts
withMatchExpressionsMixin(matchExpressions)
```

"A list of node selector requirements by node's labels."

**Note:** This function appends passed data to existing values

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.nodeSelectorTerms.withMatchFields

```ts
withMatchFields(matchFields)
```

"A list of node selector requirements by node's fields."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.nodeSelectorTerms.withMatchFieldsMixin

```ts
withMatchFieldsMixin(matchFields)
```

"A list of node selector requirements by node's fields."

**Note:** This function appends passed data to existing values

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.nodeSelectorTerms.matchExpressions

"A list of node selector requirements by node's labels."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.nodeSelectorTerms.matchExpressions.withKey

```ts
withKey(key)
```

"The label key that the selector applies to."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.nodeSelectorTerms.matchExpressions.withOperator

```ts
withOperator(operator)
```

"Represents a key's relationship to a set of values. Valid operators are In, NotIn, Exists, DoesNotExist. Gt, and Lt."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.nodeSelectorTerms.matchExpressions.withValues

```ts
withValues(values)
```

"An array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. If the operator is Gt or Lt, the values array must have a single element, which will be interpreted as an integer. This array is replaced during a strategic merge patch."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.nodeSelectorTerms.matchExpressions.withValuesMixin

```ts
withValuesMixin(values)
```

"An array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. If the operator is Gt or Lt, the values array must have a single element, which will be interpreted as an integer. This array is replaced during a strategic merge patch."

**Note:** This function appends passed data to existing values

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.nodeSelectorTerms.matchFields

"A list of node selector requirements by node's fields."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.nodeSelectorTerms.matchFields.withKey

```ts
withKey(key)
```

"The label key that the selector applies to."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.nodeSelectorTerms.matchFields.withOperator

```ts
withOperator(operator)
```

"Represents a key's relationship to a set of values. Valid operators are In, NotIn, Exists, DoesNotExist. Gt, and Lt."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.nodeSelectorTerms.matchFields.withValues

```ts
withValues(values)
```

"An array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. If the operator is Gt or Lt, the values array must have a single element, which will be interpreted as an integer. This array is replaced during a strategic merge patch."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.nodeSelectorTerms.matchFields.withValuesMixin

```ts
withValuesMixin(values)
```

"An array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. If the operator is Gt or Lt, the values array must have a single element, which will be interpreted as an integer. This array is replaced during a strategic merge patch."

**Note:** This function appends passed data to existing values

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity

"Describes pod affinity scheduling rules (e.g. co-locate this pod in the same node, zone, etc. as some other pod(s))."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.withPreferredDuringSchedulingIgnoredDuringExecution

```ts
withPreferredDuringSchedulingIgnoredDuringExecution(preferredDuringSchedulingIgnoredDuringExecution)
```

"The scheduler will prefer to schedule pods to nodes that satisfy the affinity expressions specified by this field, but it may choose a node that violates one or more of the expressions. The node that is most preferred is the one with the greatest sum of weights, i.e. for each node that meets all of the scheduling requirements (resource request, requiredDuringScheduling affinity expressions, etc.), compute a sum by iterating through the elements of this field and adding \"weight\" to the sum if the node has pods which matches the corresponding podAffinityTerm; the node(s) with the highest sum are the most preferred."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.withPreferredDuringSchedulingIgnoredDuringExecutionMixin

```ts
withPreferredDuringSchedulingIgnoredDuringExecutionMixin(preferredDuringSchedulingIgnoredDuringExecution)
```

"The scheduler will prefer to schedule pods to nodes that satisfy the affinity expressions specified by this field, but it may choose a node that violates one or more of the expressions. The node that is most preferred is the one with the greatest sum of weights, i.e. for each node that meets all of the scheduling requirements (resource request, requiredDuringScheduling affinity expressions, etc.), compute a sum by iterating through the elements of this field and adding \"weight\" to the sum if the node has pods which matches the corresponding podAffinityTerm; the node(s) with the highest sum are the most preferred."

**Note:** This function appends passed data to existing values

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.withRequiredDuringSchedulingIgnoredDuringExecution

```ts
withRequiredDuringSchedulingIgnoredDuringExecution(requiredDuringSchedulingIgnoredDuringExecution)
```

"If the affinity requirements specified by this field are not met at scheduling time, the pod will not be scheduled onto the node. If the affinity requirements specified by this field cease to be met at some point during pod execution (e.g. due to a pod label update), the system may or may not try to eventually evict the pod from its node. When there are multiple elements, the lists of nodes corresponding to each podAffinityTerm are intersected, i.e. all terms must be satisfied."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.withRequiredDuringSchedulingIgnoredDuringExecutionMixin

```ts
withRequiredDuringSchedulingIgnoredDuringExecutionMixin(requiredDuringSchedulingIgnoredDuringExecution)
```

"If the affinity requirements specified by this field are not met at scheduling time, the pod will not be scheduled onto the node. If the affinity requirements specified by this field cease to be met at some point during pod execution (e.g. due to a pod label update), the system may or may not try to eventually evict the pod from its node. When there are multiple elements, the lists of nodes corresponding to each podAffinityTerm are intersected, i.e. all terms must be satisfied."

**Note:** This function appends passed data to existing values

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution

"The scheduler will prefer to schedule pods to nodes that satisfy the affinity expressions specified by this field, but it may choose a node that violates one or more of the expressions. The node that is most preferred is the one with the greatest sum of weights, i.e. for each node that meets all of the scheduling requirements (resource request, requiredDuringScheduling affinity expressions, etc.), compute a sum by iterating through the elements of this field and adding \"weight\" to the sum if the node has pods which matches the corresponding podAffinityTerm; the node(s) with the highest sum are the most preferred."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.withWeight

```ts
withWeight(weight)
```

"weight associated with matching the corresponding podAffinityTerm, in the range 1-100."

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm

"Required. A pod affinity term, associated with the corresponding weight."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.withNamespaces

```ts
withNamespaces(namespaces)
```

"namespaces specifies a static list of namespace names that the term applies to. The term is applied to the union of the namespaces listed in this field and the ones selected by namespaceSelector. null or empty namespaces list and null namespaceSelector means \"this pod's namespace\

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.withNamespacesMixin

```ts
withNamespacesMixin(namespaces)
```

"namespaces specifies a static list of namespace names that the term applies to. The term is applied to the union of the namespaces listed in this field and the ones selected by namespaceSelector. null or empty namespaces list and null namespaceSelector means \"this pod's namespace\

**Note:** This function appends passed data to existing values

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.withTopologyKey

```ts
withTopologyKey(topologyKey)
```

"This pod should be co-located (affinity) or not co-located (anti-affinity) with the pods matching the labelSelector in the specified namespaces, where co-located is defined as running on a node whose value of the label with key topologyKey matches that of any node on which any of the selected pods is running. Empty topologyKey is not allowed."

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector

"A label query over a set of resources, in this case pods."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.withMatchExpressions

```ts
withMatchExpressions(matchExpressions)
```

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.withMatchExpressionsMixin

```ts
withMatchExpressionsMixin(matchExpressions)
```

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

**Note:** This function appends passed data to existing values

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.withMatchLabels

```ts
withMatchLabels(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels map is equivalent to an element of matchExpressions, whose key field is \"key\", the operator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels map is equivalent to an element of matchExpressions, whose key field is \"key\", the operator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

**Note:** This function appends passed data to existing values

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.matchExpressions

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.matchExpressions.withKey

```ts
withKey(key)
```

"key is the label key that the selector applies to."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.matchExpressions.withOperator

```ts
withOperator(operator)
```

"operator represents a key's relationship to a set of values. Valid operators are In, NotIn, Exists and DoesNotExist."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.matchExpressions.withValues

```ts
withValues(values)
```

"values is an array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. This array is replaced during a strategic merge patch."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.matchExpressions.withValuesMixin

```ts
withValuesMixin(values)
```

"values is an array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. This array is replaced during a strategic merge patch."

**Note:** This function appends passed data to existing values

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector

"A label query over the set of namespaces that the term applies to. The term is applied to the union of the namespaces selected by this field and the ones listed in the namespaces field. null selector and null or empty namespaces list means \"this pod's namespace\". An empty selector ({}) matches all namespaces. This field is beta-level and is only honored when PodAffinityNamespaceSelector feature is enabled."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.withMatchExpressions

```ts
withMatchExpressions(matchExpressions)
```

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.withMatchExpressionsMixin

```ts
withMatchExpressionsMixin(matchExpressions)
```

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

**Note:** This function appends passed data to existing values

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.withMatchLabels

```ts
withMatchLabels(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels map is equivalent to an element of matchExpressions, whose key field is \"key\", the operator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels map is equivalent to an element of matchExpressions, whose key field is \"key\", the operator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

**Note:** This function appends passed data to existing values

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.matchExpressions

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.matchExpressions.withKey

```ts
withKey(key)
```

"key is the label key that the selector applies to."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.matchExpressions.withOperator

```ts
withOperator(operator)
```

"operator represents a key's relationship to a set of values. Valid operators are In, NotIn, Exists and DoesNotExist."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.matchExpressions.withValues

```ts
withValues(values)
```

"values is an array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. This array is replaced during a strategic merge patch."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.matchExpressions.withValuesMixin

```ts
withValuesMixin(values)
```

"values is an array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. This array is replaced during a strategic merge patch."

**Note:** This function appends passed data to existing values

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution

"If the affinity requirements specified by this field are not met at scheduling time, the pod will not be scheduled onto the node. If the affinity requirements specified by this field cease to be met at some point during pod execution (e.g. due to a pod label update), the system may or may not try to eventually evict the pod from its node. When there are multiple elements, the lists of nodes corresponding to each podAffinityTerm are intersected, i.e. all terms must be satisfied."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.withNamespaces

```ts
withNamespaces(namespaces)
```

"namespaces specifies a static list of namespace names that the term applies to. The term is applied to the union of the namespaces listed in this field and the ones selected by namespaceSelector. null or empty namespaces list and null namespaceSelector means \"this pod's namespace\

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.withNamespacesMixin

```ts
withNamespacesMixin(namespaces)
```

"namespaces specifies a static list of namespace names that the term applies to. The term is applied to the union of the namespaces listed in this field and the ones selected by namespaceSelector. null or empty namespaces list and null namespaceSelector means \"this pod's namespace\

**Note:** This function appends passed data to existing values

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.withTopologyKey

```ts
withTopologyKey(topologyKey)
```

"This pod should be co-located (affinity) or not co-located (anti-affinity) with the pods matching the labelSelector in the specified namespaces, where co-located is defined as running on a node whose value of the label with key topologyKey matches that of any node on which any of the selected pods is running. Empty topologyKey is not allowed."

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector

"A label query over a set of resources, in this case pods."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.withMatchExpressions

```ts
withMatchExpressions(matchExpressions)
```

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.withMatchExpressionsMixin

```ts
withMatchExpressionsMixin(matchExpressions)
```

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

**Note:** This function appends passed data to existing values

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.withMatchLabels

```ts
withMatchLabels(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels map is equivalent to an element of matchExpressions, whose key field is \"key\", the operator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels map is equivalent to an element of matchExpressions, whose key field is \"key\", the operator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

**Note:** This function appends passed data to existing values

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.matchExpressions

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.matchExpressions.withKey

```ts
withKey(key)
```

"key is the label key that the selector applies to."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.matchExpressions.withOperator

```ts
withOperator(operator)
```

"operator represents a key's relationship to a set of values. Valid operators are In, NotIn, Exists and DoesNotExist."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.matchExpressions.withValues

```ts
withValues(values)
```

"values is an array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. This array is replaced during a strategic merge patch."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.matchExpressions.withValuesMixin

```ts
withValuesMixin(values)
```

"values is an array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. This array is replaced during a strategic merge patch."

**Note:** This function appends passed data to existing values

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector

"A label query over the set of namespaces that the term applies to. The term is applied to the union of the namespaces selected by this field and the ones listed in the namespaces field. null selector and null or empty namespaces list means \"this pod's namespace\". An empty selector ({}) matches all namespaces. This field is beta-level and is only honored when PodAffinityNamespaceSelector feature is enabled."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.withMatchExpressions

```ts
withMatchExpressions(matchExpressions)
```

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.withMatchExpressionsMixin

```ts
withMatchExpressionsMixin(matchExpressions)
```

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

**Note:** This function appends passed data to existing values

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.withMatchLabels

```ts
withMatchLabels(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels map is equivalent to an element of matchExpressions, whose key field is \"key\", the operator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels map is equivalent to an element of matchExpressions, whose key field is \"key\", the operator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

**Note:** This function appends passed data to existing values

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.matchExpressions

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.matchExpressions.withKey

```ts
withKey(key)
```

"key is the label key that the selector applies to."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.matchExpressions.withOperator

```ts
withOperator(operator)
```

"operator represents a key's relationship to a set of values. Valid operators are In, NotIn, Exists and DoesNotExist."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.matchExpressions.withValues

```ts
withValues(values)
```

"values is an array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. This array is replaced during a strategic merge patch."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.matchExpressions.withValuesMixin

```ts
withValuesMixin(values)
```

"values is an array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. This array is replaced during a strategic merge patch."

**Note:** This function appends passed data to existing values

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity

"Describes pod anti-affinity scheduling rules (e.g. avoid putting this pod in the same node, zone, etc. as some other pod(s))."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.withPreferredDuringSchedulingIgnoredDuringExecution

```ts
withPreferredDuringSchedulingIgnoredDuringExecution(preferredDuringSchedulingIgnoredDuringExecution)
```

"The scheduler will prefer to schedule pods to nodes that satisfy the anti-affinity expressions specified by this field, but it may choose a node that violates one or more of the expressions. The node that is most preferred is the one with the greatest sum of weights, i.e. for each node that meets all of the scheduling requirements (resource request, requiredDuringScheduling anti-affinity expressions, etc.), compute a sum by iterating through the elements of this field and adding \"weight\" to the sum if the node has pods which matches the corresponding podAffinityTerm; the node(s) with the highest sum are the most preferred."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.withPreferredDuringSchedulingIgnoredDuringExecutionMixin

```ts
withPreferredDuringSchedulingIgnoredDuringExecutionMixin(preferredDuringSchedulingIgnoredDuringExecution)
```

"The scheduler will prefer to schedule pods to nodes that satisfy the anti-affinity expressions specified by this field, but it may choose a node that violates one or more of the expressions. The node that is most preferred is the one with the greatest sum of weights, i.e. for each node that meets all of the scheduling requirements (resource request, requiredDuringScheduling anti-affinity expressions, etc.), compute a sum by iterating through the elements of this field and adding \"weight\" to the sum if the node has pods which matches the corresponding podAffinityTerm; the node(s) with the highest sum are the most preferred."

**Note:** This function appends passed data to existing values

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.withRequiredDuringSchedulingIgnoredDuringExecution

```ts
withRequiredDuringSchedulingIgnoredDuringExecution(requiredDuringSchedulingIgnoredDuringExecution)
```

"If the anti-affinity requirements specified by this field are not met at scheduling time, the pod will not be scheduled onto the node. If the anti-affinity requirements specified by this field cease to be met at some point during pod execution (e.g. due to a pod label update), the system may or may not try to eventually evict the pod from its node. When there are multiple elements, the lists of nodes corresponding to each podAffinityTerm are intersected, i.e. all terms must be satisfied."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.withRequiredDuringSchedulingIgnoredDuringExecutionMixin

```ts
withRequiredDuringSchedulingIgnoredDuringExecutionMixin(requiredDuringSchedulingIgnoredDuringExecution)
```

"If the anti-affinity requirements specified by this field are not met at scheduling time, the pod will not be scheduled onto the node. If the anti-affinity requirements specified by this field cease to be met at some point during pod execution (e.g. due to a pod label update), the system may or may not try to eventually evict the pod from its node. When there are multiple elements, the lists of nodes corresponding to each podAffinityTerm are intersected, i.e. all terms must be satisfied."

**Note:** This function appends passed data to existing values

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution

"The scheduler will prefer to schedule pods to nodes that satisfy the anti-affinity expressions specified by this field, but it may choose a node that violates one or more of the expressions. The node that is most preferred is the one with the greatest sum of weights, i.e. for each node that meets all of the scheduling requirements (resource request, requiredDuringScheduling anti-affinity expressions, etc.), compute a sum by iterating through the elements of this field and adding \"weight\" to the sum if the node has pods which matches the corresponding podAffinityTerm; the node(s) with the highest sum are the most preferred."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.withWeight

```ts
withWeight(weight)
```

"weight associated with matching the corresponding podAffinityTerm, in the range 1-100."

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm

"Required. A pod affinity term, associated with the corresponding weight."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.withNamespaces

```ts
withNamespaces(namespaces)
```

"namespaces specifies a static list of namespace names that the term applies to. The term is applied to the union of the namespaces listed in this field and the ones selected by namespaceSelector. null or empty namespaces list and null namespaceSelector means \"this pod's namespace\

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.withNamespacesMixin

```ts
withNamespacesMixin(namespaces)
```

"namespaces specifies a static list of namespace names that the term applies to. The term is applied to the union of the namespaces listed in this field and the ones selected by namespaceSelector. null or empty namespaces list and null namespaceSelector means \"this pod's namespace\

**Note:** This function appends passed data to existing values

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.withTopologyKey

```ts
withTopologyKey(topologyKey)
```

"This pod should be co-located (affinity) or not co-located (anti-affinity) with the pods matching the labelSelector in the specified namespaces, where co-located is defined as running on a node whose value of the label with key topologyKey matches that of any node on which any of the selected pods is running. Empty topologyKey is not allowed."

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector

"A label query over a set of resources, in this case pods."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.withMatchExpressions

```ts
withMatchExpressions(matchExpressions)
```

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.withMatchExpressionsMixin

```ts
withMatchExpressionsMixin(matchExpressions)
```

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

**Note:** This function appends passed data to existing values

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.withMatchLabels

```ts
withMatchLabels(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels map is equivalent to an element of matchExpressions, whose key field is \"key\", the operator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels map is equivalent to an element of matchExpressions, whose key field is \"key\", the operator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

**Note:** This function appends passed data to existing values

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.matchExpressions

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.matchExpressions.withKey

```ts
withKey(key)
```

"key is the label key that the selector applies to."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.matchExpressions.withOperator

```ts
withOperator(operator)
```

"operator represents a key's relationship to a set of values. Valid operators are In, NotIn, Exists and DoesNotExist."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.matchExpressions.withValues

```ts
withValues(values)
```

"values is an array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. This array is replaced during a strategic merge patch."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.matchExpressions.withValuesMixin

```ts
withValuesMixin(values)
```

"values is an array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. This array is replaced during a strategic merge patch."

**Note:** This function appends passed data to existing values

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector

"A label query over the set of namespaces that the term applies to. The term is applied to the union of the namespaces selected by this field and the ones listed in the namespaces field. null selector and null or empty namespaces list means \"this pod's namespace\". An empty selector ({}) matches all namespaces. This field is beta-level and is only honored when PodAffinityNamespaceSelector feature is enabled."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.withMatchExpressions

```ts
withMatchExpressions(matchExpressions)
```

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.withMatchExpressionsMixin

```ts
withMatchExpressionsMixin(matchExpressions)
```

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

**Note:** This function appends passed data to existing values

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.withMatchLabels

```ts
withMatchLabels(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels map is equivalent to an element of matchExpressions, whose key field is \"key\", the operator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels map is equivalent to an element of matchExpressions, whose key field is \"key\", the operator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

**Note:** This function appends passed data to existing values

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.matchExpressions

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.matchExpressions.withKey

```ts
withKey(key)
```

"key is the label key that the selector applies to."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.matchExpressions.withOperator

```ts
withOperator(operator)
```

"operator represents a key's relationship to a set of values. Valid operators are In, NotIn, Exists and DoesNotExist."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.matchExpressions.withValues

```ts
withValues(values)
```

"values is an array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. This array is replaced during a strategic merge patch."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.matchExpressions.withValuesMixin

```ts
withValuesMixin(values)
```

"values is an array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. This array is replaced during a strategic merge patch."

**Note:** This function appends passed data to existing values

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution

"If the anti-affinity requirements specified by this field are not met at scheduling time, the pod will not be scheduled onto the node. If the anti-affinity requirements specified by this field cease to be met at some point during pod execution (e.g. due to a pod label update), the system may or may not try to eventually evict the pod from its node. When there are multiple elements, the lists of nodes corresponding to each podAffinityTerm are intersected, i.e. all terms must be satisfied."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.withNamespaces

```ts
withNamespaces(namespaces)
```

"namespaces specifies a static list of namespace names that the term applies to. The term is applied to the union of the namespaces listed in this field and the ones selected by namespaceSelector. null or empty namespaces list and null namespaceSelector means \"this pod's namespace\

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.withNamespacesMixin

```ts
withNamespacesMixin(namespaces)
```

"namespaces specifies a static list of namespace names that the term applies to. The term is applied to the union of the namespaces listed in this field and the ones selected by namespaceSelector. null or empty namespaces list and null namespaceSelector means \"this pod's namespace\

**Note:** This function appends passed data to existing values

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.withTopologyKey

```ts
withTopologyKey(topologyKey)
```

"This pod should be co-located (affinity) or not co-located (anti-affinity) with the pods matching the labelSelector in the specified namespaces, where co-located is defined as running on a node whose value of the label with key topologyKey matches that of any node on which any of the selected pods is running. Empty topologyKey is not allowed."

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector

"A label query over a set of resources, in this case pods."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.withMatchExpressions

```ts
withMatchExpressions(matchExpressions)
```

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.withMatchExpressionsMixin

```ts
withMatchExpressionsMixin(matchExpressions)
```

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

**Note:** This function appends passed data to existing values

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.withMatchLabels

```ts
withMatchLabels(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels map is equivalent to an element of matchExpressions, whose key field is \"key\", the operator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels map is equivalent to an element of matchExpressions, whose key field is \"key\", the operator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

**Note:** This function appends passed data to existing values

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.matchExpressions

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.matchExpressions.withKey

```ts
withKey(key)
```

"key is the label key that the selector applies to."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.matchExpressions.withOperator

```ts
withOperator(operator)
```

"operator represents a key's relationship to a set of values. Valid operators are In, NotIn, Exists and DoesNotExist."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.matchExpressions.withValues

```ts
withValues(values)
```

"values is an array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. This array is replaced during a strategic merge patch."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.matchExpressions.withValuesMixin

```ts
withValuesMixin(values)
```

"values is an array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. This array is replaced during a strategic merge patch."

**Note:** This function appends passed data to existing values

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector

"A label query over the set of namespaces that the term applies to. The term is applied to the union of the namespaces selected by this field and the ones listed in the namespaces field. null selector and null or empty namespaces list means \"this pod's namespace\". An empty selector ({}) matches all namespaces. This field is beta-level and is only honored when PodAffinityNamespaceSelector feature is enabled."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.withMatchExpressions

```ts
withMatchExpressions(matchExpressions)
```

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.withMatchExpressionsMixin

```ts
withMatchExpressionsMixin(matchExpressions)
```

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

**Note:** This function appends passed data to existing values

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.withMatchLabels

```ts
withMatchLabels(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels map is equivalent to an element of matchExpressions, whose key field is \"key\", the operator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels map is equivalent to an element of matchExpressions, whose key field is \"key\", the operator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

**Note:** This function appends passed data to existing values

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.matchExpressions

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.matchExpressions.withKey

```ts
withKey(key)
```

"key is the label key that the selector applies to."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.matchExpressions.withOperator

```ts
withOperator(operator)
```

"operator represents a key's relationship to a set of values. Valid operators are In, NotIn, Exists and DoesNotExist."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.matchExpressions.withValues

```ts
withValues(values)
```

"values is an array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. This array is replaced during a strategic merge patch."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.matchExpressions.withValuesMixin

```ts
withValuesMixin(values)
```

"values is an array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. This array is replaced during a strategic merge patch."

**Note:** This function appends passed data to existing values

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.tolerations

"If specified, the pod's tolerations."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.tolerations.withEffect

```ts
withEffect(effect)
```

"Effect indicates the taint effect to match. Empty means match all taint effects. When specified, allowed values are NoSchedule, PreferNoSchedule and NoExecute."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.tolerations.withKey

```ts
withKey(key)
```

"Key is the taint key that the toleration applies to. Empty means match all taint keys. If the key is empty, operator must be Exists; this combination means to match all values and all keys."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.tolerations.withOperator

```ts
withOperator(operator)
```

"Operator represents a key's relationship to the value. Valid operators are Exists and Equal. Defaults to Equal. Exists is equivalent to wildcard for value, so that a pod can tolerate all taints of a particular category."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.tolerations.withTolerationSeconds

```ts
withTolerationSeconds(tolerationSeconds)
```

"TolerationSeconds represents the period of time the toleration (which must be of effect NoExecute, otherwise this field is ignored) tolerates the taint. By default, it is not set, which means tolerate the taint forever (do not evict). Zero and negative values will be treated as 0 (evict immediately) by the system."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.tolerations.withValue

```ts
withValue(value)
```

"Value is the taint value the toleration matches to. If the operator is Exists, the value should be empty, otherwise just a regular string."

## obj spec.acme.solvers.selector

"Selector selects a set of DNSNames on the Certificate resource that should be solved using this challenge solver. If not specified, the solver will be treated as the 'default' solver with the lowest priority, i.e. if any other solver has a more specific match, it will be used instead."

### fn spec.acme.solvers.selector.withDnsNames

```ts
withDnsNames(dnsNames)
```

"List of DNSNames that this solver will be used to solve. If specified and a match is found, a dnsNames selector will take precedence over a dnsZones selector. If multiple solvers match with the same dnsNames value, the solver with the most matching labels in matchLabels will be selected. If neither has more matches, the solver defined earlier in the list will be selected."

### fn spec.acme.solvers.selector.withDnsNamesMixin

```ts
withDnsNamesMixin(dnsNames)
```

"List of DNSNames that this solver will be used to solve. If specified and a match is found, a dnsNames selector will take precedence over a dnsZones selector. If multiple solvers match with the same dnsNames value, the solver with the most matching labels in matchLabels will be selected. If neither has more matches, the solver defined earlier in the list will be selected."

**Note:** This function appends passed data to existing values

### fn spec.acme.solvers.selector.withDnsZones

```ts
withDnsZones(dnsZones)
```

"List of DNSZones that this solver will be used to solve. The most specific DNS zone match specified here will take precedence over other DNS zone matches, so a solver specifying sys.example.com will be selected over one specifying example.com for the domain www.sys.example.com. If multiple solvers match with the same dnsZones value, the solver with the most matching labels in matchLabels will be selected. If neither has more matches, the solver defined earlier in the list will be selected."

### fn spec.acme.solvers.selector.withDnsZonesMixin

```ts
withDnsZonesMixin(dnsZones)
```

"List of DNSZones that this solver will be used to solve. The most specific DNS zone match specified here will take precedence over other DNS zone matches, so a solver specifying sys.example.com will be selected over one specifying example.com for the domain www.sys.example.com. If multiple solvers match with the same dnsZones value, the solver with the most matching labels in matchLabels will be selected. If neither has more matches, the solver defined earlier in the list will be selected."

**Note:** This function appends passed data to existing values

### fn spec.acme.solvers.selector.withMatchLabels

```ts
withMatchLabels(matchLabels)
```

"A label selector that is used to refine the set of certificate's that this challenge solver will apply to."

### fn spec.acme.solvers.selector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"A label selector that is used to refine the set of certificate's that this challenge solver will apply to."

**Note:** This function appends passed data to existing values

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