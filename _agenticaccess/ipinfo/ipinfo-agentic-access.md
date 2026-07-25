---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 50
api_specs:
- filename: ipinfo-abuse-api-openapi.yml
  format: yaml
  label: IPinfo abuse API
  slug: ipinfo-abuse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-abuse-api-openapi.yml
- filename: ipinfo-asn-api-openapi.yml
  format: yaml
  label: IPinfo asn API
  slug: ipinfo-asn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-asn-api-openapi.yml
- filename: ipinfo-carrier-api-openapi.yml
  format: yaml
  label: IPinfo carrier API
  slug: ipinfo-carrier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-carrier-api-openapi.yml
- filename: ipinfo-company-api-openapi.yml
  format: yaml
  label: IPinfo company API
  slug: ipinfo-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-company-api-openapi.yml
- filename: ipinfo-domains-api-openapi.yml
  format: yaml
  label: IPinfo domains API
  slug: ipinfo-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-domains-api-openapi.yml
- filename: ipinfo-general-api-openapi.yml
  format: yaml
  label: IPinfo general API
  slug: ipinfo-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-general-api-openapi.yml
- filename: ipinfo-ipinfo-core-api-openapi.yml
  format: yaml
  label: IPinfo ipinfo core API
  slug: ipinfo-ipinfo-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-ipinfo-core-api-openapi.yml
- filename: ipinfo-ipinfo-lite-api-openapi.yml
  format: yaml
  label: IPinfo ipinfo lite API
  slug: ipinfo-ipinfo-lite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-ipinfo-lite-api-openapi.yml
- filename: ipinfo-ipinfo-max-api-openapi.yml
  format: yaml
  label: IPinfo ipinfo max API
  slug: ipinfo-ipinfo-max-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-ipinfo-max-api-openapi.yml
- filename: ipinfo-ipinfo-plus-api-openapi.yml
  format: yaml
  label: IPinfo ipinfo plus API
  slug: ipinfo-ipinfo-plus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-ipinfo-plus-api-openapi.yml
- filename: ipinfo-places-api-openapi.yml
  format: yaml
  label: IPinfo places API
  slug: ipinfo-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-places-api-openapi.yml
- filename: ipinfo-privacy-detection-api-openapi.yml
  format: yaml
  label: IPinfo privacy detection API
  slug: ipinfo-privacy-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-privacy-detection-api-openapi.yml
- filename: ipinfo-privacy-detection-extended-api-openapi.yml
  format: yaml
  label: IPinfo privacy detection extended API
  slug: ipinfo-privacy-detection-extended-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-privacy-detection-extended-api-openapi.yml
- filename: ipinfo-ranges-api-openapi.yml
  format: yaml
  label: IPinfo ranges API
  slug: ipinfo-ranges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-ranges-api-openapi.yml
- filename: ipinfo-residential-proxy-detection-api-openapi.yml
  format: yaml
  label: IPinfo residential proxy detection API
  slug: ipinfo-residential-proxy-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-residential-proxy-detection-api-openapi.yml
- filename: ipinfo-single-api-openapi.yml
  format: yaml
  label: IPinfo single API
  slug: ipinfo-single-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-single-api-openapi.yml
- filename: ipinfo-whois-api-openapi.yml
  format: yaml
  label: IPinfo whois API
  slug: ipinfo-whois-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-whois-api-openapi.yml
consequence_counts:
  read: 50
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ipinfo Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 53
overview: 'IPinfo exposes 53 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 50 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: IPinfo
provider_slug: ipinfo
slug: ipinfo-agentic-access
source_filename: ipinfo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/ipinfo-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 53\n  by_action_class:\n    connected: 50\n    acting: 3\n  by_consequence:\n    read: 50\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /max/{ip}\n  method: get\n  operationId: getMaxInformationByIp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /places/{ip}\n  method: get\n  operationId: getPlaceByIp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: getCurrentInformation\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{ip}\n  method: get\n  operationId: getInformationByIp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me\n  method: get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /batch\n  method: post\n  operationId: batch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/summarize-ips\n  method: post\n  operationId: summarize\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/map\n  method: post\n  operationId: map\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /AS{asn}\n  method: get\n  operationId: getAsn\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{ip}/company\n  method: get\n  operationId: getCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{ip}/carrier\n\
  \  method: get\n  operationId: getCarrier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ranges/{domain}\n  method: get\n  operationId: getRanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domains/{ip}\n  method: get\n  operationId: getDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{ip}/abuse\n  method: get\n  operationId: getAbuse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{ip}/privacy\n  method: get\n  operationId: getPrivacyInformationByIp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /{ip}/resproxy\n  method: get\n  operationId: getResidentialProxyByIp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{ip}/privacy_extended\n  method: get\n  operationId: getPrivacyExtendedByIp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /whois/net/{whoisnetid}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /whois/net/{whoisip}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /whois/net/{domain}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /whois/net/AS{asn}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /whois/org/{whoisorgid}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /whois/poc/{whoispoc}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ip\n  method: get\n  operationId: getCurrentIp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{ip}/ip\n  method: get\n  operationId: getIpByIp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hostname\n  method: get\n  operationId: getCurrentHostname\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{ip}/hostname\n  method: get\n  operationId: getHostnameByIp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /city\n  method: get\n  operationId: getCurrentCity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{ip}/city\n  method: get\n  operationId: getCityByIp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /region\n  method: get\n  operationId: getCurrentRegion\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{ip}/region\n  method: get\n  operationId: getRegionByIp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /country\n  method: get\n  operationId: getCurrentCountry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{ip}/country\n  method: get\n  operationId: getCountryByIp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /loc\n  method: get\n  operationId: getCurrentLocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{ip}/loc\n  method:\
  \ get\n  operationId: getLocationByIp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /postal\n  method: get\n  operationId: getCurrentPostal\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{ip}/postal\n  method: get\n  operationId: getPostalByIp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /timezone\n  method: get\n  operationId: getCurrentTimezone\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{ip}/timezone\n  method: get\n  operationId: getTimezoneByIp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /org\n  method: get\n  operationId: getCurrentOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{ip}/org\n  method: get\n  operationId: getOrganizationByIp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lite/me\n  method: get\n  operationId: getCurrentLiteInformation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lite/{ip}\n  method: get\n  operationId: getLiteInformationByIp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lite/me/{field}\n  method: get\n  operationId: getCurrentLiteField\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lite/{ip}/{field}\n  method: get\n  operationId: getLiteFieldByIp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lookup/me\n  method: get\n  operationId: getCurrentCoreInformation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lookup/{ip}\n  method: get\n  operationId: getCoreInformationByIp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lookup/me/{field}\n  method: get\n  operationId: getCurrentCoreField\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /lookup/{ip}/{field}\n  method: get\n  operationId: getCoreFieldByIp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /plus/me\n  method: get\n  operationId: getCurrentPlusInformation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /plus/{ip}\n  method: get\n  operationId: getPlusInformationByIp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /plus/me/{field}\n  method: get\n  operationId: getCurrentPlusField\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /plus/{ip}/{field}\n  method: get\n  operationId: getPlusFieldByIp\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/agentic-access/ipinfo-agentic-access.yml
summary_line: 53 operations · 3 acting
tags:
- IP Intelligence
- IP Geolocation
- ASN
- Privacy Detection
- VPN Detection
- Threat Intelligence
- Network Data
- Mobile Carrier
- WHOIS
- Public APIs
- Development
---
