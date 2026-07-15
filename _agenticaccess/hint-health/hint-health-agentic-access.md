---
acting_count: 87
action_class_counts:
  acting: 87
  connected: 66
api_specs:
- filename: hint-health-hint-health-api-openapi.yml
  format: yaml
  label: Hint Health API
  slug: hint-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hint-health/refs/heads/main/openapi/hint-health-hint-health-api-openapi.yml
consequence_counts:
  physical: 35
  read: 66
  write: 52
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Hint Health Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /provider/charge_items
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /provider/charge_items/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /provider/charge_items/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /provider/charges
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /provider/companies/{company_id}/invoices/{invoice_id}/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /provider/companies/{company_id}/sponsorships
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /provider/companies/{company_id}/sponsorships/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /provider/companies/{company_id}/sponsorships/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /provider/customer_invoices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /provider/customer_invoices/{customer_invoice_id}/charges
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /provider/customer_invoices/{customer_invoice_id}/charges/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /provider/customer_invoices/{customer_invoice_id}/charges/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /provider/customer_invoices/{customer_invoice_id}/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /provider/customer_invoices/{customer_invoice_id}/pdf
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /provider/customer_invoices/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /provider/customer_invoices/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /provider/customer_invoices/{id}/issue
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /provider/customer_invoices/{id}/return_to_draft
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /provider/customer_invoices/{id}/void
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /provider/memberships
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /provider/memberships/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /provider/memberships/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /provider/memberships/{id}/bill
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /provider/memberships/{id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /provider/memberships/{id}/confirm
operation_count: 153
overview: 'Hint Health exposes 153 API operations that an AI agent could call, of which 87 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 66 read, 52 write, and 35 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Hint Health
provider_slug: hint-health
slug: hint-health-agentic-access
source_filename: hint-health-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/hint-health-hint-health-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 153\n  by_action_class:\n    acting: 87\n    connected: 66\n  by_consequence:\n    write: 52\n    read: 66\n    physical: 35\n  human_in_the_loop_required: 0\noperations:\n- path: /provider/patients/{patient_id}/account_access_tokens\n  method: post\n  operationId: AccountAccessToken.CreateAcccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/affiliates/{affiliate_id}/affiliate_bills\n\
  \  method: get\n  operationId: AffiliateBill.ListAffiliateBills\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provider/affiliates\n  method: get\n  operationId: Affiliate.ListAffiliates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provider/affiliates/{affiliate_id}/patients\n  method: post\n  operationId: AffiliatePatient.CreateAffiliatePatient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/affiliates/{affiliate_id}/patients/{id}\n  method: delete\n  operationId: AffiliatePatient.DestroyAffiliatePatient\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/patients/{patient_id}/affiliate\n  method: get\n  operationId: Affiliate.ShowPatientAffiliate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provider/cancellation_reasons\n  method: get\n  operationId: CancellationReason.ListCancellationReasons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provider/charges\n  method: post\n  operationId: Charge.CreateCharge\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n\
  \      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/charge_items\n  method: post\n  operationId: ChargeItem.CreateChargeItem\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/charge_items\n  method: get\n  operationId: ChargeItem.ListAllChargeItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provider/charge_items/{id}\n  method: delete\n  operationId: ChargeItem.DeleteChargeItem\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/charge_items/{id}\n  method: get\n  operationId: ChargeItem.ShowChargeItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provider/charge_items/{id}\n  method: patch\n  operationId: ChargeItem.UpdateChargeItem\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/patients/{patient_id}/interactions/clinical_note\n\
  \  method: post\n  operationId: ClinicalNoteInteraction.CreateClinicalNoteInteraction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/patients/{patient_id}/interactions/clinical_note/{id}\n  method: get\n  operationId: ClinicalNoteInteraction.ShowClinicalNoteInteraction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provider/patients/{patient_id}/interactions/clinical_note/{id}\n  method: patch\n  operationId: ClinicalNoteInteraction.UpdateClinicalNoteInteraction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/companies\n  method: post\n  operationId: Company.CreateCompany\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/companies\n  method: get\n  operationId: Company.ListAllCompanies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provider/companies/{id}/deactivate\n  method: post\n  operationId: Company.DeactivateCompany\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /provider/companies/{company_id}/company_plans\n  method: post\n  operationId: CompanyPlan.CreateCompanyPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/companies/{company_id}/company_plans\n  method: get\n  operationId: CompanyPlan.ListCompanyPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provider/companies/{company_id}/company_plans/{id}\n  method: delete\n  operationId: CompanyPlan.DestroyCompanyPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/companies/{company_id}/company_plans/{id}\n  method: patch\n  operationId: CompanyPlan.UpdateCompanyPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/companies/{id}\n  method: get\n  operationId: Company.ShowCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provider/companies/{id}\n  method: patch\n  operationId: Company.UpdateCompany\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/coupons\n  method: get\n  operationId: Coupon.ListAllCoupons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provider/coupons/{id}\n  method: get\n  operationId: Coupon.ShowCoupon\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provider/credit_categories\n  method: post\n  operationId: CreditCategory.CreateCreditCategory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/credit_categories\n  method: get\n\
  \  operationId: CreditCategory.ListCreditCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provider/credit_categories/{id}\n  method: delete\n  operationId: CreditCategory.DeleteCreditCategory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/credit_categories/{id}\n  method: get\n  operationId: CreditCategory.ShowCreditCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provider/credit_categories/{id}\n  method: patch\n  operationId: CreditCategory.UpdateCreditCategory\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/patients/{patient_id}/credits\n  method: post\n  operationId: Credit.CreateCredit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/patients/{patient_id}/credits\n  method: get\n  operationId: Credit.ListAllCredits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provider/credit_lines\n  method: get\n  operationId: CreditLine.ListCreditLines\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provider/patients/{patient_id}/credits/{id}\n  method: patch\n  operationId: Credit.UpdateCredit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/customer_invoices/{customer_invoice_id}/charges\n  method: post\n  operationId: CustomerInvoiceCharge.CreateCustomerInvoiceCharge\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/customer_invoices/{customer_invoice_id}/charges/{id}\n\
  \  method: delete\n  operationId: CustomerInvoiceCharge.DeleteCustomerInvoiceCharge\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/customer_invoices/{customer_invoice_id}/charges/{id}\n  method: patch\n  operationId: CustomerInvoiceCharge.UpdateCustomerInvoiceCharge\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/customer_invoices\n  method: post\n  operationId: CustomerInvoice.CreateCustomerInvoice\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/customer_invoices\n  method: get\n  operationId: CustomerInvoice.ListAllCustomerInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provider/customer_invoices/{customer_invoice_id}/pdf\n  method: post\n  operationId: CustomerInvoice.CreatePDF\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /provider/customer_invoices/{id}\n  method: delete\n  operationId: CustomerInvoice.DeleteCustomerInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/customer_invoices/{id}\n  method: get\n  operationId: CustomerInvoice.ShowCustomerInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provider/customer_invoices/{id}\n  method: patch\n  operationId: CustomerInvoice.UpdateCustomerInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/customer_invoices/{id}/issue\n  method: post\n  operationId: CustomerInvoice.IssueCustomerInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/customer_invoices/{customer_invoice_id}/payments\n  method: post\n  operationId: CustomerInvoicePayment.CreatePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/customer_invoices/{customer_invoice_id}/payments\n  method: get\n  operationId: CustomerInvoicePayment.ListAllPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provider/customer_invoices/{customer_invoice_id}/payments/{id}\n  method: get\n  operationId: CustomerInvoicePayment.ShowPayment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provider/customer_invoices/{id}/return_to_draft\n  method: post\n  operationId: CustomerInvoice.ReturnToDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/customer_invoices/{id}/void\n  method: post\n  operationId: CustomerInvoice.VoidCustomerInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/patients/{patient_id}/interactions/document\n  method: post\n  operationId: DocumentInteraction.CreateDocumentInteraction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /provider/patients/{patient_id}/interactions/document/{id}\n  method: get\n  operationId: DocumentInteraction.ShowDocumentInteraction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provider/patients/{patient_id}/interactions/document/{id}\n  method: patch\n  operationId: DocumentInteraction.UpdateDocumentInteraction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/companies/{company_id}/employee_divisions\n  method: get\n  operationId: EmployeeDivision.ListAllEmployeeDivisions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provider/patients/{patient_id}/form_responses\n\
  \  method: get\n  operationId: FormResponse.ListAllFormResponses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provider/patients/{patient_id}/form_responses/{id}\n  method: get\n  operationId: FormResponse.ShowFormResponse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /global_webhook_endpoints\n  method: post\n  operationId: GlobalWebhookEndpoint.CreateWebhookEndpointLegacy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /global_webhook_endpoints\n  method: get\n  operationId: GlobalWebhookEndpoint.WebhookEndpointsLegacy\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /global_webhook_endpoints/{id}\n  method: delete\n  operationId: GlobalWebhookEndpoint.DeleteWebhookEndpointLegacy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /global_webhook_endpoints/{id}\n  method: get\n  operationId: GlobalWebhookEndpoint.ShowWebhookEndpointLegacy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /global_webhook_endpoints/{id}\n  method: patch\n  operationId: GlobalWebhookEndpoint.UpdateWebhookEndpointLegacy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integrations/{id}/activate\n  method: post\n  operationId: Integration.ActivateIntegration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integrations/{id}/deactivate\n  method: post\n  operationId: Integration.DeactivateIntegration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /integrations\n  method: get\n  operationId: Integration.ListAllIntegrations\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provider/patients/{patient_id}/integration_records\n  method: get\n  operationId: IntegrationRecord.ListAllIntegrationRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrations/{id}\n  method: get\n  operationId: Integration.ShowIntegration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /integrations/{id}\n  method: patch\n  operationId: Integration.UpdateIntegration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /provider/interactions\n  method: get\n  operationId: Interaction.ListAllInteractions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provider/interactions/{interaction_id}/notifications\n  method: post\n  operationId: InteractionNotifications.CreateInteractionNotification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/companies/{company_id}/invoices\n  method: get\n  operationId: Invoice.ListAllInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provider/companies/{company_id}/invoices/{invoice_id}/payments\n\
  \  method: post\n  operationId: InvoicePayment.CreatePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/companies/{company_id}/invoices/{invoice_id}/payments\n  method: get\n  operationId: InvoicePayment.ListAllPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provider/companies/{company_id}/invoices/{invoice_id}/payments/{id}\n  method: get\n  operationId: InvoicePayment.ShowPayment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provider/companies/{company_id}/invoices/{id}\n\
  \  method: get\n  operationId: Invoice.ShowInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provider/patients/{patient_id}/interactions/lab\n  method: post\n  operationId: LabInteraction.CreateLabInteraction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/patients/{patient_id}/interactions/lab/{id}\n  method: get\n  operationId: LabInteraction.ShowLabInteraction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provider/patients/{patient_id}/interactions/lab/{id}\n  method: patch\n  operationId: LabInteraction.UpdateLabInteraction\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/lead_sources/{id}\n  method: delete\n  operationId: LeadSource.DeleteLeadSource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/lead_sources/{id}\n  method: patch\n  operationId: LeadSource.UpdateLeadSource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /provider/lead_sources\n  method: post\n  operationId: LeadSource.LeadSource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/lead_sources\n  method: get\n  operationId: LeadSource.LeadSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provider/locations\n  method: post\n  operationId: Location.CreateLocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/locations\n\
  \  method: get\n  operationId: Location.ListLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provider/locations/{id}\n  method: delete\n  operationId: Location.DeleteLocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/locations/{id}\n  method: get\n  operationId: Location.ShowLocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provider/locations/{id}\n  method: patch\n  operationId: Location.UpdateLocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/memberships/{id}/bill\n  method: post\n  operationId: Membership.BillMembership\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/memberships/{id}/cancel\n  method: post\n  operationId: Membership.CancelMembership\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n   \
  \   - high-value\n    audit: required\n- path: /provider/memberships/{id}/confirm\n  method: post\n  operationId: Membership.ConfirmMembership\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/memberships/{membership_id}/contracts\n  method: get\n  operationId: MembershipContract.ListAllMembershipContracts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provider/memberships/{membership_id}/contracts/renew\n  method: post\n  operationId: MembershipContract.RenewMembershipContract\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/memberships/{membership_id}/contracts/{id}\n  method: patch\n  operationId: MembershipContract.UpdateMembershipContract\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/memberships\n  method: post\n  operationId: Membership.CreateMembership\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/memberships\n  method: get\n  operationId: Membership.ListAllMemberships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /provider/memberships/{id}\n  method: delete\n  operationId: Membership.DeleteMembership\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /provider/memberships/{id}\n  method: get\n  operationId: Membership.ShowMembership\n  x-agentic-acc\n\n# --- truncated at 32 KB (49 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/hint-health/refs/heads/main/agentic-access/hint-health-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hint-health/refs/heads/main/agentic-access/hint-health-agentic-access.yml
summary_line: 153 operations · 87 acting
tags:
- Direct Primary Care
- DPC
- Healthcare
- Membership Management
- Patient Enrollment
- Medical Billing
- EMR
- Health Plans
---
