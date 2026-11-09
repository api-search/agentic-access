---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 11
api_specs:
- filename: abyssale-com-auth-api-openapi.yml
  format: yaml
  label: Abyssale Auth API
  slug: abyssale-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abyssale-com/openapi/abyssale-com-auth-api-openapi.yml
- filename: abyssale-com-credits-api-openapi.yml
  format: yaml
  label: Abyssale Credits API
  slug: abyssale-com-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abyssale-com/openapi/abyssale-com-credits-api-openapi.yml
- filename: abyssale-com-design-duplication-requests-api-openapi.yml
  format: yaml
  label: Abyssale Design Duplication Requests API
  slug: abyssale-com-design-duplication-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abyssale-com/openapi/abyssale-com-design-duplication-requests-api-openapi.yml
- filename: abyssale-com-designs-api-openapi.yml
  format: yaml
  label: Abyssale Designs API
  slug: abyssale-com-designs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abyssale-com/openapi/abyssale-com-designs-api-openapi.yml
- filename: abyssale-com-examples-api-openapi.yml
  format: yaml
  label: Abyssale Examples API
  slug: abyssale-com-examples-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abyssale-com/openapi/abyssale-com-examples-api-openapi.yml
- filename: abyssale-com-export-abyssale-api-openapi.yml
  format: yaml
  label: Abyssale Export Abyssale API
  slug: abyssale-com-export-abyssale-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abyssale-com/openapi/abyssale-com-export-abyssale-api-openapi.yml
- filename: abyssale-com-fonts-api-openapi.yml
  format: yaml
  label: Abyssale Fonts API
  slug: abyssale-com-fonts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abyssale-com/openapi/abyssale-com-fonts-api-openapi.yml
- filename: abyssale-com-images-api-openapi.yml
  format: yaml
  label: Abyssale Images API
  slug: abyssale-com-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abyssale-com/openapi/abyssale-com-images-api-openapi.yml
- filename: abyssale-com-projects-api-openapi.yml
  format: yaml
  label: Abyssale Projects API
  slug: abyssale-com-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abyssale-com/openapi/abyssale-com-projects-api-openapi.yml
- filename: abyssale-com-workspace-template-categories-api-openapi.yml
  format: yaml
  label: Abyssale Workspace Template Categories API
  slug: abyssale-com-workspace-template-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abyssale-com/openapi/abyssale-com-workspace-template-categories-api-openapi.yml
- filename: abyssale-com-workspace-templates-api-openapi.yml
  format: yaml
  label: Abyssale Workspace Templates API
  slug: abyssale-com-workspace-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abyssale-com/openapi/abyssale-com-workspace-templates-api-openapi.yml
consequence_counts:
  read: 11
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Abyssale Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 23
overview: 'Abyssale exposes 23 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 12 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Abyssale
provider_slug: abyssale-com
slug: abyssale-com-agentic-access
source_filename: abyssale-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/abyssale-com-openapi-generated.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    acting: 12\n    connected: 11\n  by_consequence:\n    write: 12\n    read: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /auth\n  method: post\n  operationId: post_auth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /credits\n  method: get\n  operationId: get_credits\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /design-duplication-requests/{duplicaterequestid}\n  method: get\n  operationId: get_design_duplication_requests_duplicaterequestid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /designs\n  method: get\n  operationId: get_designs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /designs\n  method: post\n  operationId: post_designs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /designs/64238d01-d402-474b-8c2d-fbc957e9d290\n  method: delete\n  operationId:\
  \ delete_designs_64238d01_d402_474b_8c2d_fbc957e9d290\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /designs/64238d01-d402-474b-8c2d-fbc957e9d290/name\n  method: put\n  operationId: put_designs_64238d01_d402_474b_8c2d_fbc957e9d290_name\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /designs/64238d01-d402-474b-8c2d-fbc957e9d290/project\n  method: put\n  operationId: put_designs_64238d01_d402_474b_8c2d_fbc957e9d290_project\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /designs/import/json\n  method: post\n  operationId: post_designs_import_json\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /designs/import/json/64238d01-d402-474b-8c2d-fbc957e9d290\n  method: get\n  operationId: get_designs_import_json_64238d01_d402_474b_8c2d_fbc957e9d290\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /designs/import/json/9c1f0f4e-…\n  method: post\n  operationId: post_designs_import_json_9c1f0f4e\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /designs/{designid}\n  method: get\n  operationId: get_designs_designid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /designs/{designid}/dynamic-image-url\n  method: post\n  operationId: post_designs_designid_dynamic_image_url\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /designs/{designid}/formats/facebook-post\n  method: get\n  operationId: get_designs_designid_formats_facebook_post\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /examples/welcome-email-banner.json\n  method: get\n  operationId: get_examples_welcome_email_banner_json\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /export-abyssale\n  method: post\n  operationId: post_export_abyssale\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fonts\n  method: get\n  operationId: get_fonts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /images\n  method: post\n  operationId: post_images\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects\n  method: get\n  operationId: get_projects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects\n  method: post\n  operationId: post_projects\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspace-template-categories\n  method: get\n  operationId: get_workspace_template_categories\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspace-templates\n  method: get\n  operationId: get_workspace_templates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspace-templates/{companytemplateid}/use\n  method: post\n  operationId: post_workspace_templates_companytemplateid_use\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/abyssale-com/agentic-access/abyssale-com-agentic-access.yml
summary_line: 23 operations · 12 acting
tags:
- Creative Automation
- Marketing
- Agencies
- Visual-Production
- Software-as-a-Service
---
