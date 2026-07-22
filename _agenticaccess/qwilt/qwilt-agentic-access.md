---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 10
api_specs:
- filename: qwilt-media-delivery-openapi.yml
  format: yaml
  label: Qwilt CDN Media Delivery (Sites) API
  slug: qwilt-cdn-media-delivery-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qwilt/refs/heads/main/openapi/qwilt-media-delivery-openapi.yml
- filename: qwilt-certificate-manager-openapi.yml
  format: yaml
  label: Qwilt CDN Certificate Manager API
  slug: qwilt-cdn-certificate-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qwilt/refs/heads/main/openapi/qwilt-certificate-manager-openapi.yml
- filename: qwilt-origin-allow-list-openapi.yml
  format: yaml
  label: Qwilt CDN Origin Allow List API
  slug: qwilt-cdn-origin-allow-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qwilt/refs/heads/main/openapi/qwilt-origin-allow-list-openapi.yml
consequence_counts:
  read: 10
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Qwilt Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'Qwilt exposes 22 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 12 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Qwilt
provider_slug: qwilt
slug: qwilt-agentic-access
source_filename: qwilt-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/qwilt-certificate-manager-openapi.yml, openapi/qwilt-media-delivery-openapi.yml,\n  openapi/qwilt-origin-allow-list-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    connected: 10\n    acting: 12\n  by_consequence:\n    read: 10\n    write: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v2/certificates\n  method: get\n  operationId: listCertificates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/certificates\n  method: post\n  operationId: createCertificate\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/certificates/{certId}\n  method: get\n  operationId: getCertificate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/certificates/{certId}\n  method: put\n  operationId: updateCertificate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/certificates/{certId}\n  method: delete\n  operationId: deleteCertificate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/certificate-templates\n  method: get\n  operationId: listCertificateTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/certificate-templates\n  method: post\n  operationId: createCertificateTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/sites\n  method: get\n  operationId: listSites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/v2/sites\n  method: post\n  operationId: createSite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/sites/{siteId}\n  method: get\n  operationId: getSite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/sites/{siteId}\n  method: put\n  operationId: updateSite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/sites/{siteId}\n  method: delete\n  operationId: deleteSite\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1/sites/{siteId}/configurations\n  method: get\n  operationId: listSiteConfigurations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/1/sites/{siteId}/configurations\n  method: post\n  operationId: createSiteConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1/sites/{siteId}/configurations/{revisionId}\n  method: get\n  operationId: getSiteConfiguration\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/sites/{siteId}/publishing-operations\n  method: get\n  operationId: listPublishingOperations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/sites/{siteId}/publishing-operations\n  method: post\n  operationId: createPublishingOperation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/sites/{siteId}/publishing-operations/{publishId}\n  method: get\n  operationId: getPublishingOperation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/v2/sites/{siteId}/publishing-operations/actions/un-publish\n  method: post\n  operationId: unpublishSite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/sites/{siteId}/publishing-operations/actions/republish\n  method: post\n  operationId: republishSite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/sites/{siteId}/publishing-operations/{publishId}/actions/cancel\n  method: post\n  operationId: cancelPublishingOperation\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/1.0/network/device-ip\n  method: get\n  operationId: getOriginAllowList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qwilt/refs/heads/main/agentic-access/qwilt-agentic-access.yml
summary_line: 22 operations · 12 acting
tags:
- Company
- Media
- CDN
- Content Delivery Network
- Edge Computing
- Video Streaming
- Open Caching
- Media Delivery
- Certificates
- Infrastructure
---
