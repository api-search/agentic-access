---
acting_count: 0
action_class_counts:
  open: 4
consequence_counts:
  read: 4
description: x-agentic-access execution contracts for the surfaces an agent can actually reach. This file REPLACES a version generated from a fabricated OpenAPI, whose three operations (/resource/8mmf-is58.json, .csv and /api/views/8mmf-is58.json) were classified against a host — data.exim.gov — that has had no DNS record since 2023-09-14. See _quarantine/NOTE.md. Every path below was fetched and returned the status recorded.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: probed
name: Export Import Bank Of The United States Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'Export-Import Bank of the United States exposes 4 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Export-Import Bank of the United States
provider_slug: export-import-bank-of-the-united-states
slug: export-import-bank-of-the-united-states-agentic-access
source_filename: export-import-bank-of-the-united-states-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live unauthenticated GETs of every reachable EXIM data surface, 2026-09-04\ndescription: >-\n  x-agentic-access execution contracts for the surfaces an agent can actually reach. This\n  file REPLACES a version generated from a fabricated OpenAPI, whose three operations\n  (/resource/8mmf-is58.json, .csv and /api/views/8mmf-is58.json) were classified against a\n  host — data.exim.gov — that has had no DNS record since 2023-09-14. See\n  _quarantine/NOTE.md. Every path below was fetched and returned the status recorded.\nsummary:\n  operations: 4\n  by_action_class:\n    open: 4\n  by_consequence:\n    read: 4\n  human_in_the_loop_required: 0\n  write_operations: 0\n  note: >-\n    EVERY EXIM surface an agent can call is read-only, anonymous and free. There is no\n    write path, no key to leak, no quota to exhaust and no reversal to plan for. The only\n    real agent hazard here is staleness: the CSV URL changes each fiscal quarter,\
  \ so an\n    agent that caches the download address will silently serve last quarter's data.\noperations:\n- url: https://img.exim.gov/s3fs-public/dataset/vbhv-d8am/data.json\n  method: get\n  http_status: 200\n  name: EXIM Project Open Data catalog\n  x-agentic-access:\n    action-class: open\n    consequence: read\n    subject: none\n    token: null\n    audit: none\n  note: >-\n    START HERE. Resolve the current CSV download URL from this document on every run\n    rather than caching it.\n- url: https://img.exim.gov/s3fs-public/dataset/vbhv-d8am/data-gov_fy26-q2.csv\n  method: get\n  http_status: 200\n  name: EXIM authorizations bulk CSV\n  x-agentic-access:\n    action-class: open\n    consequence: read\n    subject: none\n    token: null\n    audit: none\n  note: >-\n    UNSTABLE ADDRESS. The fiscal quarter is in the filename; this URL is superseded each\n    quarter. Treat it as a pointer read from data.json, never as a constant.\n- url: https://www.digitalarchives.exim.gov/digital/api/collections\n\
  \  method: get\n  http_status: 200\n  name: EXIM Digital Archives collection list\n  x-agentic-access:\n    action-class: open\n    consequence: read\n    subject: none\n    token: null\n    audit: none\n  operator: vendor\n  operator_name: OCLC CONTENTdm\n- url: https://www.digitalarchives.exim.gov/iiif/{alias}:{id}/manifest.json\n  method: get\n  http_status: 200\n  http_status_evidence: https://www.digitalarchives.exim.gov/iiif/ExImPR01:4250/manifest.json\n  name: IIIF Presentation 2.0 manifest\n  x-agentic-access:\n    action-class: open\n    consequence: read\n    subject: none\n    token: null\n    audit: none\n  operator: vendor\n  operator_name: OCLC CONTENTdm\nunreachable:\n- url: https://eximonline.exim.gov/\n  http_status: 200\n  reason: >-\n    Human login portal carrying a Controlled Unclassified Information banner. No public\n    programmatic entry point. Agents must not attempt access.\n- url: https://data.exim.gov/\n  http_status: 0\n  reason: 'Decommissioned 2023-09-14.\
  \ DNS resolution failure. Do not retry.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/export-import-bank-of-the-united-states/refs/heads/main/agentic-access/export-import-bank-of-the-united-states-agentic-access.yml
summary_line: 4 operations
tags:
- Export
- Federal-Government
- Finance
- Import
- Open Data
- Trade Finance
---
