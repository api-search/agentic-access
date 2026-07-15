---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 9
api_specs:
- filename: cisco-nexus-nxapi-rest.yml
  format: yaml
  label: Cisco NX-API REST
  slug: cisco-nx-api-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-nexus/refs/heads/main/openapi/cisco-nexus-nxapi-rest.yml
consequence_counts:
  read: 9
  safety-critical: 2
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Cisco Nexus Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /aaaLogout.json
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /mo/sys/fm.json
operation_count: 18
overview: 'Cisco Nexus Dashboard exposes 18 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 7 write, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cisco Nexus Dashboard
provider_slug: cisco-nexus
slug: cisco-nexus-agentic-access
source_filename: cisco-nexus-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/cisco-nexus-nxapi-rest.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    acting: 9\n    connected: 9\n  by_consequence:\n    write: 7\n    safety-critical: 2\n    read: 9\n  human_in_the_loop_required: 2\noperations:\n- path: /aaaLogin.json\n  method: post\n  operationId: authenticateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /aaaLogout.json\n  method: post\n  operationId: logoutUser\n  x-agentic-access:\n   \
  \ action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /mo/sys/intf/phys-[{interfaceId}].json\n  method: get\n  operationId: getPhysicalInterface\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mo/sys/intf.json\n  method: post\n  operationId: configurePhysicalInterface\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /class/l1PhysIf.json\n  method: get\n  operationId: listPhysicalInterfaces\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mo/sys/bd.json\n  method: post\n  operationId: createVlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mo/sys/bd/bd-[{vlanEncap}].json\n  method: get\n  operationId: getVlan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mo/sys/bd/bd-[{vlanEncap}].json\n  method: delete\n  operationId: deleteVlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /class/l2BD.json\n  method: get\n  operationId: listVlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mo/sys/intf/svi-[{sviId}].json\n  method: get\n  operationId: getSviInterface\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mo/sys/intf/svi-[{sviId}].json\n  method: post\n  operationId: configureSviInterface\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mo/sys/ipv4/inst.json\n  method: post\n  operationId: configureStaticRoute\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mo/sys/ipv4/inst/dom-{vrfName}/rt-[{prefix}].json\n  method: get\n  operationId: getStaticRoute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /class/ipv4Route.json\n  method: get\n  operationId: listStaticRoutes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mo/sys/bgp.json\n  method: get\n  operationId: getBgpConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mo/sys.json\n  method: get\n  operationId: getSystemInfo\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mo/sys.json\n  method: post\n  operationId: configureSystem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mo/sys/fm.json\n  method: post\n  operationId: configureFeatures\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-nexus/refs/heads/main/agentic-access/cisco-nexus-agentic-access.yml
summary_line: 18 operations · 9 acting · 2 human-in-the-loop
tags:
- Data Center
- Infrastructure
- Network Automation
- Networking
- SDN
- Switches
---
