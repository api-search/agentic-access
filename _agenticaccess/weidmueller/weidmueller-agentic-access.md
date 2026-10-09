---
acting_count: 23
action_class_counts:
  acting: 23
  connected: 30
api_specs:
- filename: weidmueller-variable-nats-asyncapi.yml
  format: yaml
  label: Weidmüller u-OS Data Hub Variable-NATS API
  slug: u-os-data-hub-variable-nats-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/asyncapi/weidmueller-variable-nats-asyncapi.yml
- filename: weidmueller-consumer-api-openapi.yml
  format: yaml
  label: Weidmüller Consumer API
  slug: weidmueller-consumer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-consumer-api-openapi.yml
- filename: weidmueller-firewall-api-openapi.yml
  format: yaml
  label: Weidmüller Firewall API
  slug: weidmueller-firewall-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-firewall-api-openapi.yml
- filename: weidmueller-logging-api-openapi.yml
  format: yaml
  label: Weidmüller Logging API
  slug: weidmueller-logging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-logging-api-openapi.yml
- filename: weidmueller-network-api-openapi.yml
  format: yaml
  label: Weidmüller Network API
  slug: weidmueller-network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-network-api-openapi.yml
- filename: weidmueller-operations-api-openapi.yml
  format: yaml
  label: Weidmüller Operations API
  slug: weidmueller-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-operations-api-openapi.yml
- filename: weidmueller-ping-api-openapi.yml
  format: yaml
  label: Weidmüller Ping API
  slug: weidmueller-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-ping-api-openapi.yml
- filename: weidmueller-realtime-api-openapi.yml
  format: yaml
  label: Weidmüller Realtime API
  slug: weidmueller-realtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-realtime-api-openapi.yml
- filename: weidmueller-recovery-api-openapi.yml
  format: yaml
  label: Weidmüller Recovery API
  slug: weidmueller-recovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-recovery-api-openapi.yml
- filename: weidmueller-security-api-openapi.yml
  format: yaml
  label: Weidmüller Security API
  slug: weidmueller-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-security-api-openapi.yml
- filename: weidmueller-serial-interfaces-api-openapi.yml
  format: yaml
  label: Weidmüller Serial Interfaces API
  slug: weidmueller-serial-interfaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-serial-interfaces-api-openapi.yml
- filename: weidmueller-syslog-api-openapi.yml
  format: yaml
  label: Weidmüller Syslog API
  slug: weidmueller-syslog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-syslog-api-openapi.yml
- filename: weidmueller-system-api-openapi.yml
  format: yaml
  label: Weidmüller System API
  slug: weidmueller-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-system-api-openapi.yml
- filename: weidmueller-time-api-openapi.yml
  format: yaml
  label: Weidmüller Time API
  slug: weidmueller-time-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-time-api-openapi.yml
- filename: weidmueller-update-api-openapi.yml
  format: yaml
  label: Weidmüller Update API
  slug: weidmueller-update-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-update-api-openapi.yml
- filename: weidmueller-open-api-api-openapi.yml
  format: yaml
  label: Weidmüller Open API
  slug: weidmueller-open-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-open-api-api-openapi.yml
consequence_counts:
  read: 30
  safety-critical: 5
  write: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 5
kind: agentic-access
layout: agentic-access
method: generated
name: Weidmueller Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /firewall/active-config
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /firewall/active-config
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /network:factory-reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /recovery:factory-reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /system:reboot
operation_count: 53
overview: 'Weidmüller exposes 53 API operations that an AI agent could call, of which 23 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 30 read, 18 write, and 5 safety-critical.


  5 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Weidmüller
provider_slug: weidmueller
slug: weidmueller-agentic-access
source_filename: weidmueller-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: generated\nsource: openapi/weidmueller-administration-openapi.yml, openapi/weidmueller-variable-http-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 53\n  by_action_class:\n    connected: 30\n    acting: 23\n  by_consequence:\n    read: 30\n    safety-critical: 5\n    write: 18\n  human_in_the_loop_required: 5\noperations:\n- path: /firewall/active-config\n  method: get\n  operationId: get_firewall_active_config\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - u-os-adm.firewall.readonly\n    - u-os-adm.firewall.readwrite\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /firewall/active-config\n  method: put\n  operationId:\
  \ set_firewall_active_config\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - u-os-adm.firewall.readwrite\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /firewall/active-config\n  method: head\n  operationId: head_firewall_active_config\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - u-os-adm.firewall.readonly\n    - u-os-adm.firewall.readwrite\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /firewall/active-config\n  method: patch\n  operationId: update_firewall_active_config\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - u-os-adm.firewall.readwrite\n    audience: null\n    token:\n      max-ttl:\
  \ 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /firewall/config\n  method: get\n  operationId: get_firewall_config\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - u-os-adm.firewall.readonly\n    - u-os-adm.firewall.readwrite\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /firewall/config\n  method: put\n  operationId: set_firewall_config\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - u-os-adm.firewall.readwrite\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /firewall/config\n  method: patch\n  operationId: update_firewall_config\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    scope:\n    - u-os-adm.firewall.readwrite\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /firewall:reload\n  method: post\n  operationId: reload_firewall_config\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - u-os-adm.firewall.readwrite\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /logging/entries\n  method: get\n  operationId: get_logging_entries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - u-os-adm.logging.readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /logging/reports\n  method: post\n  operationId:\
  \ create_logging_report\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - u-os-adm.logging.readonly\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /logging/reports/{report_id}\n  method: get\n  operationId: get_logging_report\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - u-os-adm.logging.readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /logging/sources\n  method: get\n  operationId: get_logging_sources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - u-os-adm.logging.readonly\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /network/config\n  method: get\n  operationId: get_network_config\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - u-os-adm.network.readonly\n    - u-os-adm.network.readwrite\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /network/config\n  method: put\n  operationId: set_network_config\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - u-os-adm.network.readwrite\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /network/config\n  method: patch\n  operationId: update_network_config\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - u-os-adm.network.readwrite\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /network/state\n\
  \  method: get\n  operationId: get_network_state\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - u-os-adm.network.readonly\n    - u-os-adm.network.readwrite\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /network:factory-reset\n  method: post\n  operationId: network_factory_reset\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - u-os-adm.network.readwrite\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /openapi.json\n  method: get\n  operationId: get_openapi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operations/{operation_id}\n  method: get\n  operationId: get_operation\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ping\n  method: get\n  operationId: ping\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /realtime/config\n  method: get\n  operationId: get_realtime_config\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - u-os-adm.realtime.readonly\n    - u-os-adm.realtime.readwrite\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /realtime/config\n  method: put\n  operationId: set_realtime_config\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - u-os-adm.realtime.readwrite\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /realtime/state\n  method: get\n  operationId: get_realtime_state\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - u-os-adm.realtime.readonly\n    - u-os-adm.realtime.readwrite\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recovery:factory-reset\n  method: post\n  operationId: recovery_factory_reset\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - u-os-adm.recovery.readwrite\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /security/config\n  method: get\n  operationId: get_security_settings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - u-os-adm.security.readonly\n\
  \    - u-os-adm.security.readwrite\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /security/config\n  method: put\n  operationId: set_security_settings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - u-os-adm.security.readwrite\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /serial-interfaces/config\n  method: get\n  operationId: get_serial_interface_config\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - u-os-adm.serial-interfaces.readonly\n    - u-os-adm.serial-interfaces.readwrite\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /serial-interfaces/config\n  method: put\n  operationId: set_serial_interface_config\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    scope:\n    - u-os-adm.serial-interfaces.readwrite\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /serial-interfaces/config\n  method: patch\n  operationId: update_serial_interface_config\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - u-os-adm.serial-interfaces.readwrite\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /serial-interfaces/state\n  method: get\n  operationId: get_serial_interface_state\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - u-os-adm.serial-interfaces.readonly\n    - u-os-adm.serial-interfaces.readwrite\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /syslog/certificates\n  method: get\n  operationId: get_certificates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - u-os-adm.syslog.readonly\n    - u-os-adm.syslog.readwrite\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /syslog/certificates\n  method: put\n  operationId: set_certificates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - u-os-adm.syslog.readwrite\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /syslog/certificates\n  method: patch\n  operationId: patch_certificates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - u-os-adm.syslog.readwrite\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /syslog/config\n  method: get\n  operationId: get_config\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - u-os-adm.syslog.readonly\n    - u-os-adm.syslog.readwrite\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /syslog/config\n  method: put\n  operationId: set_config\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - u-os-adm.syslog.readwrite\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /syslog/state\n  method: get\n  operationId: get_state\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - u-os-adm.syslog.readonly\n   \
  \ - u-os-adm.syslog.readwrite\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /system/disks\n  method: get\n  operationId: get_system_disks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - u-os-adm.system.readonly\n    - u-os-adm.system.readwrite\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /system/info\n  method: get\n  operationId: get_system_info\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - u-os-adm.system.readonly\n    - u-os-adm.system.readwrite\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /system/nameplate\n  method: get\n  operationId: get_system_nameplate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - u-os-adm.system.readonly\n    - u-os-adm.system.readwrite\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /system:reboot\n  method:\
  \ post\n  operationId: system_reboot\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - u-os-adm.system.readwrite\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /time/config\n  method: get\n  operationId: get_time_config\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - u-os-adm.time.readonly\n    - u-os-adm.time.readwrite\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /time/config\n  method: put\n  operationId: set_time_config\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - u-os-adm.time.readwrite\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n \
  \     triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /time/state\n  method: get\n  operationId: get_time_state\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - u-os-adm.time.readonly\n    - u-os-adm.time.readwrite\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /time/timezones\n  method: get\n  operationId: list_timezones\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - u-os-adm.time.readonly\n    - u-os-adm.time.readwrite\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /update/config\n  method: get\n  operationId: get_update_settings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - u-os-adm.update.readonly\n    - u-os-adm.update.readwrite\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /update/config\n  method: put\n  operationId:\
  \ set_update_settings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - u-os-adm.update.readwrite\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /update/config\n  method: patch\n  operationId: update_update_settings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - u-os-adm.update.readwrite\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi.json\n  method: get\n  operationId: get_openapi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /providers\n  method: get\n  operationId:\
  \ get_providers_handler\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - hub.variables.readonly\n    - hub.variables.readwrite\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /providers/{provider_id}/variables\n  method: get\n  operationId: get_variables_handler\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - hub.variables.readonly\n    - hub.variables.readwrite\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /providers/{provider_id}/variables\n  method: post\n  operationId: post_multiple_variables_handler\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - hub.variables.readwrite\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /providers/{provider_id}/variables/{variable_key}\n\
  \  method: get\n  operationId: get_single_variable_handler\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - hub.variables.readonly\n    - hub.variables.readwrite\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /providers/{provider_id}/variables/{variable_key}\n  method: post\n  operationId: post_single_variable_handler\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - hub.variables.readwrite\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/agentic-access/weidmueller-agentic-access.yml
summary_line: 53 operations · 23 acting · 5 human-in-the-loop
tags:
- Company
- Industrial Automation
- Industrial Connectivity
- Edge Computing
- IIoT
- u-OS
- Manufacturing
---
