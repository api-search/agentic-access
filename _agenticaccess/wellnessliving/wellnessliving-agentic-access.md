---
acting_count: 16
action_class_counts:
  acting: 16
  connected: 39
api_specs:
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Clients API
  slug: clients
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Classes & Schedules API
  slug: classes-schedule
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Appointments API
  slug: appointments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Booking Wizard API
  slug: booking-wizard
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Memberships & Passes API
  slug: memberships-passes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Staff API
  slug: staff
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Locations API
  slug: locations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Business API
  slug: business
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Sales & Catalog API
  slug: sales-catalog
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Payments API
  slug: payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Authentication API
  slug: authentication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Rewards & Loyalty API
  slug: rewards-loyalty
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Reviews API
  slug: reviews
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Reports API
  slug: reports
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
- filename: wellnessliving-openapi.yml
  format: yaml
  label: WellnessLiving Real-Time Notifications API
  slug: realtime-notifications
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/openapi/wellnessliving-openapi.yml
consequence_counts:
  physical: 2
  read: 39
  safety-critical: 1
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Wellnessliving Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /Thoth/WlPay/Account/Charge/Charge.json
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /Wl/Book/Process/Payment/Payment.json
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /Wl/Catalog/Payment/Payment.json
operation_count: 55
overview: 'WellnessLiving exposes 55 API operations that an AI agent could call, of which 16 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 39 read, 13 write, 2 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: WellnessLiving
provider_slug: wellnessliving
slug: wellnessliving-agentic-access
source_filename: wellnessliving-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/wellnessliving-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 55\n  by_action_class:\n    connected: 39\n    acting: 16\n  by_consequence:\n    read: 39\n    write: 13\n    physical: 2\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /Wl/Member/Info/Info.json\n  method: get\n  operationId: get_Wl_Member_Info_Info\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Wl/Profile/Purchase/PurchaseList.json\n  method: get\n  operationId: get_Wl_Profile_Purchase_PurchaseList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Wl/Profile/ProfileCreate.json\n  method: post\n  operationId: post_Wl_Profile_ProfileCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Wl/Family/Relation/FamilyRelation.json\n  method: get\n  operationId: get_Wl_Family_Relation_FamilyRelation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Wl/Classes/ClassList/List.json\n  method: get\n  operationId: get_Wl_Classes_ClassList_List\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Wl/Classes/ClassView/Element.json\n\
  \  method: get\n  operationId: get_Wl_Classes_ClassView_Element\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Wl/Schedule/ClassList/ClassList.json\n  method: get\n  operationId: get_Wl_Schedule_ClassList_ClassList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Wl/Schedule/Cancel.json\n  method: post\n  operationId: post_Wl_Schedule_Cancel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Wl/Appointment/Info/Info.json\n  method: get\n  operationId: get_Wl_Appointment_Info_Info\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Wl/Appointment/Book/Schedule/Calendar.json\n  method: get\n  operationId: get_Wl_Appointment_Book_Schedule_Calendar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Wl/Appointment/Book/Staff/List.json\n  method: get\n  operationId: get_Wl_Appointment_Book_Staff_List\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Wl/Appointment/Book/Finish/FinishMultiple.json\n  method: post\n  operationId: post_Wl_Appointment_Book_Finish_FinishMultiple\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /Wl/Book/Process/Process.json\n  method: get\n  operationId: get_Wl_Book_Process_Process\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Wl/Book/Process/Payment/Payment.json\n  method: post\n  operationId: post_Wl_Book_Process_Payment_Payment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Wl/Book/Process/Purchase/Purchase.json\n  method: get\n  operationId: get_Wl_Book_Process_Purchase_Purchase\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Wl/Book/Cancel/CancelCan.json\n\
  \  method: get\n  operationId: get_Wl_Book_Cancel_CancelCan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Wl/Promotion/Index/PromotionIndex.json\n  method: get\n  operationId: get_Wl_Promotion_Index_PromotionIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Wl/Promotion/PromotionList.json\n  method: get\n  operationId: get_Wl_Promotion_PromotionList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Wl/Promotion/Promotion.json\n  method: post\n  operationId: post_Wl_Promotion_Promotion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Wl/Login/Promotion/GuestPass/GuestPassList.json\n  method: get\n  operationId: get_Wl_Login_Promotion_GuestPass_GuestPassList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Wl/Staff/StaffList/StaffList.json\n  method: get\n  operationId: get_Wl_Staff_StaffList_StaffList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Wl/Staff/StaffView/StaffView.json\n  method: get\n  operationId: get_Wl_Staff_StaffView_StaffView\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Wl/Staff/StaffElement.json\n  method: post\n  operationId: post_Wl_Staff_StaffElement\n  x-agentic-access:\n \
  \   action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Wl/Staff/Privilege/PrivilegeList.json\n  method: get\n  operationId: get_Wl_Staff_Privilege_PrivilegeList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Wl/Location/List.json\n  method: get\n  operationId: get_Wl_Location_List\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Wl/Location/View/View.json\n  method: get\n  operationId: get_Wl_Location_View_View\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Wl/Location/Location.json\n\
  \  method: post\n  operationId: post_Wl_Location_Location\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Wl/Location/WorkTime/LocationWorkTime.json\n  method: post\n  operationId: post_Wl_Location_WorkTime_LocationWorkTime\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Wl/Business/Data.json\n  method: get\n  operationId: get_Wl_Business_Data\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Wl/Business/Config/BusinessConfig.json\n\
  \  method: get\n  operationId: get_Wl_Business_Config_BusinessConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Wl/Business/Account/Subscription/SubscriptionInfo.json\n  method: get\n  operationId: get_Wl_Business_Account_Subscription_SubscriptionInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Wl/Business/Business.json\n  method: post\n  operationId: post_Wl_Business_Business\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Wl/Catalog/CatalogList/List.json\n  method: get\n  operationId: get_Wl_Catalog_CatalogList_List\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Wl/Catalog/Cart/Cart.json\n  method: get\n  operationId: get_Wl_Catalog_Cart_Cart\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Wl/Catalog/Payment/Payment.json\n  method: post\n  operationId: post_Wl_Catalog_Payment_Payment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Wl/Purchase/Receipt/PurchaseReceipt.json\n  method: get\n  operationId: get_Wl_Purchase_Receipt_PurchaseReceipt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Thoth/WlPay/Account/Account.json\n  method: get\n  operationId: get_Thoth_WlPay_Account_Account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Thoth/WlPay/Bank/Card/List.json\n  method: get\n  operationId: get_Thoth_WlPay_Bank_Card_List\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Thoth/WlPay/Account/Charge/Charge.json\n  method: post\n  operationId: post_Thoth_WlPay_Account_Charge_Charge\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n\
  - path: /Thoth/WlPay/Transaction/Report/TransactionAllPayment.json\n  method: get\n  operationId: get_Thoth_WlPay_Transaction_Report_TransactionAllPayment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Core/Passport/Login/Enter/Enter.json\n  method: post\n  operationId: post_Core_Passport_Login_Enter_Enter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Core/Passport/Enter/Jwt/JwtToken.json\n  method: get\n  operationId: get_Core_Passport_Enter_Jwt_JwtToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Core/Passport/Login/SignOut/SignOut.json\n\
  \  method: post\n  operationId: post_Core_Passport_Login_SignOut_SignOut\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Wl/Login/Login.json\n  method: get\n  operationId: get_Wl_Login_Login\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Wl/Reward/Score/Current/Current.json\n  method: get\n  operationId: get_Wl_Reward_Score_Current_Current\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Wl/Reward/Prize/Prize.json\n  method: get\n  operationId: get_Wl_Reward_Prize_Prize\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Wl/Reward/Action/Action.json\n  method: get\n  operationId: get_Wl_Reward_Action_Action\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Wl/Reward/Board/List.json\n  method: get\n  operationId: get_Wl_Reward_Board_List\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Wl/Review/Review.json\n  method: post\n  operationId: post_Wl_Review_Review\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Wl/Review/ReviewList/ReviewList.json\n  method: get\n  operationId: get_Wl_Review_ReviewList_ReviewList\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Wl/Review/ReviewReply.json\n  method: post\n  operationId: post_Wl_Review_ReviewReply\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Wl/Report/Data.json\n  method: get\n  operationId: get_Wl_Report_Data\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Wl/Report/PageData.json\n  method: get\n  operationId: get_Wl_Report_PageData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Wl/Report/Access.json\n\
  \  method: get\n  operationId: get_Wl_Report_Access\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Core/WebSocket/Subscribe.json\n  method: post\n  operationId: post_Core_WebSocket_Subscribe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wellnessliving/refs/heads/main/agentic-access/wellnessliving-agentic-access.yml
summary_line: 55 operations · 16 acting · 1 human-in-the-loop
tags:
- Fitness
- Wellness
- Spa
- Business Management
- Scheduling
- Memberships
- Point of Sale
---
