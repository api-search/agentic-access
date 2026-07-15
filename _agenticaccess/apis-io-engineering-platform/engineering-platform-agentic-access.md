---
acting_count: 1382
action_class_counts:
  acting: 1382
  connected: 1375
api_specs:
- filename: aws-s3-openapi-original.yml
  format: yaml
  label: Amazon S3
  slug: aws-s3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-search/engineering-platform/refs/heads/main/openapi/aws-s3-openapi-original.yml
- filename: aws-lambda-openapi-original.yml
  format: yaml
  label: AWS Lambda
  slug: aws-lambda
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-search/engineering-platform/refs/heads/main/openapi/aws-lambda-openapi-original.yml
- filename: aws-api-gateway-openapi-original.yml
  format: yaml
  label: AWS API Gateway
  slug: aws-api-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-search/engineering-platform/refs/heads/main/openapi/aws-api-gateway-openapi-original.yml
- filename: aws-rds-openapi-original.yml
  format: yaml
  label: AWS RDS
  slug: aws-rds
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-search/engineering-platform/refs/heads/main/openapi/aws-rds-openapi-original.yml
- filename: aws-iam-openapi-original.yml
  format: yaml
  label: AWS IAM
  slug: aws-iam
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-search/engineering-platform/refs/heads/main/openapi/aws-iam-openapi-original.yml
- filename: microsoft-cognitive-web-search-openapi-original.yml
  format: yaml
  label: Microsoft Bing Search
  slug: microsoft-bing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-search/engineering-platform/refs/heads/main/openapi/microsoft-cognitive-web-search-openapi-original.yml
- filename: postman-openapi-original.yml
  format: yaml
  label: Postman
  slug: postman
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-search/engineering-platform/refs/heads/main/openapi/postman-openapi-original.yml
- filename: cloudflare-openapi-original.yml
  format: yaml
  label: Cloudflare
  slug: cloudflare
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-search/engineering-platform/refs/heads/main/openapi/cloudflare-openapi-original.yml
- filename: github-openapi-original.yml
  format: yaml
  label: GitHub
  slug: github
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-search/engineering-platform/refs/heads/main/openapi/github-openapi-original.yml
consequence_counts:
  physical: 58
  read: 1375
  safety-critical: 36
  write: 1288
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 36
kind: agentic-access
layout: agentic-access
method: generated
name: Engineering Platform Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#Action=ListOpenIDConnectProviderTags
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#Action=ListOpenIDConnectProviders
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /#Action=ResetServiceSpecificCredential
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /accounts/{account_id}/access/apps/{app_id}/revoke_tokens
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /accounts/{account_id}/access/organizations/revoke_user
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /accounts/{account_id}/devices/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /accounts/{account_id}/devices/unrevoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /accounts/{account_id}/intel/indicator-feeds/permissions/remove
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /accounts/{account_id}/logs/control/cmb/config
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /accounts/{account_id}/logs/control/cmb/config
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /accounts/{account_id}/r2/buckets/{bucket_name}/sippy
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /accounts/{account_id}/workers/dispatch/namespaces
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /accounts/{account_id}/workers/dispatch/namespaces/{dispatch_namespace}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /accounts/{account_id}/workers/dispatch/namespaces/{dispatch_namespace}/scripts/{script_name}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /accounts/{account_id}/workers/dispatch/namespaces/{dispatch_namespace}/scripts/{script_name}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /accounts/{account_id}/workers/dispatch/namespaces/{dispatch_namespace}/scripts/{script_name}/content
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /accounts/{account_id}/workers/dispatch/namespaces/{dispatch_namespace}/scripts/{script_name}/secrets
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /accounts/{account_id}/workers/dispatch/namespaces/{dispatch_namespace}/scripts/{script_name}/settings
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /accounts/{account_id}/workers/dispatch/namespaces/{dispatch_namespace}/scripts/{script_name}/tags
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /accounts/{account_id}/workers/dispatch/namespaces/{dispatch_namespace}/scripts/{script_name}/tags/{tag}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /accounts/{account_id}/workers/dispatch/namespaces/{dispatch_namespace}/scripts/{script_name}/tags/{tag}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /accounts/{account_id}/zt_risk_scoring/{user_id}/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /applications/{client_id}/token
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /certificates/{certificate_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /enterprises/{enterprise}/actions/permissions/organizations/{org_id}
operation_count: 2757
overview: 'APIs.io Engineering Platform exposes 2757 API operations that an AI agent could call, of which 1382 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1375 read, 1288 write, 58 physical, and 36 safety-critical.


  36 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: APIs.io Engineering Platform
provider_slug: apis-io-engineering-platform
slug: engineering-platform-agentic-access
source_filename: engineering-platform-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/aws-api-gateway-openapi-original.yml, openapi/aws-iam-openapi-original.yml,\n  openapi/aws-lambda-openapi-original.yml, openapi/cloudflare-openapi-original.yml, openapi/github-openapi-original.yml,\n  openapi/microsoft-cognitive-news-search-openapi-original.yml, openapi/microsoft-cognitive-video-search-openapi-original.yml,\n  openapi/microsoft-cognitive-web-search-openapi-original.yml, openapi/postman-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 2757\n  by_action_class:\n    acting: 1382\n    connected: 1375\n  by_consequence:\n    write: 1288\n    read: 1375\n    physical: 58\n    safety-critical: 36\n  human_in_the_loop_required: 36\noperations:\n- path: /apikeys\n\
  \  method: post\n  operationId: CreateApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apikeys\n  method: get\n  operationId: GetApiKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restapis/{restapi_id}/authorizers\n  method: post\n  operationId: CreateAuthorizer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapis/{restapi_id}/authorizers\n  method: get\n  operationId: GetAuthorizers\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domainnames/{domain_name}/basepathmappings\n  method: post\n  operationId: CreateBasePathMapping\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domainnames/{domain_name}/basepathmappings\n  method: get\n  operationId: GetBasePathMappings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restapis/{restapi_id}/deployments\n  method: post\n  operationId: CreateDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n\
  \      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapis/{restapi_id}/deployments\n  method: get\n  operationId: GetDeployments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restapis/{restapi_id}/documentation/parts\n  method: post\n  operationId: CreateDocumentationPart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapis/{restapi_id}/documentation/parts\n  method: get\n  operationId: GetDocumentationParts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /restapis/{restapi_id}/documentation/parts\n  method: put\n  operationId: ImportDocumentationParts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapis/{restapi_id}/documentation/versions\n  method: post\n  operationId: CreateDocumentationVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapis/{restapi_id}/documentation/versions\n  method: get\n  operationId: GetDocumentationVersions\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domainnames\n  method: post\n  operationId: CreateDomainName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domainnames\n  method: get\n  operationId: GetDomainNames\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restapis/{restapi_id}/models\n  method: post\n  operationId: CreateModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /restapis/{restapi_id}/models\n  method: get\n  operationId: GetModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restapis/{restapi_id}/requestvalidators\n  method: post\n  operationId: CreateRequestValidator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapis/{restapi_id}/requestvalidators\n  method: get\n  operationId: GetRequestValidators\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restapis/{restapi_id}/resources/{parent_id}\n  method: post\n  operationId: CreateResource\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapis\n  method: post\n  operationId: CreateRestApi\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapis\n  method: get\n  operationId: GetRestApis\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restapis/{restapi_id}/stages\n  method: post\n  operationId: CreateStage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapis/{restapi_id}/stages\n  method: get\n  operationId: GetStages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /usageplans\n  method: post\n  operationId: CreateUsagePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /usageplans\n  method: get\n  operationId: GetUsagePlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /usageplans/{usageplanId}/keys\n  method: post\n  operationId: CreateUsagePlanKey\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /usageplans/{usageplanId}/keys\n  method: get\n  operationId: GetUsagePlanKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vpclinks\n  method: post\n  operationId: CreateVpcLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vpclinks\n  method: get\n  operationId: GetVpcLinks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apikeys/{api_Key}\n  method: delete\n  operationId: DeleteApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apikeys/{api_Key}\n  method: get\n  operationId: GetApiKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apikeys/{api_Key}\n  method: patch\n  operationId: UpdateApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapis/{restapi_id}/authorizers/{authorizer_id}\n\
  \  method: delete\n  operationId: DeleteAuthorizer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapis/{restapi_id}/authorizers/{authorizer_id}\n  method: get\n  operationId: GetAuthorizer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restapis/{restapi_id}/authorizers/{authorizer_id}\n  method: post\n  operationId: TestInvokeAuthorizer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapis/{restapi_id}/authorizers/{authorizer_id}\n\
  \  method: patch\n  operationId: UpdateAuthorizer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domainnames/{domain_name}/basepathmappings/{base_path}\n  method: delete\n  operationId: DeleteBasePathMapping\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domainnames/{domain_name}/basepathmappings/{base_path}\n  method: get\n  operationId: GetBasePathMapping\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domainnames/{domain_name}/basepathmappings/{base_path}\n\
  \  method: patch\n  operationId: UpdateBasePathMapping\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clientcertificates/{clientcertificate_id}\n  method: delete\n  operationId: DeleteClientCertificate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clientcertificates/{clientcertificate_id}\n  method: get\n  operationId: GetClientCertificate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clientcertificates/{clientcertificate_id}\n\
  \  method: patch\n  operationId: UpdateClientCertificate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapis/{restapi_id}/deployments/{deployment_id}\n  method: delete\n  operationId: DeleteDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapis/{restapi_id}/deployments/{deployment_id}\n  method: get\n  operationId: GetDeployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /restapis/{restapi_id}/deployments/{deployment_id}\n  method: patch\n  operationId: UpdateDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapis/{restapi_id}/documentation/parts/{part_id}\n  method: delete\n  operationId: DeleteDocumentationPart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapis/{restapi_id}/documentation/parts/{part_id}\n  method: get\n  operationId: GetDocumentationPart\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restapis/{restapi_id}/documentation/parts/{part_id}\n  method: patch\n  operationId: UpdateDocumentationPart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapis/{restapi_id}/documentation/versions/{doc_version}\n  method: delete\n  operationId: DeleteDocumentationVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapis/{restapi_id}/documentation/versions/{doc_version}\n \
  \ method: get\n  operationId: GetDocumentationVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restapis/{restapi_id}/documentation/versions/{doc_version}\n  method: patch\n  operationId: UpdateDocumentationVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domainnames/{domain_name}\n  method: delete\n  operationId: DeleteDomainName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domainnames/{domain_name}\n\
  \  method: get\n  operationId: GetDomainName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domainnames/{domain_name}\n  method: patch\n  operationId: UpdateDomainName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapis/{restapi_id}/gatewayresponses/{response_type}\n  method: delete\n  operationId: DeleteGatewayResponse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapis/{restapi_id}/gatewayresponses/{response_type}\n\
  \  method: get\n  operationId: GetGatewayResponse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restapis/{restapi_id}/gatewayresponses/{response_type}\n  method: put\n  operationId: PutGatewayResponse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapis/{restapi_id}/gatewayresponses/{response_type}\n  method: patch\n  operationId: UpdateGatewayResponse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapis/{restapi_id}/resources/{resource_id}/methods/{http_method}/integration\n\
  \  method: delete\n  operationId: DeleteIntegration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapis/{restapi_id}/resources/{resource_id}/methods/{http_method}/integration\n  method: get\n  operationId: GetIntegration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restapis/{restapi_id}/resources/{resource_id}/methods/{http_method}/integration\n  method: put\n  operationId: PutIntegration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /restapis/{restapi_id}/resources/{resource_id}/methods/{http_method}/integration\n  method: patch\n  operationId: UpdateIntegration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapis/{restapi_id}/resources/{resource_id}/methods/{http_method}/integration/responses/{status_code}\n  method: delete\n  operationId: DeleteIntegrationResponse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapis/{restapi_id}/resources/{resource_id}/methods/{http_method}/integration/responses/{status_code}\n\
  \  method: get\n  operationId: GetIntegrationResponse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restapis/{restapi_id}/resources/{resource_id}/methods/{http_method}/integration/responses/{status_code}\n  method: put\n  operationId: PutIntegrationResponse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapis/{restapi_id}/resources/{resource_id}/methods/{http_method}/integration/responses/{status_code}\n  method: patch\n  operationId: UpdateIntegrationResponse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapis/{restapi_id}/resources/{resource_id}/methods/{http_method}\n  method: delete\n  operationId: DeleteMethod\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapis/{restapi_id}/resources/{resource_id}/methods/{http_method}\n  method: get\n  operationId: GetMethod\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restapis/{restapi_id}/resources/{resource_id}/methods/{http_method}\n  method: put\n  operationId: PutMethod\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapis/{restapi_id}/resources/{resource_id}/methods/{http_method}\n  method: post\n  operationId: TestInvokeMethod\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapis/{restapi_id}/resources/{resource_id}/methods/{http_method}\n  method: patch\n  operationId: UpdateMethod\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapis/{restapi_id}/resources/{resource_id}/methods/{http_method}/responses/{status_code}\n\
  \  method: delete\n  operationId: DeleteMethodResponse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapis/{restapi_id}/resources/{resource_id}/methods/{http_method}/responses/{status_code}\n  method: get\n  operationId: GetMethodResponse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restapis/{restapi_id}/resources/{resource_id}/methods/{http_method}/responses/{status_code}\n  method: put\n  operationId: PutMethodResponse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /restapis/{restapi_id}/resources/{resource_id}/methods/{http_method}/responses/{status_code}\n  method: patch\n  operationId: UpdateMethodResponse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapis/{restapi_id}/models/{model_name}\n  method: delete\n  operationId: DeleteModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapis/{restapi_id}/models/{model_name}\n  method: get\n  operationId: GetModel\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restapis/{restapi_id}/models/{model_name}\n  method: patch\n  operationId: UpdateModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapis/{restapi_id}/requestvalidators/{requestvalidator_id}\n  method: delete\n  operationId: DeleteRequestValidator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapis/{restapi_id}/requestvalidators/{requestvalidator_id}\n  method: get\n  operationId: GetRequestValidator\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restapis/{restapi_id}/requestvalidators/{requestvalidator_id}\n  method: patch\n  operationId: UpdateRequestValidator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapis/{restapi_id}/resources/{resource_id}\n  method: delete\n  operationId: DeleteResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapis/{restapi_id}/resources/{resource_id}\n  method:\
  \ get\n  operationId: GetResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restapis/{restapi_id}/resources/{resource_id}\n  method: patch\n  operationId: UpdateResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapis/{restapi_id}\n  method: delete\n  operationId: DeleteRestApi\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapis/{restapi_id}\n  method: get\n  operationId: GetRestApi\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restapis/{restapi_id}\n  method: put\n  operationId: PutRestApi\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapis/{restapi_id}\n  method: patch\n  operationId: UpdateRestApi\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapis/{restapi_id}/stages/{stage_name}\n  method: delete\n  operationId: DeleteStage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /restapis/{restapi_id}/stages/{stage_name}\n  method: get\n  operationId: GetStage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /restapis/{restapi_id}/stages/{stage_name}\n  method: patch\n  operationId: UpdateStage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /usageplans/{usageplanId}\n  method: delete\n  operationId: DeleteUsagePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n \
  \   audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /usageplans/{usageplanId}\n  method: get\n  operationId: GetUsagePlan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /usageplans/{usageplanId}\n  method: patch\n  operationId: UpdateUsagePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /usageplans/{usageplanId}/keys/{keyId}\n  method: delete\n  operationId: DeleteUsagePlanKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n   \
  \   max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /usageplans/{usageplanId}/keys/{keyId}\n  method: get\n  operationId: GetUsagePlanKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vpclinks/{vpclink_id}\n  method: delete\n  operationId: DeleteVpcLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /vpclinks/{vpclink_id}\n  method: get\n  oper\n\n# --- truncated at 32 KB (861 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/apis-io-engineering-platform/refs/heads/main/agentic-access/engineering-platform-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apis-io-engineering-platform/refs/heads/main/agentic-access/engineering-platform-agentic-access.yml
summary_line: 2757 operations · 1382 acting · 36 human-in-the-loop
tags:
- APIs.io
- Engineering
- Platform
---
