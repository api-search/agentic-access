---
acting_count: 0
action_class_counts: {}
consequence_counts: {}
description: ''
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: searched
name: Group 1 Automotive Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 1
overview: 'Group 1 Automotive exposes 1 API operation that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Group 1 Automotive
provider_slug: group-1-automotive
slug: group-1-automotive-agentic-access
source_filename: group-1-automotive-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: searched\nsource: https://www.group1auto.com/llms.txt\nsummary: >-\n  Group 1 Automotive publishes a deliberate, first-party AI-agent access contract in the form of\n  an llms.txt on two of its own hosts. It is not an API program — there is no OpenAPI, no key,\n  no portal — but it is an explicit, documented, anonymous read surface built for LLM clients,\n  and it works: the endpoints it advertises return live inventory. This artifact records that\n  surface as the company actually published it.\nsurfaces:\n  - name: Group 1 Automotive inventory (corporate retail site)\n    llms_txt: https://www.group1auto.com/llms.txt\n    llms_txt_status: 200\n    llms_txt_content_type: text/plain; charset=utf-8\n    endpoint: https://www.group1auto.com/llm/inventory/\n    representation: text/html (server-rendered, no JavaScript required)\n    authentication: none\n    observed:\n      fetched: '2026-08-28'\n      result: >-\n        GET /llm/inventory/?bodytype=SUVs&limit=2\
  \ returned a server-rendered listing page titled\n        \"SUVs Vehicle Inventory - Group 1 Automotive\" reporting \"Page 1 of 13044 (26088 total\n        vehicles)\", with per-vehicle year, model, trim, new/used status, mileage, price and VIN\n        (e.g. 2026 Ford Bronco Sport, 5 miles, $40,197, VIN 3FMCR9CN8TRE54995).\n  - name: AcceleRide (Group 1 digital-retail brand)\n    llms_txt: https://www.shopgroup1.com/llms.txt\n    llms_txt_status: 200\n    llms_txt_content_type: text/plain; charset=utf-8\n    endpoint: https://www.shopgroup1.com/llm/inventory/\n    representation: text/html (server-rendered, no JavaScript required)\n    authentication: none\n    observed:\n      fetched: '2026-08-28'\n      result: >-\n        llms.txt retrieved verbatim (1,350 bytes), headed \"# AcceleRide\", advertising the same\n        /llm/inventory/ endpoint and the same parameter set on the AcceleRide host. The endpoint\n        itself was not separately fetched; only the manifest was verified on\
  \ this host.\noperations:\n  - id: browseInventory\n    method: GET\n    path: /llm/inventory/\n    action_class: read\n    consequence: none\n    reversibility: na\n    escalation: none\n    token: none\n    description: >-\n      Browse Group 1 Automotive's live new and used vehicle inventory, filtered and paginated\n      via query string. Documented in the provider's own llms.txt.\n    parameters:\n      - name: type\n        documented_values: [new, used]\n        source: llms.txt \"Parameters\" line + the \"Browse New\" / \"Browse Used\" examples\n      - name: make\n        source: llms.txt \"Parameters\" line\n      - name: model\n        source: llms.txt \"Parameters\" line\n      - name: year_min\n        source: llms.txt \"Parameters\" line + the \"Browse 2022+\" example (year_min=2022)\n      - name: year_max\n        source: llms.txt \"Parameters\" line\n      - name: price_min\n        source: llms.txt \"Parameters\" line\n      - name: price_max\n        source: llms.txt\
  \ \"Parameters\" line + the \"Under $30k\" example (price_max=30000)\n      - name: bodytype\n        documented_values: [SUVs, Trucks, Vans, Sedans]\n        source: llms.txt \"Browse SUVs/Trucks/Vans/Sedans\" example URLs\n      - name: keyword\n        source: llms.txt \"Parameters\" line + the \"white SUVs\" example (keyword=white)\n      - name: limit\n        source: llms.txt \"Parameters\" line\n      - name: page\n        source: llms.txt \"Parameters\" line; observed in the rendered pager as page=2\nagent_policy:\n  robots_txt: https://www.group1auto.com/robots.txt\n  robots_txt_status: 200\n  user_agent_rules: 'User-agent: * — no agent is named, allowed or denied specifically.'\n  crawl_delay_seconds: 1\n  disallowed_paths:\n    - /wp-admin/\n    - /wp-includes/\n    - /wp-content/uploads/inventory/\n    - /wp-content/uploads/pb_backupbuddy/\n    - /wp-content/uploads/chromeData/\n    - /wp-content/uploads/configuratorTron/\n    - /wp-content/uploads/gravity_forms/\n  llm_paths_disallowed:\
  \ false\n  note: >-\n    robots.txt does not disallow /llm/, so the advertised agent endpoint is crawlable under the\n    site's own rules. There is no ai.txt, no AIPREF signal, and no Content-Signal header. The\n    Terms of Use at https://www.group1auto.com/terms-of-use/ (effective 2026-06-29) does contain\n    an \"AI tool usage\" section, so the company's agent posture is split across two documents that\n    do not reference each other.\ndivergence:\n  finding: >-\n    The surface Group 1 advertises to agents is reachable by a browser-class client and refused\n    to a plain HTTP client. Cloudflare bot management on www.group1auto.com answered HTTP 403 to\n    every curl request for /llm/inventory/ (and for the site root, /openapi.json, /wp-json/ and\n    /sitemap.xml) even with a current desktop browser User-Agent, while the same URL fetched\n    through a browser-class path returned the full inventory listing. /llms.txt and /robots.txt\n    themselves are served to plain clients\
  \ at 200.\n  implication: >-\n    An agent that speaks plain HTTP reads the llms.txt telling it to call /llm/inventory/, then\n    gets a 403 at that endpoint. The instruction and the enforcement disagree. This is a\n    provider-side edge-policy gap, not an absence of intent — the endpoint is real and the\n    content is there.\n  evidence:\n    - url: https://www.group1auto.com/llms.txt\n      client: curl (desktop browser UA)\n      status: 200\n    - url: https://www.group1auto.com/llm/inventory/\n      client: curl (desktop browser UA)\n      status: 403\n      body: Cloudflare \"Attention Required!\" interstitial, 4,569 bytes\n    - url: https://www.group1auto.com/llm/inventory/?bodytype=SUVs&limit=2\n      client: browser-class fetch\n      status: 200\n      body: server-rendered inventory listing, 26,088 records reported\ngaps:\n  - No JSON representation. format=json is ignored; /llm/inventory.json returns the site 404.\n  - No OpenAPI, AsyncAPI, GraphQL SDL or Postman collection\
  \ describing the endpoint.\n  - No /.well-known/api-catalog pointing at the surface (all /.well-known/ paths 404).\n  - No MCP server and no A2A agent card.\n  - llms.txt does not state a rate limit, a change policy, a contact, or terms for agent use.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/group-1-automotive/refs/heads/main/agentic-access/group-1-automotive-agentic-access.yml
summary_line: 1 operation
tags:
- Fortune 500
- Automotive
- Automotive Retail
- Vehicle Inventory
- Dealerships
- Retail
- Agentic Access
- llms-txt
---
