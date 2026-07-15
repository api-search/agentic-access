---
acting_count: 173
action_class_counts:
  acting: 173
  connected: 206
api_specs:
- filename: gremlin-openapi.yml
  format: yaml
  label: Gremlin API
  slug: gremlin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gremlin/refs/heads/main/openapi/gremlin-openapi.yml
consequence_counts:
  read: 206
  safety-critical: 32
  write: 141
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 32
kind: agentic-access
layout: agentic-access
method: generated
name: Gremlin Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /apikeys/{identifier}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /apikeys/{identifier}/activate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /attacks
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /attacks/halt
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /attacks/{guid}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /attacks/{guid}/halt
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /clients/{identifier}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /companies/{identifier}/invites/{email}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /companies/{identifier}/users/{email}/active
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /companies/{identifier}/users/{email}/active
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /companies/{identifier}/users/{email}/api-key/{api-key-id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /disaster-recovery-tests/{identifier}/halt-all
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /external-integrations
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /failure-flags/experiments/{id}/halt
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /halts
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /integration-clients/{identifier}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /kubernetes/attacks/halt
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /kubernetes/attacks/{uid}/halt
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /orgs/auth/secret/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /scenarios/halt
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /scenarios/halt/{guid}/runs/{runNumber}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /schedules/scenarios/{guid}/enabled
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /services/{serviceId}/dependencies/discovered
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /sharedAssets/requests/delete
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /sharedAssets/requests/deny
operation_count: 379
overview: 'Gremlin exposes 379 API operations that an AI agent could call, of which 173 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 206 read, 141 write, and 32 safety-critical.


  32 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Gremlin
provider_slug: gremlin
slug: gremlin-agentic-access
source_filename: gremlin-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/gremlin-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 379\n  by_action_class:\n    connected: 206\n    acting: 173\n  by_consequence:\n    read: 206\n    write: 141\n    safety-critical: 32\n  human_in_the_loop_required: 32\noperations:\n- path: /attacks/active\n  method: get\n  operationId: active\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - EXPERIMENTS_READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attacks/active/paged\n  method: get\n  operationId: activePaged\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - EXPERIMENTS_READ\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /attacks/{guid}/annotations\n  method: put\n  operationId: addAnnotations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - MINIMUM_TEAM_PRIVILEGES\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /attacks\n  method: get\n  operationId: all\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - EXPERIMENTS_READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attacks\n  method: post\n  operationId: createNewAttack\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - EXPERIMENTS_RUN\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /attacks\n  method: delete\n  operationId: halt\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /attacks/range\n  method: get\n  operationId: allAttacksInRange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - EXPERIMENTS_READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attacks/completed\n  method: get\n  operationId: completed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - EXPERIMENTS_READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attacks/completed/paged\n  method: get\n  operationId:\
  \ completedPaged\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - EXPERIMENTS_READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attacks/new\n  method: post\n  operationId: create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - EXPERIMENTS_RUN\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /attacks/{guid}\n  method: get\n  operationId: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - EXPERIMENTS_READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attacks/{guid}\n  method: delete\n  operationId: halt_1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n  \
  \  - HALT_WRITE\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /attacks/halt\n  method: post\n  operationId: haltAsPost\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /attacks/{guid}/halt\n  method: post\n  operationId: haltAsPost_1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - HALT_WRITE\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n\
  \    audit: required\n- path: /executions\n  method: get\n  operationId: forAttack\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - EXPERIMENTS_READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /halts\n  method: post\n  operationId: haltAll\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /kubernetes/attacks/{guid}\n  method: get\n  operationId: attack\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - EXPERIMENTS_READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /kubernetes/attacks\n  method: get\n  operationId: attacks\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    scope:\n    - EXPERIMENTS_READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /kubernetes/attacks/new\n  method: post\n  operationId: createAttack\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - EXPERIMENTS_WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /kubernetes/attacks/{uid}/halt\n  method: post\n  operationId: halt_2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - HALT_WRITE\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /kubernetes/attacks/halt\n  method: post\n \
  \ operationId: haltAll_1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /metadata\n  method: get\n  operationId: metadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - MINIMUM_TEAM_PRIVILEGES\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/auth/mfa/auth\n  method: post\n  operationId: auth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/auth/mfa/disable\n  method: post\n  operationId: disable\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /users/auth/mfa/enable\n  method: post\n  operationId: enable\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/auth/mfa/forceDisable\n  method: post\n  operationId: forceDisable\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - COMPANY_USERS_WRITE\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /users/auth/mfa/info\n  method: get\n  operationId: getInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - MINIMUM_COMPANY_PRIVILEGES\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/auth/mfa/{email}/enabled\n  method: get\n  operationId: isEnabled\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - SECURITY_REPORTS_READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/auth/mfa/validate\n  method: post\n  operationId: validate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integrations/{type}\n  method:\
  \ get\n  operationId: get_2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - COMPANY_INTEGRATIONS_READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrations/{type}\n  method: put\n  operationId: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - COMPANY_INTEGRATIONS_WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integrations/{type}\n  method: delete\n  operationId: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - COMPANY_INTEGRATIONS_WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /integrations\n  method: get\n  operationId: list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - COMPANY_INTEGRATIONS_READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/callback\n  method: get\n  operationId: oAuthCallback\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/login\n  method: get\n  operationId: oAuthLogin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /roles\n  method: get\n  operationId: getRolesAndPrivileges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /roles\n  method: post\n  operationId: createCustomRole\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    scope:\n    - ROLES_WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /roles/{roleId}\n  method: get\n  operationId: getRole\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /roles/{roleId}\n  method: delete\n  operationId: deleteCustomRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ROLES_WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /roles/{roleId}\n  method: patch\n  operationId: updateCustomRole\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    scope:\n    - ROLES_WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/auth\n  method: post\n  operationId: auth_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/auth\n  method: delete\n  operationId: invalidate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - MINIMUM_COMPANY_PRIVILEGES\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/auth/emailCompanies\n\
  \  method: get\n  operationId: companyAffiliationsEmail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/auth/password/reset\n  method: post\n  operationId: passwordReset\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /users/auth/password\n  method: put\n  operationId: passwordReset_1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - MINIMUM_COMPANY_PRIVILEGES\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /users/auth/password\n  method: post\n  operationId: passwordUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/auth/saml/failures\n  method: get\n  operationId: samlFailures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - COMPANY_SECURITY_READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/auth/saml/metadata\n  method: get\n  operationId: samlMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /aws/metadata/autoscaling-groups\n  method: get\n  operationId: getAutoscalingGroupsForAccount\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - MINIMUM_TEAM_PRIVILEGES\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /aws/metadata/iam-role\n  method: get\n  operationId: getAwsMetadataIamRole\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - MINIMUM_TEAM_PRIVILEGES\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /aws/metadata/load-balancers\n  method: get\n  operationId: getLoadBalancersForAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - MINIMUM_TEAM_PRIVILEGES\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datadog/monitors/{monitorId}\n  method: get\n  operationId: getMonitor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - MINIMUM_TEAM_PRIVILEGES\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /datadog/monitors\n  method: get\n  operationId: searchMonitors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - MINIMUM_TEAM_PRIVILEGES\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /grafana/alerts\n  method: get\n  operationId: alerts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - MINIMUM_TEAM_PRIVILEGES\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /grafana/dashboards\n  method: get\n  operationId: dashboards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - MINIMUM_TEAM_PRIVILEGES\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /grafana/rules\n  method: get\n  operationId: rules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - MINIMUM_TEAM_PRIVILEGES\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /grafana/monitors\n  method: get\n  operationId: searchMonitors_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - MINIMUM_TEAM_PRIVILEGES\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jira/issues\n  method: get\n  operationId: issuesForGremlinEntityIds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - INTEGRATIONS_READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jira/issues\n  method: post\n  operationId: issue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - INTEGRATIONS_WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jira/issues/count\n  method: get\n  operationId: issueCount\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - MINIMUM_TEAM_PRIVILEGES\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jira/issue-meta\n  method: get\n  operationId: issueMeta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - MINIMUM_TEAM_PRIVILEGES\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jira/issues/services\n  method: get\n  operationId: issuesForGremlinEntityIdOfType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - INTEGRATIONS_READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jira/labels\n  method: get\n  operationId: labels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - MINIMUM_TEAM_PRIVILEGES\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jira/priorities\n  method: get\n  operationId:\
  \ priorities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - MINIMUM_TEAM_PRIVILEGES\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jira/projects/{projectIdOrKey}\n  method: get\n  operationId: projectById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - MINIMUM_TEAM_PRIVILEGES\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jira/projects\n  method: get\n  operationId: projectSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - MINIMUM_TEAM_PRIVILEGES\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jira/projects/{projectIdOrKey}/users\n  method: get\n  operationId: projectUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - MINIMUM_TEAM_PRIVILEGES\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /newrelic/incidents/{incidentId}\n  method: get\n  operationId: incident\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - INTEGRATIONS_WRITE\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pagerduty/incidents\n  method: get\n  operationId: incidentsForService\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - MINIMUM_TEAM_PRIVILEGES\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pagerduty/services\n  method: get\n  operationId: services\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - MINIMUM_TEAM_PRIVILEGES\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external-integrations\n  method: get\n  operationId: get_4\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - INTEGRATIONS_READ\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /external-integrations\n  method: delete\n  operationId: revoke\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - INTEGRATIONS_WRITE\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /external-integrations/load-generator\n  method: get\n  operationId: getLoadGeneratorIntegrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - INTEGRATIONS_READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external-integrations/load-generator\n  method: put\n  operationId: updateLoadGeneratorIntegration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - INTEGRATIONS_WRITE\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /external-integrations/load-generator\n  method: post\n  operationId: createLoadGeneratorIntegration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - INTEGRATIONS_WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /external-integrations/load-generator\n  method: delete\n  operationId: removeLoadGeneratorIntegration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - INTEGRATIONS_WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    \
  \  - high-value\n    audit: required\n- path: /external-integrations/status-check\n  method: get\n  operationId: getStatusCheckIntegrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - INTEGRATIONS_READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /external-integrations/status-check\n  method: put\n  operationId: updateStatusCheckIntegration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - INTEGRATIONS_WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /external-integrations/status-check\n  method: post\n  operationId: createStatusCheckIntegration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - INTEGRATIONS_WRITE\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /external-integrations/status-check\n  method: delete\n  operationId: removeStatusCheckIntegration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - INTEGRATIONS_WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /failure-flags/apps/{name}\n  method: get\n  operationId: getApplicationForNameAndTeam\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - EXPERIMENTS_READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /failure-flags/apps\n  method: get\n  operationId: getApplicationsForTeam\n  x-agentic-access:\n    action-class: connected\n \
  \   consequence: read\n    subject: optional\n    scope:\n    - EXPERIMENTS_READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /failure-flags/apps/{name}/protect\n  method: post\n  operationId: protectApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - EXPERIMENTS_WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /failure-flags/apps/{name}/unprotect\n  method: post\n  operationId: unprotectApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - EXPERIMENTS_WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /failure-flags/experiments/{id}/runs\n\
  \  method: get\n  operationId: allRunsForExperiment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - EXPERIMENTS_READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /failure-flags/experiments\n  method: get\n  operationId: getExperimentsForTeam\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - EXPERIMENTS_READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /failure-flags/experiments\n  method: post\n  operationId: createExperiment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - EXPERIMENTS_WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /failure-flags/experiments/{id}\n  method: get\n  operationId: getExperimentForTeamAndId\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - EXPERIMENTS_READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /failure-flags/experiments/{id}\n  method: delete\n  operationId: deleteExperiment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - EXPERIMENTS_WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /failure-flags/experiments/active\n  method: get\n  operationId: getActiveExperimentsForTeam\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - EXPERIMENTS_READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /failure-flags/experiments/completed/paged\n  method: get\n  operationId: getCompletedExperimentsForTeam\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - EXPERIMENTS_READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /failure-flags/experiments/{id}/run/{startTime}\n  method: get\n  operationId: getExperimentRunDetailsForIdAndStartTime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - EXPERIMENTS_READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /failure-flags/experiments/{id}/halt\n  method: post\n  operationId: haltExperiment\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - HALT_WRITE\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /failure-flags/experiments/{id}/protect\n  method: post\n  operationId: protectExperiment\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - EXPERIMENTS_WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /failure-flags/experiments/{id}/run\n  method: post\n  operationId: runExperiment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - EXPERIMENTS_RUN\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /failure-flags/experiments/{id}/unprotect\n  method: post\n  operationId: unprotectExperiment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - EXPERIMENTS_WRITE\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /failure-flags/flags/{name}\n  method: get\n  operationId: getFailureFlagForTeamAndName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - EXPERIMENTS_READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /failure-flags/flags\n  method: get\n  operationId: getFailureFlagsForTeam\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - EXPERIMENTS_READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /failure-flags/flags/{name}/protect\n  method: post\n  operationId: protectFailureFlag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - EXPERIMENTS_WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /failure-flags/flags/{name}/unprotect\n  method: post\n  operationId: unprotectFailureFlag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - EXPERIMENTS_WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gamedays\n  method: get\n  operationId: getGameDaysForTeam\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - MINIMUM_TEAM_PRIVILEGES\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gamedays\n  method: post\n  operationId: createGameDayPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - MINIMUM_TEAM_PRIVILEGES\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gamedays/{gameDayId}/summary/images/{imageName}\n  method: delete\n  operationId: delete_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - MINIMUM_TEAM_PRIVILEGES\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gamedays/{gameDayId}/summary/images/{imageName}\n  method: patch\n  operationId: put_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - MINIMUM_TEAM_PRIVILEGES\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gamedays/{gameDayId}/summary/export\n\
  \  method: get\n  operationId: export\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - MINIMUM_T\n\n# --- truncated at 32 KB (117 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/gremlin/refs/heads/main/agentic-access/gremlin-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gremlin/refs/heads/main/agentic-access/gremlin-agentic-access.yml
summary_line: 379 operations · 173 acting · 32 human-in-the-loop
tags:
- Chaos Engineering
- Fault Injection
- Infrastructure Testing
- Reliability
- Site Reliability Engineering
---
