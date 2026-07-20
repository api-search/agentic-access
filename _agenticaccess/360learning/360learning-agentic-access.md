---
acting_count: 104
action_class_counts:
  acting: 104
  connected: 60
api_specs:
- filename: 360learning-core-api.json
  format: json
  label: 360Learning Core API v2
  slug: 360learning-core-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/360learning/refs/heads/main/openapi/360learning-core-api.json
- filename: 360learning-bulk-api.json
  format: json
  label: 360Learning Bulk API v2
  slug: 360learning-bulk-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/360learning/refs/heads/main/openapi/360learning-bulk-api.json
- filename: 360learning-webhook-api.json
  format: json
  label: 360Learning Webhook API v2
  slug: 360learning-webhook-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/360learning/refs/heads/main/openapi/360learning-webhook-api.json
- filename: 360learning-plugin-api.json
  format: json
  label: 360Learning Plugin API v2
  slug: 360learning-plugin-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/360learning/refs/heads/main/openapi/360learning-plugin-api.json
- filename: 360learning-user-authorized-api.json
  format: json
  label: 360Learning User Authorized API v2
  slug: 360learning-user-authorized-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/360learning/refs/heads/main/openapi/360learning-user-authorized-api.json
consequence_counts:
  read: 60
  safety-critical: 104
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 104
kind: agentic-access
layout: agentic-access
method: generated
name: 360Learning Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v2/bulk/groups
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/bulk/groups/catalog
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v2/bulk/groups/catalog
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/bulk/groups/library
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v2/bulk/groups/library
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/bulk/groups/memberships
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v2/bulk/groups/memberships
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v2/bulk/integrations/{integrationId}/courses
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v2/bulk/integrations/{integrationId}/courses
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/bulk/integrations/{integrationId}/stats
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/bulk/notifications/subscriptions
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v2/bulk/skills
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v2/bulk/skills
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v2/bulk/skills/jobs
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v2/bulk/skills/jobs
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v2/bulk/skills/jobs-skills
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v2/bulk/skills/libraries
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v2/bulk/skills/libraries
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/bulk/skills/reviews
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /api/v2/bulk/skills/users/jobs
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/certificate-outlines
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v2/certificate-outlines/{certificateOutlineId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/v2/certificate-outlines/{certificateOutlineId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v2/classroom-slots/{classroomSlotId}/attendance-sheets
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v2/classroom-slots/{classroomSlotId}/attendance-sheets/{attendanceSheetId}
operation_count: 164
overview: '360Learning exposes 164 API operations that an AI agent could call, of which 104 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 60 read and 104 safety-critical.


  104 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: 360Learning
provider_slug: 360learning
slug: 360learning-agentic-access
source_filename: 360learning-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: generated\nsource: openapi/360learning-bulk-api.json, openapi/360learning-core-api.json, openapi/360learning-plugin-api.json,\n  openapi/360learning-user-authorized-api.json, openapi/360learning-webhook-api.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 164\n  by_action_class:\n    acting: 104\n    connected: 60\n  by_consequence:\n    safety-critical: 104\n    read: 60\n  human_in_the_loop_required: 104\noperations:\n- path: /api/v2/bulk/groups/catalog\n  method: post\n  operationId: v2.bulk.groups.AddContentsToGroupsCatalogController_addContentsToGroupsCatalog\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n     \
  \ max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/bulk/groups/catalog\n  method: delete\n  operationId: v2.bulk.groups.RemoveContentsFromGroupsCatalogController_removeContentsFromGroupsCatalog\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/bulk/groups/library\n  method: post\n  operationId: v2.bulk.groups.AddContentsToGroupsLibraryController_addContentsToGroupsLibrary\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n\
  \      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/bulk/groups/library\n  method: delete\n  operationId: v2.bulk.groups.RemoveContentsFromGroupsLibraryController_removeContentsFromGroupsLibrary\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/bulk/groups/memberships\n  method: post\n  operationId: v2.bulk.groups.AddUsersToGroupsController_addUsersToGroups\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n\
  \    audit: required\n- path: /api/v2/bulk/groups/memberships\n  method: delete\n  operationId: v2.bulk.groups.RemoveUsersFromGroupsController_removeUsersFromGroups\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/bulk/groups\n  method: delete\n  operationId: v2.bulk.groups.DeleteGroupsController_deleteGroups\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/bulk/integrations/{integrationId}/courses\n  method: delete\n  operationId:\
  \ v2.bulk.integrations.ArchiveExternalCoursesController_archiveExternalCourses\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/bulk/integrations/{integrationId}/courses\n  method: put\n  operationId: v2.bulk.integrations.ImportExternalCoursesController_importExternalCourses\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/bulk/integrations/{integrationId}/stats\n  method: post\n  operationId: v2.bulk.integrations.ImportExternalStatisticsController_importExternalStatistics\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/bulk/operations/{bulkOperationId}\n  method: get\n  operationId: v2.bulk.operations.GetBulkOperationController_getBulkOperation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/bulk/operations/{bulkOperationId}/results\n  method: get\n  operationId: v2.bulk.operations.GetBulkOperationResultsController_getBulkOperationResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/bulk/operations\n  method: get\n  operationId: v2.bulk.operations.GetBulkOperationsController_getBulkOperations\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/bulk/skills/reviews\n  method: post\n  operationId: v2.bulk.skills.AddSkillReviewsController_addSkillReviews\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/bulk/skills/jobs\n  method: delete\n  operationId: v2.bulk.skills.DeleteJobsController_deleteJobs\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit:\
  \ required\n- path: /api/v2/bulk/skills/jobs\n  method: put\n  operationId: v2.bulk.skills.UpsertJobsController_upsertJobs\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/bulk/skills/libraries\n  method: delete\n  operationId: v2.bulk.skills.DeleteLibrariesController_deleteLibraries\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/bulk/skills/libraries\n  method: put\n  operationId: v2.bulk.skills.UpsertLibrariesController_upsertLibraries\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/bulk/skills\n  method: delete\n  operationId: v2.bulk.skills.DeleteSkillsController_deleteSkills\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/bulk/skills\n  method: put\n  operationId: v2.bulk.skills.UpsertSkillsController_upsertSkills\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/bulk/skills/jobs-skills\n  method: put\n  operationId: v2.bulk.skills.ReplaceJobsSkillsController_replaceJobsSkills\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/bulk/skills/users/jobs\n  method: put\n  operationId: v2.bulk.skills.ReplaceUsersJobsController_replaceUsersJobs\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /api/v2/bulk/notifications/subscriptions\n  method: post\n  operationId: v2.bulk.subscriptions.CreateSubscriptionEventsController_createSubscriptionEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/certificate-outlines\n  method: post\n  operationId: v2.certificateOutlines.CreateCertificateOutlineController_createCertificateOutline\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n\
  - path: /api/v2/certificate-outlines\n  method: get\n  operationId: v2.certificateOutlines.GetCertificateOutlinesController_getCertificateOutlines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/certificate-outlines/{certificateOutlineId}\n  method: delete\n  operationId: v2.certificateOutlines.DeleteCertificateOutlineController_deleteCertificateOutline\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/certificate-outlines/{certificateOutlineId}\n  method: patch\n  operationId: v2.certificateOutlines.UpdateCertificateOutlineController_updateCertificateOutline\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/classrooms\n  method: post\n  operationId: v2.classrooms.CreateClassroomController_createClassroom\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/classrooms\n  method: get\n  operationId: v2.classrooms.GetClassroomsController_getClassrooms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/classrooms/{classroomId}\n\
  \  method: get\n  operationId: v2.classrooms.GetClassroomController_getClassroom\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/classrooms/{classroomId}\n  method: patch\n  operationId: v2.classrooms.UpdateClassroomController_updateClassroom\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/classrooms/{classroomId}/registrations\n  method: get\n  operationId: v2.classrooms.GetClassroomRegistrationsController_getClassroomRegistrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/classrooms/{classroomId}/slots\n\
  \  method: post\n  operationId: v2.classrooms.CreateClassroomSlotController_createClassroomSlot\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/classrooms/{classroomId}/slots\n  method: get\n  operationId: v2.classrooms.GetClassroomSlotsController_getClassroomSlots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/classrooms/{classroomId}/slots/{classroomSlotId}\n  method: delete\n  operationId: v2.classrooms.DeleteClassroomSlotController_deleteClassroomSlot\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n   \
  \   max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/classrooms/{classroomId}/slots/{classroomSlotId}\n  method: patch\n  operationId: v2.classrooms.UpdateClassroomSlotController_updateClassroomSlot\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/classroom-slots/{classroomSlotId}/attendance-sheets\n  method: post\n  operationId: v2.classrooms.CreateAttendanceSheetController_createAttendanceSheet\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n\
  \      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/classroom-slots/{classroomSlotId}/attendance-sheets\n  method: get\n  operationId: v2.classrooms.GetAttendanceSheetsController_getAttendanceSheets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/classroom-slots/{classroomSlotId}/attendance-sheets/{attendanceSheetId}\n  method: delete\n  operationId: v2.classrooms.DeleteAttendanceSheetController_deleteAttendanceSheet\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/classroom-slots/{classroomSlotId}/attendance-sheets/{attendanceSheetId}\n\
  \  method: put\n  operationId: v2.classrooms.UpdateAttendanceSheetController_updateAttendanceSheet\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/classroom-slots/{classroomSlotId}/attendance-sheets/{attendanceSheetId}/attendances\n  method: get\n  operationId: v2.classrooms.GetAttendancesController_getAttendances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/classroom-slots/{classroomSlotId}/waitlist\n  method: get\n  operationId: v2.classrooms.GetClassroomSlotWaitlistController_getClassroomSlotWaitlist\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/classroom-slots/{classroomSlotId}/waitlist/{userId}\n  method: post\n  operationId: v2.classrooms.JoinClassroomSlotWaitlistController_joinClassroomSlotWaitlist\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/classroom-slots/{classroomSlotId}/waitlist/{userId}\n  method: delete\n  operationId: v2.classrooms.LeaveClassroomSlotWaitlistController_leaveClassroomSlotWaitlist\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /api/v2/classroom-slots/{classroomSlotId}/registrations/{userId}\n  method: post\n  operationId: v2.classrooms.AddSlotRegistrationController_addSlotRegistration\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/classroom-slots/{classroomSlotId}/registrations\n  method: get\n  operationId: v2.classrooms.GetSlotRegistrationsController_getSlotRegistrations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/classroom-slots/{classroomSlotId}/registrations/{slotRegistrationId}\n  method: patch\n  operationId: v2.classrooms.UpdateSlotRegistrationController_updateSlotRegistration\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/courses/{courseId}/archive\n  method: put\n  operationId: v2.courses.ArchiveOrUnarchiveCourseController_archiveOrUnarchiveCourse\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/courses/elearning-standard\n  method: post\n  operationId: v2.courses.CreateELearningStandardCourseController_createELearningStandardCourse\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/courses/generate-from-prompt\n  method: post\n  operationId: v2.courses.GenerateFromPromptController_generateFromPrompt\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/courses/stats\n  method: get\n  operationId: v2.courses.GetAllCourseStatsController_getAllCourseStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/courses/{courseId}\n  method: get\n\
  \  operationId: v2.courses.GetCourseController_getCourse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/courses/{courseId}/custom-fields/values\n  method: get\n  operationId: v2.courses.GetCourseCustomFieldValuesController_getCourseCustomFieldValues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/courses/{courseId}/custom-fields/values\n  method: put\n  operationId: v2.courses.UpdateCourseCustomFieldValuesController_updateCourseCustomFieldValues\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path:\
  \ /api/v2/courses\n  method: get\n  operationId: v2.courses.GetCoursesController_getCourses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/courses/{courseId}/tags\n  method: get\n  operationId: v2.courses.GetCourseTagsController_getTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/courses/{courseId}/tags\n  method: put\n  operationId: v2.courses.UpdateTagsController_updateTags\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/courses/elearning-standard/{courseId}\n  method: patch\n\
  \  operationId: v2.courses.UpdateELearningStandardCourseController_updateELearningStandardCourse\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/custom-fields\n  method: post\n  operationId: v2.customFields.CreateCustomFieldController_createCustomField\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/custom-fields\n  method: get\n  operationId: v2.customFields.GetCustomFieldsController_getCustomFields\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/custom-fields/{customFieldId}\n  method: delete\n  operationId: v2.customFields.DeleteCustomFieldController_deleteCustomField\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/custom-fields/{customFieldId}\n  method: patch\n  operationId: v2.customFields.UpdateCustomFieldController_updateCustomField\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n\
  \    audit: required\n- path: /api/v2/custom-fields/{customFieldId}/authorized-values\n  method: get\n  operationId: v2.customFields.GetAuthorizedValuesController_getAuthorizedValues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/custom-fields/{customFieldId}/authorized-values\n  method: put\n  operationId: v2.customFields.ReplaceAuthorizedValuesController_replaceAuthorizedValues\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/custom-links\n  method: post\n  operationId: v2.customLinks.CreateCustomLinkController_createCustomLink\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/custom-links\n  method: get\n  operationId: v2.customLinks.GetCustomLinksByCompanyController_getCustomLinksByCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/custom-links/{customLinkId}\n  method: delete\n  operationId: v2.customLinks.DeleteCustomLinkController_deleteCustomLink\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/custom-links/{customLinkId}\n\
  \  method: put\n  operationId: v2.customLinks.ReplaceCustomLinkController_replaceCustomLink\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/external-ids\n  method: post\n  operationId: v2.externalIds.CreateExternalIdController_createExternalId\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/external-ids\n  method: get\n  operationId: v2.externalIds.GetExternalIdsController_getExternalIds\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/external-ids/{mappingId}\n  method: delete\n  operationId: v2.externalIds.DeleteExternalIdController_deleteExternalId\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/external-ids/{mappingId}\n  method: put\n  operationId: v2.externalIds.UpdateExternalIdController_updateExternalId\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path:\
  \ /api/v2/groups/{groupId}/{role}/{userId}\n  method: post\n  operationId: v2.groups.AddUserRoleToGroupController_addUserRoleToGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/groups/{groupId}/{role}/{userId}\n  method: delete\n  operationId: v2.groups.RemoveUserRoleFromGroupController_removeUserRoleFromGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/groups\n  method: post\n  operationId: v2.groups.CreateGroupController_createGroup\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/groups\n  method: get\n  operationId: v2.groups.GetGroupsController_getGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/groups/{groupId}\n  method: delete\n  operationId: v2.groups.DeleteGroupController_deleteGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/groups/{groupId}\n\
  \  method: get\n  operationId: v2.groups.GetGroupController_getGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/groups/{groupId}\n  method: patch\n  operationId: v2.groups.UpdateGroupController_updateGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v2/groups/{groupId}/roles\n  method: get\n  operationId: v2.groups.GetGroupMembersController_getGroupMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/groups/{groupId}/catalog/{contentType}-ids\n  method: get\n  operationId:\
  \ v2.groups.GetCatalogContentIdsController_getCatalogContentIds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/groups/{groupId}/library/{contentType}-ids\n  method: get\n  operationId: v2.groups.GetLibraryContentIdsController_getLibraryContentIds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/groups/{groupId}/media\n  method: post\n  operationId: v2.groups.UploadGroupMediaController_uploadGroupMedia\n  x-agentic-access:\n    action-class:\n\n# --- truncated at 32 KB (60 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/360learning/refs/heads/main/agentic-access/360learning-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/360learning/refs/heads/main/agentic-access/360learning-agentic-access.yml
summary_line: 164 operations · 104 acting · 104 human-in-the-loop
tags:
- Company
- Edtech
- Learning Management System
- E-Learning
- Training
- Collaborative Learning
- HR Tech
- Skills
- API
---
