---
acting_count: 0
action_class_counts:
  connected: 41
api_specs:
- filename: disease-sh-covid-19-apple-api-openapi.yml
  format: yaml
  label: 'disease.sh COVID-19: Apple API'
  slug: disease-sh-covid-19-apple-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/disease-sh/refs/heads/main/openapi/disease-sh-covid-19-apple-api-openapi.yml
- filename: disease-sh-covid-19-government-api-openapi.yml
  format: yaml
  label: 'disease.sh COVID-19: Government API'
  slug: disease-sh-covid-19-government-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/disease-sh/refs/heads/main/openapi/disease-sh-covid-19-government-api-openapi.yml
- filename: disease-sh-covid-19-jhucsse-api-openapi.yml
  format: yaml
  label: 'disease.sh COVID-19: JHUCSSE API'
  slug: disease-sh-covid-19-jhucsse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/disease-sh/refs/heads/main/openapi/disease-sh-covid-19-jhucsse-api-openapi.yml
- filename: disease-sh-covid-19-nyt-api-openapi.yml
  format: yaml
  label: 'disease.sh COVID-19: NYT API'
  slug: disease-sh-covid-19-nyt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/disease-sh/refs/heads/main/openapi/disease-sh-covid-19-nyt-api-openapi.yml
- filename: disease-sh-covid-19-therapeutics-api-openapi.yml
  format: yaml
  label: 'disease.sh COVID-19: Therapeutics API'
  slug: disease-sh-covid-19-therapeutics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/disease-sh/refs/heads/main/openapi/disease-sh-covid-19-therapeutics-api-openapi.yml
- filename: disease-sh-covid-19-vaccine-api-openapi.yml
  format: yaml
  label: 'disease.sh COVID-19: Vaccine API'
  slug: disease-sh-covid-19-vaccine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/disease-sh/refs/heads/main/openapi/disease-sh-covid-19-vaccine-api-openapi.yml
- filename: disease-sh-covid-19-variants-api-openapi.yml
  format: yaml
  label: 'disease.sh COVID-19: Variants API'
  slug: disease-sh-covid-19-variants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/disease-sh/refs/heads/main/openapi/disease-sh-covid-19-variants-api-openapi.yml
- filename: disease-sh-covid-19-worldometers-api-openapi.yml
  format: yaml
  label: 'disease.sh COVID-19: Worldometers API'
  slug: disease-sh-covid-19-worldometers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/disease-sh/refs/heads/main/openapi/disease-sh-covid-19-worldometers-api-openapi.yml
- filename: disease-sh-influenza-cdc-api-openapi.yml
  format: yaml
  label: 'disease.sh Influenza: CDC API'
  slug: disease-sh-influenza-cdc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/disease-sh/refs/heads/main/openapi/disease-sh-influenza-cdc-api-openapi.yml
consequence_counts:
  read: 41
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Disease Sh Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 41
overview: 'disease.sh exposes 41 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 41 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: disease.sh
provider_slug: disease-sh
slug: disease-sh-agentic-access
source_filename: disease-sh-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 41\n  by_action_class:\n    connected: 41\n  by_consequence:\n    read: 41\n  human_in_the_loop_required: 0\noperations:\n- path: /v3/covid-19/all\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/covid-19/states\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/covid-19/states/{states}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/covid-19/continents\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/covid-19/continents/{continent}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/covid-19/countries\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/covid-19/countries/{country}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/covid-19/countries/{countries}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/covid-19/jhucsse\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/covid-19/jhucsse/counties\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/covid-19/jhucsse/counties/{county}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/covid-19/historical\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/covid-19/historical/all\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/covid-19/historical/{country}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/covid-19/historical/{countries}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/covid-19/historical/{country}/{province}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/covid-19/historical/{country}/{provinces}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/covid-19/historical/usacounties\n  method: get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/covid-19/historical/usacounties/{state}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/covid-19/nyt/states\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/covid-19/nyt/states/{state}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/covid-19/nyt/counties\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/covid-19/nyt/counties/{county}\n  method: get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/covid-19/nyt/usa\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/covid-19/apple/countries\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/covid-19/apple/countries/{country}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/covid-19/apple/countries/{country}/{subregions}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/covid-19/gov/\n  method: get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/covid-19/gov/{country}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/covid-19/vaccine\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/covid-19/vaccine/coverage\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/covid-19/vaccine/coverage/countries\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/covid-19/vaccine/coverage/countries/{country}\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/covid-19/vaccine/coverage/states\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/covid-19/vaccine/coverage/states/{state}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/covid-19/therapeutics\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/covid-19/variants/countries/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/covid-19/variants/countries/{country}\n \
  \ method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/influenza/cdc/ILINet\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/influenza/cdc/USCL\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/influenza/cdc/USPHL\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/disease-sh/refs/heads/main/agentic-access/disease-sh-agentic-access.yml
summary_line: 41 operations
tags:
- COVID-19
- Disease
- Health
- Epidemiology
- Influenza
- Vaccine
- Open Data
- Public Health
---
