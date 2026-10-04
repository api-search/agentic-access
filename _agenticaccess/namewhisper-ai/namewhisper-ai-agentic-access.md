---
acting_count: 25
action_class_counts:
  acting: 25
  connected: 19
consequence_counts:
  physical: 18
  read: 19
  write: 7
description: 'Recommended x-agentic-access execution contracts for Name Whisper''s 44 MCP tools. There is no OpenAPI, so the heuristic derive-agentic-access.py could not run; instead the action-class is read from the provider''s OWN per-tool annotations (readOnlyHint / destructiveHint / idempotentHint in tools/list) and the FREE / TRANSACTION classification in /.well-known/x402 - which is why the method is searched rather than generated. consequence is API Evangelist''s reading: every non-read tool returns unsigned calldata and moves nothing until a wallet signs it, but once signed the result is an irreversible Ethereum transaction that moves names or ETH, so the tools that register, renew, buy, sell, transfer, wrap or bind identities are rated physical with human-in-the-loop required (the wallet signature IS the human step in the provider''s own design: ''Every transaction is built for the user to sign in their own wallet''). Record-, resolver-, approval- and cancel-class tools are rated
  write. TTL ceilings mirror the agentic-access Spectral ruleset. A governance starting point; audience is left null to bind per deployment. See research/curity/agentic-governance/.'
human_in_the_loop: 18
kind: agentic-access
layout: agentic-access
method: searched
name: Namewhisper Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: required
  method: ''
  path: ''
- action_class: acting
  consequence: physical
  human_in_the_loop: required
  method: ''
  path: ''
- action_class: acting
  consequence: physical
  human_in_the_loop: required
  method: ''
  path: ''
- action_class: acting
  consequence: physical
  human_in_the_loop: required
  method: ''
  path: ''
- action_class: acting
  consequence: physical
  human_in_the_loop: required
  method: ''
  path: ''
- action_class: acting
  consequence: physical
  human_in_the_loop: required
  method: ''
  path: ''
- action_class: acting
  consequence: physical
  human_in_the_loop: required
  method: ''
  path: ''
- action_class: acting
  consequence: physical
  human_in_the_loop: required
  method: ''
  path: ''
- action_class: acting
  consequence: physical
  human_in_the_loop: required
  method: ''
  path: ''
- action_class: acting
  consequence: physical
  human_in_the_loop: required
  method: ''
  path: ''
- action_class: acting
  consequence: physical
  human_in_the_loop: required
  method: ''
  path: ''
- action_class: acting
  consequence: physical
  human_in_the_loop: required
  method: ''
  path: ''
- action_class: acting
  consequence: physical
  human_in_the_loop: required
  method: ''
  path: ''
- action_class: acting
  consequence: physical
  human_in_the_loop: required
  method: ''
  path: ''
- action_class: acting
  consequence: physical
  human_in_the_loop: required
  method: ''
  path: ''
- action_class: acting
  consequence: physical
  human_in_the_loop: required
  method: ''
  path: ''
- action_class: acting
  consequence: physical
  human_in_the_loop: required
  method: ''
  path: ''
- action_class: acting
  consequence: physical
  human_in_the_loop: required
  method: ''
  path: ''
operation_count: 44
overview: 'NameWhisper exposes 44 API operations that an AI agent could call, of which 25 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read, 7 write, and 18 physical.


  18 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: NameWhisper
provider_slug: namewhisper-ai
slug: namewhisper-ai-agentic-access
source_filename: namewhisper-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://namewhisper.ai/mcp tools/list annotations (2026-09-19) + https://namewhisper.ai/.well-known/x402\n  tool classifications\ndescription: 'Recommended x-agentic-access execution contracts for Name Whisper''s 44 MCP tools. There is no OpenAPI,\n  so the heuristic derive-agentic-access.py could not run; instead the action-class is read from the provider''s\n  OWN per-tool annotations (readOnlyHint / destructiveHint / idempotentHint in tools/list) and the FREE / TRANSACTION\n  classification in /.well-known/x402 - which is why the method is searched rather than generated. consequence is\n  API Evangelist''s reading: every non-read tool returns unsigned calldata and moves nothing until a wallet signs\n  it, but once signed the result is an irreversible Ethereum transaction that moves names or ETH, so the tools that\n  register, renew, buy, sell, transfer, wrap or bind identities are rated physical with human-in-the-loop required\n\
  \  (the wallet signature IS the human step in the provider''s own design: ''Every transaction is built for the user\n  to sign in their own wallet''). Record-, resolver-, approval- and cancel-class tools are rated write. TTL ceilings\n  mirror the agentic-access Spectral ruleset. A governance starting point; audience is left null to bind per deployment.\n  See research/curity/agentic-governance/.'\naudience: null\ncustody_note: 'The provider is non-custodial: the MCP server signs nothing and holds no keys (security.txt, terms,\n  auth.md). The consequence ratings describe what the calldata does once the caller signs it.'\nsummary:\n  operations: 44\n  by_action_class:\n    connected: 19\n    acting: 25\n  by_consequence:\n    read: 19\n    write: 7\n    physical: 18\n  human_in_the_loop_required: 18\n  provider_annotations:\n    readOnlyHint_true: 19\n    destructiveHint_true: 19\n    idempotentHint_true: 9\noperations:\n- tool: search_ens_names\n  required:\n  - query\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    provider-annotations:\n      readOnlyHint: true\n      destructiveHint: false\n      idempotentHint: false\n    provider-classification: FREE\n- tool: enumerate_entities\n  required:\n  - category\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    provider-annotations:\n      readOnlyHint: true\n      destructiveHint: false\n      idempotentHint: false\n    provider-classification: FREE\n- tool: get_name_details\n  required:\n  - name\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    provider-annotations:\n      readOnlyHint: true\n      destructiveHint: false\n      idempotentHint: false\n    provider-classification: FREE\n- tool: check_availability\n  required:\n\
  \  - names\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    provider-annotations:\n      readOnlyHint: true\n      destructiveHint: false\n      idempotentHint: false\n    provider-classification: FREE\n- tool: get_similar_names\n  required:\n  - name\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    provider-annotations:\n      readOnlyHint: true\n      destructiveHint: false\n      idempotentHint: false\n    provider-classification: FREE\n- tool: get_valuation\n  required:\n  - name\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    provider-annotations:\n      readOnlyHint: true\n      destructiveHint: false\n      idempotentHint: false\n    provider-classification: FREE\n- tool: get_market_activity\n\
  \  required: []\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    provider-annotations:\n      readOnlyHint: true\n      destructiveHint: false\n      idempotentHint: false\n    provider-classification: FREE\n- tool: get_expiring_names\n  required: []\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    provider-annotations:\n      readOnlyHint: true\n      destructiveHint: false\n      idempotentHint: false\n    provider-classification: FREE\n- tool: wash_check\n  required: []\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    provider-annotations:\n      readOnlyHint: true\n      destructiveHint: false\n      idempotentHint: false\n    provider-classification: FREE\n- tool: get_wallet_portfolio\n\
  \  required:\n  - wallet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    provider-annotations:\n      readOnlyHint: true\n      destructiveHint: false\n      idempotentHint: false\n    provider-classification: FREE\n- tool: find_alpha\n  required: []\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    provider-annotations:\n      readOnlyHint: true\n      destructiveHint: false\n      idempotentHint: false\n    provider-classification: FREE\n- tool: get_primary_name\n  required:\n  - walletAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    provider-annotations:\n      readOnlyHint: true\n      destructiveHint: false\n      idempotentHint: false\n    provider-classification: FREE\n\
  - tool: provision_agent_identity\n  required:\n  - purpose\n  - walletAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    provider-annotations:\n      readOnlyHint: true\n      destructiveHint: false\n      idempotentHint: false\n    provider-classification: FREE\n- tool: make_offer\n  required:\n  - name\n  - amountEth\n  - walletAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    token:\n      max-ttl: 300\n    audit: required\n    escalation:\n    - purpose-required\n    - human-in-the-loop\n    human-in-the-loop: required\n    provider-annotations:\n      readOnlyHint: false\n      destructiveHint: false\n      idempotentHint: false\n    provider-classification: TRANSACTION\n- tool: purchase_name\n  required:\n  - name\n  - walletAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    token:\n      max-ttl: 300\n    audit: required\n    escalation:\n    - purpose-required\n    - human-in-the-loop\n    human-in-the-loop: required\n    provider-annotations:\n      readOnlyHint: false\n      destructiveHint: true\n      idempotentHint: false\n    provider-classification: TRANSACTION\n- tool: bulk_register\n  required:\n  - names\n  - walletAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    token:\n      max-ttl: 300\n    audit: required\n    escalation:\n    - purpose-required\n    - human-in-the-loop\n    human-in-the-loop: required\n    provider-annotations:\n      readOnlyHint: false\n      destructiveHint: true\n      idempotentHint: false\n    provider-classification: TRANSACTION\n- tool: create_listing\n  required:\n  - name\n  - priceEth\n  - walletAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    token:\n      max-ttl: 300\n   \
  \ audit: required\n    escalation:\n    - purpose-required\n    - human-in-the-loop\n    human-in-the-loop: required\n    provider-annotations:\n      readOnlyHint: false\n      destructiveHint: false\n      idempotentHint: false\n    provider-classification: TRANSACTION\n- tool: cancel_listing\n  required:\n  - orderHash\n  - walletAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    token:\n      max-ttl: 900\n    audit: required\n    provider-annotations:\n      readOnlyHint: false\n      destructiveHint: true\n      idempotentHint: true\n    provider-classification: TRANSACTION\n- tool: cancel_offer\n  required:\n  - orderHash\n  - walletAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    token:\n      max-ttl: 900\n    audit: required\n    provider-annotations:\n      readOnlyHint: false\n      destructiveHint: true\n      idempotentHint: true\n    provider-classification:\
  \ TRANSACTION\n- tool: accept_offer\n  required:\n  - orderHash\n  - walletAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    token:\n      max-ttl: 300\n    audit: required\n    escalation:\n    - purpose-required\n    - human-in-the-loop\n    human-in-the-loop: required\n    provider-annotations:\n      readOnlyHint: false\n      destructiveHint: true\n      idempotentHint: false\n    provider-classification: TRANSACTION\n- tool: batch_purchase\n  required:\n  - names\n  - walletAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    token:\n      max-ttl: 300\n    audit: required\n    escalation:\n    - purpose-required\n    - human-in-the-loop\n    human-in-the-loop: required\n    provider-annotations:\n      readOnlyHint: false\n      destructiveHint: true\n      idempotentHint: false\n    provider-classification: TRANSACTION\n- tool: sweep\n  required:\n  - walletAddress\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    token:\n      max-ttl: 300\n    audit: required\n    escalation:\n    - purpose-required\n    - human-in-the-loop\n    human-in-the-loop: required\n    provider-annotations:\n      readOnlyHint: false\n      destructiveHint: true\n      idempotentHint: false\n    provider-classification: TRANSACTION\n- tool: batch_create_listings\n  required:\n  - listings\n  - walletAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    token:\n      max-ttl: 300\n    audit: required\n    escalation:\n    - purpose-required\n    - human-in-the-loop\n    human-in-the-loop: required\n    provider-annotations:\n      readOnlyHint: false\n      destructiveHint: false\n      idempotentHint: false\n    provider-classification: TRANSACTION\n- tool: renew_ens_name\n  required:\n  - names\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    token:\n      max-ttl: 300\n    audit: required\n    escalation:\n    - purpose-required\n    - human-in-the-loop\n    human-in-the-loop: required\n    provider-annotations:\n      readOnlyHint: false\n      destructiveHint: true\n      idempotentHint: false\n    provider-classification: TRANSACTION\n- tool: transfer_ens_name\n  required:\n  - name\n  - fromAddress\n  - toAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    token:\n      max-ttl: 300\n    audit: required\n    escalation:\n    - purpose-required\n    - human-in-the-loop\n    human-in-the-loop: required\n    provider-annotations:\n      readOnlyHint: false\n      destructiveHint: true\n      idempotentHint: false\n    provider-classification: TRANSACTION\n- tool: set_ens_records\n  required:\n  - name\n  - records\n  - walletAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    token:\n\
  \      max-ttl: 900\n    audit: required\n    provider-annotations:\n      readOnlyHint: false\n      destructiveHint: true\n      idempotentHint: true\n    provider-classification: TRANSACTION\n- tool: bulk_set_records\n  required:\n  - nameRecords\n  - walletAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    token:\n      max-ttl: 900\n    audit: required\n    provider-annotations:\n      readOnlyHint: false\n      destructiveHint: true\n      idempotentHint: true\n    provider-classification: TRANSACTION\n- tool: bulk_transfer_ens_names\n  required:\n  - transfers\n  - fromAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    token:\n      max-ttl: 300\n    audit: required\n    escalation:\n    - purpose-required\n    - human-in-the-loop\n    human-in-the-loop: required\n    provider-annotations:\n      readOnlyHint: false\n      destructiveHint: true\n      idempotentHint:\
  \ false\n    provider-classification: TRANSACTION\n- tool: set_primary_name\n  required:\n  - name\n  - walletAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    token:\n      max-ttl: 900\n    audit: required\n    provider-annotations:\n      readOnlyHint: false\n      destructiveHint: true\n      idempotentHint: true\n    provider-classification: TRANSACTION\n- tool: set_resolver\n  required:\n  - name\n  - resolver\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    token:\n      max-ttl: 900\n    audit: required\n    provider-annotations:\n      readOnlyHint: false\n      destructiveHint: true\n      idempotentHint: true\n    provider-classification: TRANSACTION\n- tool: manage_ens_name\n  required:\n  - name\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    provider-annotations:\n\
  \      readOnlyHint: true\n      destructiveHint: false\n      idempotentHint: false\n    provider-classification: FREE\n- tool: wrap_name\n  required:\n  - name\n  - owner\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    token:\n      max-ttl: 300\n    audit: required\n    escalation:\n    - purpose-required\n    - human-in-the-loop\n    human-in-the-loop: required\n    provider-annotations:\n      readOnlyHint: false\n      destructiveHint: true\n      idempotentHint: false\n    provider-classification: TRANSACTION\n- tool: unwrap_name\n  required:\n  - name\n  - owner\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    token:\n      max-ttl: 300\n    audit: required\n    escalation:\n    - purpose-required\n    - human-in-the-loop\n    human-in-the-loop: required\n    provider-annotations:\n      readOnlyHint: false\n      destructiveHint: true\n      idempotentHint: false\n    provider-classification:\
  \ TRANSACTION\n- tool: manage_fuses\n  required:\n  - name\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    token:\n      max-ttl: 300\n    audit: required\n    escalation:\n    - purpose-required\n    - human-in-the-loop\n    human-in-the-loop: required\n    provider-annotations:\n      readOnlyHint: false\n      destructiveHint: true\n      idempotentHint: true\n    provider-classification: TRANSACTION\n- tool: mint_subnames\n  required:\n  - parentName\n  - subnames\n  - walletAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    token:\n      max-ttl: 300\n    audit: required\n    escalation:\n    - purpose-required\n    - human-in-the-loop\n    human-in-the-loop: required\n    provider-annotations:\n      readOnlyHint: false\n      destructiveHint: false\n      idempotentHint: false\n    provider-classification: TRANSACTION\n- tool: extend_subname_expiry\n  required:\n  - name\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    token:\n      max-ttl: 300\n    audit: required\n    escalation:\n    - purpose-required\n    - human-in-the-loop\n    human-in-the-loop: required\n    provider-annotations:\n      readOnlyHint: false\n      destructiveHint: false\n      idempotentHint: false\n    provider-classification: TRANSACTION\n- tool: approve_operator\n  required:\n  - owner\n  - operator\n  - contract\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    token:\n      max-ttl: 300\n    audit: required\n    escalation:\n    - purpose-required\n    - human-in-the-loop\n    human-in-the-loop: required\n    provider-annotations:\n      readOnlyHint: false\n      destructiveHint: true\n      idempotentHint: true\n    provider-classification: TRANSACTION\n- tool: reclaim_name\n  required:\n  - name\n  - owner\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    token:\n      max-ttl: 900\n    audit: required\n    provider-annotations:\n      readOnlyHint: false\n      destructiveHint: true\n      idempotentHint: true\n    provider-classification: TRANSACTION\n- tool: register_agent\n  required:\n  - name\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    token:\n      max-ttl: 300\n    audit: required\n    escalation:\n    - purpose-required\n    - human-in-the-loop\n    human-in-the-loop: required\n    provider-annotations:\n      readOnlyHint: false\n      destructiveHint: false\n      idempotentHint: false\n    provider-classification: TRANSACTION\n- tool: get_agent_reputation\n  required:\n  - nameOrWallet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    provider-annotations:\n      readOnlyHint: true\n      destructiveHint: false\n      idempotentHint:\
  \ false\n    provider-classification: FREE\n- tool: search_agent_directory\n  required: []\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    provider-annotations:\n      readOnlyHint: true\n      destructiveHint: false\n      idempotentHint: false\n    provider-classification: FREE\n- tool: get_caller_identity\n  required: []\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    provider-annotations:\n      readOnlyHint: true\n      destructiveHint: false\n      idempotentHint: false\n    provider-classification: FREE\n- tool: search_knowledge\n  required:\n  - query\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    provider-annotations:\n      readOnlyHint: true\n      destructiveHint: false\n\
  \      idempotentHint: false\n    provider-classification: FREE\n- tool: get_usage_stats\n  required: []\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    provider-annotations:\n      readOnlyHint: true\n      destructiveHint: false\n      idempotentHint: false\n    provider-classification: FREE\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/namewhisper-ai/refs/heads/main/agentic-access/namewhisper-ai-agentic-access.yml
summary_line: 44 operations · 25 acting · 18 human-in-the-loop
tags:
- ENS
- Ethereum
- Web3
- Domain Names
- AI Agents
- MCP
- A2A
- Valuation
- NFT Marketplace
- Agent Identity
- Blockchain
---
