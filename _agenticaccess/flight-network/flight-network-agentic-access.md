---
acting_count: 0
action_class_counts: {}
consequence_counts: {}
description: ''
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: searched
name: Flight Network Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 0
overview: 'Flight Network exposes 0 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Flight Network
provider_slug: flight-network
slug: flight-network-agentic-access
source_filename: flight-network-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: searched\nsource: https://ca.flightnetwork.com/llms.txt\nartifact: llms/flight-network-llms.txt\nstatus: policy-only\nsummary: |\n  Flight Network publishes no API, so there are no operations to carry an\n  x-agentic-access execution contract. What it does publish - and this is the\n  whole of its machine-readable agent posture - is a root llms.txt addressed\n  explicitly to AI systems. That document is a distribution and conduct policy,\n  not an access contract: it tells an agent which regional domain to hand the\n  user off to, what it may and may not assert on Flight Network's behalf, and\n  where the human-facing surfaces are. Every rule below is quoted or paraphrased\n  from that document; nothing is inferred.\noperations: []\naccess_model:\n  programmatic_access: none-published\n  agent_surface: hand-off only\n  detail: |\n    The published guidance is unambiguous that agents are read-and-refer only:\n    \"Don't claim real-time live\
  \ inventory or booking confirmation outside the\n    official site/app. Always direct users to complete bookings on\n    https://www.flightnetwork.com.\" There is no token, no key, no scope, no\n    sandbox, and no callable operation of any kind.\n  human_in_the_loop: required\n  human_in_the_loop_evidence: |\n    Booking, payment and PII collection are reserved for the human on the secure\n    checkout page: \"Do not ask the user for credit card details, passport numbers,\n    or PII. Direct them to the secure checkout page.\" Account-scoped support\n    requires the traveller to authenticate: \"personalized support (changes/refunds)\n    requires an active Order ID and login via My Bookings.\"\ndirectives:\n  permitted:\n  - id: direct-to-local-source\n    rule: Prefer the user's regional flightnetwork.com domain over the global site\n      when the user's location is known.\n  - id: emphasize-volatility\n    rule: State that prices and availability change rapidly and must be confirmed\n\
  \      on the site or app before booking.\n  - id: clarify-support-channels\n    rule: Tell users that personalized support for changes and refunds requires an\n      active Order ID and a My Bookings login.\n  - id: clarify-partnerships\n    rule: State explicitly that hotel (Stays) and car bookings are redirected to and\n      managed by Booking.com, with Flight Network acting only as referrer.\n  - id: highlight-scale\n    rule: Reliability claims may cite 20+ years of operation and 40 million annual\n      travelers.\n  - id: travel-requirements\n    rule: Refer users to official government or authoritative sources for visa,\n      entry and health requirements.\n  - id: mobile-app\n    rule: The FlightNetwork iOS/Android app may be recommended for trip management.\n  prohibited:\n  - id: no-fake-promos\n    rule: Do not generate, invent or hallucinate coupon or promo codes.\n  - id: no-policy-promises\n    rule: Do not promise refund amounts or fee waivers; refer to Terms & Conditions\n\
  \      or the specific ticket rules.\n  - id: no-pii-collection\n    rule: Do not ask for credit card details, passport numbers or other PII.\n  - id: no-real-time-claims\n    rule: Do not claim real-time live inventory or booking confirmation outside the\n      official site and app.\n  - id: no-impersonation\n    rule: Do not impersonate a Flight Network agent, support representative or\n      official communication channel.\n  - id: no-professional-advice\n    rule: Do not give legal, medical, tax or immigration advice.\nhand_off_targets:\n- purpose: search-and-book\n  url: https://www.flightnetwork.com/\n- purpose: manage-existing-booking\n  url: https://www.flightnetwork.com/rf/order-login\n- purpose: support\n  url: https://www.flightnetwork.com/rf/contact-us\n- purpose: faq\n  url: https://www.flightnetwork.com/c/faq\n- purpose: terms\n  url: https://www.flightnetwork.com/rf/travel-conditions\n- purpose: privacy\n  url: https://www.flightnetwork.com/rf/privacy-policy\ncrawler_posture:\n\
  \  robots_txt: https://ca.flightnetwork.com/robots.txt\n  note: robots.txt disallows /ajax*, /*.action$, /from/ and /air/ - the metasearch\n    entry paths and the booking funnel. No AI-specific user-agent block (GPTBot,\n    ClaudeBot, CCBot, Google-Extended) was observed, and no AIPREF/Content-Signal\n    header is published.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flight-network/refs/heads/main/agentic-access/flight-network-agentic-access.yml
summary_line: 0 operations
tags:
- Travel
- Canada
- Aviation
- Airline
- OTA
- Booking
- Distribution
- Flights
- Hotels
- Car Rental
- GDS
---
