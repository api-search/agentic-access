---
acting_count: 17
action_class_counts:
  acting: 17
  connected: 22
api_specs:
- filename: datacrunch-openapi.yml
  format: yaml
  label: DataCrunch Instances API
  slug: instances
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacrunch/refs/heads/main/openapi/datacrunch-openapi.yml
- filename: datacrunch-openapi.yml
  format: yaml
  label: DataCrunch Instance Types & Availability API
  slug: instance-types
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacrunch/refs/heads/main/openapi/datacrunch-openapi.yml
- filename: datacrunch-openapi.yml
  format: yaml
  label: DataCrunch Images & Startup Scripts API
  slug: images
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacrunch/refs/heads/main/openapi/datacrunch-openapi.yml
- filename: datacrunch-openapi.yml
  format: yaml
  label: DataCrunch SSH Keys API
  slug: ssh-keys
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacrunch/refs/heads/main/openapi/datacrunch-openapi.yml
- filename: datacrunch-openapi.yml
  format: yaml
  label: DataCrunch Volumes API
  slug: volumes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacrunch/refs/heads/main/openapi/datacrunch-openapi.yml
- filename: datacrunch-openapi.yml
  format: yaml
  label: DataCrunch Serverless Inference & Containers API
  slug: serverless-inference
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacrunch/refs/heads/main/openapi/datacrunch-openapi.yml
- filename: datacrunch-openapi.yml
  format: yaml
  label: DataCrunch Balance API
  slug: balance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacrunch/refs/heads/main/openapi/datacrunch-openapi.yml
consequence_counts:
  physical: 8
  read: 22
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Datacrunch Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /container-deployments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /container-deployments/{deployment_name}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /container-deployments/{deployment_name}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /container-deployments/{deployment_name}/pause
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /container-deployments/{deployment_name}/purge-queue
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /container-deployments/{deployment_name}/resume
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /container-deployments/{deployment_name}/scaling
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /instances
operation_count: 39
overview: 'DataCrunch exposes 39 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read, 9 write, and 8 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: DataCrunch
provider_slug: datacrunch
slug: datacrunch-agentic-access
source_filename: datacrunch-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/datacrunch-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 39\n  by_action_class:\n    acting: 17\n    connected: 22\n  by_consequence:\n    write: 9\n    read: 22\n    physical: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /oauth2/token\n  method: post\n  operationId: createToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /balance\n  method: get\n  operationId: getBalance\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instances\n  method: get\n  operationId: listInstances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instances\n  method: post\n  operationId: deployInstance\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /instances\n  method: put\n  operationId: instanceAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /instances/{instance_id}\n  method: get\n  operationId: getInstance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instance-types\n  method: get\n  operationId: listInstanceTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instance-availability\n  method: get\n  operationId: listInstanceAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /instance-availability/{instance_type}\n  method: get\n  operationId: getInstanceTypeAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /images\n  method: get\n\
  \  operationId: listImages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /images/cluster\n  method: get\n  operationId: listClusterImages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scripts\n  method: get\n  operationId: listStartupScripts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scripts\n  method: post\n  operationId: createStartupScript\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scripts\n  method: delete\n  operationId:\
  \ deleteStartupScripts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scripts/{script_id}\n  method: get\n  operationId: getStartupScript\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sshkeys\n  method: get\n  operationId: listSSHKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sshkeys\n  method: post\n  operationId: addSSHKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /sshkeys\n  method: delete\n  operationId: deleteSSHKeys\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sshkeys/{sshkey_id}\n  method: get\n  operationId: getSSHKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /volumes\n  method: get\n  operationId: listVolumes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /volumes\n  method: post\n  operationId: createVolume\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /volumes\n  method: put\n  operationId: volumeAction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /volumes/{volume_id}\n  method: get\n  operationId: getVolume\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /volumes/{volume_id}\n  method: delete\n  operationId: deleteVolume\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n \
  \     triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /volumes/trash\n  method: get\n  operationId: listTrashedVolumes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /volume-types\n  method: get\n  operationId: listVolumeTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locations\n  method: get\n  operationId: listLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /container-deployments\n  method: get\n  operationId: listContainerDeployments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /container-deployments\n  method: post\n\
  \  operationId: createContainerDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /container-deployments/{deployment_name}\n  method: get\n  operationId: getContainerDeployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /container-deployments/{deployment_name}\n  method: patch\n  operationId: updateContainerDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /container-deployments/{deployment_name}\n  method: delete\n  operationId: deleteContainerDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /container-deployments/{deployment_name}/status\n  method: get\n  operationId: getContainerDeploymentStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /container-deployments/{deployment_name}/scaling\n  method: get\n  operationId: getContainerDeploymentScaling\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /container-deployments/{deployment_name}/scaling\n  method: patch\n  operationId: updateContainerDeploymentScaling\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /container-deployments/{deployment_name}/pause\n  method: post\n  operationId: pauseContainerDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /container-deployments/{deployment_name}/resume\n  method: post\n\
  \  operationId: resumeContainerDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /container-deployments/{deployment_name}/purge-queue\n  method: post\n  operationId: purgeContainerDeploymentQueue\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /container-types\n  method: get\n  operationId: listContainerTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datacrunch/refs/heads/main/agentic-access/datacrunch-agentic-access.yml
summary_line: 39 operations · 17 acting
tags:
- GPU Cloud
- Infrastructure
- Compute
- Inference
- Serverless
- Europe
---
