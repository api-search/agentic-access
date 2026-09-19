---
acting_count: 0
action_class_counts:
  connected: 52
api_specs:
- filename: johns-hopkins-university-classes-api-openapi.yml
  format: yaml
  label: Johns Hopkins University SIS Classes API
  slug: johns-hopkins-university-classes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/johns-hopkins-university/refs/heads/main/openapi/johns-hopkins-university-classes-api-openapi.yml
- filename: johns-hopkins-university-codes-api-openapi.yml
  format: yaml
  label: Johns Hopkins University SIS Codes API
  slug: johns-hopkins-university-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/johns-hopkins-university/refs/heads/main/openapi/johns-hopkins-university-codes-api-openapi.yml
- filename: johns-hopkins-university-content-api-openapi.yml
  format: yaml
  label: Johns Hopkins University Content API
  slug: johns-hopkins-university-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/johns-hopkins-university/refs/heads/main/openapi/johns-hopkins-university-content-api-openapi.yml
- filename: johns-hopkins-university-taxonomy-api-openapi.yml
  format: yaml
  label: Johns Hopkins University Taxonomy API
  slug: johns-hopkins-university-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/johns-hopkins-university/refs/heads/main/openapi/johns-hopkins-university-taxonomy-api-openapi.yml
consequence_counts:
  read: 52
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Johns Hopkins University Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 52
overview: 'Johns Hopkins University exposes 52 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 52 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Johns Hopkins University
provider_slug: johns-hopkins-university
slug: johns-hopkins-university-agentic-access
source_filename: johns-hopkins-university-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: generated\nsource: openapi/johns-hopkins-university-classes-api-openapi.yml, openapi/johns-hopkins-university-codes-api-openapi.yml,\n  openapi/johns-hopkins-university-content-api-openapi.yml, openapi/johns-hopkins-university-taxonomy-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 52\n  by_action_class:\n    connected: 52\n  by_consequence:\n    read: 52\n  human_in_the_loop_required: 0\noperations:\n- path: /classes/{courseNumber}\n  method: get\n  operationId: getCoursesByNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /classes/{courseNumber}/{term}\n  method: get\n  operationId:\
  \ getCoursesByNumberAndTerm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /classes/{school}/{department}/{term}\n  method: get\n  operationId: getCoursesBySchoolDepartmentTerm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /classes\n  method: get\n  operationId: advancedSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /classes/codes/schools\n  method: get\n  operationId: listSchools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /classes/codes/terms\n  method: get\n  operationId: listTerms\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /classes/codes/departments/{school}\n  method: get\n  operationId: listDepartments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /announcements\n  method: get\n  operationId: listAnnouncements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /announcements/{id}\n  method: get\n  operationId: getAnnouncement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /announcements/{id}/{subcollection}\n  method: get\n  operationId: getAnnouncementSubcollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /articles\n  method: get\n  operationId: listArticles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /articles/{id}\n  method: get\n  operationId: getArticle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /articles/{id}/{subcollection}\n  method: get\n  operationId: getArticleSubcollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{id}\n  method: get\n  operationId: getEvent\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{id}/{subcollection}\n  method: get\n  operationId: getEventSubcollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files\n  method: get\n  operationId: listFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/{id}\n  method: get\n  operationId: getFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/{id}/{subcollection}\n  method: get\n  operationId: getFileSubcollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /galleries\n  method: get\n  operationId:\
  \ listGalleries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /galleries/{id}\n  method: get\n  operationId: getGallerie\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /galleries/{id}/{subcollection}\n  method: get\n  operationId: getGallerieSubcollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people\n  method: get\n  operationId: listPeople\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people/{id}\n  method: get\n  operationId: getPeople\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /people/{id}/{subcollection}\n  method: get\n  operationId: getPeopleSubcollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /announcement_categories\n  method: get\n  operationId: listAnnouncementCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /announcement_categories/{id}\n  method: get\n  operationId: getAnnouncementCategorie\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /announcement_categories/{id}/{subcollection}\n  method: get\n  operationId: getAnnouncementCategorieSubcollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /channels\n  method: get\n  operationId: listChannels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /channels/{id}\n  method: get\n  operationId: getChannel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /channels/{id}/{subcollection}\n  method: get\n  operationId: getChannelSubcollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /divisions\n  method: get\n  operationId: listDivisions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /divisions/{id}\n  method: get\n  operationId: getDivision\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /divisions/{id}/{subcollection}\n  method: get\n  operationId: getDivisionSubcollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event_categories\n  method: get\n  operationId: listEventCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event_categories/{id}\n  method: get\n  operationId: getEventCategorie\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /event_categories/{id}/{subcollection}\n  method: get\n  operationId: getEventCategorieSubcollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /faculty_expert_affiliations\n  method: get\n  operationId: listFacultyExpertAffiliations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /faculty_expert_affiliations/{id}\n  method: get\n  operationId: getFacultyExpertAffiliation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /faculty_expert_affiliations/{id}/{subcollection}\n  method: get\n  operationId: getFacultyExpertAffiliationSubcollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /faculty_expert_topics\n  method: get\n  operationId: listFacultyExpertTopics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /faculty_expert_topics/{id}\n  method: get\n  operationId: getFacultyExpertTopic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /faculty_expert_topics/{id}/{subcollection}\n  method: get\n  operationId: getFacultyExpertTopicSubcollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locations\n  method: get\n  operationId: listLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locations/{id}\n  method: get\n  operationId: getLocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locations/{id}/{subcollection}\n\
  \  method: get\n  operationId: getLocationSubcollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tags\n  method: get\n  operationId: listTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tags/{id}\n  method: get\n  operationId: getTag\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tags/{id}/{subcollection}\n  method: get\n  operationId: getTagSubcollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /topics\n  method: get\n  operationId: listTopics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /topics/{id}\n  method: get\n  operationId: getTopic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /topics/{id}/{subcollection}\n  method: get\n  operationId: getTopicSubcollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/johns-hopkins-university/refs/heads/main/agentic-access/johns-hopkins-university-agentic-access.yml
summary_line: 52 operations
tags:
- University
- Higher Education
- Education
- United States
- Private Research University
- Association of American Universities
- Research
- Research Data
- Course Catalog
- Identity Federation
- OAI-PMH
- Research Repository
- News
---
