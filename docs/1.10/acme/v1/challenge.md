---
permalink: /1.10/acme/v1/challenge/
---

# acme.v1.challenge

"Challenge is a type to represent a Challenge request with an ACME server"

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
  * [`fn withAuthorizationURL(authorizationURL)`](#fn-specwithauthorizationurl)
  * [`fn withDnsName(dnsName)`](#fn-specwithdnsname)
  * [`fn withKey(key)`](#fn-specwithkey)
  * [`fn withToken(token)`](#fn-specwithtoken)
  * [`fn withType(type)`](#fn-specwithtype)
  * [`fn withUrl(url)`](#fn-specwithurl)
  * [`fn withWildcard(wildcard)`](#fn-specwithwildcard)
  * [`obj spec.issuerRef`](#obj-specissuerref)
    * [`fn withGroup(group)`](#fn-specissuerrefwithgroup)
    * [`fn withKind(kind)`](#fn-specissuerrefwithkind)
    * [`fn withName(name)`](#fn-specissuerrefwithname)
  * [`obj spec.solver`](#obj-specsolver)
    * [`obj spec.solver.dns01`](#obj-specsolverdns01)
      * [`fn withCnameStrategy(cnameStrategy)`](#fn-specsolverdns01withcnamestrategy)
      * [`obj spec.solver.dns01.acmeDNS`](#obj-specsolverdns01acmedns)
        * [`fn withHost(host)`](#fn-specsolverdns01acmednswithhost)
        * [`obj spec.solver.dns01.acmeDNS.accountSecretRef`](#obj-specsolverdns01acmednsaccountsecretref)
          * [`fn withKey(key)`](#fn-specsolverdns01acmednsaccountsecretrefwithkey)
          * [`fn withName(name)`](#fn-specsolverdns01acmednsaccountsecretrefwithname)
      * [`obj spec.solver.dns01.akamai`](#obj-specsolverdns01akamai)
        * [`fn withServiceConsumerDomain(serviceConsumerDomain)`](#fn-specsolverdns01akamaiwithserviceconsumerdomain)
        * [`obj spec.solver.dns01.akamai.accessTokenSecretRef`](#obj-specsolverdns01akamaiaccesstokensecretref)
          * [`fn withKey(key)`](#fn-specsolverdns01akamaiaccesstokensecretrefwithkey)
          * [`fn withName(name)`](#fn-specsolverdns01akamaiaccesstokensecretrefwithname)
        * [`obj spec.solver.dns01.akamai.clientSecretSecretRef`](#obj-specsolverdns01akamaiclientsecretsecretref)
          * [`fn withKey(key)`](#fn-specsolverdns01akamaiclientsecretsecretrefwithkey)
          * [`fn withName(name)`](#fn-specsolverdns01akamaiclientsecretsecretrefwithname)
        * [`obj spec.solver.dns01.akamai.clientTokenSecretRef`](#obj-specsolverdns01akamaiclienttokensecretref)
          * [`fn withKey(key)`](#fn-specsolverdns01akamaiclienttokensecretrefwithkey)
          * [`fn withName(name)`](#fn-specsolverdns01akamaiclienttokensecretrefwithname)
      * [`obj spec.solver.dns01.azureDNS`](#obj-specsolverdns01azuredns)
        * [`fn withClientID(clientID)`](#fn-specsolverdns01azurednswithclientid)
        * [`fn withEnvironment(environment)`](#fn-specsolverdns01azurednswithenvironment)
        * [`fn withHostedZoneName(hostedZoneName)`](#fn-specsolverdns01azurednswithhostedzonename)
        * [`fn withResourceGroupName(resourceGroupName)`](#fn-specsolverdns01azurednswithresourcegroupname)
        * [`fn withSubscriptionID(subscriptionID)`](#fn-specsolverdns01azurednswithsubscriptionid)
        * [`fn withTenantID(tenantID)`](#fn-specsolverdns01azurednswithtenantid)
        * [`obj spec.solver.dns01.azureDNS.clientSecretSecretRef`](#obj-specsolverdns01azurednsclientsecretsecretref)
          * [`fn withKey(key)`](#fn-specsolverdns01azurednsclientsecretsecretrefwithkey)
          * [`fn withName(name)`](#fn-specsolverdns01azurednsclientsecretsecretrefwithname)
        * [`obj spec.solver.dns01.azureDNS.managedIdentity`](#obj-specsolverdns01azurednsmanagedidentity)
          * [`fn withClientID(clientID)`](#fn-specsolverdns01azurednsmanagedidentitywithclientid)
          * [`fn withResourceID(resourceID)`](#fn-specsolverdns01azurednsmanagedidentitywithresourceid)
      * [`obj spec.solver.dns01.cloudDNS`](#obj-specsolverdns01clouddns)
        * [`fn withHostedZoneName(hostedZoneName)`](#fn-specsolverdns01clouddnswithhostedzonename)
        * [`fn withProject(project)`](#fn-specsolverdns01clouddnswithproject)
        * [`obj spec.solver.dns01.cloudDNS.serviceAccountSecretRef`](#obj-specsolverdns01clouddnsserviceaccountsecretref)
          * [`fn withKey(key)`](#fn-specsolverdns01clouddnsserviceaccountsecretrefwithkey)
          * [`fn withName(name)`](#fn-specsolverdns01clouddnsserviceaccountsecretrefwithname)
      * [`obj spec.solver.dns01.cloudflare`](#obj-specsolverdns01cloudflare)
        * [`fn withEmail(email)`](#fn-specsolverdns01cloudflarewithemail)
        * [`obj spec.solver.dns01.cloudflare.apiKeySecretRef`](#obj-specsolverdns01cloudflareapikeysecretref)
          * [`fn withKey(key)`](#fn-specsolverdns01cloudflareapikeysecretrefwithkey)
          * [`fn withName(name)`](#fn-specsolverdns01cloudflareapikeysecretrefwithname)
        * [`obj spec.solver.dns01.cloudflare.apiTokenSecretRef`](#obj-specsolverdns01cloudflareapitokensecretref)
          * [`fn withKey(key)`](#fn-specsolverdns01cloudflareapitokensecretrefwithkey)
          * [`fn withName(name)`](#fn-specsolverdns01cloudflareapitokensecretrefwithname)
      * [`obj spec.solver.dns01.digitalocean`](#obj-specsolverdns01digitalocean)
        * [`obj spec.solver.dns01.digitalocean.tokenSecretRef`](#obj-specsolverdns01digitaloceantokensecretref)
          * [`fn withKey(key)`](#fn-specsolverdns01digitaloceantokensecretrefwithkey)
          * [`fn withName(name)`](#fn-specsolverdns01digitaloceantokensecretrefwithname)
      * [`obj spec.solver.dns01.rfc2136`](#obj-specsolverdns01rfc2136)
        * [`fn withNameserver(nameserver)`](#fn-specsolverdns01rfc2136withnameserver)
        * [`fn withTsigAlgorithm(tsigAlgorithm)`](#fn-specsolverdns01rfc2136withtsigalgorithm)
        * [`fn withTsigKeyName(tsigKeyName)`](#fn-specsolverdns01rfc2136withtsigkeyname)
        * [`obj spec.solver.dns01.rfc2136.tsigSecretSecretRef`](#obj-specsolverdns01rfc2136tsigsecretsecretref)
          * [`fn withKey(key)`](#fn-specsolverdns01rfc2136tsigsecretsecretrefwithkey)
          * [`fn withName(name)`](#fn-specsolverdns01rfc2136tsigsecretsecretrefwithname)
      * [`obj spec.solver.dns01.route53`](#obj-specsolverdns01route53)
        * [`fn withAccessKeyID(accessKeyID)`](#fn-specsolverdns01route53withaccesskeyid)
        * [`fn withHostedZoneID(hostedZoneID)`](#fn-specsolverdns01route53withhostedzoneid)
        * [`fn withRegion(region)`](#fn-specsolverdns01route53withregion)
        * [`fn withRole(role)`](#fn-specsolverdns01route53withrole)
        * [`obj spec.solver.dns01.route53.accessKeyIDSecretRef`](#obj-specsolverdns01route53accesskeyidsecretref)
          * [`fn withKey(key)`](#fn-specsolverdns01route53accesskeyidsecretrefwithkey)
          * [`fn withName(name)`](#fn-specsolverdns01route53accesskeyidsecretrefwithname)
        * [`obj spec.solver.dns01.route53.secretAccessKeySecretRef`](#obj-specsolverdns01route53secretaccesskeysecretref)
          * [`fn withKey(key)`](#fn-specsolverdns01route53secretaccesskeysecretrefwithkey)
          * [`fn withName(name)`](#fn-specsolverdns01route53secretaccesskeysecretrefwithname)
      * [`obj spec.solver.dns01.webhook`](#obj-specsolverdns01webhook)
        * [`fn withConfig(config)`](#fn-specsolverdns01webhookwithconfig)
        * [`fn withGroupName(groupName)`](#fn-specsolverdns01webhookwithgroupname)
        * [`fn withSolverName(solverName)`](#fn-specsolverdns01webhookwithsolvername)
    * [`obj spec.solver.http01`](#obj-specsolverhttp01)
      * [`obj spec.solver.http01.gatewayHTTPRoute`](#obj-specsolverhttp01gatewayhttproute)
        * [`fn withLabels(labels)`](#fn-specsolverhttp01gatewayhttproutewithlabels)
        * [`fn withLabelsMixin(labels)`](#fn-specsolverhttp01gatewayhttproutewithlabelsmixin)
        * [`fn withParentRefs(parentRefs)`](#fn-specsolverhttp01gatewayhttproutewithparentrefs)
        * [`fn withParentRefsMixin(parentRefs)`](#fn-specsolverhttp01gatewayhttproutewithparentrefsmixin)
        * [`fn withServiceType(serviceType)`](#fn-specsolverhttp01gatewayhttproutewithservicetype)
        * [`obj spec.solver.http01.gatewayHTTPRoute.parentRefs`](#obj-specsolverhttp01gatewayhttprouteparentrefs)
          * [`fn withGroup(group)`](#fn-specsolverhttp01gatewayhttprouteparentrefswithgroup)
          * [`fn withKind(kind)`](#fn-specsolverhttp01gatewayhttprouteparentrefswithkind)
          * [`fn withName(name)`](#fn-specsolverhttp01gatewayhttprouteparentrefswithname)
          * [`fn withNamespace(namespace)`](#fn-specsolverhttp01gatewayhttprouteparentrefswithnamespace)
          * [`fn withPort(port)`](#fn-specsolverhttp01gatewayhttprouteparentrefswithport)
          * [`fn withSectionName(sectionName)`](#fn-specsolverhttp01gatewayhttprouteparentrefswithsectionname)
      * [`obj spec.solver.http01.ingress`](#obj-specsolverhttp01ingress)
        * [`fn withClass(class)`](#fn-specsolverhttp01ingresswithclass)
        * [`fn withName(name)`](#fn-specsolverhttp01ingresswithname)
        * [`fn withServiceType(serviceType)`](#fn-specsolverhttp01ingresswithservicetype)
        * [`obj spec.solver.http01.ingress.ingressTemplate`](#obj-specsolverhttp01ingressingresstemplate)
          * [`obj spec.solver.http01.ingress.ingressTemplate.metadata`](#obj-specsolverhttp01ingressingresstemplatemetadata)
            * [`fn withAnnotations(annotations)`](#fn-specsolverhttp01ingressingresstemplatemetadatawithannotations)
            * [`fn withAnnotationsMixin(annotations)`](#fn-specsolverhttp01ingressingresstemplatemetadatawithannotationsmixin)
            * [`fn withLabels(labels)`](#fn-specsolverhttp01ingressingresstemplatemetadatawithlabels)
            * [`fn withLabelsMixin(labels)`](#fn-specsolverhttp01ingressingresstemplatemetadatawithlabelsmixin)
        * [`obj spec.solver.http01.ingress.podTemplate`](#obj-specsolverhttp01ingresspodtemplate)
          * [`obj spec.solver.http01.ingress.podTemplate.metadata`](#obj-specsolverhttp01ingresspodtemplatemetadata)
            * [`fn withAnnotations(annotations)`](#fn-specsolverhttp01ingresspodtemplatemetadatawithannotations)
            * [`fn withAnnotationsMixin(annotations)`](#fn-specsolverhttp01ingresspodtemplatemetadatawithannotationsmixin)
            * [`fn withLabels(labels)`](#fn-specsolverhttp01ingresspodtemplatemetadatawithlabels)
            * [`fn withLabelsMixin(labels)`](#fn-specsolverhttp01ingresspodtemplatemetadatawithlabelsmixin)
          * [`obj spec.solver.http01.ingress.podTemplate.spec`](#obj-specsolverhttp01ingresspodtemplatespec)
            * [`fn withNodeSelector(nodeSelector)`](#fn-specsolverhttp01ingresspodtemplatespecwithnodeselector)
            * [`fn withNodeSelectorMixin(nodeSelector)`](#fn-specsolverhttp01ingresspodtemplatespecwithnodeselectormixin)
            * [`fn withPriorityClassName(priorityClassName)`](#fn-specsolverhttp01ingresspodtemplatespecwithpriorityclassname)
            * [`fn withServiceAccountName(serviceAccountName)`](#fn-specsolverhttp01ingresspodtemplatespecwithserviceaccountname)
            * [`fn withTolerations(tolerations)`](#fn-specsolverhttp01ingresspodtemplatespecwithtolerations)
            * [`fn withTolerationsMixin(tolerations)`](#fn-specsolverhttp01ingresspodtemplatespecwithtolerationsmixin)
            * [`obj spec.solver.http01.ingress.podTemplate.spec.affinity`](#obj-specsolverhttp01ingresspodtemplatespecaffinity)
              * [`obj spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity`](#obj-specsolverhttp01ingresspodtemplatespecaffinitynodeaffinity)
                * [`fn withPreferredDuringSchedulingIgnoredDuringExecution(preferredDuringSchedulingIgnoredDuringExecution)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitynodeaffinitywithpreferredduringschedulingignoredduringexecution)
                * [`fn withPreferredDuringSchedulingIgnoredDuringExecutionMixin(preferredDuringSchedulingIgnoredDuringExecution)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitynodeaffinitywithpreferredduringschedulingignoredduringexecutionmixin)
                * [`obj spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution`](#obj-specsolverhttp01ingresspodtemplatespecaffinitynodeaffinitypreferredduringschedulingignoredduringexecution)
                  * [`fn withWeight(weight)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitynodeaffinitypreferredduringschedulingignoredduringexecutionwithweight)
                  * [`obj spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution.preference`](#obj-specsolverhttp01ingresspodtemplatespecaffinitynodeaffinitypreferredduringschedulingignoredduringexecutionpreference)
                    * [`fn withMatchExpressions(matchExpressions)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitynodeaffinitypreferredduringschedulingignoredduringexecutionpreferencewithmatchexpressions)
                    * [`fn withMatchExpressionsMixin(matchExpressions)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitynodeaffinitypreferredduringschedulingignoredduringexecutionpreferencewithmatchexpressionsmixin)
                    * [`fn withMatchFields(matchFields)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitynodeaffinitypreferredduringschedulingignoredduringexecutionpreferencewithmatchfields)
                    * [`fn withMatchFieldsMixin(matchFields)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitynodeaffinitypreferredduringschedulingignoredduringexecutionpreferencewithmatchfieldsmixin)
                    * [`obj spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution.preference.matchExpressions`](#obj-specsolverhttp01ingresspodtemplatespecaffinitynodeaffinitypreferredduringschedulingignoredduringexecutionpreferencematchexpressions)
                      * [`fn withKey(key)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitynodeaffinitypreferredduringschedulingignoredduringexecutionpreferencematchexpressionswithkey)
                      * [`fn withOperator(operator)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitynodeaffinitypreferredduringschedulingignoredduringexecutionpreferencematchexpressionswithoperator)
                      * [`fn withValues(values)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitynodeaffinitypreferredduringschedulingignoredduringexecutionpreferencematchexpressionswithvalues)
                      * [`fn withValuesMixin(values)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitynodeaffinitypreferredduringschedulingignoredduringexecutionpreferencematchexpressionswithvaluesmixin)
                    * [`obj spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution.preference.matchFields`](#obj-specsolverhttp01ingresspodtemplatespecaffinitynodeaffinitypreferredduringschedulingignoredduringexecutionpreferencematchfields)
                      * [`fn withKey(key)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitynodeaffinitypreferredduringschedulingignoredduringexecutionpreferencematchfieldswithkey)
                      * [`fn withOperator(operator)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitynodeaffinitypreferredduringschedulingignoredduringexecutionpreferencematchfieldswithoperator)
                      * [`fn withValues(values)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitynodeaffinitypreferredduringschedulingignoredduringexecutionpreferencematchfieldswithvalues)
                      * [`fn withValuesMixin(values)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitynodeaffinitypreferredduringschedulingignoredduringexecutionpreferencematchfieldswithvaluesmixin)
                * [`obj spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution`](#obj-specsolverhttp01ingresspodtemplatespecaffinitynodeaffinityrequiredduringschedulingignoredduringexecution)
                  * [`fn withNodeSelectorTerms(nodeSelectorTerms)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitynodeaffinityrequiredduringschedulingignoredduringexecutionwithnodeselectorterms)
                  * [`fn withNodeSelectorTermsMixin(nodeSelectorTerms)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitynodeaffinityrequiredduringschedulingignoredduringexecutionwithnodeselectortermsmixin)
                  * [`obj spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.nodeSelectorTerms`](#obj-specsolverhttp01ingresspodtemplatespecaffinitynodeaffinityrequiredduringschedulingignoredduringexecutionnodeselectorterms)
                    * [`fn withMatchExpressions(matchExpressions)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitynodeaffinityrequiredduringschedulingignoredduringexecutionnodeselectortermswithmatchexpressions)
                    * [`fn withMatchExpressionsMixin(matchExpressions)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitynodeaffinityrequiredduringschedulingignoredduringexecutionnodeselectortermswithmatchexpressionsmixin)
                    * [`fn withMatchFields(matchFields)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitynodeaffinityrequiredduringschedulingignoredduringexecutionnodeselectortermswithmatchfields)
                    * [`fn withMatchFieldsMixin(matchFields)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitynodeaffinityrequiredduringschedulingignoredduringexecutionnodeselectortermswithmatchfieldsmixin)
                    * [`obj spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.nodeSelectorTerms.matchExpressions`](#obj-specsolverhttp01ingresspodtemplatespecaffinitynodeaffinityrequiredduringschedulingignoredduringexecutionnodeselectortermsmatchexpressions)
                      * [`fn withKey(key)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitynodeaffinityrequiredduringschedulingignoredduringexecutionnodeselectortermsmatchexpressionswithkey)
                      * [`fn withOperator(operator)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitynodeaffinityrequiredduringschedulingignoredduringexecutionnodeselectortermsmatchexpressionswithoperator)
                      * [`fn withValues(values)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitynodeaffinityrequiredduringschedulingignoredduringexecutionnodeselectortermsmatchexpressionswithvalues)
                      * [`fn withValuesMixin(values)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitynodeaffinityrequiredduringschedulingignoredduringexecutionnodeselectortermsmatchexpressionswithvaluesmixin)
                    * [`obj spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.nodeSelectorTerms.matchFields`](#obj-specsolverhttp01ingresspodtemplatespecaffinitynodeaffinityrequiredduringschedulingignoredduringexecutionnodeselectortermsmatchfields)
                      * [`fn withKey(key)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitynodeaffinityrequiredduringschedulingignoredduringexecutionnodeselectortermsmatchfieldswithkey)
                      * [`fn withOperator(operator)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitynodeaffinityrequiredduringschedulingignoredduringexecutionnodeselectortermsmatchfieldswithoperator)
                      * [`fn withValues(values)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitynodeaffinityrequiredduringschedulingignoredduringexecutionnodeselectortermsmatchfieldswithvalues)
                      * [`fn withValuesMixin(values)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitynodeaffinityrequiredduringschedulingignoredduringexecutionnodeselectortermsmatchfieldswithvaluesmixin)
              * [`obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity`](#obj-specsolverhttp01ingresspodtemplatespecaffinitypodaffinity)
                * [`fn withPreferredDuringSchedulingIgnoredDuringExecution(preferredDuringSchedulingIgnoredDuringExecution)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodaffinitywithpreferredduringschedulingignoredduringexecution)
                * [`fn withPreferredDuringSchedulingIgnoredDuringExecutionMixin(preferredDuringSchedulingIgnoredDuringExecution)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodaffinitywithpreferredduringschedulingignoredduringexecutionmixin)
                * [`fn withRequiredDuringSchedulingIgnoredDuringExecution(requiredDuringSchedulingIgnoredDuringExecution)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodaffinitywithrequiredduringschedulingignoredduringexecution)
                * [`fn withRequiredDuringSchedulingIgnoredDuringExecutionMixin(requiredDuringSchedulingIgnoredDuringExecution)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodaffinitywithrequiredduringschedulingignoredduringexecutionmixin)
                * [`obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution`](#obj-specsolverhttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecution)
                  * [`fn withWeight(weight)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionwithweight)
                  * [`obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm`](#obj-specsolverhttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinityterm)
                    * [`fn withNamespaces(namespaces)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermwithnamespaces)
                    * [`fn withNamespacesMixin(namespaces)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermwithnamespacesmixin)
                    * [`fn withTopologyKey(topologyKey)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermwithtopologykey)
                    * [`obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector`](#obj-specsolverhttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermlabelselector)
                      * [`fn withMatchExpressions(matchExpressions)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermlabelselectorwithmatchexpressions)
                      * [`fn withMatchExpressionsMixin(matchExpressions)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermlabelselectorwithmatchexpressionsmixin)
                      * [`fn withMatchLabels(matchLabels)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermlabelselectorwithmatchlabels)
                      * [`fn withMatchLabelsMixin(matchLabels)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermlabelselectorwithmatchlabelsmixin)
                      * [`obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.matchExpressions`](#obj-specsolverhttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermlabelselectormatchexpressions)
                        * [`fn withKey(key)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermlabelselectormatchexpressionswithkey)
                        * [`fn withOperator(operator)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermlabelselectormatchexpressionswithoperator)
                        * [`fn withValues(values)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermlabelselectormatchexpressionswithvalues)
                        * [`fn withValuesMixin(values)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermlabelselectormatchexpressionswithvaluesmixin)
                    * [`obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector`](#obj-specsolverhttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermnamespaceselector)
                      * [`fn withMatchExpressions(matchExpressions)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermnamespaceselectorwithmatchexpressions)
                      * [`fn withMatchExpressionsMixin(matchExpressions)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermnamespaceselectorwithmatchexpressionsmixin)
                      * [`fn withMatchLabels(matchLabels)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermnamespaceselectorwithmatchlabels)
                      * [`fn withMatchLabelsMixin(matchLabels)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermnamespaceselectorwithmatchlabelsmixin)
                      * [`obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.matchExpressions`](#obj-specsolverhttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermnamespaceselectormatchexpressions)
                        * [`fn withKey(key)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermnamespaceselectormatchexpressionswithkey)
                        * [`fn withOperator(operator)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermnamespaceselectormatchexpressionswithoperator)
                        * [`fn withValues(values)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermnamespaceselectormatchexpressionswithvalues)
                        * [`fn withValuesMixin(values)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermnamespaceselectormatchexpressionswithvaluesmixin)
                * [`obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution`](#obj-specsolverhttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecution)
                  * [`fn withNamespaces(namespaces)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionwithnamespaces)
                  * [`fn withNamespacesMixin(namespaces)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionwithnamespacesmixin)
                  * [`fn withTopologyKey(topologyKey)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionwithtopologykey)
                  * [`obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector`](#obj-specsolverhttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionlabelselector)
                    * [`fn withMatchExpressions(matchExpressions)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionlabelselectorwithmatchexpressions)
                    * [`fn withMatchExpressionsMixin(matchExpressions)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionlabelselectorwithmatchexpressionsmixin)
                    * [`fn withMatchLabels(matchLabels)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionlabelselectorwithmatchlabels)
                    * [`fn withMatchLabelsMixin(matchLabels)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionlabelselectorwithmatchlabelsmixin)
                    * [`obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.matchExpressions`](#obj-specsolverhttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionlabelselectormatchexpressions)
                      * [`fn withKey(key)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionlabelselectormatchexpressionswithkey)
                      * [`fn withOperator(operator)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionlabelselectormatchexpressionswithoperator)
                      * [`fn withValues(values)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionlabelselectormatchexpressionswithvalues)
                      * [`fn withValuesMixin(values)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionlabelselectormatchexpressionswithvaluesmixin)
                  * [`obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector`](#obj-specsolverhttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionnamespaceselector)
                    * [`fn withMatchExpressions(matchExpressions)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionnamespaceselectorwithmatchexpressions)
                    * [`fn withMatchExpressionsMixin(matchExpressions)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionnamespaceselectorwithmatchexpressionsmixin)
                    * [`fn withMatchLabels(matchLabels)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionnamespaceselectorwithmatchlabels)
                    * [`fn withMatchLabelsMixin(matchLabels)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionnamespaceselectorwithmatchlabelsmixin)
                    * [`obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.matchExpressions`](#obj-specsolverhttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionnamespaceselectormatchexpressions)
                      * [`fn withKey(key)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionnamespaceselectormatchexpressionswithkey)
                      * [`fn withOperator(operator)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionnamespaceselectormatchexpressionswithoperator)
                      * [`fn withValues(values)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionnamespaceselectormatchexpressionswithvalues)
                      * [`fn withValuesMixin(values)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodaffinityrequiredduringschedulingignoredduringexecutionnamespaceselectormatchexpressionswithvaluesmixin)
              * [`obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity`](#obj-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinity)
                * [`fn withPreferredDuringSchedulingIgnoredDuringExecution(preferredDuringSchedulingIgnoredDuringExecution)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinitywithpreferredduringschedulingignoredduringexecution)
                * [`fn withPreferredDuringSchedulingIgnoredDuringExecutionMixin(preferredDuringSchedulingIgnoredDuringExecution)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinitywithpreferredduringschedulingignoredduringexecutionmixin)
                * [`fn withRequiredDuringSchedulingIgnoredDuringExecution(requiredDuringSchedulingIgnoredDuringExecution)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinitywithrequiredduringschedulingignoredduringexecution)
                * [`fn withRequiredDuringSchedulingIgnoredDuringExecutionMixin(requiredDuringSchedulingIgnoredDuringExecution)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinitywithrequiredduringschedulingignoredduringexecutionmixin)
                * [`obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution`](#obj-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecution)
                  * [`fn withWeight(weight)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionwithweight)
                  * [`obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm`](#obj-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinityterm)
                    * [`fn withNamespaces(namespaces)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermwithnamespaces)
                    * [`fn withNamespacesMixin(namespaces)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermwithnamespacesmixin)
                    * [`fn withTopologyKey(topologyKey)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermwithtopologykey)
                    * [`obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector`](#obj-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermlabelselector)
                      * [`fn withMatchExpressions(matchExpressions)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermlabelselectorwithmatchexpressions)
                      * [`fn withMatchExpressionsMixin(matchExpressions)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermlabelselectorwithmatchexpressionsmixin)
                      * [`fn withMatchLabels(matchLabels)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermlabelselectorwithmatchlabels)
                      * [`fn withMatchLabelsMixin(matchLabels)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermlabelselectorwithmatchlabelsmixin)
                      * [`obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.matchExpressions`](#obj-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermlabelselectormatchexpressions)
                        * [`fn withKey(key)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermlabelselectormatchexpressionswithkey)
                        * [`fn withOperator(operator)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermlabelselectormatchexpressionswithoperator)
                        * [`fn withValues(values)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermlabelselectormatchexpressionswithvalues)
                        * [`fn withValuesMixin(values)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermlabelselectormatchexpressionswithvaluesmixin)
                    * [`obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector`](#obj-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermnamespaceselector)
                      * [`fn withMatchExpressions(matchExpressions)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermnamespaceselectorwithmatchexpressions)
                      * [`fn withMatchExpressionsMixin(matchExpressions)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermnamespaceselectorwithmatchexpressionsmixin)
                      * [`fn withMatchLabels(matchLabels)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermnamespaceselectorwithmatchlabels)
                      * [`fn withMatchLabelsMixin(matchLabels)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermnamespaceselectorwithmatchlabelsmixin)
                      * [`obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.matchExpressions`](#obj-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermnamespaceselectormatchexpressions)
                        * [`fn withKey(key)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermnamespaceselectormatchexpressionswithkey)
                        * [`fn withOperator(operator)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermnamespaceselectormatchexpressionswithoperator)
                        * [`fn withValues(values)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermnamespaceselectormatchexpressionswithvalues)
                        * [`fn withValuesMixin(values)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinitypreferredduringschedulingignoredduringexecutionpodaffinitytermnamespaceselectormatchexpressionswithvaluesmixin)
                * [`obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution`](#obj-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecution)
                  * [`fn withNamespaces(namespaces)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionwithnamespaces)
                  * [`fn withNamespacesMixin(namespaces)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionwithnamespacesmixin)
                  * [`fn withTopologyKey(topologyKey)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionwithtopologykey)
                  * [`obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector`](#obj-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionlabelselector)
                    * [`fn withMatchExpressions(matchExpressions)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionlabelselectorwithmatchexpressions)
                    * [`fn withMatchExpressionsMixin(matchExpressions)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionlabelselectorwithmatchexpressionsmixin)
                    * [`fn withMatchLabels(matchLabels)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionlabelselectorwithmatchlabels)
                    * [`fn withMatchLabelsMixin(matchLabels)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionlabelselectorwithmatchlabelsmixin)
                    * [`obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.matchExpressions`](#obj-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionlabelselectormatchexpressions)
                      * [`fn withKey(key)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionlabelselectormatchexpressionswithkey)
                      * [`fn withOperator(operator)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionlabelselectormatchexpressionswithoperator)
                      * [`fn withValues(values)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionlabelselectormatchexpressionswithvalues)
                      * [`fn withValuesMixin(values)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionlabelselectormatchexpressionswithvaluesmixin)
                  * [`obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector`](#obj-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionnamespaceselector)
                    * [`fn withMatchExpressions(matchExpressions)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionnamespaceselectorwithmatchexpressions)
                    * [`fn withMatchExpressionsMixin(matchExpressions)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionnamespaceselectorwithmatchexpressionsmixin)
                    * [`fn withMatchLabels(matchLabels)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionnamespaceselectorwithmatchlabels)
                    * [`fn withMatchLabelsMixin(matchLabels)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionnamespaceselectorwithmatchlabelsmixin)
                    * [`obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.matchExpressions`](#obj-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionnamespaceselectormatchexpressions)
                      * [`fn withKey(key)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionnamespaceselectormatchexpressionswithkey)
                      * [`fn withOperator(operator)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionnamespaceselectormatchexpressionswithoperator)
                      * [`fn withValues(values)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionnamespaceselectormatchexpressionswithvalues)
                      * [`fn withValuesMixin(values)`](#fn-specsolverhttp01ingresspodtemplatespecaffinitypodantiaffinityrequiredduringschedulingignoredduringexecutionnamespaceselectormatchexpressionswithvaluesmixin)
            * [`obj spec.solver.http01.ingress.podTemplate.spec.tolerations`](#obj-specsolverhttp01ingresspodtemplatespectolerations)
              * [`fn withEffect(effect)`](#fn-specsolverhttp01ingresspodtemplatespectolerationswitheffect)
              * [`fn withKey(key)`](#fn-specsolverhttp01ingresspodtemplatespectolerationswithkey)
              * [`fn withOperator(operator)`](#fn-specsolverhttp01ingresspodtemplatespectolerationswithoperator)
              * [`fn withTolerationSeconds(tolerationSeconds)`](#fn-specsolverhttp01ingresspodtemplatespectolerationswithtolerationseconds)
              * [`fn withValue(value)`](#fn-specsolverhttp01ingresspodtemplatespectolerationswithvalue)
    * [`obj spec.solver.selector`](#obj-specsolverselector)
      * [`fn withDnsNames(dnsNames)`](#fn-specsolverselectorwithdnsnames)
      * [`fn withDnsNamesMixin(dnsNames)`](#fn-specsolverselectorwithdnsnamesmixin)
      * [`fn withDnsZones(dnsZones)`](#fn-specsolverselectorwithdnszones)
      * [`fn withDnsZonesMixin(dnsZones)`](#fn-specsolverselectorwithdnszonesmixin)
      * [`fn withMatchLabels(matchLabels)`](#fn-specsolverselectorwithmatchlabels)
      * [`fn withMatchLabelsMixin(matchLabels)`](#fn-specsolverselectorwithmatchlabelsmixin)

## Fields

### fn new

```ts
new(name)
```

new returns an instance of Challenge

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



### fn spec.withAuthorizationURL

```ts
withAuthorizationURL(authorizationURL)
```

"The URL to the ACME Authorization resource that this challenge is a part of."

### fn spec.withDnsName

```ts
withDnsName(dnsName)
```

"dnsName is the identifier that this challenge is for, e.g. example.com. If the requested DNSName is a 'wildcard', this field MUST be set to the non-wildcard domain, e.g. for `*.example.com`, it must be `example.com`."

### fn spec.withKey

```ts
withKey(key)
```

"The ACME challenge key for this challenge For HTTP01 challenges, this is the value that must be responded with to complete the HTTP01 challenge in the format: `<private key JWK thumbprint>.<key from acme server for challenge>`. For DNS01 challenges, this is the base64 encoded SHA256 sum of the `<private key JWK thumbprint>.<key from acme server for challenge>` text that must be set as the TXT record content."

### fn spec.withToken

```ts
withToken(token)
```

"The ACME challenge token for this challenge. This is the raw value returned from the ACME server."

### fn spec.withType

```ts
withType(type)
```

"The type of ACME challenge this resource represents. One of \"HTTP-01\" or \"DNS-01\"."

### fn spec.withUrl

```ts
withUrl(url)
```

"The URL of the ACME Challenge resource for this challenge. This can be used to lookup details about the status of this challenge."

### fn spec.withWildcard

```ts
withWildcard(wildcard)
```

"wildcard will be true if this challenge is for a wildcard identifier, for example '*.example.com'."

## obj spec.issuerRef

"References a properly configured ACME-type Issuer which should be used to create this Challenge. If the Issuer does not exist, processing will be retried. If the Issuer is not an 'ACME' Issuer, an error will be returned and the Challenge will be marked as failed."

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

## obj spec.solver

"Contains the domain solving configuration that should be used to solve this challenge resource."

## obj spec.solver.dns01

"Configures cert-manager to attempt to complete authorizations by performing the DNS01 challenge flow."

### fn spec.solver.dns01.withCnameStrategy

```ts
withCnameStrategy(cnameStrategy)
```

"CNAMEStrategy configures how the DNS01 provider should handle CNAME records when found in DNS zones."

## obj spec.solver.dns01.acmeDNS

"Use the 'ACME DNS' (https://github.com/joohoi/acme-dns) API to manage DNS01 challenge records."

### fn spec.solver.dns01.acmeDNS.withHost

```ts
withHost(host)
```



## obj spec.solver.dns01.acmeDNS.accountSecretRef

"A reference to a specific 'key' within a Secret resource. In some instances, `key` is a required field."

### fn spec.solver.dns01.acmeDNS.accountSecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used. Some instances of this field may be defaulted, in others it may be required."

### fn spec.solver.dns01.acmeDNS.accountSecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.solver.dns01.akamai

"Use the Akamai DNS zone management API to manage DNS01 challenge records."

### fn spec.solver.dns01.akamai.withServiceConsumerDomain

```ts
withServiceConsumerDomain(serviceConsumerDomain)
```



## obj spec.solver.dns01.akamai.accessTokenSecretRef

"A reference to a specific 'key' within a Secret resource. In some instances, `key` is a required field."

### fn spec.solver.dns01.akamai.accessTokenSecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used. Some instances of this field may be defaulted, in others it may be required."

### fn spec.solver.dns01.akamai.accessTokenSecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.solver.dns01.akamai.clientSecretSecretRef

"A reference to a specific 'key' within a Secret resource. In some instances, `key` is a required field."

### fn spec.solver.dns01.akamai.clientSecretSecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used. Some instances of this field may be defaulted, in others it may be required."

### fn spec.solver.dns01.akamai.clientSecretSecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.solver.dns01.akamai.clientTokenSecretRef

"A reference to a specific 'key' within a Secret resource. In some instances, `key` is a required field."

### fn spec.solver.dns01.akamai.clientTokenSecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used. Some instances of this field may be defaulted, in others it may be required."

### fn spec.solver.dns01.akamai.clientTokenSecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.solver.dns01.azureDNS

"Use the Microsoft Azure DNS API to manage DNS01 challenge records."

### fn spec.solver.dns01.azureDNS.withClientID

```ts
withClientID(clientID)
```

"if both this and ClientSecret are left unset MSI will be used"

### fn spec.solver.dns01.azureDNS.withEnvironment

```ts
withEnvironment(environment)
```

"name of the Azure environment (default AzurePublicCloud)"

### fn spec.solver.dns01.azureDNS.withHostedZoneName

```ts
withHostedZoneName(hostedZoneName)
```

"name of the DNS zone that should be used"

### fn spec.solver.dns01.azureDNS.withResourceGroupName

```ts
withResourceGroupName(resourceGroupName)
```

"resource group the DNS zone is located in"

### fn spec.solver.dns01.azureDNS.withSubscriptionID

```ts
withSubscriptionID(subscriptionID)
```

"ID of the Azure subscription"

### fn spec.solver.dns01.azureDNS.withTenantID

```ts
withTenantID(tenantID)
```

"when specifying ClientID and ClientSecret then this field is also needed"

## obj spec.solver.dns01.azureDNS.clientSecretSecretRef

"if both this and ClientID are left unset MSI will be used"

### fn spec.solver.dns01.azureDNS.clientSecretSecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used. Some instances of this field may be defaulted, in others it may be required."

### fn spec.solver.dns01.azureDNS.clientSecretSecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.solver.dns01.azureDNS.managedIdentity

"managed identity configuration, can not be used at the same time as clientID, clientSecretSecretRef or tenantID"

### fn spec.solver.dns01.azureDNS.managedIdentity.withClientID

```ts
withClientID(clientID)
```

"client ID of the managed identity, can not be used at the same time as resourceID"

### fn spec.solver.dns01.azureDNS.managedIdentity.withResourceID

```ts
withResourceID(resourceID)
```

"resource ID of the managed identity, can not be used at the same time as clientID"

## obj spec.solver.dns01.cloudDNS

"Use the Google Cloud DNS API to manage DNS01 challenge records."

### fn spec.solver.dns01.cloudDNS.withHostedZoneName

```ts
withHostedZoneName(hostedZoneName)
```

"HostedZoneName is an optional field that tells cert-manager in which Cloud DNS zone the challenge record has to be created. If left empty cert-manager will automatically choose a zone."

### fn spec.solver.dns01.cloudDNS.withProject

```ts
withProject(project)
```



## obj spec.solver.dns01.cloudDNS.serviceAccountSecretRef

"A reference to a specific 'key' within a Secret resource. In some instances, `key` is a required field."

### fn spec.solver.dns01.cloudDNS.serviceAccountSecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used. Some instances of this field may be defaulted, in others it may be required."

### fn spec.solver.dns01.cloudDNS.serviceAccountSecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.solver.dns01.cloudflare

"Use the Cloudflare API to manage DNS01 challenge records."

### fn spec.solver.dns01.cloudflare.withEmail

```ts
withEmail(email)
```

"Email of the account, only required when using API key based authentication."

## obj spec.solver.dns01.cloudflare.apiKeySecretRef

"API key to use to authenticate with Cloudflare. Note: using an API token to authenticate is now the recommended method as it allows greater control of permissions."

### fn spec.solver.dns01.cloudflare.apiKeySecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used. Some instances of this field may be defaulted, in others it may be required."

### fn spec.solver.dns01.cloudflare.apiKeySecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.solver.dns01.cloudflare.apiTokenSecretRef

"API token used to authenticate with Cloudflare."

### fn spec.solver.dns01.cloudflare.apiTokenSecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used. Some instances of this field may be defaulted, in others it may be required."

### fn spec.solver.dns01.cloudflare.apiTokenSecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.solver.dns01.digitalocean

"Use the DigitalOcean DNS API to manage DNS01 challenge records."

## obj spec.solver.dns01.digitalocean.tokenSecretRef

"A reference to a specific 'key' within a Secret resource. In some instances, `key` is a required field."

### fn spec.solver.dns01.digitalocean.tokenSecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used. Some instances of this field may be defaulted, in others it may be required."

### fn spec.solver.dns01.digitalocean.tokenSecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.solver.dns01.rfc2136

"Use RFC2136 (\"Dynamic Updates in the Domain Name System\") (https://datatracker.ietf.org/doc/rfc2136/) to manage DNS01 challenge records."

### fn spec.solver.dns01.rfc2136.withNameserver

```ts
withNameserver(nameserver)
```

"The IP address or hostname of an authoritative DNS server supporting RFC2136 in the form host:port. If the host is an IPv6 address it must be enclosed in square brackets (e.g [2001:db8::1])\u00a0; port is optional. This field is required."

### fn spec.solver.dns01.rfc2136.withTsigAlgorithm

```ts
withTsigAlgorithm(tsigAlgorithm)
```

"The TSIG Algorithm configured in the DNS supporting RFC2136. Used only when ``tsigSecretSecretRef`` and ``tsigKeyName`` are defined. Supported values are (case-insensitive): ``HMACMD5`` (default), ``HMACSHA1``, ``HMACSHA256`` or ``HMACSHA512``."

### fn spec.solver.dns01.rfc2136.withTsigKeyName

```ts
withTsigKeyName(tsigKeyName)
```

"The TSIG Key name configured in the DNS. If ``tsigSecretSecretRef`` is defined, this field is required."

## obj spec.solver.dns01.rfc2136.tsigSecretSecretRef

"The name of the secret containing the TSIG value. If ``tsigKeyName`` is defined, this field is required."

### fn spec.solver.dns01.rfc2136.tsigSecretSecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used. Some instances of this field may be defaulted, in others it may be required."

### fn spec.solver.dns01.rfc2136.tsigSecretSecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.solver.dns01.route53

"Use the AWS Route53 API to manage DNS01 challenge records."

### fn spec.solver.dns01.route53.withAccessKeyID

```ts
withAccessKeyID(accessKeyID)
```

"The AccessKeyID is used for authentication. Cannot be set when SecretAccessKeyID is set. If neither the Access Key nor Key ID are set, we fall-back to using env vars, shared credentials file or AWS Instance metadata, see: https://docs.aws.amazon.com/sdk-for-go/v1/developer-guide/configuring-sdk.html#specifying-credentials"

### fn spec.solver.dns01.route53.withHostedZoneID

```ts
withHostedZoneID(hostedZoneID)
```

"If set, the provider will manage only this zone in Route53 and will not do an lookup using the route53:ListHostedZonesByName api call."

### fn spec.solver.dns01.route53.withRegion

```ts
withRegion(region)
```

"Always set the region when using AccessKeyID and SecretAccessKey"

### fn spec.solver.dns01.route53.withRole

```ts
withRole(role)
```

"Role is a Role ARN which the Route53 provider will assume using either the explicit credentials AccessKeyID/SecretAccessKey or the inferred credentials from environment variables, shared credentials file or AWS Instance metadata"

## obj spec.solver.dns01.route53.accessKeyIDSecretRef

"The SecretAccessKey is used for authentication. If set, pull the AWS access key ID from a key within a Kubernetes Secret. Cannot be set when AccessKeyID is set. If neither the Access Key nor Key ID are set, we fall-back to using env vars, shared credentials file or AWS Instance metadata, see: https://docs.aws.amazon.com/sdk-for-go/v1/developer-guide/configuring-sdk.html#specifying-credentials"

### fn spec.solver.dns01.route53.accessKeyIDSecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used. Some instances of this field may be defaulted, in others it may be required."

### fn spec.solver.dns01.route53.accessKeyIDSecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.solver.dns01.route53.secretAccessKeySecretRef

"The SecretAccessKey is used for authentication. If neither the Access Key nor Key ID are set, we fall-back to using env vars, shared credentials file or AWS Instance metadata, see: https://docs.aws.amazon.com/sdk-for-go/v1/developer-guide/configuring-sdk.html#specifying-credentials"

### fn spec.solver.dns01.route53.secretAccessKeySecretRef.withKey

```ts
withKey(key)
```

"The key of the entry in the Secret resource's `data` field to be used. Some instances of this field may be defaulted, in others it may be required."

### fn spec.solver.dns01.route53.secretAccessKeySecretRef.withName

```ts
withName(name)
```

"Name of the resource being referred to. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names"

## obj spec.solver.dns01.webhook

"Configure an external webhook based DNS01 challenge solver to manage DNS01 challenge records."

### fn spec.solver.dns01.webhook.withConfig

```ts
withConfig(config)
```

"Additional configuration that should be passed to the webhook apiserver when challenges are processed. This can contain arbitrary JSON data. Secret values should not be specified in this stanza. If secret values are needed (e.g. credentials for a DNS service), you should use a SecretKeySelector to reference a Secret resource. For details on the schema of this field, consult the webhook provider implementation's documentation."

### fn spec.solver.dns01.webhook.withGroupName

```ts
withGroupName(groupName)
```

"The API group name that should be used when POSTing ChallengePayload resources to the webhook apiserver. This should be the same as the GroupName specified in the webhook provider implementation."

### fn spec.solver.dns01.webhook.withSolverName

```ts
withSolverName(solverName)
```

"The name of the solver to use, as defined in the webhook provider implementation. This will typically be the name of the provider, e.g. 'cloudflare'."

## obj spec.solver.http01

"Configures cert-manager to attempt to complete authorizations by performing the HTTP01 challenge flow. It is not possible to obtain certificates for wildcard domain names (e.g. `*.example.com`) using the HTTP01 challenge mechanism."

## obj spec.solver.http01.gatewayHTTPRoute

"The Gateway API is a sig-network community API that models service networking in Kubernetes (https://gateway-api.sigs.k8s.io/). The Gateway solver will create HTTPRoutes with the specified labels in the same namespace as the challenge. This solver is experimental, and fields / behaviour may change in the future."

### fn spec.solver.http01.gatewayHTTPRoute.withLabels

```ts
withLabels(labels)
```

"Custom labels that will be applied to HTTPRoutes created by cert-manager while solving HTTP-01 challenges."

### fn spec.solver.http01.gatewayHTTPRoute.withLabelsMixin

```ts
withLabelsMixin(labels)
```

"Custom labels that will be applied to HTTPRoutes created by cert-manager while solving HTTP-01 challenges."

**Note:** This function appends passed data to existing values

### fn spec.solver.http01.gatewayHTTPRoute.withParentRefs

```ts
withParentRefs(parentRefs)
```

"When solving an HTTP-01 challenge, cert-manager creates an HTTPRoute. cert-manager needs to know which parentRefs should be used when creating the HTTPRoute. Usually, the parentRef references a Gateway. See: https://gateway-api.sigs.k8s.io/v1alpha2/api-types/httproute/#attaching-to-gateways"

### fn spec.solver.http01.gatewayHTTPRoute.withParentRefsMixin

```ts
withParentRefsMixin(parentRefs)
```

"When solving an HTTP-01 challenge, cert-manager creates an HTTPRoute. cert-manager needs to know which parentRefs should be used when creating the HTTPRoute. Usually, the parentRef references a Gateway. See: https://gateway-api.sigs.k8s.io/v1alpha2/api-types/httproute/#attaching-to-gateways"

**Note:** This function appends passed data to existing values

### fn spec.solver.http01.gatewayHTTPRoute.withServiceType

```ts
withServiceType(serviceType)
```

"Optional service type for Kubernetes solver service. Supported values are NodePort or ClusterIP. If unset, defaults to NodePort."

## obj spec.solver.http01.gatewayHTTPRoute.parentRefs

"When solving an HTTP-01 challenge, cert-manager creates an HTTPRoute. cert-manager needs to know which parentRefs should be used when creating the HTTPRoute. Usually, the parentRef references a Gateway. See: https://gateway-api.sigs.k8s.io/v1alpha2/api-types/httproute/#attaching-to-gateways"

### fn spec.solver.http01.gatewayHTTPRoute.parentRefs.withGroup

```ts
withGroup(group)
```

"Group is the group of the referent. \n Support: Core"

### fn spec.solver.http01.gatewayHTTPRoute.parentRefs.withKind

```ts
withKind(kind)
```

"Kind is kind of the referent. \n Support: Core (Gateway) \n Support: Custom (Other Resources)"

### fn spec.solver.http01.gatewayHTTPRoute.parentRefs.withName

```ts
withName(name)
```

"Name is the name of the referent. \n Support: Core"

### fn spec.solver.http01.gatewayHTTPRoute.parentRefs.withNamespace

```ts
withNamespace(namespace)
```

"Namespace is the namespace of the referent. When unspecified (or empty string), this refers to the local namespace of the Route. \n Support: Core"

### fn spec.solver.http01.gatewayHTTPRoute.parentRefs.withPort

```ts
withPort(port)
```

"Port is the network port this Route targets. It can be interpreted differently based on the type of parent resource. \n When the parent resource is a Gateway, this targets all listeners listening on the specified port that also support this kind of Route(and select this Route). It's not recommended to set `Port` unless the networking behaviors specified in a Route must apply to a specific port as opposed to a listener(s) whose port(s) may be changed. When both Port and SectionName are specified, the name and port of the selected listener must match both specified values. \n Implementations MAY choose to support other parent resources. Implementations supporting other types of parent resources MUST clearly document how/if Port is interpreted. \n For the purpose of status, an attachment is considered successful as long as the parent resource accepts it partially. For example, Gateway listeners can restrict which Routes can attach to them by Route kind, namespace, or hostname. If 1 of 2 Gateway listeners accept attachment from the referencing Route, the Route MUST be considered successfully attached. If no Gateway listeners accept attachment from this Route, the Route MUST be considered detached from the Gateway. \n Support: Extended \n <gateway:experimental>"

### fn spec.solver.http01.gatewayHTTPRoute.parentRefs.withSectionName

```ts
withSectionName(sectionName)
```

"SectionName is the name of a section within the target resource. In the following resources, SectionName is interpreted as the following: \n * Gateway: Listener Name. When both Port (experimental) and SectionName are specified, the name and port of the selected listener must match both specified values. \n Implementations MAY choose to support attaching Routes to other resources. If that is the case, they MUST clearly document how SectionName is interpreted. \n When unspecified (empty string), this will reference the entire resource. For the purpose of status, an attachment is considered successful if at least one section in the parent resource accepts it. For example, Gateway listeners can restrict which Routes can attach to them by Route kind, namespace, or hostname. If 1 of 2 Gateway listeners accept attachment from the referencing Route, the Route MUST be considered successfully attached. If no Gateway listeners accept attachment from this Route, the Route MUST be considered detached from the Gateway. \n Support: Core"

## obj spec.solver.http01.ingress

"The ingress based HTTP01 challenge solver will solve challenges by creating or modifying Ingress resources in order to route requests for '/.well-known/acme-challenge/XYZ' to 'challenge solver' pods that are provisioned by cert-manager for each Challenge to be completed."

### fn spec.solver.http01.ingress.withClass

```ts
withClass(class)
```

"The ingress class to use when creating Ingress resources to solve ACME challenges that use this challenge solver. Only one of 'class' or 'name' may be specified."

### fn spec.solver.http01.ingress.withName

```ts
withName(name)
```

"The name of the ingress resource that should have ACME challenge solving routes inserted into it in order to solve HTTP01 challenges. This is typically used in conjunction with ingress controllers like ingress-gce, which maintains a 1:1 mapping between external IPs and ingress resources."

### fn spec.solver.http01.ingress.withServiceType

```ts
withServiceType(serviceType)
```

"Optional service type for Kubernetes solver service. Supported values are NodePort or ClusterIP. If unset, defaults to NodePort."

## obj spec.solver.http01.ingress.ingressTemplate

"Optional ingress template used to configure the ACME challenge solver ingress used for HTTP01 challenges."

## obj spec.solver.http01.ingress.ingressTemplate.metadata

"ObjectMeta overrides for the ingress used to solve HTTP01 challenges. Only the 'labels' and 'annotations' fields may be set. If labels or annotations overlap with in-built values, the values here will override the in-built values."

### fn spec.solver.http01.ingress.ingressTemplate.metadata.withAnnotations

```ts
withAnnotations(annotations)
```

"Annotations that should be added to the created ACME HTTP01 solver ingress."

### fn spec.solver.http01.ingress.ingressTemplate.metadata.withAnnotationsMixin

```ts
withAnnotationsMixin(annotations)
```

"Annotations that should be added to the created ACME HTTP01 solver ingress."

**Note:** This function appends passed data to existing values

### fn spec.solver.http01.ingress.ingressTemplate.metadata.withLabels

```ts
withLabels(labels)
```

"Labels that should be added to the created ACME HTTP01 solver ingress."

### fn spec.solver.http01.ingress.ingressTemplate.metadata.withLabelsMixin

```ts
withLabelsMixin(labels)
```

"Labels that should be added to the created ACME HTTP01 solver ingress."

**Note:** This function appends passed data to existing values

## obj spec.solver.http01.ingress.podTemplate

"Optional pod template used to configure the ACME challenge solver pods used for HTTP01 challenges."

## obj spec.solver.http01.ingress.podTemplate.metadata

"ObjectMeta overrides for the pod used to solve HTTP01 challenges. Only the 'labels' and 'annotations' fields may be set. If labels or annotations overlap with in-built values, the values here will override the in-built values."

### fn spec.solver.http01.ingress.podTemplate.metadata.withAnnotations

```ts
withAnnotations(annotations)
```

"Annotations that should be added to the create ACME HTTP01 solver pods."

### fn spec.solver.http01.ingress.podTemplate.metadata.withAnnotationsMixin

```ts
withAnnotationsMixin(annotations)
```

"Annotations that should be added to the create ACME HTTP01 solver pods."

**Note:** This function appends passed data to existing values

### fn spec.solver.http01.ingress.podTemplate.metadata.withLabels

```ts
withLabels(labels)
```

"Labels that should be added to the created ACME HTTP01 solver pods."

### fn spec.solver.http01.ingress.podTemplate.metadata.withLabelsMixin

```ts
withLabelsMixin(labels)
```

"Labels that should be added to the created ACME HTTP01 solver pods."

**Note:** This function appends passed data to existing values

## obj spec.solver.http01.ingress.podTemplate.spec

"PodSpec defines overrides for the HTTP01 challenge solver pod. Only the 'priorityClassName', 'nodeSelector', 'affinity', 'serviceAccountName' and 'tolerations' fields are supported currently. All other fields will be ignored."

### fn spec.solver.http01.ingress.podTemplate.spec.withNodeSelector

```ts
withNodeSelector(nodeSelector)
```

"NodeSelector is a selector which must be true for the pod to fit on a node. Selector which must match a node's labels for the pod to be scheduled on that node. More info: https://kubernetes.io/docs/concepts/configuration/assign-pod-node/"

### fn spec.solver.http01.ingress.podTemplate.spec.withNodeSelectorMixin

```ts
withNodeSelectorMixin(nodeSelector)
```

"NodeSelector is a selector which must be true for the pod to fit on a node. Selector which must match a node's labels for the pod to be scheduled on that node. More info: https://kubernetes.io/docs/concepts/configuration/assign-pod-node/"

**Note:** This function appends passed data to existing values

### fn spec.solver.http01.ingress.podTemplate.spec.withPriorityClassName

```ts
withPriorityClassName(priorityClassName)
```

"If specified, the pod's priorityClassName."

### fn spec.solver.http01.ingress.podTemplate.spec.withServiceAccountName

```ts
withServiceAccountName(serviceAccountName)
```

"If specified, the pod's service account"

### fn spec.solver.http01.ingress.podTemplate.spec.withTolerations

```ts
withTolerations(tolerations)
```

"If specified, the pod's tolerations."

### fn spec.solver.http01.ingress.podTemplate.spec.withTolerationsMixin

```ts
withTolerationsMixin(tolerations)
```

"If specified, the pod's tolerations."

**Note:** This function appends passed data to existing values

## obj spec.solver.http01.ingress.podTemplate.spec.affinity

"If specified, the pod's scheduling constraints"

## obj spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity

"Describes node affinity scheduling rules for the pod."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.withPreferredDuringSchedulingIgnoredDuringExecution

```ts
withPreferredDuringSchedulingIgnoredDuringExecution(preferredDuringSchedulingIgnoredDuringExecution)
```

"The scheduler will prefer to schedule pods to nodes that satisfy the affinity expressions specified by this field, but it may choose a node that violates one or more of the expressions. The node that is most preferred is the one with the greatest sum of weights, i.e. for each node that meets all of the scheduling requirements (resource request, requiredDuringScheduling affinity expressions, etc.), compute a sum by iterating through the elements of this field and adding \"weight\" to the sum if the node matches the corresponding matchExpressions; the node(s) with the highest sum are the most preferred."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.withPreferredDuringSchedulingIgnoredDuringExecutionMixin

```ts
withPreferredDuringSchedulingIgnoredDuringExecutionMixin(preferredDuringSchedulingIgnoredDuringExecution)
```

"The scheduler will prefer to schedule pods to nodes that satisfy the affinity expressions specified by this field, but it may choose a node that violates one or more of the expressions. The node that is most preferred is the one with the greatest sum of weights, i.e. for each node that meets all of the scheduling requirements (resource request, requiredDuringScheduling affinity expressions, etc.), compute a sum by iterating through the elements of this field and adding \"weight\" to the sum if the node matches the corresponding matchExpressions; the node(s) with the highest sum are the most preferred."

**Note:** This function appends passed data to existing values

## obj spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution

"The scheduler will prefer to schedule pods to nodes that satisfy the affinity expressions specified by this field, but it may choose a node that violates one or more of the expressions. The node that is most preferred is the one with the greatest sum of weights, i.e. for each node that meets all of the scheduling requirements (resource request, requiredDuringScheduling affinity expressions, etc.), compute a sum by iterating through the elements of this field and adding \"weight\" to the sum if the node matches the corresponding matchExpressions; the node(s) with the highest sum are the most preferred."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution.withWeight

```ts
withWeight(weight)
```

"Weight associated with matching the corresponding nodeSelectorTerm, in the range 1-100."

## obj spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution.preference

"A node selector term, associated with the corresponding weight."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution.preference.withMatchExpressions

```ts
withMatchExpressions(matchExpressions)
```

"A list of node selector requirements by node's labels."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution.preference.withMatchExpressionsMixin

```ts
withMatchExpressionsMixin(matchExpressions)
```

"A list of node selector requirements by node's labels."

**Note:** This function appends passed data to existing values

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution.preference.withMatchFields

```ts
withMatchFields(matchFields)
```

"A list of node selector requirements by node's fields."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution.preference.withMatchFieldsMixin

```ts
withMatchFieldsMixin(matchFields)
```

"A list of node selector requirements by node's fields."

**Note:** This function appends passed data to existing values

## obj spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution.preference.matchExpressions

"A list of node selector requirements by node's labels."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution.preference.matchExpressions.withKey

```ts
withKey(key)
```

"The label key that the selector applies to."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution.preference.matchExpressions.withOperator

```ts
withOperator(operator)
```

"Represents a key's relationship to a set of values. Valid operators are In, NotIn, Exists, DoesNotExist. Gt, and Lt."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution.preference.matchExpressions.withValues

```ts
withValues(values)
```

"An array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. If the operator is Gt or Lt, the values array must have a single element, which will be interpreted as an integer. This array is replaced during a strategic merge patch."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution.preference.matchExpressions.withValuesMixin

```ts
withValuesMixin(values)
```

"An array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. If the operator is Gt or Lt, the values array must have a single element, which will be interpreted as an integer. This array is replaced during a strategic merge patch."

**Note:** This function appends passed data to existing values

## obj spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution.preference.matchFields

"A list of node selector requirements by node's fields."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution.preference.matchFields.withKey

```ts
withKey(key)
```

"The label key that the selector applies to."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution.preference.matchFields.withOperator

```ts
withOperator(operator)
```

"Represents a key's relationship to a set of values. Valid operators are In, NotIn, Exists, DoesNotExist. Gt, and Lt."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution.preference.matchFields.withValues

```ts
withValues(values)
```

"An array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. If the operator is Gt or Lt, the values array must have a single element, which will be interpreted as an integer. This array is replaced during a strategic merge patch."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.preferredDuringSchedulingIgnoredDuringExecution.preference.matchFields.withValuesMixin

```ts
withValuesMixin(values)
```

"An array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. If the operator is Gt or Lt, the values array must have a single element, which will be interpreted as an integer. This array is replaced during a strategic merge patch."

**Note:** This function appends passed data to existing values

## obj spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution

"If the affinity requirements specified by this field are not met at scheduling time, the pod will not be scheduled onto the node. If the affinity requirements specified by this field cease to be met at some point during pod execution (e.g. due to an update), the system may or may not try to eventually evict the pod from its node."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.withNodeSelectorTerms

```ts
withNodeSelectorTerms(nodeSelectorTerms)
```

"Required. A list of node selector terms. The terms are ORed."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.withNodeSelectorTermsMixin

```ts
withNodeSelectorTermsMixin(nodeSelectorTerms)
```

"Required. A list of node selector terms. The terms are ORed."

**Note:** This function appends passed data to existing values

## obj spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.nodeSelectorTerms

"Required. A list of node selector terms. The terms are ORed."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.nodeSelectorTerms.withMatchExpressions

```ts
withMatchExpressions(matchExpressions)
```

"A list of node selector requirements by node's labels."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.nodeSelectorTerms.withMatchExpressionsMixin

```ts
withMatchExpressionsMixin(matchExpressions)
```

"A list of node selector requirements by node's labels."

**Note:** This function appends passed data to existing values

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.nodeSelectorTerms.withMatchFields

```ts
withMatchFields(matchFields)
```

"A list of node selector requirements by node's fields."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.nodeSelectorTerms.withMatchFieldsMixin

```ts
withMatchFieldsMixin(matchFields)
```

"A list of node selector requirements by node's fields."

**Note:** This function appends passed data to existing values

## obj spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.nodeSelectorTerms.matchExpressions

"A list of node selector requirements by node's labels."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.nodeSelectorTerms.matchExpressions.withKey

```ts
withKey(key)
```

"The label key that the selector applies to."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.nodeSelectorTerms.matchExpressions.withOperator

```ts
withOperator(operator)
```

"Represents a key's relationship to a set of values. Valid operators are In, NotIn, Exists, DoesNotExist. Gt, and Lt."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.nodeSelectorTerms.matchExpressions.withValues

```ts
withValues(values)
```

"An array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. If the operator is Gt or Lt, the values array must have a single element, which will be interpreted as an integer. This array is replaced during a strategic merge patch."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.nodeSelectorTerms.matchExpressions.withValuesMixin

```ts
withValuesMixin(values)
```

"An array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. If the operator is Gt or Lt, the values array must have a single element, which will be interpreted as an integer. This array is replaced during a strategic merge patch."

**Note:** This function appends passed data to existing values

## obj spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.nodeSelectorTerms.matchFields

"A list of node selector requirements by node's fields."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.nodeSelectorTerms.matchFields.withKey

```ts
withKey(key)
```

"The label key that the selector applies to."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.nodeSelectorTerms.matchFields.withOperator

```ts
withOperator(operator)
```

"Represents a key's relationship to a set of values. Valid operators are In, NotIn, Exists, DoesNotExist. Gt, and Lt."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.nodeSelectorTerms.matchFields.withValues

```ts
withValues(values)
```

"An array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. If the operator is Gt or Lt, the values array must have a single element, which will be interpreted as an integer. This array is replaced during a strategic merge patch."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.nodeAffinity.requiredDuringSchedulingIgnoredDuringExecution.nodeSelectorTerms.matchFields.withValuesMixin

```ts
withValuesMixin(values)
```

"An array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. If the operator is Gt or Lt, the values array must have a single element, which will be interpreted as an integer. This array is replaced during a strategic merge patch."

**Note:** This function appends passed data to existing values

## obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity

"Describes pod affinity scheduling rules (e.g. co-locate this pod in the same node, zone, etc. as some other pod(s))."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.withPreferredDuringSchedulingIgnoredDuringExecution

```ts
withPreferredDuringSchedulingIgnoredDuringExecution(preferredDuringSchedulingIgnoredDuringExecution)
```

"The scheduler will prefer to schedule pods to nodes that satisfy the affinity expressions specified by this field, but it may choose a node that violates one or more of the expressions. The node that is most preferred is the one with the greatest sum of weights, i.e. for each node that meets all of the scheduling requirements (resource request, requiredDuringScheduling affinity expressions, etc.), compute a sum by iterating through the elements of this field and adding \"weight\" to the sum if the node has pods which matches the corresponding podAffinityTerm; the node(s) with the highest sum are the most preferred."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.withPreferredDuringSchedulingIgnoredDuringExecutionMixin

```ts
withPreferredDuringSchedulingIgnoredDuringExecutionMixin(preferredDuringSchedulingIgnoredDuringExecution)
```

"The scheduler will prefer to schedule pods to nodes that satisfy the affinity expressions specified by this field, but it may choose a node that violates one or more of the expressions. The node that is most preferred is the one with the greatest sum of weights, i.e. for each node that meets all of the scheduling requirements (resource request, requiredDuringScheduling affinity expressions, etc.), compute a sum by iterating through the elements of this field and adding \"weight\" to the sum if the node has pods which matches the corresponding podAffinityTerm; the node(s) with the highest sum are the most preferred."

**Note:** This function appends passed data to existing values

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.withRequiredDuringSchedulingIgnoredDuringExecution

```ts
withRequiredDuringSchedulingIgnoredDuringExecution(requiredDuringSchedulingIgnoredDuringExecution)
```

"If the affinity requirements specified by this field are not met at scheduling time, the pod will not be scheduled onto the node. If the affinity requirements specified by this field cease to be met at some point during pod execution (e.g. due to a pod label update), the system may or may not try to eventually evict the pod from its node. When there are multiple elements, the lists of nodes corresponding to each podAffinityTerm are intersected, i.e. all terms must be satisfied."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.withRequiredDuringSchedulingIgnoredDuringExecutionMixin

```ts
withRequiredDuringSchedulingIgnoredDuringExecutionMixin(requiredDuringSchedulingIgnoredDuringExecution)
```

"If the affinity requirements specified by this field are not met at scheduling time, the pod will not be scheduled onto the node. If the affinity requirements specified by this field cease to be met at some point during pod execution (e.g. due to a pod label update), the system may or may not try to eventually evict the pod from its node. When there are multiple elements, the lists of nodes corresponding to each podAffinityTerm are intersected, i.e. all terms must be satisfied."

**Note:** This function appends passed data to existing values

## obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution

"The scheduler will prefer to schedule pods to nodes that satisfy the affinity expressions specified by this field, but it may choose a node that violates one or more of the expressions. The node that is most preferred is the one with the greatest sum of weights, i.e. for each node that meets all of the scheduling requirements (resource request, requiredDuringScheduling affinity expressions, etc.), compute a sum by iterating through the elements of this field and adding \"weight\" to the sum if the node has pods which matches the corresponding podAffinityTerm; the node(s) with the highest sum are the most preferred."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.withWeight

```ts
withWeight(weight)
```

"weight associated with matching the corresponding podAffinityTerm, in the range 1-100."

## obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm

"Required. A pod affinity term, associated with the corresponding weight."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.withNamespaces

```ts
withNamespaces(namespaces)
```

"namespaces specifies a static list of namespace names that the term applies to. The term is applied to the union of the namespaces listed in this field and the ones selected by namespaceSelector. null or empty namespaces list and null namespaceSelector means \"this pod's namespace\"."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.withNamespacesMixin

```ts
withNamespacesMixin(namespaces)
```

"namespaces specifies a static list of namespace names that the term applies to. The term is applied to the union of the namespaces listed in this field and the ones selected by namespaceSelector. null or empty namespaces list and null namespaceSelector means \"this pod's namespace\"."

**Note:** This function appends passed data to existing values

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.withTopologyKey

```ts
withTopologyKey(topologyKey)
```

"This pod should be co-located (affinity) or not co-located (anti-affinity) with the pods matching the labelSelector in the specified namespaces, where co-located is defined as running on a node whose value of the label with key topologyKey matches that of any node on which any of the selected pods is running. Empty topologyKey is not allowed."

## obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector

"A label query over a set of resources, in this case pods."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.withMatchExpressions

```ts
withMatchExpressions(matchExpressions)
```

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.withMatchExpressionsMixin

```ts
withMatchExpressionsMixin(matchExpressions)
```

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

**Note:** This function appends passed data to existing values

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.withMatchLabels

```ts
withMatchLabels(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels map is equivalent to an element of matchExpressions, whose key field is \"key\", the operator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels map is equivalent to an element of matchExpressions, whose key field is \"key\", the operator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

**Note:** This function appends passed data to existing values

## obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.matchExpressions

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.matchExpressions.withKey

```ts
withKey(key)
```

"key is the label key that the selector applies to."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.matchExpressions.withOperator

```ts
withOperator(operator)
```

"operator represents a key's relationship to a set of values. Valid operators are In, NotIn, Exists and DoesNotExist."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.matchExpressions.withValues

```ts
withValues(values)
```

"values is an array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. This array is replaced during a strategic merge patch."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.matchExpressions.withValuesMixin

```ts
withValuesMixin(values)
```

"values is an array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. This array is replaced during a strategic merge patch."

**Note:** This function appends passed data to existing values

## obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector

"A label query over the set of namespaces that the term applies to. The term is applied to the union of the namespaces selected by this field and the ones listed in the namespaces field. null selector and null or empty namespaces list means \"this pod's namespace\". An empty selector ({}) matches all namespaces."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.withMatchExpressions

```ts
withMatchExpressions(matchExpressions)
```

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.withMatchExpressionsMixin

```ts
withMatchExpressionsMixin(matchExpressions)
```

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

**Note:** This function appends passed data to existing values

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.withMatchLabels

```ts
withMatchLabels(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels map is equivalent to an element of matchExpressions, whose key field is \"key\", the operator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels map is equivalent to an element of matchExpressions, whose key field is \"key\", the operator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

**Note:** This function appends passed data to existing values

## obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.matchExpressions

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.matchExpressions.withKey

```ts
withKey(key)
```

"key is the label key that the selector applies to."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.matchExpressions.withOperator

```ts
withOperator(operator)
```

"operator represents a key's relationship to a set of values. Valid operators are In, NotIn, Exists and DoesNotExist."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.matchExpressions.withValues

```ts
withValues(values)
```

"values is an array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. This array is replaced during a strategic merge patch."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.matchExpressions.withValuesMixin

```ts
withValuesMixin(values)
```

"values is an array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. This array is replaced during a strategic merge patch."

**Note:** This function appends passed data to existing values

## obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution

"If the affinity requirements specified by this field are not met at scheduling time, the pod will not be scheduled onto the node. If the affinity requirements specified by this field cease to be met at some point during pod execution (e.g. due to a pod label update), the system may or may not try to eventually evict the pod from its node. When there are multiple elements, the lists of nodes corresponding to each podAffinityTerm are intersected, i.e. all terms must be satisfied."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.withNamespaces

```ts
withNamespaces(namespaces)
```

"namespaces specifies a static list of namespace names that the term applies to. The term is applied to the union of the namespaces listed in this field and the ones selected by namespaceSelector. null or empty namespaces list and null namespaceSelector means \"this pod's namespace\"."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.withNamespacesMixin

```ts
withNamespacesMixin(namespaces)
```

"namespaces specifies a static list of namespace names that the term applies to. The term is applied to the union of the namespaces listed in this field and the ones selected by namespaceSelector. null or empty namespaces list and null namespaceSelector means \"this pod's namespace\"."

**Note:** This function appends passed data to existing values

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.withTopologyKey

```ts
withTopologyKey(topologyKey)
```

"This pod should be co-located (affinity) or not co-located (anti-affinity) with the pods matching the labelSelector in the specified namespaces, where co-located is defined as running on a node whose value of the label with key topologyKey matches that of any node on which any of the selected pods is running. Empty topologyKey is not allowed."

## obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector

"A label query over a set of resources, in this case pods."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.withMatchExpressions

```ts
withMatchExpressions(matchExpressions)
```

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.withMatchExpressionsMixin

```ts
withMatchExpressionsMixin(matchExpressions)
```

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

**Note:** This function appends passed data to existing values

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.withMatchLabels

```ts
withMatchLabels(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels map is equivalent to an element of matchExpressions, whose key field is \"key\", the operator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels map is equivalent to an element of matchExpressions, whose key field is \"key\", the operator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

**Note:** This function appends passed data to existing values

## obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.matchExpressions

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.matchExpressions.withKey

```ts
withKey(key)
```

"key is the label key that the selector applies to."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.matchExpressions.withOperator

```ts
withOperator(operator)
```

"operator represents a key's relationship to a set of values. Valid operators are In, NotIn, Exists and DoesNotExist."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.matchExpressions.withValues

```ts
withValues(values)
```

"values is an array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. This array is replaced during a strategic merge patch."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.matchExpressions.withValuesMixin

```ts
withValuesMixin(values)
```

"values is an array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. This array is replaced during a strategic merge patch."

**Note:** This function appends passed data to existing values

## obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector

"A label query over the set of namespaces that the term applies to. The term is applied to the union of the namespaces selected by this field and the ones listed in the namespaces field. null selector and null or empty namespaces list means \"this pod's namespace\". An empty selector ({}) matches all namespaces."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.withMatchExpressions

```ts
withMatchExpressions(matchExpressions)
```

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.withMatchExpressionsMixin

```ts
withMatchExpressionsMixin(matchExpressions)
```

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

**Note:** This function appends passed data to existing values

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.withMatchLabels

```ts
withMatchLabels(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels map is equivalent to an element of matchExpressions, whose key field is \"key\", the operator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels map is equivalent to an element of matchExpressions, whose key field is \"key\", the operator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

**Note:** This function appends passed data to existing values

## obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.matchExpressions

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.matchExpressions.withKey

```ts
withKey(key)
```

"key is the label key that the selector applies to."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.matchExpressions.withOperator

```ts
withOperator(operator)
```

"operator represents a key's relationship to a set of values. Valid operators are In, NotIn, Exists and DoesNotExist."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.matchExpressions.withValues

```ts
withValues(values)
```

"values is an array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. This array is replaced during a strategic merge patch."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.matchExpressions.withValuesMixin

```ts
withValuesMixin(values)
```

"values is an array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. This array is replaced during a strategic merge patch."

**Note:** This function appends passed data to existing values

## obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity

"Describes pod anti-affinity scheduling rules (e.g. avoid putting this pod in the same node, zone, etc. as some other pod(s))."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.withPreferredDuringSchedulingIgnoredDuringExecution

```ts
withPreferredDuringSchedulingIgnoredDuringExecution(preferredDuringSchedulingIgnoredDuringExecution)
```

"The scheduler will prefer to schedule pods to nodes that satisfy the anti-affinity expressions specified by this field, but it may choose a node that violates one or more of the expressions. The node that is most preferred is the one with the greatest sum of weights, i.e. for each node that meets all of the scheduling requirements (resource request, requiredDuringScheduling anti-affinity expressions, etc.), compute a sum by iterating through the elements of this field and adding \"weight\" to the sum if the node has pods which matches the corresponding podAffinityTerm; the node(s) with the highest sum are the most preferred."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.withPreferredDuringSchedulingIgnoredDuringExecutionMixin

```ts
withPreferredDuringSchedulingIgnoredDuringExecutionMixin(preferredDuringSchedulingIgnoredDuringExecution)
```

"The scheduler will prefer to schedule pods to nodes that satisfy the anti-affinity expressions specified by this field, but it may choose a node that violates one or more of the expressions. The node that is most preferred is the one with the greatest sum of weights, i.e. for each node that meets all of the scheduling requirements (resource request, requiredDuringScheduling anti-affinity expressions, etc.), compute a sum by iterating through the elements of this field and adding \"weight\" to the sum if the node has pods which matches the corresponding podAffinityTerm; the node(s) with the highest sum are the most preferred."

**Note:** This function appends passed data to existing values

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.withRequiredDuringSchedulingIgnoredDuringExecution

```ts
withRequiredDuringSchedulingIgnoredDuringExecution(requiredDuringSchedulingIgnoredDuringExecution)
```

"If the anti-affinity requirements specified by this field are not met at scheduling time, the pod will not be scheduled onto the node. If the anti-affinity requirements specified by this field cease to be met at some point during pod execution (e.g. due to a pod label update), the system may or may not try to eventually evict the pod from its node. When there are multiple elements, the lists of nodes corresponding to each podAffinityTerm are intersected, i.e. all terms must be satisfied."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.withRequiredDuringSchedulingIgnoredDuringExecutionMixin

```ts
withRequiredDuringSchedulingIgnoredDuringExecutionMixin(requiredDuringSchedulingIgnoredDuringExecution)
```

"If the anti-affinity requirements specified by this field are not met at scheduling time, the pod will not be scheduled onto the node. If the anti-affinity requirements specified by this field cease to be met at some point during pod execution (e.g. due to a pod label update), the system may or may not try to eventually evict the pod from its node. When there are multiple elements, the lists of nodes corresponding to each podAffinityTerm are intersected, i.e. all terms must be satisfied."

**Note:** This function appends passed data to existing values

## obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution

"The scheduler will prefer to schedule pods to nodes that satisfy the anti-affinity expressions specified by this field, but it may choose a node that violates one or more of the expressions. The node that is most preferred is the one with the greatest sum of weights, i.e. for each node that meets all of the scheduling requirements (resource request, requiredDuringScheduling anti-affinity expressions, etc.), compute a sum by iterating through the elements of this field and adding \"weight\" to the sum if the node has pods which matches the corresponding podAffinityTerm; the node(s) with the highest sum are the most preferred."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.withWeight

```ts
withWeight(weight)
```

"weight associated with matching the corresponding podAffinityTerm, in the range 1-100."

## obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm

"Required. A pod affinity term, associated with the corresponding weight."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.withNamespaces

```ts
withNamespaces(namespaces)
```

"namespaces specifies a static list of namespace names that the term applies to. The term is applied to the union of the namespaces listed in this field and the ones selected by namespaceSelector. null or empty namespaces list and null namespaceSelector means \"this pod's namespace\"."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.withNamespacesMixin

```ts
withNamespacesMixin(namespaces)
```

"namespaces specifies a static list of namespace names that the term applies to. The term is applied to the union of the namespaces listed in this field and the ones selected by namespaceSelector. null or empty namespaces list and null namespaceSelector means \"this pod's namespace\"."

**Note:** This function appends passed data to existing values

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.withTopologyKey

```ts
withTopologyKey(topologyKey)
```

"This pod should be co-located (affinity) or not co-located (anti-affinity) with the pods matching the labelSelector in the specified namespaces, where co-located is defined as running on a node whose value of the label with key topologyKey matches that of any node on which any of the selected pods is running. Empty topologyKey is not allowed."

## obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector

"A label query over a set of resources, in this case pods."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.withMatchExpressions

```ts
withMatchExpressions(matchExpressions)
```

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.withMatchExpressionsMixin

```ts
withMatchExpressionsMixin(matchExpressions)
```

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

**Note:** This function appends passed data to existing values

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.withMatchLabels

```ts
withMatchLabels(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels map is equivalent to an element of matchExpressions, whose key field is \"key\", the operator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels map is equivalent to an element of matchExpressions, whose key field is \"key\", the operator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

**Note:** This function appends passed data to existing values

## obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.matchExpressions

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.matchExpressions.withKey

```ts
withKey(key)
```

"key is the label key that the selector applies to."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.matchExpressions.withOperator

```ts
withOperator(operator)
```

"operator represents a key's relationship to a set of values. Valid operators are In, NotIn, Exists and DoesNotExist."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.matchExpressions.withValues

```ts
withValues(values)
```

"values is an array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. This array is replaced during a strategic merge patch."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.labelSelector.matchExpressions.withValuesMixin

```ts
withValuesMixin(values)
```

"values is an array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. This array is replaced during a strategic merge patch."

**Note:** This function appends passed data to existing values

## obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector

"A label query over the set of namespaces that the term applies to. The term is applied to the union of the namespaces selected by this field and the ones listed in the namespaces field. null selector and null or empty namespaces list means \"this pod's namespace\". An empty selector ({}) matches all namespaces."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.withMatchExpressions

```ts
withMatchExpressions(matchExpressions)
```

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.withMatchExpressionsMixin

```ts
withMatchExpressionsMixin(matchExpressions)
```

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

**Note:** This function appends passed data to existing values

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.withMatchLabels

```ts
withMatchLabels(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels map is equivalent to an element of matchExpressions, whose key field is \"key\", the operator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels map is equivalent to an element of matchExpressions, whose key field is \"key\", the operator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

**Note:** This function appends passed data to existing values

## obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.matchExpressions

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.matchExpressions.withKey

```ts
withKey(key)
```

"key is the label key that the selector applies to."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.matchExpressions.withOperator

```ts
withOperator(operator)
```

"operator represents a key's relationship to a set of values. Valid operators are In, NotIn, Exists and DoesNotExist."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.matchExpressions.withValues

```ts
withValues(values)
```

"values is an array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. This array is replaced during a strategic merge patch."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.preferredDuringSchedulingIgnoredDuringExecution.podAffinityTerm.namespaceSelector.matchExpressions.withValuesMixin

```ts
withValuesMixin(values)
```

"values is an array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. This array is replaced during a strategic merge patch."

**Note:** This function appends passed data to existing values

## obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution

"If the anti-affinity requirements specified by this field are not met at scheduling time, the pod will not be scheduled onto the node. If the anti-affinity requirements specified by this field cease to be met at some point during pod execution (e.g. due to a pod label update), the system may or may not try to eventually evict the pod from its node. When there are multiple elements, the lists of nodes corresponding to each podAffinityTerm are intersected, i.e. all terms must be satisfied."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.withNamespaces

```ts
withNamespaces(namespaces)
```

"namespaces specifies a static list of namespace names that the term applies to. The term is applied to the union of the namespaces listed in this field and the ones selected by namespaceSelector. null or empty namespaces list and null namespaceSelector means \"this pod's namespace\"."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.withNamespacesMixin

```ts
withNamespacesMixin(namespaces)
```

"namespaces specifies a static list of namespace names that the term applies to. The term is applied to the union of the namespaces listed in this field and the ones selected by namespaceSelector. null or empty namespaces list and null namespaceSelector means \"this pod's namespace\"."

**Note:** This function appends passed data to existing values

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.withTopologyKey

```ts
withTopologyKey(topologyKey)
```

"This pod should be co-located (affinity) or not co-located (anti-affinity) with the pods matching the labelSelector in the specified namespaces, where co-located is defined as running on a node whose value of the label with key topologyKey matches that of any node on which any of the selected pods is running. Empty topologyKey is not allowed."

## obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector

"A label query over a set of resources, in this case pods."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.withMatchExpressions

```ts
withMatchExpressions(matchExpressions)
```

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.withMatchExpressionsMixin

```ts
withMatchExpressionsMixin(matchExpressions)
```

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

**Note:** This function appends passed data to existing values

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.withMatchLabels

```ts
withMatchLabels(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels map is equivalent to an element of matchExpressions, whose key field is \"key\", the operator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels map is equivalent to an element of matchExpressions, whose key field is \"key\", the operator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

**Note:** This function appends passed data to existing values

## obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.matchExpressions

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.matchExpressions.withKey

```ts
withKey(key)
```

"key is the label key that the selector applies to."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.matchExpressions.withOperator

```ts
withOperator(operator)
```

"operator represents a key's relationship to a set of values. Valid operators are In, NotIn, Exists and DoesNotExist."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.matchExpressions.withValues

```ts
withValues(values)
```

"values is an array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. This array is replaced during a strategic merge patch."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.labelSelector.matchExpressions.withValuesMixin

```ts
withValuesMixin(values)
```

"values is an array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. This array is replaced during a strategic merge patch."

**Note:** This function appends passed data to existing values

## obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector

"A label query over the set of namespaces that the term applies to. The term is applied to the union of the namespaces selected by this field and the ones listed in the namespaces field. null selector and null or empty namespaces list means \"this pod's namespace\". An empty selector ({}) matches all namespaces."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.withMatchExpressions

```ts
withMatchExpressions(matchExpressions)
```

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.withMatchExpressionsMixin

```ts
withMatchExpressionsMixin(matchExpressions)
```

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

**Note:** This function appends passed data to existing values

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.withMatchLabels

```ts
withMatchLabels(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels map is equivalent to an element of matchExpressions, whose key field is \"key\", the operator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels map is equivalent to an element of matchExpressions, whose key field is \"key\", the operator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

**Note:** This function appends passed data to existing values

## obj spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.matchExpressions

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.matchExpressions.withKey

```ts
withKey(key)
```

"key is the label key that the selector applies to."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.matchExpressions.withOperator

```ts
withOperator(operator)
```

"operator represents a key's relationship to a set of values. Valid operators are In, NotIn, Exists and DoesNotExist."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.matchExpressions.withValues

```ts
withValues(values)
```

"values is an array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. This array is replaced during a strategic merge patch."

### fn spec.solver.http01.ingress.podTemplate.spec.affinity.podAntiAffinity.requiredDuringSchedulingIgnoredDuringExecution.namespaceSelector.matchExpressions.withValuesMixin

```ts
withValuesMixin(values)
```

"values is an array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. This array is replaced during a strategic merge patch."

**Note:** This function appends passed data to existing values

## obj spec.solver.http01.ingress.podTemplate.spec.tolerations

"If specified, the pod's tolerations."

### fn spec.solver.http01.ingress.podTemplate.spec.tolerations.withEffect

```ts
withEffect(effect)
```

"Effect indicates the taint effect to match. Empty means match all taint effects. When specified, allowed values are NoSchedule, PreferNoSchedule and NoExecute."

### fn spec.solver.http01.ingress.podTemplate.spec.tolerations.withKey

```ts
withKey(key)
```

"Key is the taint key that the toleration applies to. Empty means match all taint keys. If the key is empty, operator must be Exists; this combination means to match all values and all keys."

### fn spec.solver.http01.ingress.podTemplate.spec.tolerations.withOperator

```ts
withOperator(operator)
```

"Operator represents a key's relationship to the value. Valid operators are Exists and Equal. Defaults to Equal. Exists is equivalent to wildcard for value, so that a pod can tolerate all taints of a particular category."

### fn spec.solver.http01.ingress.podTemplate.spec.tolerations.withTolerationSeconds

```ts
withTolerationSeconds(tolerationSeconds)
```

"TolerationSeconds represents the period of time the toleration (which must be of effect NoExecute, otherwise this field is ignored) tolerates the taint. By default, it is not set, which means tolerate the taint forever (do not evict). Zero and negative values will be treated as 0 (evict immediately) by the system."

### fn spec.solver.http01.ingress.podTemplate.spec.tolerations.withValue

```ts
withValue(value)
```

"Value is the taint value the toleration matches to. If the operator is Exists, the value should be empty, otherwise just a regular string."

## obj spec.solver.selector

"Selector selects a set of DNSNames on the Certificate resource that should be solved using this challenge solver. If not specified, the solver will be treated as the 'default' solver with the lowest priority, i.e. if any other solver has a more specific match, it will be used instead."

### fn spec.solver.selector.withDnsNames

```ts
withDnsNames(dnsNames)
```

"List of DNSNames that this solver will be used to solve. If specified and a match is found, a dnsNames selector will take precedence over a dnsZones selector. If multiple solvers match with the same dnsNames value, the solver with the most matching labels in matchLabels will be selected. If neither has more matches, the solver defined earlier in the list will be selected."

### fn spec.solver.selector.withDnsNamesMixin

```ts
withDnsNamesMixin(dnsNames)
```

"List of DNSNames that this solver will be used to solve. If specified and a match is found, a dnsNames selector will take precedence over a dnsZones selector. If multiple solvers match with the same dnsNames value, the solver with the most matching labels in matchLabels will be selected. If neither has more matches, the solver defined earlier in the list will be selected."

**Note:** This function appends passed data to existing values

### fn spec.solver.selector.withDnsZones

```ts
withDnsZones(dnsZones)
```

"List of DNSZones that this solver will be used to solve. The most specific DNS zone match specified here will take precedence over other DNS zone matches, so a solver specifying sys.example.com will be selected over one specifying example.com for the domain www.sys.example.com. If multiple solvers match with the same dnsZones value, the solver with the most matching labels in matchLabels will be selected. If neither has more matches, the solver defined earlier in the list will be selected."

### fn spec.solver.selector.withDnsZonesMixin

```ts
withDnsZonesMixin(dnsZones)
```

"List of DNSZones that this solver will be used to solve. The most specific DNS zone match specified here will take precedence over other DNS zone matches, so a solver specifying sys.example.com will be selected over one specifying example.com for the domain www.sys.example.com. If multiple solvers match with the same dnsZones value, the solver with the most matching labels in matchLabels will be selected. If neither has more matches, the solver defined earlier in the list will be selected."

**Note:** This function appends passed data to existing values

### fn spec.solver.selector.withMatchLabels

```ts
withMatchLabels(matchLabels)
```

"A label selector that is used to refine the set of certificate's that this challenge solver will apply to."

### fn spec.solver.selector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"A label selector that is used to refine the set of certificate's that this challenge solver will apply to."

**Note:** This function appends passed data to existing values