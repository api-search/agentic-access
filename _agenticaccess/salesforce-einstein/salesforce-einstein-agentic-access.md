---
acting_count: 35
action_class_counts:
  acting: 35
  connected: 35
api_specs:
- filename: salesforce-einstein-ai-record-insights-api-openapi.yml
  format: yaml
  label: Salesforce Einstein AI Record Insights API
  slug: salesforce-einstein-ai-record-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-ai-record-insights-api-openapi.yml
- filename: salesforce-einstein-api-usage-api-openapi.yml
  format: yaml
  label: Salesforce Einstein API Usage API
  slug: salesforce-einstein-api-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-api-usage-api-openapi.yml
- filename: salesforce-einstein-bot-definitions-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Bot Definitions API
  slug: salesforce-einstein-bot-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-bot-definitions-api-openapi.yml
- filename: salesforce-einstein-bot-versions-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Bot Versions API
  slug: salesforce-einstein-bot-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-bot-versions-api-openapi.yml
- filename: salesforce-einstein-dashboards-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Dashboards API
  slug: salesforce-einstein-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-dashboards-api-openapi.yml
- filename: salesforce-einstein-datasets-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Datasets API
  slug: salesforce-einstein-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-datasets-api-openapi.yml
- filename: salesforce-einstein-examples-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Examples API
  slug: salesforce-einstein-examples-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-examples-api-openapi.yml
- filename: salesforce-einstein-feedback-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Feedback API
  slug: salesforce-einstein-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-feedback-api-openapi.yml
- filename: salesforce-einstein-generations-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Generations API
  slug: salesforce-einstein-generations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-generations-api-openapi.yml
- filename: salesforce-einstein-lenses-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Lenses API
  slug: salesforce-einstein-lenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-lenses-api-openapi.yml
- filename: salesforce-einstein-messages-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Messages API
  slug: salesforce-einstein-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-messages-api-openapi.yml
- filename: salesforce-einstein-models-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Models API
  slug: salesforce-einstein-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-models-api-openapi.yml
- filename: salesforce-einstein-prediction-definitions-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Prediction Definitions API
  slug: salesforce-einstein-prediction-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-prediction-definitions-api-openapi.yml
- filename: salesforce-einstein-predictions-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Predictions API
  slug: salesforce-einstein-predictions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-predictions-api-openapi.yml
- filename: salesforce-einstein-prompt-templates-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Prompt Templates API
  slug: salesforce-einstein-prompt-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-prompt-templates-api-openapi.yml
- filename: salesforce-einstein-sessions-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Sessions API
  slug: salesforce-einstein-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-sessions-api-openapi.yml
- filename: salesforce-einstein-stories-api-openapi.yml
  format: yaml
  label: Salesforce Einstein Stories API
  slug: salesforce-einstein-stories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/openapi/salesforce-einstein-stories-api-openapi.yml
consequence_counts:
  physical: 1
  read: 35
  write: 34
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Salesforce Einstein Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /einstein/bots/{botId}/sessions/{sessionId}/messages
operation_count: 70
overview: 'Salesforce Einstein exposes 70 API operations that an AI agent could call, of which 35 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 35 read, 34 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Salesforce Einstein
provider_slug: salesforce-einstein
slug: salesforce-einstein-agentic-access
source_filename: salesforce-einstein-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/salesforce-einstein-bots-openapi.yml, openapi/salesforce-einstein-discovery-openapi.yml,\n  openapi/salesforce-einstein-gpt-openapi.yml, openapi/salesforce-einstein-language-openapi.yml,\n  openapi/salesforce-einstein-prediction-builder-openapi.yml, openapi/salesforce-einstein-vision-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 70\n  by_action_class:\n    connected: 35\n    acting: 35\n  by_consequence:\n    read: 35\n    write: 34\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /einstein/bots\n  method: get\n  operationId: listBots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /einstein/bots/{botId}\n  method: get\n  operationId: getBot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /einstein/bots/{botId}/versions\n  method: get\n  operationId: listBotVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /einstein/bots/{botId}/versions/{versionId}\n  method: get\n  operationId: getBotVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /einstein/bots/{botId}/sessions\n  method: post\n  operationId: createSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /einstein/bots/{botId}/sessions/{sessionId}\n  method: get\n  operationId: getSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /einstein/bots/{botId}/sessions/{sessionId}\n  method: delete\n  operationId: endSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /einstein/bots/{botId}/sessions/{sessionId}/messages\n  method: post\n  operationId: sendMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /einstein/bots/{botId}/sessions/{sessionId}/messages\n  method: get\n  operationId: getMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wave/stories\n  method: get\n  operationId: listStories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wave/stories\n  method: post\n  operationId: createStory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wave/stories/{storyId}\n  method: get\n  operationId:\
  \ getStory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wave/stories/{storyId}\n  method: patch\n  operationId: updateStory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wave/stories/{storyId}\n  method: delete\n  operationId: deleteStory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wave/stories/{storyId}/stats\n  method: get\n  operationId: getStoryStats\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wave/models\n  method: get\n  operationId: listModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wave/models/{modelId}\n  method: get\n  operationId: getModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wave/models/{modelId}\n  method: delete\n  operationId: deleteModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wave/prediction\n  method: post\n  operationId: predict\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wave/lenses\n  method: get\n  operationId: listLenses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wave/lenses/{lensId}\n  method: get\n  operationId: getLens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wave/dashboards\n  method: get\n  operationId: listDashboards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wave/dashboards/{dashboardId}\n  method: get\n  operationId: getDashboard\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /einstein/llm/prompt/generations\n  method: post\n  operationId: generateFromPrompt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /einstein/llm/prompt/completions\n  method: post\n  operationId: completePrompt\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /einstein/llm/prompt/chat/generations\n  method: post\n  operationId: chatGeneration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /einstein/llm/prompt/templates\n  method: get\n  operationId: listPromptTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /einstein/llm/prompt/templates\n  method: post\n  operationId: createPromptTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /einstein/llm/prompt/templates/{templateId}\n  method: get\n  operationId: getPromptTemplate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /einstein/llm/prompt/templates/{templateId}\n  method: patch\n  operationId: updatePromptTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /einstein/llm/prompt/templates/{templateId}\n  method: delete\n  operationId: deletePromptTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /einstein/llm/models\n  method: get\n  operationId: listModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /einstein/llm/models/{modelId}\n  method: get\n  operationId: getModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /einstein/llm/feedback\n  method: post\n  operationId: submitFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets\n  method: get\n  operationId: listDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets\n  method: post\n  operationId: createDataset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets/{datasetId}\n  method: get\n  operationId: getDataset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets/{datasetId}\n  method: delete\n  operationId: deleteDataset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets/{datasetId}/examples\n  method: get\n  operationId: listExamples\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets/{datasetId}/examples\n  method:\
  \ post\n  operationId: addExample\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets/{datasetId}/models\n  method: get\n  operationId: listModelsForDataset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /train\n  method: post\n  operationId: trainModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /retrain\n  method: post\n  operationId: retrainModel\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /models/{modelId}\n  method: get\n  operationId: getModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models/{modelId}\n  method: delete\n  operationId: deleteModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sentiment\n  method: post\n  operationId: analyzeSentiment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /intent\n  method: post\n  operationId: detectIntent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apiusage\n  method: get\n  operationId: getApiUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /einstein/prediction-definitions\n  method: get\n  operationId: listPredictionDefinitions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /einstein/prediction-definitions\n  method: post\n  operationId: createPredictionDefinition\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /einstein/prediction-definitions/{predictionDefinitionId}\n  method: get\n  operationId: getPredictionDefinition\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /einstein/prediction-definitions/{predictionDefinitionId}\n  method: patch\n  operationId: updatePredictionDefinition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /einstein/prediction-definitions/{predictionDefinitionId}\n\
  \  method: delete\n  operationId: deletePredictionDefinition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /einstein/prediction-definitions/{predictionDefinitionId}/predictions\n  method: get\n  operationId: listPredictions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /einstein/ai-record-insights\n  method: post\n  operationId: getAIRecordInsights\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets\n  method:\
  \ get\n  operationId: listDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets\n  method: post\n  operationId: createDataset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets/{datasetId}\n  method: get\n  operationId: getDataset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets/{datasetId}\n  method: delete\n  operationId: deleteDataset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets/{datasetId}/examples\n  method: get\n  operationId: listExamples\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets/{datasetId}/examples\n  method: post\n  operationId: addExample\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /datasets/{datasetId}/models\n  method: get\n  operationId: listModelsForDataset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /train\n  method: post\n  operationId: trainModel\n  x-agentic-access:\n  \
  \  action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /retrain\n  method: post\n  operationId: retrainModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /models/{modelId}\n  method: get\n  operationId: getModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models/{modelId}\n  method: delete\n  operationId: deleteModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /models/{modelId}/lc\n  method: get\n  operationId: getModelLearningCurve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /predict\n  method: post\n  operationId: predictImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /detect\n  method: post\n  operationId: detectObjects\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /apiusage\n  method: get\n  operationId: getApiUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesforce-einstein/refs/heads/main/agentic-access/salesforce-einstein-agentic-access.yml
summary_line: 70 operations · 35 acting
tags:
- Artificial Intelligence
- Computer-Vision
- CRM
- Machine-Learning
- Natural Language Processing
- Predictive Analytics
- Salesforce
---
