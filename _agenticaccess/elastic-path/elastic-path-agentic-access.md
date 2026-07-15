---
acting_count: 294
action_class_counts:
  acting: 294
  connected: 247
api_specs:
- filename: elastic-path-commerce-apis.zip
  format: yaml
  label: Elastic Path Commerce Cloud API
  slug: commerce-cloud-api
  spec_type: OpenAPI
  url: https://developer.elasticpath.com/elastic-path-commerce-apis.zip
consequence_counts:
  physical: 60
  read: 247
  safety-critical: 3
  write: 231
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Elastic Path Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /pcm/catalogs/search/stopword-sets
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /pcm/catalogs/search/stopword-sets/{stopword_set_id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /pcm/catalogs/search/stopword-sets/{stopword_set_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pcm/custom-relationships
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /pcm/custom-relationships/{customRelationshipSlug}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /pcm/custom-relationships/{customRelationshipSlug}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pcm/hierarchies/{hierarchyID}/nodes/{nodeID}/relationships/children
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /pcm/hierarchies/{hierarchyID}/nodes/{nodeID}/relationships/parent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /pcm/hierarchies/{hierarchyID}/nodes/{nodeID}/relationships/parent
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pcm/hierarchies/{hierarchyID}/nodes/{nodeID}/relationships/products
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /pcm/hierarchies/{hierarchyID}/nodes/{nodeID}/relationships/products
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pcm/hierarchies/{hierarchyID}/relationships/children
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pcm/products/{productID}/custom-relationships
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /pcm/products/{productID}/custom-relationships
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pcm/products/{productID}/custom-relationships/{customRelationshipSlug}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /pcm/products/{productID}/custom-relationships/{customRelationshipSlug}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pcm/products/{productID}/relationships/files
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /pcm/products/{productID}/relationships/files
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /pcm/products/{productID}/relationships/files
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pcm/products/{productID}/relationships/main_image
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /pcm/products/{productID}/relationships/main_image
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /pcm/products/{productID}/relationships/main_image
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pcm/products/{productID}/relationships/templates
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /pcm/products/{productID}/relationships/templates
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pcm/products/{productID}/relationships/variations
operation_count: 541
overview: 'Elastic Path exposes 541 API operations that an AI agent could call, of which 294 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 247 read, 231 write, 60 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Elastic Path
provider_slug: elastic-path
slug: elastic-path-agentic-access
source_filename: elastic-path-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/account-addresses.yaml, openapi/accounts.yaml, openapi/application-keys.yaml,\n  openapi/authentication.yaml, openapi/carts.yaml, openapi/catalog-search.yaml, openapi/catalog.yaml,\n  openapi/commerce-extensions.yaml, openapi/currencies.yaml, openapi/customer-addresses.yaml,\n  openapi/exporter.yaml, openapi/files.yaml, openapi/flows.yaml, openapi/integrations.yaml,\n  openapi/inventory-legacy.yaml, openapi/inventory.yaml, openapi/merchant-realm-mappings.yaml,\n  openapi/payments.yaml, openapi/permissions.yaml, openapi/personal-data.yaml, openapi/pim.yaml,\n  openapi/pricebooks.yaml, openapi/promotions-builder.yaml, openapi/promotions.yaml, openapi/settings.yaml,\n  openapi/single-sign-on.yaml, openapi/subscriptions.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience\
  \ per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 541\n  by_action_class:\n    acting: 294\n    connected: 247\n  by_consequence:\n    write: 231\n    read: 247\n    physical: 60\n    safety-critical: 3\n  human_in_the_loop_required: 3\noperations:\n- path: /v2/accounts/{accountID}/addresses\n  method: post\n  operationId: post-v2-account-address\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{accountID}/addresses\n  method: get\n  operationId: get-v2-account-addresses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{accountID}/addresses/{addressID}\n  method: get\n  operationId: get-v2-account-address\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{accountID}/addresses/{addressID}\n  method: put\n  operationId: put-v2-account-address\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{accountID}/addresses/{addressID}\n  method: delete\n  operationId: delete-v2-account-address\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts\n  method: post\n  operationId: post-v2-accounts\n \
  \ x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts\n  method: get\n  operationId: get-v2-accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{accountID}\n  method: get\n  operationId: get-v2-accounts-accountID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{accountID}\n  method: put\n  operationId: put-v2-accounts-accountID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{accountID}\n  method: delete\n  operationId: delete-v2-accounts-accountID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{accountID}/relationships/account-tags\n  method: get\n  operationId: GetAnAccountTagsRelationship\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{accountID}/relationships/account-tags\n  method: post\n  operationId: AddAccountTagsOnAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n \
  \     exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{accountID}/relationships/account-tags\n  method: delete\n  operationId: RemoveAccountTagsOnAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account-members\n  method: get\n  operationId: get-v2-account-members\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/account-members/{accountMemberID}\n  method: get\n  operationId: get-v2-account-members-accountMemberID\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/account-members/{accountMemberID}\n  method: put\n  operationId: put-v2-account-members-accountMemberID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{accountID}/account-memberships\n  method: post\n  operationId: post-v2-accounts-accountID-account-memberships\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{accountID}/account-memberships\n\
  \  method: get\n  operationId: get-v2-accounts-accountID-account-memberships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/account-members/{accountMemberId}/account-memberships\n  method: get\n  operationId: get-v2-account-members-accountMemberId-account-memberships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{accountID}/account-memberships/unassigned-account-members\n  method: get\n  operationId: get-v2-accounts-accountID-account-memberships-unassigned-account-members\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{accountID}/account-memberships/{membershipID}\n  method: get\n  operationId: get-v2-accounts-accountID-account-memberships-membershipID\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{accountID}/account-memberships/{membershipID}\n  method: put\n  operationId: put-v2-accounts-accountID-account-memberships-membershipID\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts/{accountID}/account-memberships/{membershipID}\n  method: delete\n  operationId: delete-v2-accounts-accountID-account-memberships-membershipID\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/settings/account-membership\n  method: get\n  operationId: get-v2-settings-account-membership\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/settings/account-membership\n  method: put\n  operationId: put-v2-settings-account-membership\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/settings/account-authentication\n  method: get\n  operationId: get-v2-settings-account-authentication\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/settings/account-authentication\n  method: put\n  operationId: put-v2-settings-account-authentication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account-members/tokens\n  method: post\n  operationId: post-v2-account-members-tokens\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account-tags\n  method: post\n  operationId: CreateAnAccountTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n  \
  \  subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account-tags\n  method: get\n  operationId: ListAccountTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/account-tags/{tag_id}\n  method: get\n  operationId: GetAnAccountTag\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/account-tags/{tag_id}\n  method: put\n  operationId: UpdateAnAccountTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v2/account-tags/{tag_id}\n  method: delete\n  operationId: DeleteAnAccountTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/application-keys\n  method: post\n  operationId: CreateAnApplicationKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/application-keys\n  method: get\n  operationId: ListApplicationKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/application-keys/{application-key-id}\n\
  \  method: get\n  operationId: GetAnApplicationKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/application-keys/{application-key-id}\n  method: put\n  operationId: UpdateAnApplicationKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/application-keys/{application-key-id}\n  method: delete\n  operationId: DeleteAnApplicationKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/access_token\n  method:\
  \ post\n  operationId: CreateAnAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/carts\n  method: get\n  operationId: getCarts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/carts\n  method: post\n  operationId: createACart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/carts/{cartID}\n  method: get\n  operationId: getACart\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/carts/{cartID}\n  method: put\n  operationId: updateACart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/carts/{cartID}\n  method: delete\n  operationId: deleteACart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/carts/{cartID}/items\n  method: get\n  operationId: getCartItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v2/carts/{cartID}/items\n  method: put\n  operationId: bulkUpdateItemsInCart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/carts/{cartID}/items\n  method: post\n  operationId: manageCarts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/carts/{cartID}/items\n  method: delete\n  operationId: deleteAllCartItems\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/carts/{cartID}/items/{cartitemID}\n  method: put\n  operationId: updateACartItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/carts/{cartID}/items/{cartitemID}\n  method: delete\n  operationId: deleteACartItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/carts/{cartID}/relationships/accounts\n  method: post\n  operationId: createAccountCartAssociation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/carts/{cartID}/relationships/accounts\n  method: delete\n  operationId: deleteAccountCartAssociation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/carts/{cartID}/relationships/customers\n  method: post\n  operationId: createCustomerCartAssociation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/carts/{cartID}/relationships/customers\n  method: delete\n  operationId: deleteCustomerCartAssociation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/carts/{cartID}/discounts/{promoCode}\n  method: delete\n  operationId: deleteAPromotionViaPromotionCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/carts/{cartID}/items/{cartitemID}/taxes\n\
  \  method: post\n  operationId: addTaxItemToCart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/carts/{cartID}/items/{cartitemID}/components/{productID}/taxes\n  method: post\n  operationId: addTaxItemToCartItemComponent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/carts/{cartID}/items/{cartitemID}/components/{productID}/taxes/{taxitemID}\n  method: put\n  operationId: updateTaxItemFromCartItemComponent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/carts/{cartID}/items/{cartitemID}/components/{productID}/taxes/{taxitemID}\n  method: delete\n  operationId: deleteTaxItemFromCartItemComponent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/carts/{cartID}/taxes\n  method: post\n  operationId: bulkAddTaxItemsToCart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/carts/{cartID}/taxes\n\
  \  method: delete\n  operationId: bulkDeleteTaxItemsFromCart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/carts/{cartID}/items/{cartitemID}/taxes/{taxitemID}\n  method: put\n  operationId: updateATaxItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/carts/{cartID}/items/{cartitemID}/taxes/{taxitemID}\n  method: delete\n  operationId: deleteATaxItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/carts/{cartID}/custom-discounts\n  method: post\n  operationId: bulkAddCustomDiscountsToCart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/carts/{cartID}/custom-discounts\n  method: delete\n  operationId: bulkDeleteCustomDiscountsFromCart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/carts/{cartID}/custom-discounts/{customdiscountID}\n  method: put\n  operationId: updateCustomDiscountForCart\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/carts/{cartID}/custom-discounts/{customdiscountID}\n  method: delete\n  operationId: deleteCustomDiscountFromCart\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/carts/{cartID}/items/{cartitemID}/custom-discounts\n  method: post\n  operationId: addCustomDiscountToCartItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/carts/{cartID}/items/{cartitemID}/custom-discounts/{customdiscountID}\n  method: put\n  operationId: updateCustomDiscountForCartItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/carts/{cartID}/items/{cartitemID}/custom-discounts/{customdiscountID}\n  method: delete\n  operationId: deleteCustomDiscountFromCartItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/carts/{cartID}/shipping-groups\n  method: get\n  operationId:\
  \ getShippingGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/carts/{cartID}/shipping-groups\n  method: post\n  operationId: createShippingGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/carts/{cartId}/shipping-groups/{shippingGroupId}\n  method: get\n  operationId: getShippingGroupById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/carts/{cartId}/shipping-groups/{shippingGroupId}\n  method: put\n  operationId: updateShippingGroup\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/carts/{cartId}/shipping-groups/{shippingGroupId}\n  method: delete\n  operationId: deleteCartShippingGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/carts/{cartID}/payments\n  method: post\n  operationId: createCartPaymentIntent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/carts/{cartID}/payments/{paymentIntentID}\n  method: put\n  operationId: updateCartPaymentIntent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/carts/{cartID}/checkout\n  method: post\n  operationId: checkoutAPI\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v2/orders\n  method: get\n  operationId: getCustomerOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/orders/{orderID}\n  method: get\n  operationId: getAnOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/orders/{orderID}\n  method: put\n  operationId: updateAnOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/orders/{orderID}/items\n  method: get\n  operationId: getOrderItems\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/orders/anonymize\n  method: post\n  operationId: anonymizeOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/orders/{orderID}/confirm\n  method: post\n  operationId: confirmOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/orders/{orderID}/payments\n  method: post\n  operationId: paymentSetup\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/orders/{orderID}/transactions/{transactionID}/confirm\n  method: post\n  operationId: confirmPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/orders/{orderID}/transactions/{transactionID}/capture\n  method: post\n  operationId: captureATransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/orders/{orderID}/transactions/{transactionID}/refund\n  method: post\n  operationId: refundATransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/orders/{orderID}/transactions\n  method: get\n  operationId: getOrderTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/orders/{orderID}/transactions/{transactionID}\n  method: get\n  operationId: getATransaction\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/orders/{orderID}/transactions/{transactionID}/cancel\n  method: post\n  operationId: cancelATransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/orders/{orderID}/shipping-groups\n  method: get\n  operationId: getOrderShippingGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/orders/{orderID}/shipping-groups\n  method: post\n  operationId: createOrderShippin\n\n# --- truncated at 32 KB (169 KB total) ---\n# Full source:\
  \ https://raw.githubusercontent.com/api-evangelist/elastic-path/refs/heads/main/agentic-access/elastic-path-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elastic-path/refs/heads/main/agentic-access/elastic-path-agentic-access.yml
summary_line: 541 operations · 294 acting · 3 human-in-the-loop
tags:
- Commerce
- Headless Commerce
- Composable Commerce
- eCommerce
- B2B
- Products
- Catalogs
- Orders
- Promotions
- Subscriptions
- Payments
---
