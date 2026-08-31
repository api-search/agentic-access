---
acting_count: 0
action_class_counts:
  acting: 0
  connected: 16
api_specs:
- filename: carnegie-mellon-university-articles-api-openapi.yml
  format: yaml
  label: Carnegie Mellon University Articles API
  slug: carnegie-mellon-university-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carnegie-mellon-university/refs/heads/main/openapi/carnegie-mellon-university-articles-api-openapi.yml
- filename: carnegie-mellon-university-covidcast-api-openapi.yml
  format: yaml
  label: Carnegie Mellon University Covidcast API
  slug: carnegie-mellon-university-covidcast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carnegie-mellon-university/refs/heads/main/openapi/carnegie-mellon-university-covidcast-api-openapi.yml
- filename: carnegie-mellon-university-feeds-api-openapi.yml
  format: yaml
  label: Carnegie Mellon University Feeds API
  slug: carnegie-mellon-university-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carnegie-mellon-university/refs/heads/main/openapi/carnegie-mellon-university-feeds-api-openapi.yml
- filename: carnegie-mellon-university-fluview-api-openapi.yml
  format: yaml
  label: Carnegie Mellon University Fluview API
  slug: carnegie-mellon-university-fluview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carnegie-mellon-university/refs/heads/main/openapi/carnegie-mellon-university-fluview-api-openapi.yml
- filename: carnegie-mellon-university-forecasts-api-openapi.yml
  format: yaml
  label: Carnegie Mellon University Forecasts API
  slug: carnegie-mellon-university-forecasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carnegie-mellon-university/refs/heads/main/openapi/carnegie-mellon-university-forecasts-api-openapi.yml
- filename: carnegie-mellon-university-issues-api-openapi.yml
  format: yaml
  label: Carnegie Mellon University Issues API
  slug: carnegie-mellon-university-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carnegie-mellon-university/refs/heads/main/openapi/carnegie-mellon-university-issues-api-openapi.yml
- filename: carnegie-mellon-university-journals-api-openapi.yml
  format: yaml
  label: Carnegie Mellon University Journals API
  slug: carnegie-mellon-university-journals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carnegie-mellon-university/refs/heads/main/openapi/carnegie-mellon-university-journals-api-openapi.yml
- filename: carnegie-mellon-university-meta-api-openapi.yml
  format: yaml
  label: Carnegie Mellon University Meta API
  slug: carnegie-mellon-university-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carnegie-mellon-university/refs/heads/main/openapi/carnegie-mellon-university-meta-api-openapi.yml
- filename: carnegie-mellon-university-notes-api-openapi.yml
  format: yaml
  label: Carnegie Mellon University Notes API
  slug: carnegie-mellon-university-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carnegie-mellon-university/refs/heads/main/openapi/carnegie-mellon-university-notes-api-openapi.yml
- filename: carnegie-mellon-university-oai-pmh-api-openapi.yml
  format: yaml
  label: Carnegie Mellon University Oai Pmh API
  slug: carnegie-mellon-university-oai-pmh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carnegie-mellon-university/refs/heads/main/openapi/carnegie-mellon-university-oai-pmh-api-openapi.yml
- filename: carnegie-mellon-university-preprints-api-openapi.yml
  format: yaml
  label: Carnegie Mellon University Preprints API
  slug: carnegie-mellon-university-preprints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carnegie-mellon-university/refs/heads/main/openapi/carnegie-mellon-university-preprints-api-openapi.yml
- filename: carnegie-mellon-university-vendors-api-openapi.yml
  format: yaml
  label: Carnegie Mellon University Vendors API
  slug: carnegie-mellon-university-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carnegie-mellon-university/refs/heads/main/openapi/carnegie-mellon-university-vendors-api-openapi.yml
consequence_counts:
  read: 16
  safety-critical: 0
  write: 0
description: 'Recommended x-agentic-access execution contracts for the API surfaces Carnegie Mellon University actually operates. Rewritten 2026-08-19. The file this replaces described 157 operations (/altmetric/institutions, /articles, /projects, /symplectic...) classified 76 connected / 81 acting, with 79 writes and 2 safety-critical operations requiring a human in the loop. Not one of those operations was Carnegie Mellon''s — every one came from the figshare v2 contract, and the governance posture it recommended was governance of a vendor''s product under a university''s name. The real posture is far simpler and far duller: every institution-operated CMU endpoint is a public, anonymous, read-only GET. There are no writes, no credentials, no subjects and nothing safety-critical, so there is nothing here for an agent to do irreversibly. The genuine agent hazard on these surfaces is not consequence but MISREADING: both research APIs return errors with HTTP 200, so an agent that branches
  on status will treat a malformed query as an empty success. See errors/carnegie-mellon-university-errors.yml.'
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: derived
name: Carnegie Mellon University Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'Carnegie Mellon University exposes 16 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Carnegie Mellon University
provider_slug: carnegie-mellon-university
slug: carnegie-mellon-university-agentic-access
source_filename: carnegie-mellon-university-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: derived\nsource: openapi/carnegie-mellon-university-delphi-epidata-openapi.yml, openapi/carnegie-mellon-university-cert-vulnerability-notes-openapi.yml,\n  openapi/carnegie-mellon-university-library-publishing-openapi.yml — each itself derived from live probes\n  on 2026-08-19\nx-operator: institution\ndescription: 'Recommended x-agentic-access execution contracts for the API surfaces Carnegie Mellon University\n  actually operates. Rewritten 2026-08-19. The file this replaces described 157 operations (/altmetric/institutions,\n  /articles, /projects, /symplectic...) classified 76 connected / 81 acting, with 79 writes and 2 safety-critical\n  operations requiring a human in the loop. Not one of those operations was Carnegie Mellon''s — every\n  one came from the figshare v2 contract, and the governance posture it recommended was governance of\n  a vendor''s product under a university''s name. The real posture is far simpler and far duller: every\n\
  \  institution-operated CMU endpoint is a public, anonymous, read-only GET. There are no writes, no credentials,\n  no subjects and nothing safety-critical, so there is nothing here for an agent to do irreversibly. The\n  genuine agent hazard on these surfaces is not consequence but MISREADING: both research APIs return\n  errors with HTTP 200, so an agent that branches on status will treat a malformed query as an empty success.\n  See errors/carnegie-mellon-university-errors.yml.'\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 16\n    acting: 0\n  by_consequence:\n    read: 16\n    write: 0\n    safety-critical: 0\n  human_in_the_loop_required: 0\n  surfaces: 3\nagent_hazards:\n- hazard: error-in-200\n  surfaces:\n  - https://api.delphi.cmu.edu/epidata\n  - https://kb.cert.org/vuls/api\n  detail: Delphi returns {\"epidata\":[],\"message\":\"missing parameter...\",\"result\":-1} with HTTP 200; CERT/CC\n    returns {\"error\":\"Content requested either does not exist or\
  \ you do not have permissions to view it!\"}\n    with HTTP 200 for an unknown identifier AND for every unimplemented path. An agent must validate the\n    body. Neither API can be safely explored by probing, because a not-found is indistinguishable from\n    a not-implemented and from a not-authorized.\n- hazard: no-versioning-boundary\n  surfaces:\n  - https://api.delphi.cmu.edu/epidata\n  - https://kb.cert.org/vuls/api\n  detail: Neither API has a versioned base path or media-type version. Delphi exposes a service version\n    at /epidata/version (4.1.44 on 2026-08-19) but nothing to pin a contract to. A response shape can\n    change without a boundary an agent can detect.\n- hazard: unannounced-retirement\n  surfaces:\n  - https://api.heinz.cmu.edu/courses_api/\n  detail: CMU publishes no deprecation policy. api.heinz.cmu.edu/courses_api retired into an HTML page\n    with no Sunset header, no notice and no successor. An agent holding a cached CMU endpoint has no signal\n    that\
  \ it has stopped being an API.\noperations:\n- aid: carnegie-mellon-university:delphi-epidata\n  server: https://api.delphi.cmu.edu/epidata\n  path: /version\n  method: get\n  operationId: getVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: none\n    token: none\n    human-in-the-loop: false\n    rationale: Public, anonymous, read-only GET on an institution-operated host.\n- aid: carnegie-mellon-university:delphi-epidata\n  server: https://api.delphi.cmu.edu/epidata\n  path: /covidcast_meta/\n  method: get\n  operationId: getCovidcastMeta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: none\n    token: none\n    human-in-the-loop: false\n    rationale: Public, anonymous, read-only GET on an institution-operated host.\n- aid: carnegie-mellon-university:delphi-epidata\n  server: https://api.delphi.cmu.edu/epidata\n  path: /covidcast/\n  method: get\n  operationId: getCovidcast\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: none\n    token: none\n    human-in-the-loop: false\n    rationale: Public, anonymous, read-only GET on an institution-operated host.\n- aid: carnegie-mellon-university:delphi-epidata\n  server: https://api.delphi.cmu.edu/epidata\n  path: /fluview/\n  method: get\n  operationId: getFluview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: none\n    token: none\n    human-in-the-loop: false\n    rationale: Public, anonymous, read-only GET on an institution-operated host.\n- aid: carnegie-mellon-university:delphi-epidata\n  server: https://api.delphi.cmu.edu/epidata\n  path: /delphi/\n  method: get\n  operationId: getDelphiForecast\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: none\n    token: none\n    human-in-the-loop: false\n    rationale: Public, anonymous, read-only GET on an institution-operated host.\n- aid: carnegie-mellon-university:cert-vulnerability-notes\n\
  \  server: https://kb.cert.org\n  path: /vuls/api/{idnumber}/\n  method: get\n  operationId: getVulnerabilityNote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: none\n    token: none\n    human-in-the-loop: false\n    rationale: Public, anonymous, read-only GET on an institution-operated host.\n- aid: carnegie-mellon-university:cert-vulnerability-notes\n  server: https://kb.cert.org\n  path: /vuls/api/{idnumber}/vuls/\n  method: get\n  operationId: listNoteVulnerabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: none\n    token: none\n    human-in-the-loop: false\n    rationale: Public, anonymous, read-only GET on an institution-operated host.\n- aid: carnegie-mellon-university:cert-vulnerability-notes\n  server: https://kb.cert.org\n  path: /vuls/api/{idnumber}/vendors/\n  method: get\n  operationId: listNoteVendors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ none\n    token: none\n    human-in-the-loop: false\n    rationale: Public, anonymous, read-only GET on an institution-operated host.\n- aid: carnegie-mellon-university:cert-vulnerability-notes\n  server: https://kb.cert.org\n  path: /vuls/atomfeed/\n  method: get\n  operationId: getVulnerabilityNotesFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: none\n    token: none\n    human-in-the-loop: false\n    rationale: Public, anonymous, read-only GET on an institution-operated host.\n- aid: carnegie-mellon-university:library-publishing\n  server: https://lps.library.cmu.edu\n  path: /api/\n  method: get\n  operationId: getApiRoot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: none\n    token: none\n    human-in-the-loop: false\n    rationale: Public, anonymous, read-only GET on an institution-operated host.\n- aid: carnegie-mellon-university:library-publishing\n  server: https://lps.library.cmu.edu\n  path:\
  \ /api/journals/\n  method: get\n  operationId: listJournals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: none\n    token: none\n    human-in-the-loop: false\n    rationale: Public, anonymous, read-only GET on an institution-operated host.\n- aid: carnegie-mellon-university:library-publishing\n  server: https://lps.library.cmu.edu\n  path: /api/issues/\n  method: get\n  operationId: listIssues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: none\n    token: none\n    human-in-the-loop: false\n    rationale: Public, anonymous, read-only GET on an institution-operated host.\n- aid: carnegie-mellon-university:library-publishing\n  server: https://lps.library.cmu.edu\n  path: /api/articles/\n  method: get\n  operationId: listArticles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: none\n    token: none\n    human-in-the-loop: false\n    rationale: Public, anonymous, read-only\
  \ GET on an institution-operated host.\n- aid: carnegie-mellon-university:library-publishing\n  server: https://lps.library.cmu.edu\n  path: /api/preprints/\n  method: get\n  operationId: listPreprints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: none\n    token: none\n    human-in-the-loop: false\n    rationale: Public, anonymous, read-only GET on an institution-operated host.\n- aid: carnegie-mellon-university:library-publishing\n  server: https://lps.library.cmu.edu\n  path: /api/keywords/\n  method: get\n  operationId: listKeywords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: none\n    token: none\n    human-in-the-loop: false\n    rationale: Public, anonymous, read-only GET on an institution-operated host.\n- aid: carnegie-mellon-university:library-publishing\n  server: https://lps.library.cmu.edu\n  path: /api/oai/\n  method: get\n  operationId: oaiPmh\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: none\n    token: none\n    human-in-the-loop: false\n    rationale: Public, anonymous, read-only GET on an institution-operated host.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carnegie-mellon-university/refs/heads/main/agentic-access/carnegie-mellon-university-agentic-access.yml
summary_line: 16 operations
tags:
- University
- Higher Education
- Education
- United States
- Private Research University
- Research
- Epidemiology
- Public Health
- Cybersecurity
- Vulnerability Disclosure
- Scholarly Publishing
- Institutional Repository
- Identity Federation
- Open Access
- Open Data
---
