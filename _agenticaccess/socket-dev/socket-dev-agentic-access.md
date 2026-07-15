---
acting_count: 41
action_class_counts:
  acting: 41
  connected: 40
api_specs:
- filename: socket-packages-api-openapi.yml
  format: yaml
  label: Socket Packages API
  slug: socket-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-packages-api-openapi.yml
- filename: socket-full-scans-api-openapi.yml
  format: yaml
  label: Socket Full Scans API
  slug: socket-full-scans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-full-scans-api-openapi.yml
- filename: socket-diff-scans-api-openapi.yml
  format: yaml
  label: Socket Diff Scans API
  slug: socket-diff-scans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-diff-scans-api-openapi.yml
- filename: socket-alerts-api-openapi.yml
  format: yaml
  label: Socket Alerts API
  slug: socket-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-alerts-api-openapi.yml
- filename: socket-triage-api-openapi.yml
  format: yaml
  label: Socket Triage API
  slug: socket-triage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-triage-api-openapi.yml
- filename: socket-repos-api-openapi.yml
  format: yaml
  label: Socket Repos API
  slug: socket-repos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-repos-api-openapi.yml
- filename: socket-org-settings-api-openapi.yml
  format: yaml
  label: Socket Organization Settings API
  slug: socket-org-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-org-settings-api-openapi.yml
- filename: socket-webhooks-api-openapi.yml
  format: yaml
  label: Socket Webhooks API
  slug: socket-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-webhooks-api-openapi.yml
- filename: socket-threat-feed-api-openapi.yml
  format: yaml
  label: Socket Threat Feed API
  slug: socket-threat-feed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-threat-feed-api-openapi.yml
- filename: socket-fixes-api-openapi.yml
  format: yaml
  label: Socket Fixes API
  slug: socket-fixes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-fixes-api-openapi.yml
- filename: socket-dependencies-api-openapi.yml
  format: yaml
  label: Socket Dependencies API
  slug: socket-dependencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-dependencies-api-openapi.yml
- filename: socket-api-tokens-api-openapi.yml
  format: yaml
  label: Socket API Tokens API
  slug: socket-api-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-api-tokens-api-openapi.yml
- filename: socket-audit-log-api-openapi.yml
  format: yaml
  label: Socket Audit Log API
  slug: socket-audit-log-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-audit-log-api-openapi.yml
- filename: socket-org-snapshots-api-openapi.yml
  format: yaml
  label: Socket Organization Snapshots API
  slug: socket-org-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-org-snapshots-api-openapi.yml
- filename: socket-metadata-api-openapi.yml
  format: yaml
  label: Socket Metadata API
  slug: socket-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-metadata-api-openapi.yml
consequence_counts:
  read: 40
  safety-critical: 1
  write: 40
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Socket Dev Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /orgs/{org_slug}/api-tokens/revoke
operation_count: 81
overview: 'Socket exposes 81 API operations that an AI agent could call, of which 41 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 40 read, 40 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Socket
provider_slug: socket-dev
slug: socket-dev-agentic-access
source_filename: socket-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/socket-alerts-api-openapi.yml, openapi/socket-api-tokens-api-openapi.yml, openapi/socket-audit-log-api-openapi.yml,\n  openapi/socket-dependencies-api-openapi.yml, openapi/socket-diff-scans-api-openapi.yml, openapi/socket-fixes-api-openapi.yml,\n  openapi/socket-full-scans-api-openapi.yml, openapi/socket-metadata-api-openapi.yml, openapi/socket-org-settings-api-openapi.yml,\n  openapi/socket-org-snapshots-api-openapi.yml, openapi/socket-packages-api-openapi.yml, openapi/socket-repos-api-openapi.yml,\n  openapi/socket-threat-feed-api-openapi.yml, openapi/socket-triage-api-openapi.yml, openapi/socket-webhooks-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 81\n  by_action_class:\n\
  \    connected: 40\n    acting: 41\n  by_consequence:\n    read: 40\n    write: 40\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /orgs/{org_slug}/historical/alerts\n  method: get\n  operationId: historicalAlertsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - historical:alerts-list\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_slug}/historical/alerts/trend\n  method: get\n  operationId: historicalAlertsTrend\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - historical:alerts-trend\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_slug}/alerts\n  method: get\n  operationId: alertsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - alerts:list\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_slug}/alert-full-scan-search\n\
  \  method: get\n  operationId: alertFullScans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - alerts:list\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_slug}/api-tokens\n  method: post\n  operationId: postAPIToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api-tokens:create\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_slug}/api-tokens\n  method: get\n  operationId: getAPITokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api-tokens:list\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_slug}/api-tokens/update\n  method: post\n  operationId: postAPITokenUpdate\n  x-agentic-access:\n \
  \   action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api-tokens:create\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_slug}/api-tokens/rotate\n  method: post\n  operationId: postAPITokensRotate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api-tokens:rotate\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_slug}/api-tokens/revoke\n  method: post\n  operationId: postAPITokensRevoke\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - api-tokens:revoke\n    audience: null\n    token:\n      max-ttl: 120\n      exchange:\
  \ true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /quota\n  method: get\n  operationId: getQuota\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations\n  method: get\n  operationId: getOrganizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_slug}/audit-log\n  method: get\n  operationId: getAuditLogEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - audit-log:list\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dependencies/search\n  method: post\n  operationId: searchDependencies\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_slug}/historical/dependencies/trend\n  method: get\n  operationId: historicalDependenciesTrend\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - historical:dependencies-trend\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_slug}/diff-scans\n  method: get\n  operationId: listOrgDiffScans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - diff-scans:list\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_slug}/diff-scans/{diff_scan_id}\n  method: get\n  operationId: getDiffScanById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - diff-scans:list\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_slug}/diff-scans/{diff_scan_id}\n  method: delete\n  operationId: deleteOrgDiffScan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - diff-scans:delete\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_slug}/diff-scans/{diff_scan_id}/gfm\n  method: get\n  operationId: GetDiffScanGfm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - diff-scans:list\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_slug}/diff-scans/from-repo/{repo_slug}\n  method: post\n  operationId: createOrgRepoDiff\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - diff-scans:create\n    - full-scans:create\n\
  \    - repo:list\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_slug}/diff-scans/from-ids\n  method: post\n  operationId: createOrgDiffScanFromIds\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - diff-scans:create\n    - full-scans:list\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_slug}/supported-files\n  method: get\n  operationId: getSupportedFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /alert-types\n  method: post\n  operationId: alertTypes\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_slug}/fixes\n  method: get\n  operationId: fetch-fixes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - fixes:list\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_slug}/full-scans\n  method: get\n  operationId: getOrgFullScanList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - full-scans:list\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_slug}/full-scans\n  method: post\n  operationId: CreateOrgFullScan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - full-scans:create\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_slug}/full-scans/{full_scan_id}\n  method: get\n  operationId: getOrgFullScan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - full-scans:list\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_slug}/full-scans/{full_scan_id}\n  method: delete\n  operationId: deleteOrgFullScan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - full-scans:delete\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_slug}/full-scans/{full_scan_id}/metadata\n  method: get\n  operationId: getOrgFullScanMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    scope:\n    - full-scans:list\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_slug}/full-scans/{full_scan_id}/files/tar\n  method: get\n  operationId: downloadOrgFullScanFilesAsTar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - full-scans:list\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_slug}/full-scans/archive\n  method: post\n  operationId: CreateOrgFullScanArchive\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - full-scans:create\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_slug}/full-scans/{full_scan_id}/rescan\n  method: post\n  operationId: rescanOrgFullScan\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    scope:\n    - full-scans:create\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_slug}/full-scans/{full_scan_id}/format/csv\n  method: post\n  operationId: getOrgFullScanCsv\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - full-scans:list\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_slug}/full-scans/{full_scan_id}/format/pdf\n  method: post\n  operationId: getOrgFullScanPdf\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - full-scans:list\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_slug}/export/cdx/{id}\n  method: get\n  operationId: exportCDX\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - report:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_slug}/export/openvex/{id}\n  method: get\n  operationId: exportOpenVEX\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - report:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_slug}/export/spdx/{id}\n  method: get\n  operationId: exportSPDX\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - report:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_slug}/supported-files\n  method: get\n  operationId: getSupportedFiles\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /alert-types\n  method: post\n  operationId: alertTypes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_slug}/supported-files\n  method: get\n  operationId: getSupportedFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /license-metadata\n  method: post\n  operationId: licenseMetadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /alert-types\n  method: post\n  operationId: alertTypes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi\n  method: get\n  operationId: getOpenAPI\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi.json\n  method: get\n  operationId: getOpenAPIJSON\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_slug}/settings/integrations/{integration_id}/events\n  method: get\n  operationId: getIntegrationEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    scope:\n    - integration:list\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_slug}/settings/security-policy\n  method: get\n  operationId: getOrgSecurityPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - security-policy:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_slug}/settings/security-policy\n  method: post\n  operationId: updateOrgSecurityPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - security-policy:update\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_slug}/settings/license-policy\n  method: post\n  operationId: updateOrgLicensePolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    scope:\n    - license-policy:update\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_slug}/settings/license-policy/view\n  method: get\n  operationId: viewLicensePolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - license-policy:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_slug}/settings/socket-basics\n  method: get\n  operationId: getSocketBasicsConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - socket-basics:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_slug}/telemetry/config\n  method: get\n  operationId: getOrgTelemetryConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_slug}/telemetry/config\n  method: put\n  operationId: updateOrgTelemetryConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - telemetry-policy:update\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /license-policy\n  method: post\n  operationId: licensePolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - license-policy:read\n    - packages:list\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /license-metadata\n  method: post\n  operationId: licenseMetadata\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_slug}/historical/snapshots\n  method: get\n  operationId: historicalSnapshotsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - historical:snapshots-list\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_slug}/historical/snapshots\n  method: post\n  operationId: historicalSnapshotsStart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - historical:snapshots-start\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /purl\n  method: post\n  operationId:\
  \ batchPackageFetch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - packages:list\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_slug}/purl\n  method: post\n  operationId: batchPackageFetchByOrg\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - packages:list\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_slug}/repos\n  method: get\n  operationId: getOrgRepoList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - repo:list\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_slug}/repos\n\
  \  method: post\n  operationId: createOrgRepo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - repo:create\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_slug}/repos/{repo_slug}\n  method: get\n  operationId: getOrgRepo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - repo:list\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_slug}/repos/{repo_slug}\n  method: post\n  operationId: updateOrgRepo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - repo:update\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /orgs/{org_slug}/repos/{repo_slug}\n  method: delete\n  operationId: deleteOrgRepo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - repo:delete\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_slug}/repos/labels/{label_id}/associate\n  method: post\n  operationId: associateOrgRepoLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - repo-label:update\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_slug}/repos/labels\n  method: post\n  operationId: createOrgRepoLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    scope:\n    - repo-label:create\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_slug}/repos/labels\n  method: get\n  operationId: getOrgRepoLabelList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - repo-label:list\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_slug}/repos/labels/{label_id}\n  method: delete\n  operationId: deleteOrgRepoLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - repo-label:delete\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_slug}/repos/labels/{label_id}\n  method: get\n  operationId:\
  \ getOrgRepoLabel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - repo-label:list\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_slug}/repos/labels/{label_id}\n  method: put\n  operationId: updateOrgRepoLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - repo-label:update\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_slug}/repos/labels/{label_id}/label-setting\n  method: delete\n  operationId: deleteOrgRepoLabelSetting\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - repo-label:update\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_slug}/repos/labels/{label_id}/label-setting\n  method: get\n  operationId: getOrgRepoLabelSetting\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - repo-label:list\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_slug}/repos/labels/{label_id}/label-setting\n  method: put\n  operationId: updateOrgRepoLabelSetting\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - repo-label:update\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_slug}/repos/labels/{label_id}/disassociate\n  method: post\n  operationId: disassociateOrgRepoLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    scope:\n    - repo-label:update\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_slug}/threat-feed\n  method: get\n  operationId: getOrgThreatFeedItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - threat-feed:list\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_slug}/triage/alerts\n  method: get\n  operationId: getOrgTriage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - triage:alerts-list\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_slug}/triage/alerts\n  method: post\n  operationId: updateOrgAlertTriage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - triage:alerts-update\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_slug}/triage/alerts/{uuid}\n  method: delete\n  operationId: deleteOrgAlertTriage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - triage:alerts-update\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_slug}/webhooks\n  method: get\n  operationId: getOrgWebhooksList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - webhooks:list\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_slug}/webhooks\n  method: post\n  operationId: createOrgWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    scope:\n    - webhooks:create\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_slug}/webhooks/{webhook_id}\n  method: get\n  operationId: getOrgWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - webhooks:list\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orgs/{org_slug}/webhooks/{webhook_id}\n  method: put\n  operationId: updateOrgWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - webhooks:update\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orgs/{org_slug}/webhooks/{webhook_id}\n  method: delete\n  operationId:\
  \ deleteOrgWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - webhooks:delete\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/agentic-access/socket-dev-agentic-access.yml
summary_line: 81 operations · 41 acting · 1 human-in-the-loop
tags:
- Supply Chain Security
- Open Source Security
- Software Composition Analysis
- SCA
- Malware Detection
- Dependency Scanning
- SBOM
- npm
- PyPI
- Go
- Maven
- Cargo
- NuGet
- RubyGems
- Developer Security
---
