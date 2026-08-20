---
acting_count: 0
action_class_counts:
  acting: 0
  connected: 4
api_specs:
- filename: university-of-manchester-iiif-presentation-api-openapi.yml
  format: yaml
  label: Manchester Digital Collections — IIIF Presentation API
  slug: iiif-presentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-manchester/refs/heads/main/openapi/university-of-manchester-iiif-presentation-api-openapi.yml
- filename: university-of-manchester-iiif-image-api-openapi.yml
  format: yaml
  label: Manchester Digital Collections — IIIF Image API
  slug: iiif-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-manchester/refs/heads/main/openapi/university-of-manchester-iiif-image-api-openapi.yml
consequence_counts:
  read: 4
  safety-critical: 0
  write: 0
description: 'Recommended x-agentic-access execution contracts for the surfaces the University of Manchester actually operates. Both are anonymous, read-only, cacheable public-heritage APIs — about as safe a target for autonomous agents as exists — so the governance question here is not consequence but courtesy: there is no published rate-limit table and no status page, and an agent that walks 398 canvases per manuscript across 61 manuscripts in one collection can trivially outrun a library image server.'
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: derived
name: University Of Manchester Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'University of Manchester exposes 4 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: University of Manchester
provider_slug: university-of-manchester
slug: university-of-manchester-agentic-access
source_filename: university-of-manchester-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "---\ngenerated: '2026-08-19'\nmethod: derived\nsource: >-\n  Derived from the two institution-operated contracts in openapi/ (Manchester Digital Collections\n  IIIF Presentation and Image APIs). Replaces a previous artifact that classified 951 operations\n  from Elsevier's Pure specification and is now quarantined.\nx-operator: institution\ndescription: >-\n  Recommended x-agentic-access execution contracts for the surfaces the University of Manchester\n  actually operates. Both are anonymous, read-only, cacheable public-heritage APIs — about as safe a\n  target for autonomous agents as exists — so the governance question here is not consequence but\n  courtesy: there is no published rate-limit table and no status page, and an agent that walks 398\n  canvases per manuscript across 61 manuscripts in one collection can trivially outrun a library\n  image server.\nsummary:\n  operations: 4\n  by_action_class:\n    connected: 4\n    acting: 0\n  by_consequence:\n    read: 4\n \
  \   write: 0\n    safety-critical: 0\n  human_in_the_loop_required: 0\n  authentication_required: false\noperations:\n- path: /iiif/{documentId}\n  method: get\n  operationId: getManifest\n  surface: iiif-presentation-api\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    audience: public\n    human-in-the-loop: false\n    idempotent: true\n    cacheable: true\n    notes: >-\n      Manifests are large — the verified example was 378 KB for 398 canvases. Agents should cache by\n      documentId and avoid re-fetching a manifest to reach a single canvas.\n- path: /iiif/collection/{collectionId}\n  method: get\n  operationId: getCollection\n  surface: iiif-presentation-api\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    audience: public\n    human-in-the-loop: false\n    idempotent: true\n    cacheable: true\n    notes: The correct entry point for discovery; enumerate here rather than guessing document ids.\n- path: /iiif/{identifier}/info.json\n\
  \  method: get\n  operationId: getImageInfo\n  surface: iiif-image-api\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    audience: public\n    human-in-the-loop: false\n    idempotent: true\n    cacheable: true\n- path: /iiif/{identifier}/{region}/{size}/{rotation}/{quality}.{format}\n  method: get\n  operationId: getImage\n  surface: iiif-image-api\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    audience: public\n    human-in-the-loop: false\n    idempotent: true\n    cacheable: true\n    notes: >-\n      Bounded by the server's own maxWidth/maxHeight of 2000. Prefer the pre-generated sizes listed\n      in info.json over arbitrary derivative requests; each novel region/size combination is work the\n      server has to do.\nguidance:\n  rate_limits: >-\n    None published and none observed in response headers. Treat as a shared academic resource:\n    serialize requests, honour any Retry-After, and contact the Library before bulk\
  \ harvesting.\n  reuse_terms: https://www.digitalcollections.manchester.ac.uk/terms/\n  attribution_required: >-\n    Yes. Every manifest carries an attribution string naming the University of Manchester and the\n    University of Manchester Library, and agents reproducing content must carry it through.\nexcluded:\n- surface: Elsevier Pure CRIS\n  reason: >-\n    Tenant-operated. The contract, the api-key scheme and the operation set are Elsevier's; agentic\n    governance for it belongs against Elsevier's own profile, not Manchester's.\n- surface: Shibboleth SAML Identity Provider\n  reason: >-\n    Not an agent-callable API. An assertion cannot be obtained without service-provider registration\n    in the UK Access Management Federation.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-manchester/refs/heads/main/agentic-access/university-of-manchester-agentic-access.yml
summary_line: 4 operations
tags:
- University
- Higher Education
- Education
- Research
- United Kingdom
- Russell Group
- Library
- Digital Collections
- IIIF
- Identity Federation
- Research Data
- Research Computing
---
