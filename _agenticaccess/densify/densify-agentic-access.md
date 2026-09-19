---
acting_count: 36
action_class_counts:
  acting: 36
  connected: 37
api_specs:
- filename: densify-analysis-webhook-api-openapi.yml
  format: yaml
  label: Densify Analysis Webhook API
  slug: densify-analysis-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-analysis-webhook-api-openapi.yml
- filename: densify-authentication-api-openapi.yml
  format: yaml
  label: Densify Authentication API
  slug: densify-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-authentication-api-openapi.yml
- filename: densify-aws-analysis-api-openapi.yml
  format: yaml
  label: Densify AWS Analysis API
  slug: densify-aws-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-aws-analysis-api-openapi.yml
- filename: densify-aws-analyze-api-openapi.yml
  format: yaml
  label: Densify AWS Analyze API
  slug: densify-aws-analyze-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-aws-analyze-api-openapi.yml
- filename: densify-azure-analysis-api-openapi.yml
  format: yaml
  label: Densify Azure Analysis API
  slug: densify-azure-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-azure-analysis-api-openapi.yml
- filename: densify-cloud-analysis-api-openapi.yml
  format: yaml
  label: Densify Cloud Analysis API
  slug: densify-cloud-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-cloud-analysis-api-openapi.yml
- filename: densify-gcp-analysis-api-openapi.yml
  format: yaml
  label: Densify GCP Analysis API
  slug: densify-gcp-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-gcp-analysis-api-openapi.yml
- filename: densify-kubernetes-api-openapi.yml
  format: yaml
  label: Densify Kubernetes API
  slug: densify-kubernetes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-kubernetes-api-openapi.yml
- filename: densify-kubernetes-cluster-results-api-openapi.yml
  format: yaml
  label: Densify Kubernetes Cluster Results API
  slug: densify-kubernetes-cluster-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-kubernetes-cluster-results-api-openapi.yml
- filename: densify-kubernetes-clusters-api-openapi.yml
  format: yaml
  label: Densify Kubernetes Clusters API
  slug: densify-kubernetes-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-kubernetes-clusters-api-openapi.yml
- filename: densify-recommendations-api-openapi.yml
  format: yaml
  label: Densify Recommendations API
  slug: densify-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-recommendations-api-openapi.yml
- filename: densify-subscriptions-api-openapi.yml
  format: yaml
  label: Densify Subscriptions API
  slug: densify-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-subscriptions-api-openapi.yml
- filename: densify-subscriptions-properties-api-openapi.yml
  format: yaml
  label: Densify Subscriptions Properties API
  slug: densify-subscriptions-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-subscriptions-properties-api-openapi.yml
- filename: densify-subscriptions-suppressions-api-openapi.yml
  format: yaml
  label: Densify Subscriptions Suppressions API
  slug: densify-subscriptions-suppressions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-subscriptions-suppressions-api-openapi.yml
- filename: densify-subscriptions-tags-api-openapi.yml
  format: yaml
  label: Densify Subscriptions Tags API
  slug: densify-subscriptions-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-subscriptions-tags-api-openapi.yml
- filename: densify-system-api-openapi.yml
  format: yaml
  label: Densify System API
  slug: densify-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-system-api-openapi.yml
- filename: densify-systems-api-openapi.yml
  format: yaml
  label: Densify Systems API
  slug: densify-systems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/openapi/densify-systems-api-openapi.yml
consequence_counts:
  read: 37
  write: 36
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Densify Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 73
overview: 'Densify exposes 73 API operations that an AI agent could call, of which 36 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 37 read and 36 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Densify
provider_slug: densify
slug: densify-agentic-access
source_filename: densify-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: generated\nsource: openapi/densify-analysis-webhook-api-openapi.yml, openapi/densify-authentication-api-openapi.yml,\n  openapi/densify-aws-analysis-api-openapi.yml, openapi/densify-aws-analyze-api-openapi.yml,\n  openapi/densify-azure-analysis-api-openapi.yml, openapi/densify-cloud-analysis-api-openapi.yml,\n  openapi/densify-gcp-analysis-api-openapi.yml, openapi/densify-kubernetes-api-openapi.yml,\n  openapi/densify-kubernetes-cluster-results-api-openapi.yml, openapi/densify-kubernetes-clusters-api-openapi.yml,\n  openapi/densify-recommendations-api-openapi.yml, openapi/densify-subscriptions-api-openapi.yml,\n  openapi/densify-subscriptions-properties-api-openapi.yml, openapi/densify-subscriptions-suppressions-api-openapi.yml,\n  openapi/densify-subscriptions-tags-api-openapi.yml, openapi/densify-system-api-openapi.yml,\n  openapi/densify-systems-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically\
  \ from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 73\n  by_action_class:\n    connected: 37\n    acting: 36\n  by_consequence:\n    read: 37\n    write: 36\n  human_in_the_loop_required: 0\noperations:\n- path: /webhook/analysis/{platformType}\n  method: get\n  operationId: listAnalysisWebhooksByPlatform\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook/analysis/{platformType}/{platformSubType}/{analysisId}\n  method: get\n  operationId: getAnalysisWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook/analysis/{platformType}/{platformSubType}/{analysisId}\n  method: post\n  operationId: addAnalysisWebhook\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook/analysis/{platformType}/{platformSubType}/{analysisId}\n  method: put\n  operationId: updateAnalysisWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook/analysis/{platformType}/{platformSubType}/{analysisId}\n  method: delete\n  operationId: deleteAnalysisWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /authorize\n  method: post\n  operationId: authorize\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analysis/cloud/aws/{analysisId}\n  method: delete\n  operationId: deleteAwsAnalysis\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analysis/cloud/aws/{analysisId}/results\n  method: get\n  operationId: getAwsRecommendations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /analysis/cloud/aws/analyze\n  method: post\n  operationId: analyzeAws\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analysis/cloud/aws\n  method: get\n  operationId: listAwsAnalyses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analysis/azure/analyze\n  method: post\n  operationId: analyzeAzure\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analysis/cloud/azure\n  method: get\n \
  \ operationId: listAzureAnalyses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analysis/azure/{subscriptionId}/status\n  method: get\n  operationId: getAzureAnalysisStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analysis/cloud/azure/{analysisId}\n  method: delete\n  operationId: deleteAzureAnalysisAudit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analysis/cloud/azure/{analysisId}/results\n  method: get\n  operationId: listAzureRecommendations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analysis/aws\n  method: post\n  operationId: startAwsAnalysis\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analysis/azure\n  method: post\n  operationId: startAzureAnalysis\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analysis/gcp\n  method: post\n  operationId: startGcpAnalysis\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analysis/gcp/analyze\n  method: post\n  operationId: analyzeGcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analysis/cloud/gcp/analyze\n  method: post\n  operationId: historicalAuditGcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analysis/cloud/gcp\n  method: get\n  operationId: listGcpAnalyses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /analysis/cloud/gcp/{analysisId}\n  method: delete\n  operationId: deleteGcpAnalysisAudit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analysis/cloud/gcp/{analysisId}/results\n  method: get\n  operationId: listGcpRecommendations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /kubernetes/clusters\n  method: get\n  operationId: listKubernetesClusters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /kubernetes/clusters/{clusterName}/containers\n  method: get\n  operationId: getKubernetesContainers\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /kubernetes/clusters/{clusterName}/containers\n  method: get\n  operationId: getKubernetesClusterContainers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /kubernetes/clusters/{clusterName}/containers?details=true\n  method: get\n  operationId: getKubernetesClusterContainersDetailed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /kubernetes/clusters\n  method: get\n  operationId: listKubernetesClusters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /kubernetes/clusters/{clusterName}\n  method: get\n  operationId: getKubernetesClusterDetails\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analysis/aws/{analysisId}/recommendations\n  method: get\n  operationId: getAwsRecommendations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analysis/azure/{analysisId}/recommendations\n  method: get\n  operationId: getAzureRecommendations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analysis/gcp/{analysisId}/recommendations\n  method: get\n  operationId: getGcpRecommendations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions\n  method: get\n  operationId: listSubscriptionsDefaultPlatform\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/{platformType}\n  method: get\n  operationId: listSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/{platformType}\n  method: post\n  operationId: createSubscriptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{platformType}\n  method: delete\n  operationId: deleteSubscriptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{platformType}/{subscriptionRef}\n  method: put\n  operationId: replaceSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{platformType}/{subscriptionRef}\n  method: delete\n  operationId: deleteSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{platformType}/{subscriptionRef}\n  method: get\n  operationId: getSubscriptionResults\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/{subscriptionRef}\n  method: get\n  operationId: getSubscriptionResultsDefaultPlatform\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/{platformType}/{subscriptionRef}/status\n  method: get\n  operationId: getSubscriptionStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/{subscriptionRef}/status\n  method: get\n  operationId: getSubscriptionStatusDefaultPlatform\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/{platformType}/properties\n  method: get\n  operationId: listSubscriptionProperties\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/{platformType}/properties\n  method: post\n  operationId: addSubscriptionProperties\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{platformType}/properties\n  method: put\n  operationId: replaceSubscriptionProperties\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{platformType}/properties\n  method: delete\n  operationId:\
  \ deleteSubscriptionProperties\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{platformType}/properties/{propertyRef}\n  method: get\n  operationId: getSubscriptionProperty\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/{platformType}/properties/{propertyRef}\n  method: put\n  operationId: replaceSubscriptionProperty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{platformType}/properties/{propertyRef}\n\
  \  method: delete\n  operationId: deleteSubscriptionProperty\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/properties\n  method: get\n  operationId: listSubscriptionPropertiesDefaultPlatform\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/{platformType}/suppressions\n  method: get\n  operationId: listSuppressions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/{platformType}/suppressions\n  method: post\n  operationId: createSuppressions\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{platformType}/suppressions\n  method: put\n  operationId: replaceSuppressions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{platformType}/suppressions\n  method: delete\n  operationId: deleteSuppressions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{platformType}/suppressions/{suppressionRef}\n\
  \  method: get\n  operationId: getSuppression\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/{platformType}/suppressions/{suppressionRef}\n  method: put\n  operationId: replaceSuppression\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{platformType}/suppressions/{suppressionRef}\n  method: delete\n  operationId: deleteSuppression\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/suppressions\n\
  \  method: get\n  operationId: listSuppressionsDefaultPlatform\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/{platformType}/tags\n  method: get\n  operationId: listSubscriptionTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/{platformType}/tags\n  method: post\n  operationId: addSubscriptionTags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{platformType}/tags\n  method: put\n  operationId: replaceSubscriptionTags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{platformType}/tags\n  method: delete\n  operationId: deleteSubscriptionTags\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{platformType}/tags/{tagRef}\n  method: get\n  operationId: getSubscriptionTag\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions/{platformType}/tags/{tagRef}\n  method: put\n  operationId: replaceSubscriptionTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/{platformType}/tags/{tagRef}\n  method: delete\n  operationId: deleteSubscriptionTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /subscriptions/tags\n  method: get\n  operationId: listSubscriptionTagsDefaultPlatform\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ping\n  method: get\n  operationId: ping\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /systems\n  method: get\n  operationId: listSystems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /systems/{id}\n  method: get\n  operationId: getSystem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /systems/{id}/analysis-details\n  method: post\n  operationId: getSystemAnalysisDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /systems/{id}/analysis-report\n  method: get\n  operationId: downloadAnalysisReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /systems/{id}/attributes\n  method: put\n  operationId: modifySystemAttributes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /systems/{id}/attributes\n  method: delete\n  operationId: deleteSystemAttributes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/densify/refs/heads/main/agentic-access/densify-agentic-access.yml
summary_line: 73 operations · 36 acting
tags:
- Cloud Cost
- Container Optimization
- FinOps
- Kubernetes
- Machine-Learning
- Recommendations
- Rightsizing
---
