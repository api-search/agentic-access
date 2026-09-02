---
acting_count: 32
action_class_counts:
  acting: 32
  connected: 8
api_specs:
- filename: aider-chat-api-openapi.yml
  format: yaml
  label: Aider Chat API
  slug: aider-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aider/refs/heads/main/openapi/aider-chat-api-openapi.yml
- filename: aider-editing-api-openapi.yml
  format: yaml
  label: Aider Editing API
  slug: aider-editing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aider/refs/heads/main/openapi/aider-editing-api-openapi.yml
- filename: aider-files-api-openapi.yml
  format: yaml
  label: Aider Files API
  slug: aider-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aider/refs/heads/main/openapi/aider-files-api-openapi.yml
- filename: aider-git-api-openapi.yml
  format: yaml
  label: Aider Git API
  slug: aider-git-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aider/refs/heads/main/openapi/aider-git-api-openapi.yml
- filename: aider-io-api-openapi.yml
  format: yaml
  label: Aider IO API
  slug: aider-io-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aider/refs/heads/main/openapi/aider-io-api-openapi.yml
- filename: aider-launch-api-openapi.yml
  format: yaml
  label: Aider Launch API
  slug: aider-launch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aider/refs/heads/main/openapi/aider-launch-api-openapi.yml
- filename: aider-map-api-openapi.yml
  format: yaml
  label: Aider Map API
  slug: aider-map-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aider/refs/heads/main/openapi/aider-map-api-openapi.yml
- filename: aider-models-api-openapi.yml
  format: yaml
  label: Aider Models API
  slug: aider-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aider/refs/heads/main/openapi/aider-models-api-openapi.yml
- filename: aider-modes-api-openapi.yml
  format: yaml
  label: Aider Modes API
  slug: aider-modes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aider/refs/heads/main/openapi/aider-modes-api-openapi.yml
- filename: aider-quality-api-openapi.yml
  format: yaml
  label: Aider Quality API
  slug: aider-quality-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aider/refs/heads/main/openapi/aider-quality-api-openapi.yml
- filename: aider-session-api-openapi.yml
  format: yaml
  label: Aider Session API
  slug: aider-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aider/refs/heads/main/openapi/aider-session-api-openapi.yml
- filename: aider-settings-api-openapi.yml
  format: yaml
  label: Aider Settings API
  slug: aider-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aider/refs/heads/main/openapi/aider-settings-api-openapi.yml
- filename: aider-voice-api-openapi.yml
  format: yaml
  label: Aider Voice API
  slug: aider-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aider/refs/heads/main/openapi/aider-voice-api-openapi.yml
- filename: aider-web-api-openapi.yml
  format: yaml
  label: Aider Web API
  slug: aider-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aider/refs/heads/main/openapi/aider-web-api-openapi.yml
consequence_counts:
  read: 8
  safety-critical: 1
  write: 31
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Aider Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /commands/reset
operation_count: 40
overview: 'Aider exposes 40 API operations that an AI agent could call, of which 32 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 31 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Aider
provider_slug: aider
slug: aider-agentic-access
source_filename: aider-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/aider-cli-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 40\n  by_action_class:\n    acting: 32\n    connected: 8\n  by_consequence:\n    write: 31\n    read: 8\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /commands/add\n  method: post\n  operationId: addFiles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commands/drop\n  method: post\n  operationId: dropFiles\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commands/read-only\n  method: post\n  operationId: addReadOnlyFiles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commands/ls\n  method: get\n  operationId: listFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /commands/code\n  method: post\n  operationId: requestCodeEdit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commands/architect\n  method: post\n  operationId: architectMode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commands/ask\n  method: post\n  operationId: askQuestion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commands/chat-mode\n  method: post\n  operationId: switchChatMode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commands/diff\n  method: get\n  operationId: showDiff\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /commands/undo\n  method: post\n  operationId: undoLastCommit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commands/commit\n  method: post\n  operationId: commitChanges\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commands/git\n  method: post\n  operationId: runGitCommand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commands/model\n  method: post\n  operationId: switchMainModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commands/weak-model\n  method: post\n  operationId: switchWeakModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commands/editor-model\n  method: post\n  operationId: switchEditorModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commands/models\n  method: get\n  operationId: listAvailableModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /commands/clear\n  method: post\n  operationId: clearChatHistory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n    \
  \  triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commands/reset\n  method: post\n  operationId: resetSession\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /commands/tokens\n  method: get\n  operationId: reportTokenUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /commands/reasoning-effort\n  method: post\n  operationId: setReasoningEffort\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /commands/think-tokens\n  method: post\n  operationId: setThinkingTokens\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commands/settings\n  method: get\n  operationId: showSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /commands/map\n  method: get\n  operationId: showRepositoryMap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /commands/map-refresh\n  method: post\n  operationId: refreshRepositoryMap\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commands/run\n  method: post\n  operationId: runShellCommand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commands/test\n  method: post\n  operationId: runTestCommand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commands/lint\n  method: post\n  operationId: runLint\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commands/voice\n  method: post\n  operationId: recordVoiceInput\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commands/web\n  method: post\n  operationId: scrapeWebPage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commands/paste\n  method: post\n  operationId: pasteFromClipboard\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commands/copy\n  method: post\n  operationId: copyLastMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commands/copy-context\n  method: post\n  operationId: copyChatContext\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commands/editor\n\
  \  method: post\n  operationId: openEditorPrompt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commands/load\n  method: post\n  operationId: loadCommandScript\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commands/save\n  method: post\n  operationId: saveCommandScript\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /commands/help\n  method: get\n  operationId: getHelp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /commands/report\n  method: post\n  operationId: openGitHubIssue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /commands/exit\n  method: post\n  operationId: exitSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /launch/config\n  method: get\n  operationId: getLaunchConfig\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /launch/config\n  method: put\n  operationId: updateLaunchConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aider/refs/heads/main/agentic-access/aider-agentic-access.yml
summary_line: 40 operations · 32 acting · 1 human-in-the-loop
tags:
- Artificial Intelligence
- AI Pair Programming
- Developer Tools
- CLI
- Command Line
- Coding Assistant
- Code Generation
- Open-Source
- Python
- Apache 2.0
- LLM
- Git
- BYO LLM
- Terminal
- Polyglot
- Tree-sitter
- Repository Map
- Pair Programming
---
