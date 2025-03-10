---
title: "policyRoot resource type"
description: "Resource type exposing navigation properties for the policies singleton."
author: "rkarim-ms"
ms.localizationpriority: medium
ms.prod: "governance"
doc_type: resourcePageType
---

# policyRoot resource type

Namespace: microsoft.graph

Resource type exposing navigation properties for the policies singleton. Inherits from [entity](../resources/entity.md).

## Methods
None

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|Unique identifier of the policy. Inherited from [entity](../resources/entity.md).|


## Relationships
| Relationship                              | Type                                                                                                      | Description                                                                                                                                                          |
|:------------------------------------------|:----------------------------------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| activityBasedTimeoutPolicies              | [activityBasedTimeoutPolicy](activitybasedtimeoutpolicy.md) collection                                    | The policy that controls the idle time out for web sessions for applications.                                                                                        |
| adminConsentRequestPolicy                 | [adminConsentRequestPolicy](adminconsentrequestpolicy.md)                                                 | The policy by which consent requests are created and managed for the entire tenant.                                                                                  |
| authenticationFlowsPolicy                 | [authenticationFlowsPolicy](authenticationflowspolicy.md)                                                 | The policy configuration of the self-service sign-up experience of external users.                                                                                   |
| authenticationMethodsPolicy               | [authenticationMethodsPolicy](authenticationmethodspolicy.md)                                             | The authentication methods and the users that are allowed to use them to sign in and perform multi-factor authentication (MFA) in Azure Active Directory (Azure AD). |
| authorizationPolicy                       | [authorizationPolicy](authorizationpolicy.md) collection                                                  | The policy that controls Azure AD authorization settings.                                                                                                            |
| claimsMappingPolicies                     | [claimsMappingPolicy](claimsmappingpolicy.md) collection                                                  | The claim-mapping policies for WS-Fed, SAML, OAuth 2.0, and OpenID Connect protocols, for tokens issued to a specific application.                                   |
| conditionalAccessPolicies                 | [conditionalAccessPolicy](conditionalaccesspolicy.md)                                                     | The custom rules that define an access scenario.                                                                                                                     |
| crossTenantAccessPolicy                   | [crossTenantAccessPolicy](crosstenantaccesspolicy.md)                           | The custom rules that define an access scenario when interacting with external Azure AD tenants.                                                                                                                     |
| featureRolloutPolicies                    | [featureRolloutPolicy](featurerolloutpolicy.md) collection                                                | The feature rollout policy associated with a directory object.                                                                                                       |
| homeRealmDiscoveryPolicies                | [homeRealmDiscoveryPolicy](homerealmdiscoverypolicy.md) collection                                        | The policy to control Azure AD authentication behavior for federated users.                                                                                          |
| identitySecurityDefaultsEnforcementPolicy | [identitySecurityDefaultsEnforcementPolicy](identitysecuritydefaultsenforcementpolicy.md)                 | The policy that represents the security defaults that protect against common attacks.                                                                                |
| permissionGrantPolicies                   | [permissionGrantPolicy](permissiongrantpolicy.md) collection                                              | The policy that specifies the conditions under which consent can be granted.                                                                                         |
|roleManagementPolicies|[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) collection| Specifies the various policies associated with scopes and roles. |
|roleManagementPolicyAssignments|[unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) collection| The assignment of a role management policy to a role definition object. |
| tokenIssuancePolicies                     | [tokenIssuancePolicy](tokenissuancepolicy.md) collection                                                  | The policy that specifies the characteristics of SAML tokens issued by Azure AD.                                                                                     |
| tokenLifetimePolicies                     | [tokenLifetimePolicy](tokenlifetimepolicy.md) collection                                                  | The policy that controls the lifetime of a JWT access token, an ID token, or a SAML 1.1/2.0 token issued by Azure AD.                                                |


## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.policyRoot",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.policyRoot",
  "id": "String (identifier)"
}
```

