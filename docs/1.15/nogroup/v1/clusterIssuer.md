---
permalink: /1.15/nogroup/v1/clusterIssuer/
---

# nogroup.v1.clusterIssuer

"A ClusterIssuer represents a certificate issuing authority which can be\nreferenced as part of `issuerRef` fields.\nIt is similar to an Issuer, however it is cluster-scoped and therefore can\nbe referenced by resources that exist in *any* namespace, not just the same\nnamespace as the referent."

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
    * [`fn withCaBundle(caBundle)`](#fn-specacmewithcabundle)
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
        * [`obj spec.acme.solvers.dns01.acmeDNS`](#obj-specacmesolversdns01acmedns)
          * [`fn withHost(host)`](#fn-specacmesolversdns01acmednswithhost)
          * [`obj spec.acme.solvers.dns01.acmeDNS.accountSecretRef`](#obj-specacmesolversdns01acmednsaccountsecretref)
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
        * [`obj spec.acme.solvers.dns01.azureDNS`](#obj-specacmesolversdns01azuredns)
          * [`fn withClientID(clientID)`](#fn-specacmesolversdns01azurednswithclientid)
          * [`fn withEnvironment(environment)`](#fn-specacmesolversdns01azurednswithenvironment)
          * [`fn withHostedZoneName(hostedZoneName)`](#fn-specacmesolversdns01azurednswithhostedzonename)
          * [`fn withResourceGroupName(resourceGroupName)`](#fn-specacmesolversdns01azurednswithresourcegroupname)
          * [`fn withSubscriptionID(subscriptionID)`](#fn-specacmesolversdns01azurednswithsubscriptionid)
          * [`fn withTenantID(tenantID)`](#fn-specacmesolversdns01azurednswithtenantid)
          * [`obj spec.acme.solvers.dns01.azureDNS.clientSecretSecretRef`](#obj-specacmesolversdns01azurednsclientsecretsecretref)
            * [`fn withKey(key)`](#fn-specacmesolversdns01azurednsclientsecretsecretrefwithkey)
            * [`fn withName(name)`](#fn-specacmesolversdns01azurednsclientsecretsecretrefwithname)
          * [`obj spec.acme.solvers.dns01.azureDNS.managedIdentity`](#obj-specacmesolversdns01azurednsmanagedidentity)
            * [`fn withClientID(clientID)`](#fn-specacmesolversdns01azurednsmanagedidentitywithclientid)
            * [`fn withResourceID(resourceID)`](#fn-specacmesolversdns01azurednsmanagedidentitywithresourceid)
        * [`obj spec.acme.solvers.dns01.cloudDNS`](#obj-specacmesolversdns01clouddns)
          * [`fn withHostedZoneName(hostedZoneName)`](#fn-specacmesolversdns01clouddnswithhostedzonename)
          * [`fn withProject(project)`](#fn-specacmesolversdns01clouddnswithproject)
          * [`obj spec.acme.solvers.dns01.cloudDNS.serviceAccountSecretRef`](#obj-specacmesolversdns01clouddnsserviceaccountsecretref)
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
          * [`obj spec.acme.solvers.dns01.route53.accessKeyIDSecretRef`](#obj-specacmesolversdns01route53accesskeyidsecretref)
            * [`fn withKey(key)`](#fn-specacmesolversdns01route53accesskeyidsecretrefwithkey)
            * [`fn withName(name)`](#fn-specacmesolversdns01route53accesskeyidsecretrefwithname)
          * [`obj spec.acme.solvers.dns01.route53.auth`](#obj-specacmesolversdns01route53auth)
            * [`obj spec.acme.solvers.dns01.route53.auth.kubernetes`](#obj-specacmesolversdns01route53authkubernetes)
              * [`obj spec.acme.solvers.dns01.route53.auth.kubernetes.serviceAccountRef`](#obj-specacmesolversdns01route53authkubernetesserviceaccountref)
                * [`fn withAudiences(audiences)`](#fn-specacmesolversdns01route53authkubernetesserviceaccountrefwithaudiences)
                * [`fn withAudiencesMixin(audiences)`](#fn-specacmesolversdns01route53authkubernetesserviceaccountrefwithaudiencesmixin)
                * [`fn withName(name)`](#fn-specacmesolversdns01route53authkubernetesserviceaccountrefwithname)
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
          * [`fn withParentRefs(parentRefs)`](#fn-specacmesolvershttp01gatewayhttproutewithparentrefs)
          * [`fn withParentRefsMixin(parentRefs)`](#fn-specacmesolvershttp01gatewayhttproutewithparentrefsmixin)
          * [`fn withServiceType(serviceType)`](#fn-specacmesolvershttp01gatewayhttproutewithservicetype)
          * [`obj spec.acme.solvers.http01.gatewayHTTPRoute.parentRefs`](#obj-specacmesolvershttp01gatewayhttprouteparentrefs)
            * [`fn withGroup(group)`](#fn-specacmesolvershttp01gatewayhttprouteparentrefswithgroup)
            * [`fn withKind(kind)`](#fn-specacmesolvershttp01gatewayhttprouteparentrefswithkind)
            * [`fn withName(name)`](#fn-specacmesolvershttp01gatewayhttprouteparentrefswithname)
            * [`fn withNamespace(namespace)`](#fn-specacmesolvershttp01gatewayhttprouteparentrefswithnamespace)
            * [`fn withPort(port)`](#fn-specacmesolvershttp01gatewayhttprouteparentrefswithport)
            * [`fn withSectionName(sectionName)`](#fn-specacmesolvershttp01gatewayhttprouteparentrefswithsectionname)
        * [`obj spec.acme.solvers.http01.ingress`](#obj-specacmesolvershttp01ingress)
          * [`fn withClass(class)`](#fn-specacmesolvershttp01ingresswithclass)
          * [`fn withIngressClassName(ingressClassName)`](#fn-specacmesolvershttp01ingresswithingressclassname)
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
              * [`fn withImagePullSecrets(imagePullSecrets)`](#fn-specacmesolvershttp01ingresspodtemplatespecwithimagepullsecrets)
              * [`fn withImagePullSecretsMixin(imagePullSecrets)`](#fn-specacmesolvershttp01ingresspodtemplatespecwithimagepullsecretsmixin)
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
                      * [`fn withMatchLabelKeys(matchLabelKeys)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermwithmatchlabelkeys)
                      * [`fn withMatchLabelKeysMixin(matchLabelKeys)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermwithmatchlabelkeysmixin)
                      * [`fn withMismatchLabelKeys(mismatchLabelKeys)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermwithmismatchlabelkeys)
                      * [`fn withMismatchLabelKeysMixin(mismatchLabelKeys)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermwithmismatchlabelkeysmixin)
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
                    * [`fn withMatchLabelKeys(matchLabelKeys)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionwithmatchlabelkeys)
                    * [`fn withMatchLabelKeysMixin(matchLabelKeys)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionwithmatchlabelkeysmixin)
                    * [`fn withMismatchLabelKeys(mismatchLabelKeys)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionwithmismatchlabelkeys)
                    * [`fn withMismatchLabelKeysMixin(mismatchLabelKeys)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionwithmismatchlabelkeysmixin)
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
                      * [`fn withMatchLabelKeys(matchLabelKeys)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermwithmatchlabelkeys)
                      * [`fn withMatchLabelKeysMixin(matchLabelKeys)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermwithmatchlabelkeysmixin)
                      * [`fn withMismatchLabelKeys(mismatchLabelKeys)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermwithmismatchlabelkeys)
                      * [`fn withMismatchLabelKeysMixin(mismatchLabelKeys)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermwithmismatchlabelkeysmixin)
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
                    * [`fn withMatchLabelKeys(matchLabelKeys)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionwithmatchlabelkeys)
                    * [`fn withMatchLabelKeysMixin(matchLabelKeys)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionwithmatchlabelkeysmixin)
                    * [`fn withMismatchLabelKeys(mismatchLabelKeys)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionwithmismatchlabelkeys)
                    * [`fn withMismatchLabelKeysMixin(mismatchLabelKeys)`](#fn-specacmesolvershttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionwithmismatchlabelkeysmixin)
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
              * [`obj spec.acme.solvers.http01.ingress.podTemplate.spec.imagePullSecrets`](#obj-specacmesolvershttp01ingresspodtemplatespecimagepullsecrets)
                * [`fn withName(name)`](#fn-specacmesolvershttp01ingresspodtemplatespecimagepullsecretswithname)
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
    * [`fn withIssuingCertificateURLs(issuingCertificateURLs)`](#fn-speccawithissuingcertificateurls)
    * [`fn withIssuingCertificateURLsMixin(issuingCertificateURLs)`](#fn-speccawithissuingcertificateurlsmixin)
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
        * [`obj spec.vault.auth.kubernetes.serviceAccountRef`](#obj-specvaultauthkubernetesserviceaccountref)
          * [`fn withAudiences(audiences)`](#fn-specvaultauthkubernetesserviceaccountrefwithaudiences)
          * [`fn withAudiencesMixin(audiences)`](#fn-specvaultauthkubernetesserviceaccountrefwithaudiencesmixin)
          * [`fn withName(name)`](#fn-specvaultauthkubernetesserviceaccountrefwithname)
      * [`obj spec.vault.auth.tokenSecretRef`](#obj-specvaultauthtokensecretref)
        * [`fn withKey(key)`](#fn-specvaultauthtokensecretrefwithkey)
        * [`fn withName(name)`](#fn-specvaultauthtokensecretrefwithname)
    * [`obj spec.vault.caBundleSecretRef`](#obj-specvaultcabundlesecretref)
      * [`fn withKey(key)`](#fn-specvaultcabundlesecretrefwithkey)
      * [`fn withName(name)`](#fn-specvaultcabundlesecretrefwithname)
    * [`obj spec.vault.clientCertSecretRef`](#obj-specvaultclientcertsecretref)
      * [`fn withKey(key)`](#fn-specvaultclientcertsecretrefwithkey)
      * [`fn withName(name)`](#fn-specvaultclientcertsecretrefwithname)
    * [`obj spec.vault.clientKeySecretRef`](#obj-specvaultclientkeysecretref)
      * [`fn withKey(key)`](#fn-specvaultclientkeysecretrefwithkey)
      * [`fn withName(name)`](#fn-specvaultclientkeysecretrefwithname)
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

"ACME configures this issuer to communicate with a RFC8555 (ACME) server\nto obtain signed x509 certificates."

### fn spec.acme.withCaBundle

```ts
withCaBundle(caBundle)
```

"Base64-encoded bundle of PEM CAs which can be used to validate the certificate\nchain presented by the ACME server.\nMutually exclusive with SkipTLSVerify; prefer using CABundle to prevent various\nkinds of security vulnerabilities.\nIf CABundle and SkipTLSVerify are unset, the system certificate bundle inside\nthe container is used to validate the TLS connection."

### fn spec.acme.withDisableAccountKeyGeneration

```ts
withDisableAccountKeyGeneration(disableAccountKeyGeneration)
```

"Enables or disables generating a new ACME account key.\nIf true, the Issuer resource will *not* request a new account but will expect\nthe account key to be supplied via an existing secret.\nIf false, the cert-manager system will generate a new ACME account key\nfor the Issuer.\nDefaults to false."

### fn spec.acme.withEmail

```ts
withEmail(email)
```

"Email is the email address to be associated with the ACME account.\nThis field is optional, but it is strongly recommended to be set.\nIt will be used to contact you in case of issues with your account or\ncertificates, including expiry notification emails.\nThis field may be updated after the account is initially registered."

### fn spec.acme.withEnableDurationFeature

```ts
withEnableDurationFeature(enableDurationFeature)
```

"Enables requesting a Not After date on certificates that matches the\nduration of the certificate. This is not supported by all ACME servers\nlike Let's Encrypt. If set to true when the ACME server does not support\nit, it will create an error on the Order.\nDefaults to false."

### fn spec.acme.withPreferredChain

```ts
withPreferredChain(preferredChain)
```

"PreferredChain is the chain to use if the ACME server outputs multiple.\nPreferredChain is no guarantee that this one gets delivered by the ACME\nendpoint.\nFor example, for Let's Encrypt's DST crosssign you would use:\n\"DST Root CA X3\" or \"ISRG Root X1\" for the newer Let's Encrypt root CA.\nThis value picks the first certificate bundle in the combined set of\nACME default and alternative chains that has a root-most certificate with\nthis value as its issuer's commonname."

### fn spec.acme.withServer

```ts
withServer(server)
```

"Server is the URL used to access the ACME server's 'directory' endpoint.\nFor example, for Let's Encrypt's staging endpoint, you would use:\n\"https://acme-staging-v02.api.letsencrypt.org/directory\".\nOnly ACME v2 endpoints (i.e. RFC 8555) are supported."

### fn spec.acme.withSkipTLSVerify

```ts
withSkipTLSVerify(skipTLSVerify)
```

"INSECURE: Enables or disables validation of the ACME server TLS certificate.\nIf true, requests to the ACME server will not have the TLS certificate chain\nvalidated.\nMutually exclusive with CABundle; prefer using CABundle to prevent various\nkinds of security vulnerabilities.\nOnly enable this option in development environments.\nIf CABundle and SkipTLSVerify are unset, the system certificate bundle inside\nthe container is used to validate the TLS connection.\nDefaults to false."

### fn spec.acme.withSolvers

```ts
withSolvers(solvers)
```

"Solvers is a list of challenge solvers that will be used to solve\nACME challenges for the matching domains.\nSolver configurations must be provided in order to obtain certificates\nfrom an ACME server.\nFor more information, see: https://cert-manager.io/docs/configuration/acme/"

### fn spec.acme.withSolversMixin

```ts
withSolversMixin(solvers)
```

"Solvers is a list of challenge solvers that will be used to solve\nACME challenges for the matching domains.\nSolver configurations must be provided in order to obtain certificates\nfrom an ACME server.\nFor more information, see: https://cert-manager.io/docs/configuration/acme/"

**Note:** This function appends passed data to existing values

## obj spec.acme.externalAccountBinding

"ExternalAccountBinding is a reference to a CA external account of the ACME\nserver.\nIf set, upon registration cert-manager will attempt to associate the given\nexternal account credentials with the registered ACME account."

### fn spec.acme.externalAccountBinding.withKeyAlgorithm

```ts
withKeyAlgorithm(keyAlgorithm)
```

"Deprecated: keyAlgorithm field exists for historical compatibility\nreasons and should not be used. The algorithm is now hardcoded to HS256\nin golang/x/crypto/acme."

### fn spec.acme.externalAccountBinding.withKeyID

```ts
withKeyID(keyID)
```

"keyID is the ID of the CA key that the External Account is bound to."

## obj spec.acme.externalAccountBinding.keySecretRef

"keySecretRef is a Secret Key Selector referencing a data item in a Kubernetes\nSecret which holds the symmetric MAC key of the External Account Binding.\nThe `key` is the index string that is paired with the key data in the\nSecret and should not be confused with the key data itself, or indeed with\nthe External Account Binding keyID above.\nThe secret key stored in the Secret **must** be un-padded, base64 URL\nencoded data."

### fn spec.acme.externalAccountBinding.keySecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used.\nSome instances of this field may be defaulted, in others it may be\nrequired."

### fn spec.acme.externalAccountBinding.keySecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to.\nMore info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.acme.privateKeySecretRef

"PrivateKey is the name of a Kubernetes Secret resource that will be used to\nstore the automatically generated ACME account private key.\nOptionally, a `key` may be specified to select a specific entry within\nthe named Secret resource.\nIf `key` is not specified, a default of `tls.key` will be used."

### fn spec.acme.privateKeySecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used.\nSome instances of this field may be defaulted, in others it may be\nrequired."

### fn spec.acme.privateKeySecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to.\nMore info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.acme.solvers

"Solvers is a list of challenge solvers that will be used to solve\nACME challenges for the matching domains.\nSolver configurations must be provided in order to obtain certificates\nfrom an ACME server.\nFor more information, see: https://cert-manager.io/docs/configuration/acme/"

## obj spec.acme.solvers.dns01

"Configures cert-manager to attempt to complete authorizations by\nperforming the DNS01 challenge flow."

### fn spec.acme.solvers.dns01.withCnameStrategy

```ts
withCnameStrategy(cnameStrategy)
```

"CNAMEStrategy configures how the DNS01 provider should handle CNAME\nrecords when found in DNS zones."

## obj spec.acme.solvers.dns01.acmeDNS

"Use the 'ACME DNS' (https://github.com/joohoi/acme-dns) API to manage\nDNS01 challenge records."

### fn spec.acme.solvers.dns01.acmeDNS.withHost

```ts
withHost(host)
```



## obj spec.acme.solvers.dns01.acmeDNS.accountSecretRef

"A reference to a specific 'key' within a Secret resource.\nIn some instances, `key` is a required field."

### fn spec.acme.solvers.dns01.acmeDNS.accountSecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used.\nSome instances of this field may be defaulted, in others it may be\nrequired."

### fn spec.acme.solvers.dns01.acmeDNS.accountSecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to.\nMore info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.acme.solvers.dns01.akamai

"Use the Akamai DNS zone management API to manage DNS01 challenge records."

### fn spec.acme.solvers.dns01.akamai.withServiceConsumerDomain

```ts
withServiceConsumerDomain(serviceConsumerDomain)
```



## obj spec.acme.solvers.dns01.akamai.accessTokenSecretRef

"A reference to a specific 'key' within a Secret resource.\nIn some instances, `key` is a required field."

### fn spec.acme.solvers.dns01.akamai.accessTokenSecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used.\nSome instances of this field may be defaulted, in others it may be\nrequired."

### fn spec.acme.solvers.dns01.akamai.accessTokenSecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to.\nMore info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.acme.solvers.dns01.akamai.clientSecretSecretRef

"A reference to a specific 'key' within a Secret resource.\nIn some instances, `key` is a required field."

### fn spec.acme.solvers.dns01.akamai.clientSecretSecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used.\nSome instances of this field may be defaulted, in others it may be\nrequired."

### fn spec.acme.solvers.dns01.akamai.clientSecretSecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to.\nMore info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.acme.solvers.dns01.akamai.clientTokenSecretRef

"A reference to a specific 'key' within a Secret resource.\nIn some instances, `key` is a required field."

### fn spec.acme.solvers.dns01.akamai.clientTokenSecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used.\nSome instances of this field may be defaulted, in others it may be\nrequired."

### fn spec.acme.solvers.dns01.akamai.clientTokenSecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to.\nMore info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.acme.solvers.dns01.azureDNS

"Use the Microsoft Azure DNS API to manage DNS01 challenge records."

### fn spec.acme.solvers.dns01.azureDNS.withClientID

```ts
withClientID(clientID)
```

"Auth: Azure Service Principal:\nThe ClientID of the Azure Service Principal used to authenticate with Azure DNS.\nIf set, ClientSecret and TenantID must also be set."

### fn spec.acme.solvers.dns01.azureDNS.withEnvironment

```ts
withEnvironment(environment)
```

"name of the Azure environment (default AzurePublicCloud)"

### fn spec.acme.solvers.dns01.azureDNS.withHostedZoneName

```ts
withHostedZoneName(hostedZoneName)
```

"name of the DNS zone that should be used"

### fn spec.acme.solvers.dns01.azureDNS.withResourceGroupName

```ts
withResourceGroupName(resourceGroupName)
```

"resource group the DNS zone is located in"

### fn spec.acme.solvers.dns01.azureDNS.withSubscriptionID

```ts
withSubscriptionID(subscriptionID)
```

"ID of the Azure subscription"

### fn spec.acme.solvers.dns01.azureDNS.withTenantID

```ts
withTenantID(tenantID)
```

"Auth: Azure Service Principal:\nThe TenantID of the Azure Service Principal used to authenticate with Azure DNS.\nIf set, ClientID and ClientSecret must also be set."

## obj spec.acme.solvers.dns01.azureDNS.clientSecretSecretRef

"Auth: Azure Service Principal:\nA reference to a Secret containing the password associated with the Service Principal.\nIf set, ClientID and TenantID must also be set."

### fn spec.acme.solvers.dns01.azureDNS.clientSecretSecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used.\nSome instances of this field may be defaulted, in others it may be\nrequired."

### fn spec.acme.solvers.dns01.azureDNS.clientSecretSecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to.\nMore info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.acme.solvers.dns01.azureDNS.managedIdentity

"Auth: Azure Workload Identity or Azure Managed Service Identity:\nSettings to enable Azure Workload Identity or Azure Managed Service Identity\nIf set, ClientID, ClientSecret and TenantID must not be set."

### fn spec.acme.solvers.dns01.azureDNS.managedIdentity.withClientID

```ts
withClientID(clientID)
```

"client ID of the managed identity, can not be used at the same time as resourceID"

### fn spec.acme.solvers.dns01.azureDNS.managedIdentity.withResourceID

```ts
withResourceID(resourceID)
```

"resource ID of the managed identity, can not be used at the same time as clientID\nCannot be used for Azure Managed Service Identity"

## obj spec.acme.solvers.dns01.cloudDNS

"Use the Google Cloud DNS API to manage DNS01 challenge records."

### fn spec.acme.solvers.dns01.cloudDNS.withHostedZoneName

```ts
withHostedZoneName(hostedZoneName)
```

"HostedZoneName is an optional field that tells cert-manager in which\nCloud DNS zone the challenge record has to be created.\nIf left empty cert-manager will automatically choose a zone."

### fn spec.acme.solvers.dns01.cloudDNS.withProject

```ts
withProject(project)
```



## obj spec.acme.solvers.dns01.cloudDNS.serviceAccountSecretRef

"A reference to a specific 'key' within a Secret resource.\nIn some instances, `key` is a required field."

### fn spec.acme.solvers.dns01.cloudDNS.serviceAccountSecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used.\nSome instances of this field may be defaulted, in others it may be\nrequired."

### fn spec.acme.solvers.dns01.cloudDNS.serviceAccountSecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to.\nMore info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.acme.solvers.dns01.cloudflare

"Use the Cloudflare API to manage DNS01 challenge records."

### fn spec.acme.solvers.dns01.cloudflare.withEmail

```ts
withEmail(email)
```

"Email of the account, only required when using API key based authentication."

## obj spec.acme.solvers.dns01.cloudflare.apiKeySecretRef

"API key to use to authenticate with Cloudflare.\nNote: using an API token to authenticate is now the recommended method\nas it allows greater control of permissions."

### fn spec.acme.solvers.dns01.cloudflare.apiKeySecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used.\nSome instances of this field may be defaulted, in others it may be\nrequired."

### fn spec.acme.solvers.dns01.cloudflare.apiKeySecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to.\nMore info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.acme.solvers.dns01.cloudflare.apiTokenSecretRef

"API token used to authenticate with Cloudflare."

### fn spec.acme.solvers.dns01.cloudflare.apiTokenSecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used.\nSome instances of this field may be defaulted, in others it may be\nrequired."

### fn spec.acme.solvers.dns01.cloudflare.apiTokenSecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to.\nMore info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.acme.solvers.dns01.digitalocean

"Use the DigitalOcean DNS API to manage DNS01 challenge records."

## obj spec.acme.solvers.dns01.digitalocean.tokenSecretRef

"A reference to a specific 'key' within a Secret resource.\nIn some instances, `key` is a required field."

### fn spec.acme.solvers.dns01.digitalocean.tokenSecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used.\nSome instances of this field may be defaulted, in others it may be\nrequired."

### fn spec.acme.solvers.dns01.digitalocean.tokenSecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to.\nMore info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.acme.solvers.dns01.rfc2136

"Use RFC2136 (\"Dynamic Updates in the Domain Name System\") (https://datatracker.ietf.org/doc/rfc2136/)\nto manage DNS01 challenge records."

### fn spec.acme.solvers.dns01.rfc2136.withNameserver

```ts
withNameserver(nameserver)
```

"The IP address or hostname of an authoritative DNS server supporting\nRFC2136 in the form host:port. If the host is an IPv6 address it must be\nenclosed in square brackets (e.g [2001:db8::1])\u00a0; port is optional.\nThis field is required."

### fn spec.acme.solvers.dns01.rfc2136.withTsigAlgorithm

```ts
withTsigAlgorithm(tsigAlgorithm)
```

"The TSIG Algorithm configured in the DNS supporting RFC2136. Used only\nwhen ``tsigSecretSecretRef`` and ``tsigKeyName`` are defined.\nSupported values are (case-insensitive): ``HMACMD5`` (default),\n``HMACSHA1``, ``HMACSHA256`` or ``HMACSHA512``."

### fn spec.acme.solvers.dns01.rfc2136.withTsigKeyName

```ts
withTsigKeyName(tsigKeyName)
```

"The TSIG Key name configured in the DNS.\nIf ``tsigSecretSecretRef`` is defined, this field is required."

## obj spec.acme.solvers.dns01.rfc2136.tsigSecretSecretRef

"The name of the secret containing the TSIG value.\nIf ``tsigKeyName`` is defined, this field is required."

### fn spec.acme.solvers.dns01.rfc2136.tsigSecretSecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used.\nSome instances of this field may be defaulted, in others it may be\nrequired."

### fn spec.acme.solvers.dns01.rfc2136.tsigSecretSecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to.\nMore info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.acme.solvers.dns01.route53

"Use the AWS Route53 API to manage DNS01 challenge records."

### fn spec.acme.solvers.dns01.route53.withAccessKeyID

```ts
withAccessKeyID(accessKeyID)
```

"The AccessKeyID is used for authentication.\nCannot be set when SecretAccessKeyID is set.\nIf neither the Access Key nor Key ID are set, we fall-back to using env\nvars, shared credentials file or AWS Instance metadata,\nsee: https://docs.aws.amazon.com/sdk-for-go/v1/developer-guide/configuring-sdk.html#specifying-credentials"

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

"Role is a Role ARN which the Route53 provider will assume using either the explicit credentials AccessKeyID/SecretAccessKey\nor the inferred credentials from environment variables, shared credentials file or AWS Instance metadata"

## obj spec.acme.solvers.dns01.route53.accessKeyIDSecretRef

"The SecretAccessKey is used for authentication. If set, pull the AWS\naccess key ID from a key within a Kubernetes Secret.\nCannot be set when AccessKeyID is set.\nIf neither the Access Key nor Key ID are set, we fall-back to using env\nvars, shared credentials file or AWS Instance metadata,\nsee: https://docs.aws.amazon.com/sdk-for-go/v1/developer-guide/configuring-sdk.html#specifying-credentials"

### fn spec.acme.solvers.dns01.route53.accessKeyIDSecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used.\nSome instances of this field may be defaulted, in others it may be\nrequired."

### fn spec.acme.solvers.dns01.route53.accessKeyIDSecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to.\nMore info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.acme.solvers.dns01.route53.auth

"Auth configures how cert-manager authenticates."

## obj spec.acme.solvers.dns01.route53.auth.kubernetes

"Kubernetes authenticates with Route53 using AssumeRoleWithWebIdentity\nby passing a bound ServiceAccount token."

## obj spec.acme.solvers.dns01.route53.auth.kubernetes.serviceAccountRef

"A reference to a service account that will be used to request a bound\ntoken (also known as \"projected token\"). To use this field, you must\nconfigure an RBAC rule to let cert-manager request a token."

### fn spec.acme.solvers.dns01.route53.auth.kubernetes.serviceAccountRef.withAudiences

```ts
withAudiences(audiences)
```

"TokenAudiences is an optional list of audiences to include in the\ntoken passed to AWS. The default token consisting of the issuer's namespace\nand name is always included.\nIf unset the audience defaults to `sts.amazonaws.com`."

### fn spec.acme.solvers.dns01.route53.auth.kubernetes.serviceAccountRef.withAudiencesMixin

```ts
withAudiencesMixin(audiences)
```

"TokenAudiences is an optional list of audiences to include in the\ntoken passed to AWS. The default token consisting of the issuer's namespace\nand name is always included.\nIf unset the audience defaults to `sts.amazonaws.com`."

**Note:** This function appends passed data to existing values

### fn spec.acme.solvers.dns01.route53.auth.kubernetes.serviceAccountRef.withName

```ts
withName(name)
```

"Name of the ServiceAccount used to request a token."

## obj spec.acme.solvers.dns01.route53.secretAccessKeySecretRef

"The SecretAccessKey is used for authentication.\nIf neither the Access Key nor Key ID are set, we fall-back to using env\nvars, shared credentials file or AWS Instance metadata,\nsee: https://docs.aws.amazon.com/sdk-for-go/v1/developer-guide/configuring-sdk.html#specifying-credentials"

### fn spec.acme.solvers.dns01.route53.secretAccessKeySecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used.\nSome instances of this field may be defaulted, in others it may be\nrequired."

### fn spec.acme.solvers.dns01.route53.secretAccessKeySecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to.\nMore info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.acme.solvers.dns01.webhook

"Configure an external webhook based DNS01 challenge solver to manage\nDNS01 challenge records."

### fn spec.acme.solvers.dns01.webhook.withConfig

```ts
withConfig(config)
```

"Additional configuration that should be passed to the webhook apiserver\nwhen challenges are processed.\nThis can contain arbitrary JSON data.\nSecret values should not be specified in this stanza.\nIf secret values are needed (e.g. credentials for a DNS service), you\nshould use a SecretKeySelector to reference a Secret resource.\nFor details on the schema of this field, consult the webhook provider\nimplementation's documentation."

### fn spec.acme.solvers.dns01.webhook.withGroupName

```ts
withGroupName(groupName)
```

"The API group name that should be used when POSTing ChallengePayload\nresources to the webhook apiserver.\nThis should be the same as the GroupName specified in the webhook\nprovider implementation."

### fn spec.acme.solvers.dns01.webhook.withSolverName

```ts
withSolverName(solverName)
```

"The name of the solver to use, as defined in the webhook provider\nimplementation.\nThis will typically be the name of the provider, e.g. 'cloudflare'."

## obj spec.acme.solvers.http01

"Configures cert-manager to attempt to complete authorizations by\nperforming the HTTP01 challenge flow.\nIt is not possible to obtain certificates for wildcard domain names\n(e.g. `*.example.com`) using the HTTP01 challenge mechanism."

## obj spec.acme.solvers.http01.gatewayHTTPRoute

"The Gateway API is a sig-network community API that models service networking\nin Kubernetes (https://gateway-api.sigs.k8s.io/). The Gateway solver will\ncreate HTTPRoutes with the specified labels in the same namespace as the challenge.\nThis solver is experimental, and fields / behaviour may change in the future."

### fn spec.acme.solvers.http01.gatewayHTTPRoute.withLabels

```ts
withLabels(labels)
```

"Custom labels that will be applied to HTTPRoutes created by cert-manager\nwhile solving HTTP-01 challenges."

### fn spec.acme.solvers.http01.gatewayHTTPRoute.withLabelsMixin

```ts
withLabelsMixin(labels)
```

"Custom labels that will be applied to HTTPRoutes created by cert-manager\nwhile solving HTTP-01 challenges."

**Note:** This function appends passed data to existing values

### fn spec.acme.solvers.http01.gatewayHTTPRoute.withParentRefs

```ts
withParentRefs(parentRefs)
```

"When solving an HTTP-01 challenge, cert-manager creates an HTTPRoute.\ncert-manager needs to know which parentRefs should be used when creating\nthe HTTPRoute. Usually, the parentRef references a Gateway. See:\nhttps://gateway-api.sigs.k8s.io/api-types/httproute/#attaching-to-gateways"

### fn spec.acme.solvers.http01.gatewayHTTPRoute.withParentRefsMixin

```ts
withParentRefsMixin(parentRefs)
```

"When solving an HTTP-01 challenge, cert-manager creates an HTTPRoute.\ncert-manager needs to know which parentRefs should be used when creating\nthe HTTPRoute. Usually, the parentRef references a Gateway. See:\nhttps://gateway-api.sigs.k8s.io/api-types/httproute/#attaching-to-gateways"

**Note:** This function appends passed data to existing values

### fn spec.acme.solvers.http01.gatewayHTTPRoute.withServiceType

```ts
withServiceType(serviceType)
```

"Optional service type for Kubernetes solver service. Supported values\nare NodePort or ClusterIP. If unset, defaults to NodePort."

## obj spec.acme.solvers.http01.gatewayHTTPRoute.parentRefs

"When solving an HTTP-01 challenge, cert-manager creates an HTTPRoute.\ncert-manager needs to know which parentRefs should be used when creating\nthe HTTPRoute. Usually, the parentRef references a Gateway. See:\nhttps://gateway-api.sigs.k8s.io/api-types/httproute/#attaching-to-gateways"

### fn spec.acme.solvers.http01.gatewayHTTPRoute.parentRefs.withGroup

```ts
withGroup(group)
```

"Group is the group of the referent.\nWhen unspecified, \"gateway.networking.k8s.io\" is inferred.\nTo set the core API group (such as for a \"Service\" kind referent),\nGroup must be explicitly set to \"\" (empty string).\n\n\nSupport: Core"

### fn spec.acme.solvers.http01.gatewayHTTPRoute.parentRefs.withKind

```ts
withKind(kind)
```

"Kind is kind of the referent.\n\n\nThere are two kinds of parent resources with \"Core\" support:\n\n\n* Gateway (Gateway conformance profile)\n* Service (Mesh conformance profile, ClusterIP Services only)\n\n\nSupport for other resources is Implementation-Specific."

### fn spec.acme.solvers.http01.gatewayHTTPRoute.parentRefs.withName

```ts
withName(name)
```

"Name is the name of the referent.\n\n\nSupport: Core"

### fn spec.acme.solvers.http01.gatewayHTTPRoute.parentRefs.withNamespace

```ts
withNamespace(namespace)
```

"Namespace is the namespace of the referent. When unspecified, this refers\nto the local namespace of the Route.\n\n\nNote that there are specific rules for ParentRefs which cross namespace\nboundaries. Cross-namespace references are only valid if they are explicitly\nallowed by something in the namespace they are referring to. For example:\nGateway has the AllowedRoutes field, and ReferenceGrant provides a\ngeneric way to enable any other kind of cross-namespace reference.\n\n\n<gateway:experimental:description>\nParentRefs from a Route to a Service in the same namespace are \"producer\"\nroutes, which apply default routing rules to inbound connections from\nany namespace to the Service.\n\n\nParentRefs from a Route to a Service in a different namespace are\n\"consumer\" routes, and these routing rules are only applied to outbound\nconnections originating from the same namespace as the Route, for which\nthe intended destination of the connections are a Service targeted as a\nParentRef of the Route.\n</gateway:experimental:description>\n\n\nSupport: Core"

### fn spec.acme.solvers.http01.gatewayHTTPRoute.parentRefs.withPort

```ts
withPort(port)
```

"Port is the network port this Route targets. It can be interpreted\ndifferently based on the type of parent resource.\n\n\nWhen the parent resource is a Gateway, this targets all listeners\nlistening on the specified port that also support this kind of Route(and\nselect this Route). It's not recommended to set `Port` unless the\nnetworking behaviors specified in a Route must apply to a specific port\nas opposed to a listener(s) whose port(s) may be changed. When both Port\nand SectionName are specified, the name and port of the selected listener\nmust match both specified values.\n\n\n<gateway:experimental:description>\nWhen the parent resource is a Service, this targets a specific port in the\nService spec. When both Port (experimental) and SectionName are specified,\nthe name and port of the selected port must match both specified values.\n</gateway:experimental:description>\n\n\nImplementations MAY choose to support other parent resources.\nImplementations supporting other types of parent resources MUST clearly\ndocument how/if Port is interpreted.\n\n\nFor the purpose of status, an attachment is considered successful as\nlong as the parent resource accepts it partially. For example, Gateway\nlisteners can restrict which Routes can attach to them by Route kind,\nnamespace, or hostname. If 1 of 2 Gateway listeners accept attachment\nfrom the referencing Route, the Route MUST be considered successfully\nattached. If no Gateway listeners accept attachment from this Route,\nthe Route MUST be considered detached from the Gateway.\n\n\nSupport: Extended"

### fn spec.acme.solvers.http01.gatewayHTTPRoute.parentRefs.withSectionName

```ts
withSectionName(sectionName)
```

"SectionName is the name of a section within the target resource. In the\nfollowing resources, SectionName is interpreted as the following:\n\n\n* Gateway: Listener name. When both Port (experimental) and SectionName\nare specified, the name and port of the selected listener must match\nboth specified values.\n* Service: Port name. When both Port (experimental) and SectionName\nare specified, the name and port of the selected listener must match\nboth specified values.\n\n\nImplementations MAY choose to support attaching Routes to other resources.\nIf that is the case, they MUST clearly document how SectionName is\ninterpreted.\n\n\nWhen unspecified (empty string), this will reference the entire resource.\nFor the purpose of status, an attachment is considered successful if at\nleast one section in the parent resource accepts it. For example, Gateway\nlisteners can restrict which Routes can attach to them by Route kind,\nnamespace, or hostname. If 1 of 2 Gateway listeners accept attachment from\nthe referencing Route, the Route MUST be considered successfully\nattached. If no Gateway listeners accept attachment from this Route, the\nRoute MUST be considered detached from the Gateway.\n\n\nSupport: Core"

## obj spec.acme.solvers.http01.ingress

"The ingress based HTTP01 challenge solver will solve challenges by\ncreating or modifying Ingress resources in order to route requests for\n'/.well-known/acme-challenge/XYZ' to 'challenge solver' pods that are\nprovisioned by cert-manager for each Challenge to be completed."

### fn spec.acme.solvers.http01.ingress.withClass

```ts
withClass(class)
```

"This field configures the annotation `kubernetes.io/ingress.class` when\ncreating Ingress resources to solve ACME challenges that use this\nchallenge solver. Only one of `class`, `name` or `ingressClassName` may\nbe specified."

### fn spec.acme.solvers.http01.ingress.withIngressClassName

```ts
withIngressClassName(ingressClassName)
```

"This field configures the field `ingressClassName` on the created Ingress\nresources used to solve ACME challenges that use this challenge solver.\nThis is the recommended way of configuring the ingress class. Only one of\n`class`, `name` or `ingressClassName` may be specified."

### fn spec.acme.solvers.http01.ingress.withName

```ts
withName(name)
```

"The name of the ingress resource that should have ACME challenge solving\nroutes inserted into it in order to solve HTTP01 challenges.\nThis is typically used in conjunction with ingress controllers like\ningress-gce, which maintains a 1:1 mapping between external IPs and\ningress resources. Only one of `class`, `name` or `ingressClassName` may\nbe specified."

### fn spec.acme.solvers.http01.ingress.withServiceType

```ts
withServiceType(serviceType)
```

"Optional service type for Kubernetes solver service. Supported values\nare NodePort or ClusterIP. If unset, defaults to NodePort."

## obj spec.acme.solvers.http01.ingress.ingressTemplate

"Optional ingress template used to configure the ACME challenge solver\ningress used for HTTP01 challenges."

## obj spec.acme.solvers.http01.ingress.ingressTemplate.metadata

"ObjectMeta overrides for the ingress used to solve HTTP01 challenges.\nOnly the 'labels' and 'annotations' fields may be set.\nIf labels or annotations overlap with in-built values, the values here\nwill override the in-built values."

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

"Optional pod template used to configure the ACME challenge solver pods\nused for HTTP01 challenges."

## obj spec.acme.solvers.http01.ingress.podTemplate.metadata

"ObjectMeta overrides for the pod used to solve HTTP01 challenges.\nOnly the 'labels' and 'annotations' fields may be set.\nIf labels or annotations overlap with in-built values, the values here\nwill override the in-built values."

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

"PodSpec defines overrides for the HTTP01 challenge solver pod.\nCheck ACMEChallengeSolverHTTP01IngressPodSpec to find out currently supported fields.\nAll other fields will be ignored."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.withImagePullSecrets

```ts
withImagePullSecrets(imagePullSecrets)
```

"If specified, the pod's imagePullSecrets"

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.withImagePullSecretsMixin

```ts
withImagePullSecretsMixin(imagePullSecrets)
```

"If specified, the pod's imagePullSecrets"

**Note:** This function appends passed data to existing values

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.withNodeSelector

```ts
withNodeSelector(nodeSelector)
```

"NodeSelector is a selector which must be true for the pod to fit on a node.\nSelector which must match a node's labels for the pod to be scheduled on that node.\nMore info: https://kubernetes.io/docs/concepts/configuration/assign-pod-node/"

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.withNodeSelectorMixin

```ts
withNodeSelectorMixin(nodeSelector)
```

"NodeSelector is a selector which must be true for the pod to fit on a node.\nSelector which must match a node's labels for the pod to be scheduled on that node.\nMore info: https://kubernetes.io/docs/concepts/configuration/assign-pod-node/"

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

"The scheduler will prefer to schedule pods to nodes that satisfy\nthe affinity expressions specified by this field, but it may choose\na node that violates one or more of the expressions. The node that is\nmost preferred is the one with the greatest sum of weights, i.e.\nfor each node that meets all of the scheduling requirements (resource\nrequest, requiredDuringScheduling affinity expressions, etc.),\ncompute a sum by iterating through the elements of this field and adding\n\"weight\" to the sum if the node matches the corresponding matchExpressions; the\nnode(s) with the highest sum are the most preferred."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.withPreferredDuringSchedulingIgnoredDuringExecutionMixin

```ts
withPreferredDuringSchedulingIgnoredDuringExecutionMixin(preferredDuringSchedulingIgnoredDuringExecution)
```

"The scheduler will prefer to schedule pods to nodes that satisfy\nthe affinity expressions specified by this field, but it may choose\na node that violates one or more of the expressions. The node that is\nmost preferred is the one with the greatest sum of weights, i.e.\nfor each node that meets all of the scheduling requirements (resource\nrequest, requiredDuringScheduling affinity expressions, etc.),\ncompute a sum by iterating through the elements of this field and adding\n\"weight\" to the sum if the node matches the corresponding matchExpressions; the\nnode(s) with the highest sum are the most preferred."

**Note:** This function appends passed data to existing values

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution

"The scheduler will prefer to schedule pods to nodes that satisfy\nthe affinity expressions specified by this field, but it may choose\na node that violates one or more of the expressions. The node that is\nmost preferred is the one with the greatest sum of weights, i.e.\nfor each node that meets all of the scheduling requirements (resource\nrequest, requiredDuringScheduling affinity expressions, etc.),\ncompute a sum by iterating through the elements of this field and adding\n\"weight\" to the sum if the node matches the corresponding matchExpressions; the\nnode(s) with the highest sum are the most preferred."

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

"Represents a key's relationship to a set of values.\nValid operators are In, NotIn, Exists, DoesNotExist. Gt, and Lt."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution.preference.matchExpressions.withValues

```ts
withValues(values)
```

"An array of string values. If the operator is In or NotIn,\nthe values array must be non-empty. If the operator is Exists or DoesNotExist,\nthe values array must be empty. If the operator is Gt or Lt, the values\narray must have a single element, which will be interpreted as an integer.\nThis array is replaced during a strategic merge patch."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution.preference.matchExpressions.withValuesMixin

```ts
withValuesMixin(values)
```

"An array of string values. If the operator is In or NotIn,\nthe values array must be non-empty. If the operator is Exists or DoesNotExist,\nthe values array must be empty. If the operator is Gt or Lt, the values\narray must have a single element, which will be interpreted as an integer.\nThis array is replaced during a strategic merge patch."

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

"Represents a key's relationship to a set of values.\nValid operators are In, NotIn, Exists, DoesNotExist. Gt, and Lt."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution.preference.matchFields.withValues

```ts
withValues(values)
```

"An array of string values. If the operator is In or NotIn,\nthe values array must be non-empty. If the operator is Exists or DoesNotExist,\nthe values array must be empty. If the operator is Gt or Lt, the values\narray must have a single element, which will be interpreted as an integer.\nThis array is replaced during a strategic merge patch."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution.preference.matchFields.withValuesMixin

```ts
withValuesMixin(values)
```

"An array of string values. If the operator is In or NotIn,\nthe values array must be non-empty. If the operator is Exists or DoesNotExist,\nthe values array must be empty. If the operator is Gt or Lt, the values\narray must have a single element, which will be interpreted as an integer.\nThis array is replaced during a strategic merge patch."

**Note:** This function appends passed data to existing values

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution

"If the affinity requirements specified by this field are not met at\nscheduling time, the pod will not be scheduled onto the node.\nIf the affinity requirements specified by this field cease to be met\nat some point during pod execution (e.g. due to an update), the system\nmay or may not try to eventually evict the pod from its node."

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

"Represents a key's relationship to a set of values.\nValid operators are In, NotIn, Exists, DoesNotExist. Gt, and Lt."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.nodeSelectorTerms.matchExpressions.withValues

```ts
withValues(values)
```

"An array of string values. If the operator is In or NotIn,\nthe values array must be non-empty. If the operator is Exists or DoesNotExist,\nthe values array must be empty. If the operator is Gt or Lt, the values\narray must have a single element, which will be interpreted as an integer.\nThis array is replaced during a strategic merge patch."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.nodeSelectorTerms.matchExpressions.withValuesMixin

```ts
withValuesMixin(values)
```

"An array of string values. If the operator is In or NotIn,\nthe values array must be non-empty. If the operator is Exists or DoesNotExist,\nthe values array must be empty. If the operator is Gt or Lt, the values\narray must have a single element, which will be interpreted as an integer.\nThis array is replaced during a strategic merge patch."

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

"Represents a key's relationship to a set of values.\nValid operators are In, NotIn, Exists, DoesNotExist. Gt, and Lt."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.nodeSelectorTerms.matchFields.withValues

```ts
withValues(values)
```

"An array of string values. If the operator is In or NotIn,\nthe values array must be non-empty. If the operator is Exists or DoesNotExist,\nthe values array must be empty. If the operator is Gt or Lt, the values\narray must have a single element, which will be interpreted as an integer.\nThis array is replaced during a strategic merge patch."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.nodeSelectorTerms.matchFields.withValuesMixin

```ts
withValuesMixin(values)
```

"An array of string values. If the operator is In or NotIn,\nthe values array must be non-empty. If the operator is Exists or DoesNotExist,\nthe values array must be empty. If the operator is Gt or Lt, the values\narray must have a single element, which will be interpreted as an integer.\nThis array is replaced during a strategic merge patch."

**Note:** This function appends passed data to existing values

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity

"Describes pod affinity scheduling rules (e.g. co-locate this pod in the same node, zone, etc. as some other pod(s))."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.withPreferredDuringSchedulingIgnoredDuringExecution

```ts
withPreferredDuringSchedulingIgnoredDuringExecution(preferredDuringSchedulingIgnoredDuringExecution)
```

"The scheduler will prefer to schedule pods to nodes that satisfy\nthe affinity expressions specified by this field, but it may choose\na node that violates one or more of the expressions. The node that is\nmost preferred is the one with the greatest sum of weights, i.e.\nfor each node that meets all of the scheduling requirements (resource\nrequest, requiredDuringScheduling affinity expressions, etc.),\ncompute a sum by iterating through the elements of this field and adding\n\"weight\" to the sum if the node has pods which matches the corresponding podAffinityTerm; the\nnode(s) with the highest sum are the most preferred."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.withPreferredDuringSchedulingIgnoredDuringExecutionMixin

```ts
withPreferredDuringSchedulingIgnoredDuringExecutionMixin(preferredDuringSchedulingIgnoredDuringExecution)
```

"The scheduler will prefer to schedule pods to nodes that satisfy\nthe affinity expressions specified by this field, but it may choose\na node that violates one or more of the expressions. The node that is\nmost preferred is the one with the greatest sum of weights, i.e.\nfor each node that meets all of the scheduling requirements (resource\nrequest, requiredDuringScheduling affinity expressions, etc.),\ncompute a sum by iterating through the elements of this field and adding\n\"weight\" to the sum if the node has pods which matches the corresponding podAffinityTerm; the\nnode(s) with the highest sum are the most preferred."

**Note:** This function appends passed data to existing values

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.withRequiredDuringSchedulingIgnoredDuringExecution

```ts
withRequiredDuringSchedulingIgnoredDuringExecution(requiredDuringSchedulingIgnoredDuringExecution)
```

"If the affinity requirements specified by this field are not met at\nscheduling time, the pod will not be scheduled onto the node.\nIf the affinity requirements specified by this field cease to be met\nat some point during pod execution (e.g. due to a pod label update), the\nsystem may or may not try to eventually evict the pod from its node.\nWhen there are multiple elements, the lists of nodes corresponding to each\npodAffinityTerm are intersected, i.e. all terms must be satisfied."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.withRequiredDuringSchedulingIgnoredDuringExecutionMixin

```ts
withRequiredDuringSchedulingIgnoredDuringExecutionMixin(requiredDuringSchedulingIgnoredDuringExecution)
```

"If the affinity requirements specified by this field are not met at\nscheduling time, the pod will not be scheduled onto the node.\nIf the affinity requirements specified by this field cease to be met\nat some point during pod execution (e.g. due to a pod label update), the\nsystem may or may not try to eventually evict the pod from its node.\nWhen there are multiple elements, the lists of nodes corresponding to each\npodAffinityTerm are intersected, i.e. all terms must be satisfied."

**Note:** This function appends passed data to existing values

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution

"The scheduler will prefer to schedule pods to nodes that satisfy\nthe affinity expressions specified by this field, but it may choose\na node that violates one or more of the expressions. The node that is\nmost preferred is the one with the greatest sum of weights, i.e.\nfor each node that meets all of the scheduling requirements (resource\nrequest, requiredDuringScheduling affinity expressions, etc.),\ncompute a sum by iterating through the elements of this field and adding\n\"weight\" to the sum if the node has pods which matches the corresponding podAffinityTerm; the\nnode(s) with the highest sum are the most preferred."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.withWeight

```ts
withWeight(weight)
```

"weight associated with matching the corresponding podAffinityTerm,\nin the range 1-100."

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm

"Required. A pod affinity term, associated with the corresponding weight."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.withMatchLabelKeys

```ts
withMatchLabelKeys(matchLabelKeys)
```

"MatchLabelKeys is a set of pod label keys to select which pods will\nbe taken into consideration. The keys are used to lookup values from the\nincoming pod labels, those key-value labels are merged with `labelSelector` as `key in (value)`\nto select the group of existing pods which pods will be taken into consideration\nfor the incoming pod's pod (anti) affinity. Keys that don't exist in the incoming\npod labels will be ignored. The default value is empty.\nThe same key is forbidden to exist in both matchLabelKeys and labelSelector.\nAlso, matchLabelKeys cannot be set when labelSelector isn't set.\nThis is an alpha field and requires enabling MatchLabelKeysInPodAffinity feature gate."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.withMatchLabelKeysMixin

```ts
withMatchLabelKeysMixin(matchLabelKeys)
```

"MatchLabelKeys is a set of pod label keys to select which pods will\nbe taken into consideration. The keys are used to lookup values from the\nincoming pod labels, those key-value labels are merged with `labelSelector` as `key in (value)`\nto select the group of existing pods which pods will be taken into consideration\nfor the incoming pod's pod (anti) affinity. Keys that don't exist in the incoming\npod labels will be ignored. The default value is empty.\nThe same key is forbidden to exist in both matchLabelKeys and labelSelector.\nAlso, matchLabelKeys cannot be set when labelSelector isn't set.\nThis is an alpha field and requires enabling MatchLabelKeysInPodAffinity feature gate."

**Note:** This function appends passed data to existing values

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.withMismatchLabelKeys

```ts
withMismatchLabelKeys(mismatchLabelKeys)
```

"MismatchLabelKeys is a set of pod label keys to select which pods will\nbe taken into consideration. The keys are used to lookup values from the\nincoming pod labels, those key-value labels are merged with `labelSelector` as `key notin (value)`\nto select the group of existing pods which pods will be taken into consideration\nfor the incoming pod's pod (anti) affinity. Keys that don't exist in the incoming\npod labels will be ignored. The default value is empty.\nThe same key is forbidden to exist in both mismatchLabelKeys and labelSelector.\nAlso, mismatchLabelKeys cannot be set when labelSelector isn't set.\nThis is an alpha field and requires enabling MatchLabelKeysInPodAffinity feature gate."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.withMismatchLabelKeysMixin

```ts
withMismatchLabelKeysMixin(mismatchLabelKeys)
```

"MismatchLabelKeys is a set of pod label keys to select which pods will\nbe taken into consideration. The keys are used to lookup values from the\nincoming pod labels, those key-value labels are merged with `labelSelector` as `key notin (value)`\nto select the group of existing pods which pods will be taken into consideration\nfor the incoming pod's pod (anti) affinity. Keys that don't exist in the incoming\npod labels will be ignored. The default value is empty.\nThe same key is forbidden to exist in both mismatchLabelKeys and labelSelector.\nAlso, mismatchLabelKeys cannot be set when labelSelector isn't set.\nThis is an alpha field and requires enabling MatchLabelKeysInPodAffinity feature gate."

**Note:** This function appends passed data to existing values

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.withNamespaces

```ts
withNamespaces(namespaces)
```

"namespaces specifies a static list of namespace names that the term applies to.\nThe term is applied to the union of the namespaces listed in this field\nand the ones selected by namespaceSelector.\nnull or empty namespaces list and null namespaceSelector means \"this pod's namespace\"."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.withNamespacesMixin

```ts
withNamespacesMixin(namespaces)
```

"namespaces specifies a static list of namespace names that the term applies to.\nThe term is applied to the union of the namespaces listed in this field\nand the ones selected by namespaceSelector.\nnull or empty namespaces list and null namespaceSelector means \"this pod's namespace\"."

**Note:** This function appends passed data to existing values

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.withTopologyKey

```ts
withTopologyKey(topologyKey)
```

"This pod should be co-located (affinity) or not co-located (anti-affinity) with the pods matching\nthe labelSelector in the specified namespaces, where co-located is defined as running on a node\nwhose value of the label with key topologyKey matches that of any node on which any of the\nselected pods is running.\nEmpty topologyKey is not allowed."

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector

"A label query over a set of resources, in this case pods.\nIf it's null, this PodAffinityTerm matches with no Pods."

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

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels\nmap is equivalent to an element of matchExpressions, whose key field is \"key\", the\noperator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels\nmap is equivalent to an element of matchExpressions, whose key field is \"key\", the\noperator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

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

"operator represents a key's relationship to a set of values.\nValid operators are In, NotIn, Exists and DoesNotExist."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.matchExpressions.withValues

```ts
withValues(values)
```

"values is an array of string values. If the operator is In or NotIn,\nthe values array must be non-empty. If the operator is Exists or DoesNotExist,\nthe values array must be empty. This array is replaced during a strategic\nmerge patch."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.matchExpressions.withValuesMixin

```ts
withValuesMixin(values)
```

"values is an array of string values. If the operator is In or NotIn,\nthe values array must be non-empty. If the operator is Exists or DoesNotExist,\nthe values array must be empty. This array is replaced during a strategic\nmerge patch."

**Note:** This function appends passed data to existing values

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector

"A label query over the set of namespaces that the term applies to.\nThe term is applied to the union of the namespaces selected by this field\nand the ones listed in the namespaces field.\nnull selector and null or empty namespaces list means \"this pod's namespace\".\nAn empty selector ({}) matches all namespaces."

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

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels\nmap is equivalent to an element of matchExpressions, whose key field is \"key\", the\noperator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels\nmap is equivalent to an element of matchExpressions, whose key field is \"key\", the\noperator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

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

"operator represents a key's relationship to a set of values.\nValid operators are In, NotIn, Exists and DoesNotExist."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.matchExpressions.withValues

```ts
withValues(values)
```

"values is an array of string values. If the operator is In or NotIn,\nthe values array must be non-empty. If the operator is Exists or DoesNotExist,\nthe values array must be empty. This array is replaced during a strategic\nmerge patch."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.matchExpressions.withValuesMixin

```ts
withValuesMixin(values)
```

"values is an array of string values. If the operator is In or NotIn,\nthe values array must be non-empty. If the operator is Exists or DoesNotExist,\nthe values array must be empty. This array is replaced during a strategic\nmerge patch."

**Note:** This function appends passed data to existing values

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution

"If the affinity requirements specified by this field are not met at\nscheduling time, the pod will not be scheduled onto the node.\nIf the affinity requirements specified by this field cease to be met\nat some point during pod execution (e.g. due to a pod label update), the\nsystem may or may not try to eventually evict the pod from its node.\nWhen there are multiple elements, the lists of nodes corresponding to each\npodAffinityTerm are intersected, i.e. all terms must be satisfied."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.withMatchLabelKeys

```ts
withMatchLabelKeys(matchLabelKeys)
```

"MatchLabelKeys is a set of pod label keys to select which pods will\nbe taken into consideration. The keys are used to lookup values from the\nincoming pod labels, those key-value labels are merged with `labelSelector` as `key in (value)`\nto select the group of existing pods which pods will be taken into consideration\nfor the incoming pod's pod (anti) affinity. Keys that don't exist in the incoming\npod labels will be ignored. The default value is empty.\nThe same key is forbidden to exist in both matchLabelKeys and labelSelector.\nAlso, matchLabelKeys cannot be set when labelSelector isn't set.\nThis is an alpha field and requires enabling MatchLabelKeysInPodAffinity feature gate."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.withMatchLabelKeysMixin

```ts
withMatchLabelKeysMixin(matchLabelKeys)
```

"MatchLabelKeys is a set of pod label keys to select which pods will\nbe taken into consideration. The keys are used to lookup values from the\nincoming pod labels, those key-value labels are merged with `labelSelector` as `key in (value)`\nto select the group of existing pods which pods will be taken into consideration\nfor the incoming pod's pod (anti) affinity. Keys that don't exist in the incoming\npod labels will be ignored. The default value is empty.\nThe same key is forbidden to exist in both matchLabelKeys and labelSelector.\nAlso, matchLabelKeys cannot be set when labelSelector isn't set.\nThis is an alpha field and requires enabling MatchLabelKeysInPodAffinity feature gate."

**Note:** This function appends passed data to existing values

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.withMismatchLabelKeys

```ts
withMismatchLabelKeys(mismatchLabelKeys)
```

"MismatchLabelKeys is a set of pod label keys to select which pods will\nbe taken into consideration. The keys are used to lookup values from the\nincoming pod labels, those key-value labels are merged with `labelSelector` as `key notin (value)`\nto select the group of existing pods which pods will be taken into consideration\nfor the incoming pod's pod (anti) affinity. Keys that don't exist in the incoming\npod labels will be ignored. The default value is empty.\nThe same key is forbidden to exist in both mismatchLabelKeys and labelSelector.\nAlso, mismatchLabelKeys cannot be set when labelSelector isn't set.\nThis is an alpha field and requires enabling MatchLabelKeysInPodAffinity feature gate."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.withMismatchLabelKeysMixin

```ts
withMismatchLabelKeysMixin(mismatchLabelKeys)
```

"MismatchLabelKeys is a set of pod label keys to select which pods will\nbe taken into consideration. The keys are used to lookup values from the\nincoming pod labels, those key-value labels are merged with `labelSelector` as `key notin (value)`\nto select the group of existing pods which pods will be taken into consideration\nfor the incoming pod's pod (anti) affinity. Keys that don't exist in the incoming\npod labels will be ignored. The default value is empty.\nThe same key is forbidden to exist in both mismatchLabelKeys and labelSelector.\nAlso, mismatchLabelKeys cannot be set when labelSelector isn't set.\nThis is an alpha field and requires enabling MatchLabelKeysInPodAffinity feature gate."

**Note:** This function appends passed data to existing values

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.withNamespaces

```ts
withNamespaces(namespaces)
```

"namespaces specifies a static list of namespace names that the term applies to.\nThe term is applied to the union of the namespaces listed in this field\nand the ones selected by namespaceSelector.\nnull or empty namespaces list and null namespaceSelector means \"this pod's namespace\"."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.withNamespacesMixin

```ts
withNamespacesMixin(namespaces)
```

"namespaces specifies a static list of namespace names that the term applies to.\nThe term is applied to the union of the namespaces listed in this field\nand the ones selected by namespaceSelector.\nnull or empty namespaces list and null namespaceSelector means \"this pod's namespace\"."

**Note:** This function appends passed data to existing values

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.withTopologyKey

```ts
withTopologyKey(topologyKey)
```

"This pod should be co-located (affinity) or not co-located (anti-affinity) with the pods matching\nthe labelSelector in the specified namespaces, where co-located is defined as running on a node\nwhose value of the label with key topologyKey matches that of any node on which any of the\nselected pods is running.\nEmpty topologyKey is not allowed."

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector

"A label query over a set of resources, in this case pods.\nIf it's null, this PodAffinityTerm matches with no Pods."

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

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels\nmap is equivalent to an element of matchExpressions, whose key field is \"key\", the\noperator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels\nmap is equivalent to an element of matchExpressions, whose key field is \"key\", the\noperator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

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

"operator represents a key's relationship to a set of values.\nValid operators are In, NotIn, Exists and DoesNotExist."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.matchExpressions.withValues

```ts
withValues(values)
```

"values is an array of string values. If the operator is In or NotIn,\nthe values array must be non-empty. If the operator is Exists or DoesNotExist,\nthe values array must be empty. This array is replaced during a strategic\nmerge patch."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.matchExpressions.withValuesMixin

```ts
withValuesMixin(values)
```

"values is an array of string values. If the operator is In or NotIn,\nthe values array must be non-empty. If the operator is Exists or DoesNotExist,\nthe values array must be empty. This array is replaced during a strategic\nmerge patch."

**Note:** This function appends passed data to existing values

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector

"A label query over the set of namespaces that the term applies to.\nThe term is applied to the union of the namespaces selected by this field\nand the ones listed in the namespaces field.\nnull selector and null or empty namespaces list means \"this pod's namespace\".\nAn empty selector ({}) matches all namespaces."

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

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels\nmap is equivalent to an element of matchExpressions, whose key field is \"key\", the\noperator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels\nmap is equivalent to an element of matchExpressions, whose key field is \"key\", the\noperator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

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

"operator represents a key's relationship to a set of values.\nValid operators are In, NotIn, Exists and DoesNotExist."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.matchExpressions.withValues

```ts
withValues(values)
```

"values is an array of string values. If the operator is In or NotIn,\nthe values array must be non-empty. If the operator is Exists or DoesNotExist,\nthe values array must be empty. This array is replaced during a strategic\nmerge patch."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.matchExpressions.withValuesMixin

```ts
withValuesMixin(values)
```

"values is an array of string values. If the operator is In or NotIn,\nthe values array must be non-empty. If the operator is Exists or DoesNotExist,\nthe values array must be empty. This array is replaced during a strategic\nmerge patch."

**Note:** This function appends passed data to existing values

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity

"Describes pod anti-affinity scheduling rules (e.g. avoid putting this pod in the same node, zone, etc. as some other pod(s))."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.withPreferredDuringSchedulingIgnoredDuringExecution

```ts
withPreferredDuringSchedulingIgnoredDuringExecution(preferredDuringSchedulingIgnoredDuringExecution)
```

"The scheduler will prefer to schedule pods to nodes that satisfy\nthe anti-affinity expressions specified by this field, but it may choose\na node that violates one or more of the expressions. The node that is\nmost preferred is the one with the greatest sum of weights, i.e.\nfor each node that meets all of the scheduling requirements (resource\nrequest, requiredDuringScheduling anti-affinity expressions, etc.),\ncompute a sum by iterating through the elements of this field and adding\n\"weight\" to the sum if the node has pods which matches the corresponding podAffinityTerm; the\nnode(s) with the highest sum are the most preferred."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.withPreferredDuringSchedulingIgnoredDuringExecutionMixin

```ts
withPreferredDuringSchedulingIgnoredDuringExecutionMixin(preferredDuringSchedulingIgnoredDuringExecution)
```

"The scheduler will prefer to schedule pods to nodes that satisfy\nthe anti-affinity expressions specified by this field, but it may choose\na node that violates one or more of the expressions. The node that is\nmost preferred is the one with the greatest sum of weights, i.e.\nfor each node that meets all of the scheduling requirements (resource\nrequest, requiredDuringScheduling anti-affinity expressions, etc.),\ncompute a sum by iterating through the elements of this field and adding\n\"weight\" to the sum if the node has pods which matches the corresponding podAffinityTerm; the\nnode(s) with the highest sum are the most preferred."

**Note:** This function appends passed data to existing values

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.withRequiredDuringSchedulingIgnoredDuringExecution

```ts
withRequiredDuringSchedulingIgnoredDuringExecution(requiredDuringSchedulingIgnoredDuringExecution)
```

"If the anti-affinity requirements specified by this field are not met at\nscheduling time, the pod will not be scheduled onto the node.\nIf the anti-affinity requirements specified by this field cease to be met\nat some point during pod execution (e.g. due to a pod label update), the\nsystem may or may not try to eventually evict the pod from its node.\nWhen there are multiple elements, the lists of nodes corresponding to each\npodAffinityTerm are intersected, i.e. all terms must be satisfied."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.withRequiredDuringSchedulingIgnoredDuringExecutionMixin

```ts
withRequiredDuringSchedulingIgnoredDuringExecutionMixin(requiredDuringSchedulingIgnoredDuringExecution)
```

"If the anti-affinity requirements specified by this field are not met at\nscheduling time, the pod will not be scheduled onto the node.\nIf the anti-affinity requirements specified by this field cease to be met\nat some point during pod execution (e.g. due to a pod label update), the\nsystem may or may not try to eventually evict the pod from its node.\nWhen there are multiple elements, the lists of nodes corresponding to each\npodAffinityTerm are intersected, i.e. all terms must be satisfied."

**Note:** This function appends passed data to existing values

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution

"The scheduler will prefer to schedule pods to nodes that satisfy\nthe anti-affinity expressions specified by this field, but it may choose\na node that violates one or more of the expressions. The node that is\nmost preferred is the one with the greatest sum of weights, i.e.\nfor each node that meets all of the scheduling requirements (resource\nrequest, requiredDuringScheduling anti-affinity expressions, etc.),\ncompute a sum by iterating through the elements of this field and adding\n\"weight\" to the sum if the node has pods which matches the corresponding podAffinityTerm; the\nnode(s) with the highest sum are the most preferred."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.withWeight

```ts
withWeight(weight)
```

"weight associated with matching the corresponding podAffinityTerm,\nin the range 1-100."

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm

"Required. A pod affinity term, associated with the corresponding weight."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.withMatchLabelKeys

```ts
withMatchLabelKeys(matchLabelKeys)
```

"MatchLabelKeys is a set of pod label keys to select which pods will\nbe taken into consideration. The keys are used to lookup values from the\nincoming pod labels, those key-value labels are merged with `labelSelector` as `key in (value)`\nto select the group of existing pods which pods will be taken into consideration\nfor the incoming pod's pod (anti) affinity. Keys that don't exist in the incoming\npod labels will be ignored. The default value is empty.\nThe same key is forbidden to exist in both matchLabelKeys and labelSelector.\nAlso, matchLabelKeys cannot be set when labelSelector isn't set.\nThis is an alpha field and requires enabling MatchLabelKeysInPodAffinity feature gate."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.withMatchLabelKeysMixin

```ts
withMatchLabelKeysMixin(matchLabelKeys)
```

"MatchLabelKeys is a set of pod label keys to select which pods will\nbe taken into consideration. The keys are used to lookup values from the\nincoming pod labels, those key-value labels are merged with `labelSelector` as `key in (value)`\nto select the group of existing pods which pods will be taken into consideration\nfor the incoming pod's pod (anti) affinity. Keys that don't exist in the incoming\npod labels will be ignored. The default value is empty.\nThe same key is forbidden to exist in both matchLabelKeys and labelSelector.\nAlso, matchLabelKeys cannot be set when labelSelector isn't set.\nThis is an alpha field and requires enabling MatchLabelKeysInPodAffinity feature gate."

**Note:** This function appends passed data to existing values

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.withMismatchLabelKeys

```ts
withMismatchLabelKeys(mismatchLabelKeys)
```

"MismatchLabelKeys is a set of pod label keys to select which pods will\nbe taken into consideration. The keys are used to lookup values from the\nincoming pod labels, those key-value labels are merged with `labelSelector` as `key notin (value)`\nto select the group of existing pods which pods will be taken into consideration\nfor the incoming pod's pod (anti) affinity. Keys that don't exist in the incoming\npod labels will be ignored. The default value is empty.\nThe same key is forbidden to exist in both mismatchLabelKeys and labelSelector.\nAlso, mismatchLabelKeys cannot be set when labelSelector isn't set.\nThis is an alpha field and requires enabling MatchLabelKeysInPodAffinity feature gate."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.withMismatchLabelKeysMixin

```ts
withMismatchLabelKeysMixin(mismatchLabelKeys)
```

"MismatchLabelKeys is a set of pod label keys to select which pods will\nbe taken into consideration. The keys are used to lookup values from the\nincoming pod labels, those key-value labels are merged with `labelSelector` as `key notin (value)`\nto select the group of existing pods which pods will be taken into consideration\nfor the incoming pod's pod (anti) affinity. Keys that don't exist in the incoming\npod labels will be ignored. The default value is empty.\nThe same key is forbidden to exist in both mismatchLabelKeys and labelSelector.\nAlso, mismatchLabelKeys cannot be set when labelSelector isn't set.\nThis is an alpha field and requires enabling MatchLabelKeysInPodAffinity feature gate."

**Note:** This function appends passed data to existing values

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.withNamespaces

```ts
withNamespaces(namespaces)
```

"namespaces specifies a static list of namespace names that the term applies to.\nThe term is applied to the union of the namespaces listed in this field\nand the ones selected by namespaceSelector.\nnull or empty namespaces list and null namespaceSelector means \"this pod's namespace\"."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.withNamespacesMixin

```ts
withNamespacesMixin(namespaces)
```

"namespaces specifies a static list of namespace names that the term applies to.\nThe term is applied to the union of the namespaces listed in this field\nand the ones selected by namespaceSelector.\nnull or empty namespaces list and null namespaceSelector means \"this pod's namespace\"."

**Note:** This function appends passed data to existing values

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.withTopologyKey

```ts
withTopologyKey(topologyKey)
```

"This pod should be co-located (affinity) or not co-located (anti-affinity) with the pods matching\nthe labelSelector in the specified namespaces, where co-located is defined as running on a node\nwhose value of the label with key topologyKey matches that of any node on which any of the\nselected pods is running.\nEmpty topologyKey is not allowed."

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector

"A label query over a set of resources, in this case pods.\nIf it's null, this PodAffinityTerm matches with no Pods."

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

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels\nmap is equivalent to an element of matchExpressions, whose key field is \"key\", the\noperator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels\nmap is equivalent to an element of matchExpressions, whose key field is \"key\", the\noperator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

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

"operator represents a key's relationship to a set of values.\nValid operators are In, NotIn, Exists and DoesNotExist."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.matchExpressions.withValues

```ts
withValues(values)
```

"values is an array of string values. If the operator is In or NotIn,\nthe values array must be non-empty. If the operator is Exists or DoesNotExist,\nthe values array must be empty. This array is replaced during a strategic\nmerge patch."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.matchExpressions.withValuesMixin

```ts
withValuesMixin(values)
```

"values is an array of string values. If the operator is In or NotIn,\nthe values array must be non-empty. If the operator is Exists or DoesNotExist,\nthe values array must be empty. This array is replaced during a strategic\nmerge patch."

**Note:** This function appends passed data to existing values

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector

"A label query over the set of namespaces that the term applies to.\nThe term is applied to the union of the namespaces selected by this field\nand the ones listed in the namespaces field.\nnull selector and null or empty namespaces list means \"this pod's namespace\".\nAn empty selector ({}) matches all namespaces."

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

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels\nmap is equivalent to an element of matchExpressions, whose key field is \"key\", the\noperator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels\nmap is equivalent to an element of matchExpressions, whose key field is \"key\", the\noperator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

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

"operator represents a key's relationship to a set of values.\nValid operators are In, NotIn, Exists and DoesNotExist."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.matchExpressions.withValues

```ts
withValues(values)
```

"values is an array of string values. If the operator is In or NotIn,\nthe values array must be non-empty. If the operator is Exists or DoesNotExist,\nthe values array must be empty. This array is replaced during a strategic\nmerge patch."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.matchExpressions.withValuesMixin

```ts
withValuesMixin(values)
```

"values is an array of string values. If the operator is In or NotIn,\nthe values array must be non-empty. If the operator is Exists or DoesNotExist,\nthe values array must be empty. This array is replaced during a strategic\nmerge patch."

**Note:** This function appends passed data to existing values

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution

"If the anti-affinity requirements specified by this field are not met at\nscheduling time, the pod will not be scheduled onto the node.\nIf the anti-affinity requirements specified by this field cease to be met\nat some point during pod execution (e.g. due to a pod label update), the\nsystem may or may not try to eventually evict the pod from its node.\nWhen there are multiple elements, the lists of nodes corresponding to each\npodAffinityTerm are intersected, i.e. all terms must be satisfied."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.withMatchLabelKeys

```ts
withMatchLabelKeys(matchLabelKeys)
```

"MatchLabelKeys is a set of pod label keys to select which pods will\nbe taken into consideration. The keys are used to lookup values from the\nincoming pod labels, those key-value labels are merged with `labelSelector` as `key in (value)`\nto select the group of existing pods which pods will be taken into consideration\nfor the incoming pod's pod (anti) affinity. Keys that don't exist in the incoming\npod labels will be ignored. The default value is empty.\nThe same key is forbidden to exist in both matchLabelKeys and labelSelector.\nAlso, matchLabelKeys cannot be set when labelSelector isn't set.\nThis is an alpha field and requires enabling MatchLabelKeysInPodAffinity feature gate."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.withMatchLabelKeysMixin

```ts
withMatchLabelKeysMixin(matchLabelKeys)
```

"MatchLabelKeys is a set of pod label keys to select which pods will\nbe taken into consideration. The keys are used to lookup values from the\nincoming pod labels, those key-value labels are merged with `labelSelector` as `key in (value)`\nto select the group of existing pods which pods will be taken into consideration\nfor the incoming pod's pod (anti) affinity. Keys that don't exist in the incoming\npod labels will be ignored. The default value is empty.\nThe same key is forbidden to exist in both matchLabelKeys and labelSelector.\nAlso, matchLabelKeys cannot be set when labelSelector isn't set.\nThis is an alpha field and requires enabling MatchLabelKeysInPodAffinity feature gate."

**Note:** This function appends passed data to existing values

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.withMismatchLabelKeys

```ts
withMismatchLabelKeys(mismatchLabelKeys)
```

"MismatchLabelKeys is a set of pod label keys to select which pods will\nbe taken into consideration. The keys are used to lookup values from the\nincoming pod labels, those key-value labels are merged with `labelSelector` as `key notin (value)`\nto select the group of existing pods which pods will be taken into consideration\nfor the incoming pod's pod (anti) affinity. Keys that don't exist in the incoming\npod labels will be ignored. The default value is empty.\nThe same key is forbidden to exist in both mismatchLabelKeys and labelSelector.\nAlso, mismatchLabelKeys cannot be set when labelSelector isn't set.\nThis is an alpha field and requires enabling MatchLabelKeysInPodAffinity feature gate."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.withMismatchLabelKeysMixin

```ts
withMismatchLabelKeysMixin(mismatchLabelKeys)
```

"MismatchLabelKeys is a set of pod label keys to select which pods will\nbe taken into consideration. The keys are used to lookup values from the\nincoming pod labels, those key-value labels are merged with `labelSelector` as `key notin (value)`\nto select the group of existing pods which pods will be taken into consideration\nfor the incoming pod's pod (anti) affinity. Keys that don't exist in the incoming\npod labels will be ignored. The default value is empty.\nThe same key is forbidden to exist in both mismatchLabelKeys and labelSelector.\nAlso, mismatchLabelKeys cannot be set when labelSelector isn't set.\nThis is an alpha field and requires enabling MatchLabelKeysInPodAffinity feature gate."

**Note:** This function appends passed data to existing values

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.withNamespaces

```ts
withNamespaces(namespaces)
```

"namespaces specifies a static list of namespace names that the term applies to.\nThe term is applied to the union of the namespaces listed in this field\nand the ones selected by namespaceSelector.\nnull or empty namespaces list and null namespaceSelector means \"this pod's namespace\"."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.withNamespacesMixin

```ts
withNamespacesMixin(namespaces)
```

"namespaces specifies a static list of namespace names that the term applies to.\nThe term is applied to the union of the namespaces listed in this field\nand the ones selected by namespaceSelector.\nnull or empty namespaces list and null namespaceSelector means \"this pod's namespace\"."

**Note:** This function appends passed data to existing values

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.withTopologyKey

```ts
withTopologyKey(topologyKey)
```

"This pod should be co-located (affinity) or not co-located (anti-affinity) with the pods matching\nthe labelSelector in the specified namespaces, where co-located is defined as running on a node\nwhose value of the label with key topologyKey matches that of any node on which any of the\nselected pods is running.\nEmpty topologyKey is not allowed."

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector

"A label query over a set of resources, in this case pods.\nIf it's null, this PodAffinityTerm matches with no Pods."

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

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels\nmap is equivalent to an element of matchExpressions, whose key field is \"key\", the\noperator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels\nmap is equivalent to an element of matchExpressions, whose key field is \"key\", the\noperator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

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

"operator represents a key's relationship to a set of values.\nValid operators are In, NotIn, Exists and DoesNotExist."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.matchExpressions.withValues

```ts
withValues(values)
```

"values is an array of string values. If the operator is In or NotIn,\nthe values array must be non-empty. If the operator is Exists or DoesNotExist,\nthe values array must be empty. This array is replaced during a strategic\nmerge patch."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.matchExpressions.withValuesMixin

```ts
withValuesMixin(values)
```

"values is an array of string values. If the operator is In or NotIn,\nthe values array must be non-empty. If the operator is Exists or DoesNotExist,\nthe values array must be empty. This array is replaced during a strategic\nmerge patch."

**Note:** This function appends passed data to existing values

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector

"A label query over the set of namespaces that the term applies to.\nThe term is applied to the union of the namespaces selected by this field\nand the ones listed in the namespaces field.\nnull selector and null or empty namespaces list means \"this pod's namespace\".\nAn empty selector ({}) matches all namespaces."

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

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels\nmap is equivalent to an element of matchExpressions, whose key field is \"key\", the\noperator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels\nmap is equivalent to an element of matchExpressions, whose key field is \"key\", the\noperator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

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

"operator represents a key's relationship to a set of values.\nValid operators are In, NotIn, Exists and DoesNotExist."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.matchExpressions.withValues

```ts
withValues(values)
```

"values is an array of string values. If the operator is In or NotIn,\nthe values array must be non-empty. If the operator is Exists or DoesNotExist,\nthe values array must be empty. This array is replaced during a strategic\nmerge patch."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.matchExpressions.withValuesMixin

```ts
withValuesMixin(values)
```

"values is an array of string values. If the operator is In or NotIn,\nthe values array must be non-empty. If the operator is Exists or DoesNotExist,\nthe values array must be empty. This array is replaced during a strategic\nmerge patch."

**Note:** This function appends passed data to existing values

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.imagePullSecrets

"If specified, the pod's imagePullSecrets"

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.imagePullSecrets.withName

```ts
withName(name)
```

"Name of the referent.\nThis field is effectively required, but due to backwards compatibility is\nallowed to be empty. Instances of this type with an empty value here are\nalmost certainly wrong.\nTODO: Add other useful fields. apiVersion, kind, uid?\nMore info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names\nTODO: Drop `kubebuilder:default` when controller-gen doesn't need it https://github.com/kubernetes-sigs/kubebuilder/issues/3896."

## obj spec.acme.solvers.http01.ingress.podTemplate.spec.tolerations

"If specified, the pod's tolerations."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.tolerations.withEffect

```ts
withEffect(effect)
```

"Effect indicates the taint effect to match. Empty means match all taint effects.\nWhen specified, allowed values are NoSchedule, PreferNoSchedule and NoExecute."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.tolerations.withKey

```ts
withKey(key)
```

"Key is the taint key that the toleration applies to. Empty means match all taint keys.\nIf the key is empty, operator must be Exists; this combination means to match all values and all keys."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.tolerations.withOperator

```ts
withOperator(operator)
```

"Operator represents a key's relationship to the value.\nValid operators are Exists and Equal. Defaults to Equal.\nExists is equivalent to wildcard for value, so that a pod can\ntolerate all taints of a particular category."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.tolerations.withTolerationSeconds

```ts
withTolerationSeconds(tolerationSeconds)
```

"TolerationSeconds represents the period of time the toleration (which must be\nof effect NoExecute, otherwise this field is ignored) tolerates the taint. By default,\nit is not set, which means tolerate the taint forever (do not evict). Zero and\nnegative values will be treated as 0 (evict immediately) by the system."

### fn spec.acme.solvers.http01.ingress.podTemplate.spec.tolerations.withValue

```ts
withValue(value)
```

"Value is the taint value the toleration matches to.\nIf the operator is Exists, the value should be empty, otherwise just a regular string."

## obj spec.acme.solvers.selector

"Selector selects a set of DNSNames on the Certificate resource that\nshould be solved using this challenge solver.\nIf not specified, the solver will be treated as the 'default' solver\nwith the lowest priority, i.e. if any other solver has a more specific\nmatch, it will be used instead."

### fn spec.acme.solvers.selector.withDnsNames

```ts
withDnsNames(dnsNames)
```

"List of DNSNames that this solver will be used to solve.\nIf specified and a match is found, a dnsNames selector will take\nprecedence over a dnsZones selector.\nIf multiple solvers match with the same dnsNames value, the solver\nwith the most matching labels in matchLabels will be selected.\nIf neither has more matches, the solver defined earlier in the list\nwill be selected."

### fn spec.acme.solvers.selector.withDnsNamesMixin

```ts
withDnsNamesMixin(dnsNames)
```

"List of DNSNames that this solver will be used to solve.\nIf specified and a match is found, a dnsNames selector will take\nprecedence over a dnsZones selector.\nIf multiple solvers match with the same dnsNames value, the solver\nwith the most matching labels in matchLabels will be selected.\nIf neither has more matches, the solver defined earlier in the list\nwill be selected."

**Note:** This function appends passed data to existing values

### fn spec.acme.solvers.selector.withDnsZones

```ts
withDnsZones(dnsZones)
```

"List of DNSZones that this solver will be used to solve.\nThe most specific DNS zone match specified here will take precedence\nover other DNS zone matches, so a solver specifying sys.example.com\nwill be selected over one specifying example.com for the domain\nwww.sys.example.com.\nIf multiple solvers match with the same dnsZones value, the solver\nwith the most matching labels in matchLabels will be selected.\nIf neither has more matches, the solver defined earlier in the list\nwill be selected."

### fn spec.acme.solvers.selector.withDnsZonesMixin

```ts
withDnsZonesMixin(dnsZones)
```

"List of DNSZones that this solver will be used to solve.\nThe most specific DNS zone match specified here will take precedence\nover other DNS zone matches, so a solver specifying sys.example.com\nwill be selected over one specifying example.com for the domain\nwww.sys.example.com.\nIf multiple solvers match with the same dnsZones value, the solver\nwith the most matching labels in matchLabels will be selected.\nIf neither has more matches, the solver defined earlier in the list\nwill be selected."

**Note:** This function appends passed data to existing values

### fn spec.acme.solvers.selector.withMatchLabels

```ts
withMatchLabels(matchLabels)
```

"A label selector that is used to refine the set of certificate's that\nthis challenge solver will apply to."

### fn spec.acme.solvers.selector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"A label selector that is used to refine the set of certificate's that\nthis challenge solver will apply to."

**Note:** This function appends passed data to existing values

## obj spec.ca

"CA configures this issuer to sign certificates using a signing CA keypair\nstored in a Secret resource.\nThis is used to build internal PKIs that are managed by cert-manager."

### fn spec.ca.withCrlDistributionPoints

```ts
withCrlDistributionPoints(crlDistributionPoints)
```

"The CRL distribution points is an X.509 v3 certificate extension which identifies\nthe location of the CRL from which the revocation of this certificate can be checked.\nIf not set, certificates will be issued without distribution points set."

### fn spec.ca.withCrlDistributionPointsMixin

```ts
withCrlDistributionPointsMixin(crlDistributionPoints)
```

"The CRL distribution points is an X.509 v3 certificate extension which identifies\nthe location of the CRL from which the revocation of this certificate can be checked.\nIf not set, certificates will be issued without distribution points set."

**Note:** This function appends passed data to existing values

### fn spec.ca.withIssuingCertificateURLs

```ts
withIssuingCertificateURLs(issuingCertificateURLs)
```

"IssuingCertificateURLs is a list of URLs which this issuer should embed into certificates\nit creates. See https://www.rfc-editor.org/rfc/rfc5280#section-4.2.2.1 for more details.\nAs an example, such a URL might be \"http://ca.domain.com/ca.crt\"."

### fn spec.ca.withIssuingCertificateURLsMixin

```ts
withIssuingCertificateURLsMixin(issuingCertificateURLs)
```

"IssuingCertificateURLs is a list of URLs which this issuer should embed into certificates\nit creates. See https://www.rfc-editor.org/rfc/rfc5280#section-4.2.2.1 for more details.\nAs an example, such a URL might be \"http://ca.domain.com/ca.crt\"."

**Note:** This function appends passed data to existing values

### fn spec.ca.withOcspServers

```ts
withOcspServers(ocspServers)
```

"The OCSP server list is an X.509 v3 extension that defines a list of\nURLs of OCSP responders. The OCSP responders can be queried for the\nrevocation status of an issued certificate. If not set, the\ncertificate will be issued with no OCSP servers set. For example, an\nOCSP server URL could be \"http://ocsp.int-x3.letsencrypt.org\"."

### fn spec.ca.withOcspServersMixin

```ts
withOcspServersMixin(ocspServers)
```

"The OCSP server list is an X.509 v3 extension that defines a list of\nURLs of OCSP responders. The OCSP responders can be queried for the\nrevocation status of an issued certificate. If not set, the\ncertificate will be issued with no OCSP servers set. For example, an\nOCSP server URL could be \"http://ocsp.int-x3.letsencrypt.org\"."

**Note:** This function appends passed data to existing values

### fn spec.ca.withSecretName

```ts
withSecretName(secretName)
```

"SecretName is the name of the secret used to sign Certificates issued\nby this Issuer."

## obj spec.selfSigned

"SelfSigned configures this issuer to 'self sign' certificates using the\nprivate key used to create the CertificateRequest object."

### fn spec.selfSigned.withCrlDistributionPoints

```ts
withCrlDistributionPoints(crlDistributionPoints)
```

"The CRL distribution points is an X.509 v3 certificate extension which identifies\nthe location of the CRL from which the revocation of this certificate can be checked.\nIf not set certificate will be issued without CDP. Values are strings."

### fn spec.selfSigned.withCrlDistributionPointsMixin

```ts
withCrlDistributionPointsMixin(crlDistributionPoints)
```

"The CRL distribution points is an X.509 v3 certificate extension which identifies\nthe location of the CRL from which the revocation of this certificate can be checked.\nIf not set certificate will be issued without CDP. Values are strings."

**Note:** This function appends passed data to existing values

## obj spec.vault

"Vault configures this issuer to sign certificates using a HashiCorp Vault\nPKI backend."

### fn spec.vault.withCaBundle

```ts
withCaBundle(caBundle)
```

"Base64-encoded bundle of PEM CAs which will be used to validate the certificate\nchain presented by Vault. Only used if using HTTPS to connect to Vault and\nignored for HTTP connections.\nMutually exclusive with CABundleSecretRef.\nIf neither CABundle nor CABundleSecretRef are defined, the certificate bundle in\nthe cert-manager controller container is used to validate the TLS connection."

### fn spec.vault.withNamespace

```ts
withNamespace(namespace)
```

"Name of the vault namespace. Namespaces is a set of features within Vault Enterprise that allows Vault environments to support Secure Multi-tenancy. e.g: \"ns1\"\nMore about namespaces can be found here https://www.vaultproject.io/docs/enterprise/namespaces"

### fn spec.vault.withPath

```ts
withPath(path)
```

"Path is the mount path of the Vault PKI backend's `sign` endpoint, e.g:\n\"my_pki_mount/sign/my-role-name\"."

### fn spec.vault.withServer

```ts
withServer(server)
```

"Server is the connection address for the Vault server, e.g: \"https://vault.example.com:8200\"."

## obj spec.vault.auth

"Auth configures how cert-manager authenticates with the Vault server."

## obj spec.vault.auth.appRole

"AppRole authenticates with Vault using the App Role auth mechanism,\nwith the role and secret stored in a Kubernetes Secret resource."

### fn spec.vault.auth.appRole.withPath

```ts
withPath(path)
```

"Path where the App Role authentication backend is mounted in Vault, e.g:\n\"approle\

### fn spec.vault.auth.appRole.withRoleId

```ts
withRoleId(roleId)
```

"RoleID configured in the App Role authentication backend when setting\nup the authentication backend in Vault."

## obj spec.vault.auth.appRole.secretRef

"Reference to a key in a Secret that contains the App Role secret used\nto authenticate with Vault.\nThe `key` field must be specified and denotes which entry within the Secret\nresource is used as the app role secret."

### fn spec.vault.auth.appRole.secretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used.\nSome instances of this field may be defaulted, in others it may be\nrequired."

### fn spec.vault.auth.appRole.secretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to.\nMore info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.vault.auth.kubernetes

"Kubernetes authenticates with Vault by passing the ServiceAccount\ntoken stored in the named Secret resource to the Vault server."

### fn spec.vault.auth.kubernetes.withMountPath

```ts
withMountPath(mountPath)
```

"The Vault mountPath here is the mount path to use when authenticating with\nVault. For example, setting a value to `/v1/auth/foo`, will use the path\n`/v1/auth/foo/login` to authenticate with Vault. If unspecified, the\ndefault value \"/v1/auth/kubernetes\" will be used."

### fn spec.vault.auth.kubernetes.withRole

```ts
withRole(role)
```

"A required field containing the Vault Role to assume. A Role binds a\nKubernetes ServiceAccount with a set of Vault policies."

## obj spec.vault.auth.kubernetes.secretRef

"The required Secret field containing a Kubernetes ServiceAccount JWT used\nfor authenticating with Vault. Use of 'ambient credentials' is not\nsupported."

### fn spec.vault.auth.kubernetes.secretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used.\nSome instances of this field may be defaulted, in others it may be\nrequired."

### fn spec.vault.auth.kubernetes.secretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to.\nMore info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.vault.auth.kubernetes.serviceAccountRef

"A reference to a service account that will be used to request a bound\ntoken (also known as \"projected token\"). Compared to using \"secretRef\",\nusing this field means that you don't rely on statically bound tokens. To\nuse this field, you must configure an RBAC rule to let cert-manager\nrequest a token."

### fn spec.vault.auth.kubernetes.serviceAccountRef.withAudiences

```ts
withAudiences(audiences)
```

"TokenAudiences is an optional list of extra audiences to include in the token passed to Vault. The default token\nconsisting of the issuer's namespace and name is always included."

### fn spec.vault.auth.kubernetes.serviceAccountRef.withAudiencesMixin

```ts
withAudiencesMixin(audiences)
```

"TokenAudiences is an optional list of extra audiences to include in the token passed to Vault. The default token\nconsisting of the issuer's namespace and name is always included."

**Note:** This function appends passed data to existing values

### fn spec.vault.auth.kubernetes.serviceAccountRef.withName

```ts
withName(name)
```

"Name of the ServiceAccount used to request a token."

## obj spec.vault.auth.tokenSecretRef

"TokenSecretRef authenticates with Vault by presenting a token."

### fn spec.vault.auth.tokenSecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used.\nSome instances of this field may be defaulted, in others it may be\nrequired."

### fn spec.vault.auth.tokenSecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to.\nMore info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.vault.caBundleSecretRef

"Reference to a Secret containing a bundle of PEM-encoded CAs to use when\nverifying the certificate chain presented by Vault when using HTTPS.\nMutually exclusive with CABundle.\nIf neither CABundle nor CABundleSecretRef are defined, the certificate bundle in\nthe cert-manager controller container is used to validate the TLS connection.\nIf no key for the Secret is specified, cert-manager will default to 'ca.crt'."

### fn spec.vault.caBundleSecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used.\nSome instances of this field may be defaulted, in others it may be\nrequired."

### fn spec.vault.caBundleSecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to.\nMore info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.vault.clientCertSecretRef

"Reference to a Secret containing a PEM-encoded Client Certificate to use when the\nVault server requires mTLS."

### fn spec.vault.clientCertSecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used.\nSome instances of this field may be defaulted, in others it may be\nrequired."

### fn spec.vault.clientCertSecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to.\nMore info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.vault.clientKeySecretRef

"Reference to a Secret containing a PEM-encoded Client Private Key to use when the\nVault server requires mTLS."

### fn spec.vault.clientKeySecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used.\nSome instances of this field may be defaulted, in others it may be\nrequired."

### fn spec.vault.clientKeySecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to.\nMore info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.venafi

"Venafi configures this issuer to sign certificates using a Venafi TPP\nor Venafi Cloud policy zone."

### fn spec.venafi.withZone

```ts
withZone(zone)
```

"Zone is the Venafi Policy Zone to use for this issuer.\nAll requests made to the Venafi platform will be restricted by the named\nzone policy.\nThis field is required."

## obj spec.venafi.cloud

"Cloud specifies the Venafi cloud configuration settings.\nOnly one of TPP or Cloud may be specified."

### fn spec.venafi.cloud.withUrl

```ts
withUrl(url)
```

"URL is the base URL for Venafi Cloud.\nDefaults to \"https://api.venafi.cloud/v1\"."

## obj spec.venafi.cloud.apiTokenSecretRef

"APITokenSecretRef is a secret key selector for the Venafi Cloud API token."

### fn spec.venafi.cloud.apiTokenSecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used.\nSome instances of this field may be defaulted, in others it may be\nrequired."

### fn spec.venafi.cloud.apiTokenSecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to.\nMore info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.venafi.tpp

"TPP specifies Trust Protection Platform configuration settings.\nOnly one of TPP or Cloud may be specified."

### fn spec.venafi.tpp.withCaBundle

```ts
withCaBundle(caBundle)
```

"Base64-encoded bundle of PEM CAs which will be used to validate the certificate\nchain presented by the TPP server. Only used if using HTTPS; ignored for HTTP.\nIf undefined, the certificate bundle in the cert-manager controller container\nis used to validate the chain."

### fn spec.venafi.tpp.withUrl

```ts
withUrl(url)
```

"URL is the base URL for the vedsdk endpoint of the Venafi TPP instance,\nfor example: \"https://tpp.example.com/vedsdk\"."

## obj spec.venafi.tpp.credentialsRef

"CredentialsRef is a reference to a Secret containing the username and\npassword for the TPP server.\nThe secret must contain two keys, 'username' and 'password'."

### fn spec.venafi.tpp.credentialsRef.withName

```ts
withName(name)
```

"Name of the resource being referred to.\nMore info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"