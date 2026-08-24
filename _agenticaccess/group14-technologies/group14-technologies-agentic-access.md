---
acting_count: 0
action_class_counts: {}
api_specs:
- filename: group14-technologies-resources-openapi.yml
  format: yaml
  label: Group14 Technologies Resources API
  slug: group14-technologies-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/group14-technologies/refs/heads/main/openapi/group14-technologies-resources-openapi.yml
- filename: group14-technologies-content-openapi.yml
  format: yaml
  label: Group14 Technologies Content API
  slug: group14-technologies-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/group14-technologies/refs/heads/main/openapi/group14-technologies-content-openapi.yml
- filename: group14-technologies-careers-openapi.yml
  format: yaml
  label: Group14 Technologies Careers API
  slug: group14-technologies-careers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/group14-technologies/refs/heads/main/openapi/group14-technologies-careers-openapi.yml
- filename: group14-technologies-locations-openapi.yml
  format: yaml
  label: Group14 Technologies Locations API
  slug: group14-technologies-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/group14-technologies/refs/heads/main/openapi/group14-technologies-locations-openapi.yml
- filename: group14-technologies-media-openapi.yml
  format: yaml
  label: Group14 Technologies Media API
  slug: group14-technologies-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/group14-technologies/refs/heads/main/openapi/group14-technologies-media-openapi.yml
- filename: group14-technologies-search-openapi.yml
  format: yaml
  label: Group14 Technologies Search API
  slug: group14-technologies-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/group14-technologies/refs/heads/main/openapi/group14-technologies-search-openapi.yml
- filename: group14-technologies-discovery-openapi.yml
  format: yaml
  label: Group14 Technologies Discovery API
  slug: group14-technologies-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/group14-technologies/refs/heads/main/openapi/group14-technologies-discovery-openapi.yml
consequence_counts: {}
description: Recommended x-agentic-access contract for the Group14 Technologies surface. Group14 publishes no agent policy, so this is API Evangelist's classification of what an autonomous agent may safely do here — generated from the derived operations, not asserted on the provider's behalf.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Group14 Technologies Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 1
overview: 'Group14 Technologies exposes 1 API operation that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Group14 Technologies
provider_slug: group14-technologies
slug: group14-technologies-agentic-access
source_filename: group14-technologies-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: generated\nsource: openapi/ (7 specs, 31 operations) + probed access behaviour on https://group14.technology\ndescription: >-\n  Recommended x-agentic-access contract for the Group14 Technologies surface. Group14 publishes no\n  agent policy, so this is API Evangelist's classification of what an autonomous agent may safely do\n  here — generated from the derived operations, not asserted on the provider's behalf.\nposture:\n  agent_readable: true\n  agent_writable: false\n  credential_required: false\n  robots_permits_crawl: true\n  robots_evidence: 'https://group14.technology/robots.txt returns \"User-agent: * / Disallow:\" — nothing is disallowed.'\n  llms_txt_published: true\n  llms_txt_evidence: 'https://group14.technology/llms.txt (Yoast SEO v28.2 generated) — saved to llms/'\n  paid_agent_access: false\n  cloaking_observed: false\n  cloaking_note: >-\n    Anonymous curl with a default agent User-Agent and with a browser User-Agent returned\
  \ identical\n    status codes on every probed path. No agent-specific gate, challenge or differential payload was\n    observed.\ndefault_policy:\n  action_class: read\n  consequence: none\n  scope: public-content\n  token: none\n  escalation: not-possible\n  detail: >-\n    Every operation in openapi/ is an anonymous GET over published marketing content. There is no\n    action an agent can take here that spends money, sends a message, changes state, or exposes\n    personal data. The correct default is: read freely, cache for the stated 600 seconds, and never\n    attempt a write.\noperations:\n- class: read\n  consequence: none\n  reversibility: na\n  operations: [listResources, getResource, listResourceCategories, getResourceCategory, listPages, getPage, listPosts, getPost, listCategories, getCategory, listTags, getTag, listJobOpenings, getJobOpening, listJobDepartments, getJobDepartment, listJobLocations, getJobLocation, listLocations, getLocation, listMediaItems, getMediaItem, listVideos,\
  \ getVideo, listVideoCategories, getVideoCategory, listSearchResults, listContentTypes, listTaxonomies, listStatuses, getApiIndex]\n  guidance: >-\n    Safe to call unattended. Use `_fields` to request only what is needed, honour X-WP-TotalPages\n    rather than probing past the end, and pace against the 600-second cache-control window.\nforbidden:\n- surface: /wp-json/mcp/mcp-adapter-default-server\n  reason: >-\n    Registered but authentication-gated (401 rest_forbidden). Group14 publishes no credential path.\n    An agent must treat this as closed and must not retry, brute-force, or attempt to obtain\n    credentials.\n- surface: /wp-json/wp-abilities/v1/*\n  reason: Gated administration surface (401).\n- surface: /wp-json/wp/v2/users\n  reason: 'Gated (401). Author records are deliberately not exposed on this host — respect that.'\n- surface: 'every POST / PUT / PATCH / DELETE method declared on wp/v2 routes'\n  reason: >-\n    Write methods exist in the WordPress route table but\
  \ require credentials with no public issuance\n    path. They are the site's own CMS controls, not an API product. An agent must never attempt them.\nescalation:\n  path: none\n  detail: >-\n    There is no way for an agent, or the human behind it, to obtain elevated access. There is no\n    developer signup, no API key, no OAuth, and no support channel for machine access. Commercial\n    contact at https://group14.technology/contact-us/ is for battery material enquiries.\ndata_sensitivity:\n  pii: false\n  detail: >-\n    The public surface carries published marketing content, job postings and facility descriptions.\n    No customer, employee or personal data is exposed anonymously; the users route that would carry\n    author records returns 401.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/group14-technologies/refs/heads/main/agentic-access/group14-technologies-agentic-access.yml
summary_line: 1 operation
tags:
- Company
- Materials Science
- Battery Materials
- Silicon Anode
- Lithium-Ion
- Energy Storage
- Electric Vehicles
- Advanced Manufacturing
- Clean Energy
- Content
---
