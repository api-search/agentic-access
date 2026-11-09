---
acting_count: 253
action_class_counts:
  acting: 253
  connected: 170
consequence_counts:
  physical: 28
  read: 170
  safety-critical: 11
  write: 214
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 11
kind: agentic-access
layout: agentic-access
method: generated
name: Hostinger Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/billing/v1/subscriptions/{subscriptionId}/auto-renewal/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/dns/v1/zones/{domain}/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/domains/v1/portfolio/{domain}/domain-lock
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/domains/v1/portfolio/{domain}/privacy-protection
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/hosting/v1/accounts/{username}/websites/{domain}/cdn/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/hosting/v1/accounts/{username}/websites/{domain}/php/extensions/reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/mail/v1/api-tokens/{tokenId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/vps/v1/virtual-machines/{virtualMachineId}/docker/{projectName}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/vps/v1/virtual-machines/{virtualMachineId}/hostname
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/vps/v1/virtual-machines/{virtualMachineId}/recovery
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/vps/v1/virtual-machines/{virtualMachineId}/stop
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/agency-hosting/v1/orders/{order_id}/websites/setups
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/billing/v1/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/billing/v1/payment-methods/{paymentMethodId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/billing/v1/payment-methods/{paymentMethodId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/domains/v1/portfolio
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/domains/v1/transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/domains/v1/transfers/claim
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/ecommerce/v1/stores/{store_id}/orders/{order_id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/ecommerce/v1/stores/{store_id}/orders/{order_id}/fulfill
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/ecommerce/v1/stores/{store_id}/payment-methods/manual
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/ecommerce/v1/stores/{store_id}/payment-providers/{provider_id}/connect-link
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/ecommerce/v1/stores/{store_id}/shipping
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/hosting/v1/accounts/{username}/websites/{domain}/deploy
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/hosting/v1/accounts/{username}/websites/{domain}/git/auto-deployments/settings
operation_count: 423
overview: 'Hostinger exposes 423 API operations that an AI agent could call, of which 253 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 170 read, 214 write, 28 physical, and 11 safety-critical.


  11 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Hostinger
provider_slug: hostinger
slug: hostinger-agentic-access
source_filename: hostinger-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: generated\nsource: openapi/hostinger-agency-hosting-cache-api-openapi.yml, openapi/hostinger-agency-hosting-cron-jobs-api-openapi.yml,\n  openapi/hostinger-agency-hosting-databases-api-openapi.yml, openapi/hostinger-agency-hosting-datacenters-api-openapi.yml,\n  openapi/hostinger-agency-hosting-domains-api-openapi.yml, openapi/hostinger-agency-hosting-files-api-openapi.yml,\n  openapi/hostinger-agency-hosting-metrics-api-openapi.yml, openapi/hostinger-agency-hosting-orders-api-openapi.yml,\n  openapi/hostinger-agency-hosting-php-api-openapi.yml, openapi/hostinger-agency-hosting-ssl-api-openapi.yml,\n  openapi/hostinger-agency-hosting-website-setups-api-openapi.yml, openapi/hostinger-agency-hosting-websites-api-openapi.yml,\n  openapi/hostinger-agency-hosting-wordpress-api-openapi.yml, openapi/hostinger-agent-readiness-checks-api-openapi.yml,\n  openapi/hostinger-agent-readiness-scans-api-openapi.yml, openapi/hostinger-billing-catalog-api-openapi.yml,\n\
  \  openapi/hostinger-billing-orders-api-openapi.yml, openapi/hostinger-billing-payment-methods-api-openapi.yml,\n  openapi/hostinger-billing-subscriptions-api-openapi.yml, openapi/hostinger-dns-snapshot-api-openapi.yml,\n  openapi/hostinger-dns-zone-api-openapi.yml, openapi/hostinger-domain-access-verifier-verifications-api-openapi.yml,\n  openapi/hostinger-domains-availability-api-openapi.yml, openapi/hostinger-domains-forwarding-api-openapi.yml,\n  openapi/hostinger-domains-move-api-openapi.yml, openapi/hostinger-domains-portfolio-api-openapi.yml,\n  openapi/hostinger-domains-transfer-api-openapi.yml, openapi/hostinger-domains-whois-api-openapi.yml,\n  openapi/hostinger-ecommerce-discounts-api-openapi.yml, openapi/hostinger-ecommerce-miscellaneous-api-openapi.yml,\n  openapi/hostinger-ecommerce-orders-api-openapi.yml, openapi/hostinger-ecommerce-payments-api-openapi.yml,\n  openapi/hostinger-ecommerce-product-variants-api-openapi.yml, openapi/hostinger-ecommerce-products-api-openapi.yml,\n\
  \  openapi/hostinger-ecommerce-sales-channels-api-openapi.yml, openapi/hostinger-ecommerce-shipping-api-openapi.yml,\n  openapi/hostinger-ecommerce-stores-api-openapi.yml, openapi/hostinger-horizons-websites-api-openapi.yml,\n  openapi/hostinger-hosting-cache-api-openapi.yml, openapi/hostinger-hosting-cdn-api-openapi.yml,\n  openapi/hostinger-hosting-cron-jobs-api-openapi.yml, openapi/hostinger-hosting-databases-api-openapi.yml,\n  openapi/hostinger-hosting-datacenters-api-openapi.yml, openapi/hostinger-hosting-domains-api-openapi.yml,\n  openapi/hostinger-hosting-files-api-openapi.yml, openapi/hostinger-hosting-git-api-openapi.yml,\n  openapi/hostinger-hosting-headless-api-openapi.yml, openapi/hostinger-hosting-nodejs-api-openapi.yml,\n  openapi/hostinger-hosting-orders-api-openapi.yml, openapi/hostinger-hosting-php-api-openapi.yml,\n  openapi/hostinger-hosting-redirects-api-openapi.yml, openapi/hostinger-hosting-ssl-api-openapi.yml,\n  openapi/hostinger-hosting-websites-api-openapi.yml,\
  \ openapi/hostinger-mail-aliases-api-openapi.yml,\n  openapi/hostinger-mail-api-tokens-api-openapi.yml, openapi/hostinger-mail-autoreplies-api-openapi.yml,\n  openapi/hostinger-mail-catchalls-api-openapi.yml, openapi/hostinger-mail-forwarders-api-openapi.yml,\n  openapi/hostinger-mail-logs-api-openapi.yml, openapi/hostinger-mail-mailboxes-api-openapi.yml,\n  openapi/hostinger-mail-orders-api-openapi.yml, openapi/hostinger-mail-webhooks-api-openapi.yml,\n  openapi/hostinger-reach-automations-api-openapi.yml, openapi/hostinger-reach-campaigns-api-openapi.yml,\n  openapi/hostinger-reach-contact-fields-api-openapi.yml, openapi/hostinger-reach-contacts-api-openapi.yml,\n  openapi/hostinger-reach-forms-api-openapi.yml, openapi/hostinger-reach-profiles-api-openapi.yml,\n  openapi/hostinger-reach-segments-api-openapi.yml, openapi/hostinger-reach-tags-api-openapi.yml,\n  openapi/hostinger-reach-templates-api-openapi.yml, openapi/hostinger-vps-actions-api-openapi.yml,\n  openapi/hostinger-vps-backups-api-openapi.yml,\
  \ openapi/hostinger-vps-data-centers-api-openapi.yml,\n  openapi/hostinger-vps-docker-manager-api-openapi.yml, openapi/hostinger-vps-firewall-api-openapi.yml,\n  openapi/hostinger-vps-malware-scanner-api-openapi.yml, openapi/hostinger-vps-os-templates-api-openapi.yml,\n  openapi/hostinger-vps-post-install-scripts-api-openapi.yml, openapi/hostinger-vps-ptr-records-api-openapi.yml,\n  openapi/hostinger-vps-public-keys-api-openapi.yml, openapi/hostinger-vps-recovery-api-openapi.yml,\n  openapi/hostinger-vps-snapshots-api-openapi.yml, openapi/hostinger-vps-ssh-keys-api-openapi.yml,\n  openapi/hostinger-vps-virtual-machine-api-openapi.yml, openapi/hostinger-wordpress-ai-content-api-openapi.yml,\n  openapi/hostinger-wordpress-ai-tools-api-openapi.yml, openapi/hostinger-wordpress-installations-api-openapi.yml,\n  openapi/hostinger-wordpress-litespeed-cache-api-openapi.yml, openapi/hostinger-wordpress-login-api-openapi.yml,\n  openapi/hostinger-wordpress-maintenance-api-openapi.yml, openapi/hostinger-wordpress-object-cache-api-openapi.yml,\n\
  \  openapi/hostinger-wordpress-plugins-api-openapi.yml, openapi/hostinger-wordpress-themes-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 423\n  by_action_class:\n    acting: 253\n    connected: 170\n  by_consequence:\n    write: 214\n    read: 170\n    physical: 28\n    safety-critical: 11\n  human_in_the_loop_required: 11\noperations:\n- path: /api/agency-hosting/v1/websites/{website_uid}/cache\n  method: delete\n  operationId: agency-hosting_clearWebsiteCacheV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/agency-hosting/v1/websites/{website_uid}/cron-jobs\n  method: get\n  operationId: agency-hosting_listWebsiteCronJobsV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agency-hosting/v1/websites/{website_uid}/cron-jobs\n  method: post\n  operationId: agency-hosting_createWebsiteCronJobV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agency-hosting/v1/websites/{website_uid}/cron-jobs/{uuid}\n  method: delete\n  operationId: agency-hosting_deleteWebsiteCronJobV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n \
  \     human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agency-hosting/v1/websites/{website_uid}/databases\n  method: get\n  operationId: agency-hosting_listWebsiteDatabasesV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agency-hosting/v1/websites/{website_uid}/databases\n  method: post\n  operationId: agency-hosting_createWebsiteDatabaseV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agency-hosting/v1/websites/{website_uid}/databases/{database_name}\n  method: delete\n  operationId: agency-hosting_deleteWebsiteDatabaseV1\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agency-hosting/v1/websites/{website_uid}/databases/{database_name}/users\n  method: post\n  operationId: agency-hosting_createWebsiteDatabaseUserV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agency-hosting/v1/websites/{website_uid}/databases/{database_name}/users/{database_user_name}\n  method: delete\n  operationId: agency-hosting_deleteWebsiteDatabaseUserV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agency-hosting/v1/orders/{order_id}/datacenters\n  method: get\n  operationId: agency-hosting_listAvailableDatacentersV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agency-hosting/v1/websites/{website_uid}/domains/{from_domain}\n  method: put\n  operationId: agency-hosting_changeWebsiteDomainV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agency-hosting/v1/websites/{website_uid}/domains\n  method: post\n  operationId: agency-hosting_linkDomainToWebsiteV1\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agency-hosting/v1/domains\n  method: get\n  operationId: agency-hosting_listDomainsV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agency-hosting/v1/websites/{website_uid}/domains/{domain}\n  method: delete\n  operationId: agency-hosting_unlinkDomainFromWebsiteV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agency-hosting/v1/websites/{website_uid}/files/upload-urls\n  method: post\n\
  \  operationId: agency-hosting_generateUploadURLV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agency-hosting/v1/websites/{website_uid}/files/import-archive\n  method: post\n  operationId: agency-hosting_importWebsiteFromArchiveV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agency-hosting/v1/orders/{order_id}/disk-usage-metrics\n  method: get\n  operationId: agency-hosting_listAgencyPlanOrderDiskUsageMetricsV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agency-hosting/v1/orders/{order_id}/resource-usage-metrics\n  method: get\n  operationId: agency-hosting_listOrderResourceUsageMetricsV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agency-hosting/v1/orders\n  method: get\n  operationId: agency-hosting_listOrdersV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agency-hosting/v1/websites/{website_uid}/php-settings/extensions\n  method: get\n  operationId: agency-hosting_listPHPExtensionsForAWebsiteV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agency-hosting/v1/websites/{website_uid}/php-settings/extensions\n  method: put\n  operationId:\
  \ agency-hosting_replaceWebsitePHPExtensionsV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agency-hosting/v1/websites/{website_uid}/php-settings/options\n  method: get\n  operationId: agency-hosting_listPHPOptionsForAWebsiteV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agency-hosting/v1/websites/{website_uid}/php-settings/options\n  method: put\n  operationId: agency-hosting_replaceWebsitePHPOptionsV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/agency-hosting/v1/orders/{order_id}/websites/php-settings/versions\n  method: get\n  operationId: agency-hosting_listAvailablePHPVersionsForAnOrderV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agency-hosting/v1/websites/{website_uid}/php-settings/versions\n  method: get\n  operationId: agency-hosting_listAvailablePHPVersionsForAWebsiteV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agency-hosting/v1/websites/{website_uid}/php-settings/version\n  method: patch\n  operationId: agency-hosting_updateWebsitePHPVersionV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agency-hosting/v1/websites/{website_uid}/domains/{domain}/ssl/reinstall\n  method: post\n  operationId: agency-hosting_reinstallWebsiteSSLV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agency-hosting/v1/websites/{website_uid}/domains/{domain}/ssl/setup\n  method: post\n  operationId: agency-hosting_installWebsiteSSLV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agency-hosting/v1/websites/{website_uid}/domains/{domain}/ssl/status\n\
  \  method: get\n  operationId: agency-hosting_getWebsiteSSLStatusV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agency-hosting/v1/websites/{website_uid}/domains/{domain}/ssl\n  method: delete\n  operationId: agency-hosting_uninstallWebsiteSSLV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agency-hosting/v1/orders/{order_id}/websites/setups\n  method: post\n  operationId: agency-hosting_createANewWebsiteV1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agency-hosting/v1/orders/{order_id}/websites/setups/{setup_uuid}\n  method: get\n  operationId: agency-hosting_getWebsiteSetupStatusV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agency-hosting/v1/websites/{website_uid}/build-assets\n  method: post\n  operationId: agency-hosting_buildWebsiteNodeJSAssetsV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agency-hosting/v1/websites/{website_uid}\n  method: get\n  operationId: agency-hosting_getWebsiteDetailsV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agency-hosting/v1/websites/{website_uid}\n  method: delete\n  operationId: agency-hosting_deleteWebsiteV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agency-hosting/v1/websites\n  method: get\n  operationId: agency-hosting_listAgencyPlanWebsitesV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agency-hosting/v1/websites/{website_uid}/processes\n  method: get\n  operationId: agency-hosting_listWebsiteProcessesV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/agency-hosting/v1/websites/{website_uid}/wordpress/settings/version\n  method: patch\n  operationId: agency-hosting_changeWordPressVersionV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agency-hosting/v1/websites/{website_uid}/wordpress/settings\n  method: get\n  operationId: agency-hosting_getWordPressSettingsV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agency-hosting/v1/websites/{website_uid}/wordpress/settings/versions\n  method: get\n  operationId: agency-hosting_listAvailableWordPressVersionsV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/agent-readiness/v1/checks\n  method: get\n  operationId: agent-readiness_listChecksV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent-readiness/v1/scans\n  method: post\n  operationId: agent-readiness_runAgentReadinessScanV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agent-readiness/v1/scans/{domain}\n  method: get\n  operationId: agent-readiness_getAgentReadinessScanV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/billing/v1/catalog\n  method: get\n  operationId:\
  \ billing_getCatalogItemListV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/billing/v1/orders\n  method: post\n  operationId: billing_createPurchaseOrderV1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/billing/v1/payment-methods/{paymentMethodId}\n  method: post\n  operationId: billing_setDefaultPaymentMethodV1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/billing/v1/payment-methods/{paymentMethodId}\n  method: delete\n  operationId: billing_deletePaymentMethodV1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/billing/v1/payment-methods\n  method: get\n  operationId: billing_getPaymentMethodListV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/billing/v1/subscriptions\n  method: get\n  operationId: billing_getSubscriptionListV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/billing/v1/subscriptions/{subscriptionId}/auto-renewal/disable\n  method: delete\n  operationId: billing_disableAutoRenewalV1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/billing/v1/subscriptions/{subscriptionId}/auto-renewal/enable\n  method: patch\n  operationId: billing_enableAutoRenewalV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/billing/v1/subscriptions/{subscriptionId}/renew\n  method: post\n  operationId: billing_renewSubscriptionV1\n \
  \ x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/dns/v1/snapshots/{domain}/{snapshotId}\n  method: get\n  operationId: DNS_getDNSSnapshotV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/dns/v1/snapshots/{domain}\n  method: get\n  operationId: DNS_getDNSSnapshotListV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/dns/v1/snapshots/{domain}/{snapshotId}/restore\n  method: post\n  operationId: DNS_restoreDNSSnapshotV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/dns/v1/zones/{domain}\n  method: get\n  operationId: DNS_getDNSRecordsV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/dns/v1/zones/{domain}\n  method: put\n  operationId: DNS_updateDNSRecordsV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/dns/v1/zones/{domain}\n  method: delete\n  operationId: DNS_deleteDNSRecordsV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/dns/v1/zones/{domain}/reset\n  method: post\n  operationId: DNS_resetDNSRecordsV1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/dns/v1/zones/{domain}/validate\n  method: post\n  operationId: DNS_validateDNSRecordsV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/direct/verifications/active\n  method: get\n  operationId: v2_getDomainVerificationsDIRECT\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/domains/v1/availability/alternatives-from-description\n  method: post\n  operationId: domains_suggestDomainNamesFromADescriptionV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/domains/v1/availability/alternatives-from-domain\n  method: post\n  operationId: domains_suggestDomainNamesFromADomainV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/domains/v1/availability\n\
  \  method: post\n  operationId: domains_checkDomainAvailabilityV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/domains/v1/forwarding/{domain}\n  method: get\n  operationId: domains_getDomainForwardingV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/domains/v1/forwarding/{domain}\n  method: put\n  operationId: domains_updateDomainForwardingV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/domains/v1/forwarding/{domain}\n\
  \  method: delete\n  operationId: domains_deleteDomainForwardingV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/domains/v1/forwarding\n  method: post\n  operationId: domains_createDomainForwardingV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/domains/v1/move/incoming/{domain}\n  method: get\n  operationId: domains_getIncomingDomainMoveV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/domains/v1/move/incoming/{domain}\n\
  \  method: put\n  operationId: domains_acceptIncomingDomainMoveV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/domains/v1/move/incoming/{domain}\n  method: delete\n  operationId: domains_rejectIncomingDomainMoveV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/domains/v1/move/incoming\n  method: get\n  operationId: domains_getIncomingDomainMoveListV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/domains/v1/move/outgoing/{domain}\n\
  \  method: get\n  operationId: domains_getOutgoingDomainMoveV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/domains/v1/move/outgoing/{domain}\n  method: post\n  operationId: domains_startOutgoingDomainMoveV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/domains/v1/move/outgoing/{domain}\n  method: delete\n  operationId: domains_cancelOutgoingDomainMoveV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /api/domains/v1/move/outgoing\n  method: get\n  operationId: domains_getOutgoingDomainMoveListV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/domains/v1/portfolio/{domain}/auth-code\n  method: get\n  operationId: domains_getDomainAuthorizationCodeV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/domains/v1/portfolio/claim\n  method: post\n  operationId: domains_claimFreeDomainV1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/domains/v1/portfolio/{domain}/domain-lock\n  method: put\n  operationId: domains_enableDomainLockV1\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\n\n# --- truncated at 32 KB (145 KB total) ---\n# Full source: https://artifacts.apis.io/hostinger/agentic-access/hostinger-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/hostinger/agentic-access/hostinger-agentic-access.yml
summary_line: 423 operations · 253 acting · 11 human-in-the-loop
tags:
- Company
- Hosting
- Cloud
- Domains
---
