---
acting_count: 75
action_class_counts:
  acting: 75
  connected: 70
api_specs:
- filename: university-of-vienna-directory-api-openapi.yml
  format: yaml
  label: PHAIDRA directory API (University of Vienna)
  slug: university-of-vienna-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-vienna/refs/heads/main/openapi/university-of-vienna-directory-api-openapi.yml
- filename: university-of-vienna-imageserver-api-openapi.yml
  format: yaml
  label: PHAIDRA imageserver API (University of Vienna)
  slug: university-of-vienna-imageserver-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-vienna/refs/heads/main/openapi/university-of-vienna-imageserver-api-openapi.yml
- filename: university-of-vienna-lists-api-openapi.yml
  format: yaml
  label: PHAIDRA lists API (University of Vienna)
  slug: university-of-vienna-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-vienna/refs/heads/main/openapi/university-of-vienna-lists-api-openapi.yml
- filename: university-of-vienna-misc-api-openapi.yml
  format: yaml
  label: PHAIDRA misc API (University of Vienna)
  slug: university-of-vienna-misc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-vienna/refs/heads/main/openapi/university-of-vienna-misc-api-openapi.yml
- filename: university-of-vienna-oai-pmh-api-openapi.yml
  format: yaml
  label: PHAIDRA oai-pmh API (University of Vienna)
  slug: university-of-vienna-oai-pmh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-vienna/refs/heads/main/openapi/university-of-vienna-oai-pmh-api-openapi.yml
- filename: university-of-vienna-object-advanced-api-openapi.yml
  format: yaml
  label: PHAIDRA object-advanced API (University of Vienna)
  slug: university-of-vienna-object-advanced-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-vienna/refs/heads/main/openapi/university-of-vienna-object-advanced-api-openapi.yml
- filename: university-of-vienna-object-basics-api-openapi.yml
  format: yaml
  label: PHAIDRA object-basics API (University of Vienna)
  slug: university-of-vienna-object-basics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-vienna/refs/heads/main/openapi/university-of-vienna-object-basics-api-openapi.yml
- filename: university-of-vienna-relationships-api-openapi.yml
  format: yaml
  label: PHAIDRA relationships API (University of Vienna)
  slug: university-of-vienna-relationships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-vienna/refs/heads/main/openapi/university-of-vienna-relationships-api-openapi.yml
- filename: university-of-vienna-search-api-openapi.yml
  format: yaml
  label: PHAIDRA search API (University of Vienna)
  slug: university-of-vienna-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-vienna/refs/heads/main/openapi/university-of-vienna-search-api-openapi.yml
- filename: university-of-vienna-session-api-openapi.yml
  format: yaml
  label: PHAIDRA session API (University of Vienna)
  slug: university-of-vienna-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-vienna/refs/heads/main/openapi/university-of-vienna-session-api-openapi.yml
- filename: university-of-vienna-stats-api-openapi.yml
  format: yaml
  label: PHAIDRA stats API (University of Vienna)
  slug: university-of-vienna-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-vienna/refs/heads/main/openapi/university-of-vienna-stats-api-openapi.yml
- filename: university-of-vienna-templates-api-openapi.yml
  format: yaml
  label: PHAIDRA templates API (University of Vienna)
  slug: university-of-vienna-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-vienna/refs/heads/main/openapi/university-of-vienna-templates-api-openapi.yml
- filename: university-of-vienna-vocabularies-api-openapi.yml
  format: yaml
  label: PHAIDRA vocabularies API (University of Vienna)
  slug: university-of-vienna-vocabularies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-vienna/refs/heads/main/openapi/university-of-vienna-vocabularies-api-openapi.yml
- filename: university-of-vienna-data-stream-api-openapi.yml
  format: yaml
  label: University of Vienna Data Stream API
  slug: university-of-vienna-data-stream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-vienna/refs/heads/main/openapi/university-of-vienna-data-stream-api-openapi.yml
consequence_counts:
  physical: 10
  read: 70
  write: 65
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: University Of Vienna Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /collection/{pid}/members/add
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /collection/{pid}/members/order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /collection/{pid}/members/remove
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /collection/{pid}/members/{itempid}/order/{position}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /container/{pid}/members/order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /container/{pid}/members/{itempid}/order/{position}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /members/order/json2xml
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /members/order/xml2json
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /object/{pid}/relationship/add
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /object/{pid}/relationship/remove
operation_count: 145
overview: 'University of Vienna exposes 145 API operations that an AI agent could call, of which 75 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 70 read, 65 write, and 10 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: University of Vienna
provider_slug: university-of-vienna
slug: university-of-vienna-agentic-access
source_filename: university-of-vienna-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/university-of-vienna-data-stream-api-openapi.yml, openapi/university-of-vienna-directory-api-openapi.yml,\n  openapi/university-of-vienna-imageserver-api-openapi.yml, openapi/university-of-vienna-lists-api-openapi.yml,\n  openapi/university-of-vienna-misc-api-openapi.yml, openapi/university-of-vienna-oai-pmh-api-openapi.yml,\n  openapi/university-of-vienna-object-advanced-api-openapi.yml, openapi/university-of-vienna-object-basics-api-openapi.yml,\n  openapi/university-of-vienna-relationships-api-openapi.yml, openapi/university-of-vienna-search-api-openapi.yml,\n  openapi/university-of-vienna-session-api-openapi.yml, openapi/university-of-vienna-stats-api-openapi.yml,\n  openapi/university-of-vienna-templates-api-openapi.yml, openapi/university-of-vienna-vocabularies-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point\
  \ for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 145\n  by_action_class:\n    connected: 70\n    acting: 75\n  by_consequence:\n    read: 70\n    write: 65\n    physical: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /uwmetadata/tree\n  method: get\n  operationId: getUwmetadataTree\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /uwmetadata/json2xml\n  method: post\n  operationId: postUwmetadataJson2xml\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uwmetadata/xml2json\n  method: post\n  operationId: postUwmetadataXml2json\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uwmetadata/validate\n  method: post\n  operationId: postUwmetadataValidate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uwmetadata/json2xml_validate\n  method: post\n  operationId: postUwmetadataJson2xmlValidate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /mods/tree\n  method: get\n  operationId: getModsTree\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mods/json2xml\n  method: post\n  operationId: postModsJson2xml\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mods/xml2json\n  method: post\n  operationId: postModsXml2json\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mods/validate\n  method: post\n  operationId: postModsValidate\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mods/json2xml_validate\n  method: post\n  operationId: postModsJson2xmlValidate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rights/json2xml\n  method: post\n  operationId: postRightsJson2xml\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rights/xml2json\n\
  \  method: post\n  operationId: postRightsXml2json\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rights/validate\n  method: post\n  operationId: postRightsValidate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rights/json2xml_validate\n  method: post\n  operationId: postRightsJson2xmlValidate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n    \
  \  - abnormal\n      - high-value\n    audit: required\n- path: /geo/json2xml\n  method: post\n  operationId: postGeoJson2xml\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /geo/xml2json\n  method: post\n  operationId: postGeoXml2json\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /geo/validate\n  method: post\n  operationId: postGeoValidate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /geo/json2xml_validate\n  method: post\n  operationId: postGeoJson2xmlValidate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /members/order/json2xml\n  method: post\n  operationId: postMembersOrderJson2xml\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /members/order/xml2json\n  method: post\n  operationId: postMembersOrderXml2json\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /annotations/json2xml\n  method: post\n  operationId: postAnnotationsJson2xml\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /annotations/xml2json\n  method: post\n  operationId: postAnnotationsXml2json\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /annotations/validate\n  method: post\n  operationId: postAnnotationsValidate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /annotations/json2xml_validate\n  method: post\n  operationId: postAnnotationsJson2xmlValidate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /directory/org_get_subunits\n  method: get\n  operationId: getDirectoryOrgGetSubunits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /directory/org_get_superunits\n  method: get\n  operationId: getDirectoryOrgGetSuperunits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /directory/org_get_parentpath\n  method: get\n  operationId: getDirectoryOrgGetParentpath\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /directory/org_get_units\n  method: get\n  operationId: getDirectoryOrgGetUnits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /directory/user/{username}/data\n  method: get\n  operationId: getDirectoryUserByUsernameData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /directory/user/{username}/name\n\
  \  method: get\n  operationId: getDirectoryUserByUsernameName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /directory/user/{username}/email\n  method: get\n  operationId: getDirectoryUserByUsernameEmail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /directory/user/search\n  method: get\n  operationId: getDirectoryUserSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /directory/user/data\n  method: get\n  operationId: getDirectoryUserData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups\n  method: get\n  operationId: getGroups\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /group/{gid}\n  method: get\n  operationId: getGroupByGid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /group/add\n  method: post\n  operationId: postGroupAdd\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /group/{gid}/remove\n  method: post\n  operationId: postGroupByGidRemove\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /group/{gid}/members/add\n  method: post\n  operationId: postGroupByGidMembersAdd\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /group/{gid}/members/remove\n  method: post\n  operationId: postGroupByGidMembersRemove\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /imageserver\n  method: get\n  operationId: getImageserver\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /imageserver/{pid}/status\n  method: get\n  operationId: getImageserverByPidStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /imageserver/process\n  method: post\n  operationId: postImageserverProcess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /imageserver/{pid}/process\n  method: post\n  operationId: postImageserverByPidProcess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /list/token/{token}\n\
  \  method: get\n  operationId: getListTokenByToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lists\n  method: get\n  operationId: getLists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /list/{lid}\n  method: get\n  operationId: getListByLid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /list/add\n  method: post\n  operationId: postListAdd\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /list/{lid}/token/create\n  method: post\n\
  \  operationId: postListByLidTokenCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /list/{lid}/token/delete\n  method: post\n  operationId: postListByLidTokenDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /list/{lid}/remove\n  method: post\n  operationId: postListByLidRemove\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /list/{lid}/members/add\n  method: post\n  operationId: postListByLidMembersAdd\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /list/{lid}/members/remove\n  method: post\n  operationId: postListByLidMembersRemove\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /state\n  method: get\n  operationId: getState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /utils/get_all_pids\n\
  \  method: get\n  operationId: getUtilsGetAllPids\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /termsofuse\n  method: get\n  operationId: getTermsofuse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /termsofuse/agree/{version}\n  method: post\n  operationId: postTermsofuseAgreeByVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings\n  method: post\n  operationId: postSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /settings\n  method: get\n  operationId: getSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /streaming/{pid}/key\n  method: get\n  operationId: getStreamingByPidKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /termsofuse/getagreed\n  method: get\n  operationId: getTermsofuseGetagreed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oai\n  method: get\n  operationId: getOai\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oai\n  method:\
  \ post\n  operationId: postOai\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /object/{pid}/uwmetadata\n  method: get\n  operationId: getObjectByPidUwmetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /object/{pid}/uwmetadata\n  method: post\n  operationId: postObjectByPidUwmetadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /object/{pid}/mods\n  method: get\n  operationId: getObjectByPidMods\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /object/{pid}/mods\n  method: post\n  operationId: postObjectByPidMods\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /object/{pid}/jsonld\n  method: get\n  operationId: getObjectByPidJsonld\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /object/{pid}/jsonld\n  method: post\n  operationId: postObjectByPidJsonld\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n   \
  \   triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /object/{pid}/json-ld\n  method: get\n  operationId: getObjectByPidJsonLd\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /object/{pid}/geo\n  method: get\n  operationId: getObjectByPidGeo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /object/{pid}/geo\n  method: post\n  operationId: postObjectByPidGeo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /object/{pid}/members/order\n  method: get\n  operationId: getObjectByPidMembersOrder\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /object/{pid}/annotations\n  method: get\n  operationId: getObjectByPidAnnotations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /object/{pid}/annotations\n  method: post\n  operationId: postObjectByPidAnnotations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /object/{pid}/index/dc\n  method: get\n  operationId: getObjectByPidIndexDc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /object/{pid}/index/relationships\n\
  \  method: get\n  operationId: getObjectByPidIndexRelationships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /object/{pid}/index/members\n  method: get\n  operationId: getObjectByPidIndexMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /object/{pid}/datacite\n  method: get\n  operationId: getObjectByPidDatacite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /object/{pid}/state\n  method: get\n  operationId: getObjectByPidState\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /object/{pid}/cmodel\n  method: get\n  operationId: getObjectByPidCmodel\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /object/{pid}/relationships\n  method: get\n  operationId: getObjectByPidRelationships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /object/{pid}/iiifmanifest\n  method: get\n  operationId: getObjectByPidIiifmanifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /object/{pid}/iiifmanifest\n  method: post\n  operationId: postObjectByPidIiifmanifest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /object/{pid}/id\n\
  \  method: get\n  operationId: getObjectByPidId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authz/check/{pid}/{op}\n  method: get\n  operationId: getAuthzCheckByPidByOp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /object/{pid}/metadata\n  method: get\n  operationId: getObjectByPidMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /object/{pid}/fulltext\n  method: get\n  operationId: getObjectByPidFulltext\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /object/{pid}/jsonldprivate\n  method: get\n  operationId: getObjectByPidJsonldprivate\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /object/{pid}/jsonldprivate\n  method: post\n  operationId: postObjectByPidJsonldprivate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: '/index '\n  method: post\n  operationId: 'postIndex '\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /object/{pid}/modify\n  method: post\n  operationId: postObjectByPidModify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n  \
  \  subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /object/{pid}/id/add\n  method: post\n  operationId: postObjectByPidIdAdd\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /object/{pid}/id/remove\n  method: post\n  operationId: postObjectByPidIdRemove\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /object/{pid}/datastream/{dsid}\n  method: post\n  operationId:\
  \ postObjectByPidDatastreamByDsid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /object/{pid}/data\n  method: post\n  operationId: postObjectByPidData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /resource/create\n  method: post\n  operationId: postResourceCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /page/create\n  method: post\n  operationId: postPageCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /object/create\n  method: post\n  operationId: postObjectCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /object/create/{cmodel}\n  method: post\n  operationId: postObjectCreateByCmodel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /picture/create\n  method: post\n  operationId: postPictureCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /audio/create\n  method: post\n  operationId: postAudioCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /video/create\n  method: post\n  operationId: postVideoCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/create\n  method: post\n  operationId: postDocumentCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /unknown/create\n  method: post\n  operationId: postUnknownCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collection/create\n  method: post\n  operationId: postCollectionCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /container/create\n  method: post\n  operationId: postContainerCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /object/{pid}/info\n  method: get\n  operationId: getObjectByPidInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /object/{pid}/thumbnail\n  method: get\n  operationId: getObjectByPidThumbnail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\n\n\
  # --- truncated at 32 KB (42 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/university-of-vienna/refs/heads/main/agentic-access/university-of-vienna-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-vienna/refs/heads/main/agentic-access/university-of-vienna-agentic-access.yml
summary_line: 145 operations · 75 acting
tags:
- Education
- Higher Education
- University
- Public Research University
- Austria
- Europe
- Research
- Research Data
- Repository
- Open Source
- Digital Preservation
- Identity Federation
- OAI-PMH
- Library
- Course Catalog
---
