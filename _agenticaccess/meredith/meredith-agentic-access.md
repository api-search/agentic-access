---
acting_count: 0
action_class_counts: {}
consequence_counts: {}
description: 'People Inc has no authenticated developer API, so its "agentic access"

  contract is not an x-agentic-access block over OpenAPI operations — it is a

  DENY-AND-PRICE policy enforced at the CDN edge over the whole content

  estate. This artifact records that contract as it was actually observed on

  the wire, not as it is described in marketing.


  The headline finding: every People Inc host answers HTTP 402 Payment

  Required — with a licensing contact in the body — to a request that

  identifies itself as ClaudeBot. This is a machine-readable commercial

  signal, and it is the single clearest statement of the company''s agent

  posture anywhere on its public surface.

  '
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: probed
name: Meredith Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 0
overview: 'Dotdash Meredith / People Inc exposes 0 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Dotdash Meredith / People Inc
provider_slug: meredith
slug: meredith-agentic-access
source_filename: meredith-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live HTTP probes of people.inc and the brand estate, 2026-08-12\ndescription: |\n  People Inc has no authenticated developer API, so its \"agentic access\"\n  contract is not an x-agentic-access block over OpenAPI operations — it is a\n  DENY-AND-PRICE policy enforced at the CDN edge over the whole content\n  estate. This artifact records that contract as it was actually observed on\n  the wire, not as it is described in marketing.\n\n  The headline finding: every People Inc host answers HTTP 402 Payment\n  Required — with a licensing contact in the body — to a request that\n  identifies itself as ClaudeBot. This is a machine-readable commercial\n  signal, and it is the single clearest statement of the company's agent\n  posture anywhere on its public surface.\n\nposture:\n  stance: deny-then-license\n  enforcement: edge\n  edge_vendor: Cloudflare\n  robots_policy: comprehensive-ai-denylist\n  paid_crawl_signal: true\n  licensing_contact:\
  \ contentlicensing@people.inc\n  summary: |\n    Editorial content is closed to AI crawlers by robots.txt AND by an edge\n    rule that returns 402. Discovery metadata (robots.txt, sitemaps,\n    security.txt) stays open to everyone. Sponsored/branded content is\n    explicitly carved OUT of the AI denylist and left crawlable.\n\nobserved_responses:\n\n  - probe: HTTP GET with User-Agent \"ClaudeBot/1.0 (+https://www.anthropic.com/claude-bot)\"\n    hosts:\n      - url: https://www.people.inc/news-awards\n        status: 402\n        content_type: text/plain\n        bytes: 109\n      - url: https://people.com/\n        status: 402\n        content_type: text/plain\n        bytes: 109\n      - url: https://www.allrecipes.com/\n        status: 402\n        content_type: text/plain\n        bytes: 109\n      - url: https://www.investopedia.com/\n        status: 402\n        content_type: text/plain\n        bytes: 109\n    body: |\n      Payment Required - If you wish to license content\
  \ from People Inc, please contact contentlicensing@people.inc\n    response_headers_of_note:\n      server: cloudflare\n      cache-control: private, max-age=0, no-store, no-cache, must-revalidate\n      strict-transport-security: max-age=15552000\n    reading: |\n      402 is the correct and honest status for this: not \"you are forbidden\"\n      but \"this costs money, here is who to ask\". It is a priced boundary, and\n      an agent can act on it. Very few publishers in the catalog return 402 at\n      all; most return 403 or a soft-200 paywall shell that an agent cannot\n      distinguish from content.\n\n  - probe: HTTP GET with User-Agent \"GPTBot/1.2\"\n    hosts:\n      - url: https://www.people.inc/news-awards\n        status: 403\n        content_type: text/html\n        bytes: 680204\n    reading: |\n      DIFFERENT AGENTS GET DIFFERENT ANSWERS. GPTBot is refused with the\n      generic bot-management interstitial (403 + ~680KB of HTML), not the\n      402 licensing offer.\
  \ Only the Anthropic crawler received the priced\n      response in this probe. Whether that reflects a per-vendor rule or a\n      different rule ordering is not determinable from outside; what is\n      recorded here is the observed divergence.\n\n  - probe: HTTP GET with a desktop Chrome user-agent over curl\n    hosts:\n      - url: https://www.people.inc/news-awards\n        status: 403\n        content_type: text/html\n        bytes: 680482\n      - url: https://people.com/\n        status: 403\n        content_type: text/html\n      - url: https://people.com/feed\n        status: 403\n        content_type: text/html\n    reading: |\n      A browser user-agent is NOT sufficient. The edge fingerprints the client\n      beyond the UA string, so every non-browser client is refused on HTML\n      paths regardless of what it claims to be. This is why the RSS feed\n      endpoints recorded in apis.yml cannot be verified from a script.\n\n  - probe: allowlisted machine paths, any user-agent\
  \ including ClaudeBot\n    hosts:\n      - url: https://people.com/robots.txt\n        status: 200\n        content_type: text/plain\n      - url: https://people.com/sitemap.xml\n        status: 200\n        content_type: text/xml\n      - url: https://people.com/google-news-sitemap.xml\n        status: 200\n        content_type: text/xml\n      - url: https://people.com/.well-known/security.txt\n        status: 200\n        content_type: text/plain\n    reading: |\n      The discovery layer is deliberately left open to everyone, including the\n      crawlers the same edge charges for content. People Inc is closing the\n      corpus, not the map.\n\nrobots_policy:\n  source: https://people.com/robots.txt\n  status: 200\n  fetched: '2026-08-12'\n  user_agent_directives: 78\n  license_notice_in_comments: true\n  license_notice: |\n    People Inc. content is made available for your non-commercial use subject\n    to Terms of Use at https://www.people.inc/brands-termsofservice. Use of\n  \
  \  any crawler to data mine or scrape for any purpose other than directing\n    traffic or serving authorized advertisements is prohibited without prior\n    written permission. Prohibited uses expressly include: (1) text and data\n    mining under Art. 4 of the EU Directive on Copyright in the Digital Single\n    Market; (2) development or operation of any AI, ML, or LLM technology,\n    including training, fine-tuning, or retrieval-augmented generation; and\n    (3) creating data sets containing People Inc. content or sharing it.\n    Contact contentlicensing@people.inc.\n  legal_hooks:\n    - EU DSM Directive Art. 4 TDM reservation (machine-readable opt-out)\n    - explicit RAG prohibition\n    - explicit dataset-creation prohibition\n  fully_denied_examples:\n    - Google-Extended\n    - anthropic-ai\n    - Claude-SearchBot\n    - ClaudeBot\n    - Claude-User\n    - Claude-Web\n    - CCBot\n    - cohere-ai\n    - cohere-training-data-crawler\n    - Meta-ExternalAgent\n    - Meta-ExternalFetcher\n\
  \    - meta-webindexer\n    - PerplexityBot\n    - Perplexity-User\n    - Bytespider\n    - Applebot-Extended\n    - Amazonbot\n    - AmazonBuyForMe\n    - Amzn-SearchBot\n    - MistralAI-Index\n    - MistralAI-user\n    - DuckAssistBot\n    - Google-CloudVertexBot\n    - FirecrawlAgent\n    - ImagesiftBot\n    - Kagibot\n    - YouBot\n    - iAskBot\n    - Quora-Bot\n    - Webzio-Extended\n  partial_allow:\n    - user_agents: [GPTBot, OAI-SearchBot, ChatGPT-User]\n      rule: 'Disallow: /thmb/'\n      reading: |\n        The OpenAI crawlers are the ONE family not blanket-denied in\n        robots.txt — only the /thmb/ image-thumbnail path is disallowed.\n        People Inc has a commercial relationship with OpenAI; this asymmetry\n        is the robots.txt expression of it.\n    - user_agents: [Pinterest, Pinterestbot]\n      rule: 'Disallow: (empty value — full allow)'\n    - user_agents: [AmazonAdBot]\n      rule: 'Allow: /'\n  sponsored_content_carve_out:\n    rule: |\n      Under the\
  \ block that denies Google-Extended, anthropic-ai, CCBot,\n      Claude-SearchBot, cohere-ai, Meta-ExternalAgent, meta-webindexer and\n      PerplexityBot with \"Disallow: /\", two Allow lines reopen specific paths:\n        Allow: */presented/\n        Allow: */integrated/\n    reading: |\n      SPONSORED AND BRANDED CONTENT IS EXEMPTED FROM THE AI BLOCK. The paths\n      People Inc keeps open to the AI crawlers it otherwise denies are the\n      paths that carry advertiser-paid content. Editorial is withheld;\n      advertising is offered. This is the clearest instance of agent-facing\n      commercial asymmetry in the media segment of the catalog and it is\n      stated in the provider's own published file, not inferred.\n\ncorporate_host_policy:\n  source: https://www.people.inc/robots.txt\n  status: 200\n  fetched: '2026-08-12'\n  note: |\n    The corporate host runs a SEPARATE, differently-authored robots.txt with\n    section-header comments (\"AI TRAINING & CONTENT SCRAPING BOTS\
  \ - BLOCKED\").\n    It includes two wildcard user-agent patterns — \"User-agent: *Claude*\" and\n    \"User-agent: *AI*\" — which are NOT valid Robots Exclusion Protocol; RFC\n    9309 user-agent matching is a prefix match on a token, with no glob\n    support. Those two groups match nothing and enforce nothing. The 402 edge\n    rule is what actually holds this host closed.\n  invalid_directives:\n    - directive: 'User-agent: *Claude*'\n      reason: RFC 9309 does not support glob patterns in user-agent tokens.\n    - directive: 'User-agent: *AI*'\n      reason: RFC 9309 does not support glob patterns in user-agent tokens.\n\nconsent_signals:\n  aipref: false\n  content_signals: false\n  tdm_reservation_protocol: false\n  web_bot_auth: false\n  http_message_signatures: false\n  robots_txt_tdm_reservation: true\n  note: |\n    The TDM opt-out is asserted in robots.txt PROSE (a comment block naming\n    EU DSM Art. 4), not in any of the machine-parseable consent standards.\n    No /.well-known/\
  \ consent document, no Content-Signal header, no AIPREF\n    vocabulary. An agent must read English to learn the policy, or read a 402.\n\nagent_readiness_reading:\n  callable_surface: false\n  priced_refusal: true\n  discovery_open: true\n  summary: |\n    There is nothing here for an agent to CALL. What there is, is unusually\n    well-formed refusal: a documented denylist, a priced 402 with a named\n    counterparty, and an open discovery layer. For a publisher that is a\n    coherent posture, and it is more legible to an agent than most publishers\n    who simply return 403 or a soft-200 paywall shell.\n\nx-evidence:\n  fetched: '2026-08-12'\n  method: curl with varied User-Agent strings; no credentials used\n  user_agents_tested:\n    - ClaudeBot/1.0 (+https://www.anthropic.com/claude-bot)\n    - GPTBot/1.2\n    - Mozilla/5.0 ... Chrome/124.0 Safari/537.36\n    - curl/8.7.1\n    - Mozilla/5.0 (compatible; Googlebot/2.1; +http://www.google.com/bot.html)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meredith/refs/heads/main/agentic-access/meredith-agentic-access.yml
summary_line: 0 operations
tags:
- Media
- Publishing
- Magazines
- Content
- Advertising
- Contextual Advertising
- Lifestyle
- News
- RSS
- Sitemaps
- Robots
- AI Policy
- IAC
---
