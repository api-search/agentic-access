---
acting_count: 81
action_class_counts:
  acting: 81
  connected: 61
api_specs:
- filename: ispring-assignments-api-openapi.yml
  format: yaml
  label: iSpring Learn Assignments API
  slug: ispring-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-assignments-api-openapi.yml
- filename: ispring-certificate-api-openapi.yml
  format: yaml
  label: iSpring Learn Certificate API
  slug: ispring-certificate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-certificate-api-openapi.yml
- filename: ispring-content-api-openapi.yml
  format: yaml
  label: iSpring Learn Content API
  slug: ispring-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-content-api-openapi.yml
- filename: ispring-department-api-openapi.yml
  format: yaml
  label: iSpring Learn Department API
  slug: ispring-department-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-department-api-openapi.yml
- filename: ispring-departments-api-openapi.yml
  format: yaml
  label: iSpring Learn Departments API
  slug: ispring-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-departments-api-openapi.yml
- filename: ispring-enrollment-api-openapi.yml
  format: yaml
  label: iSpring Learn Enrollment API
  slug: ispring-enrollment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-enrollment-api-openapi.yml
- filename: ispring-gamification-api-openapi.yml
  format: yaml
  label: iSpring Learn Gamification API
  slug: ispring-gamification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-gamification-api-openapi.yml
- filename: ispring-group-api-openapi.yml
  format: yaml
  label: iSpring Learn Group API
  slug: ispring-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-group-api-openapi.yml
- filename: ispring-jobtraining-api-openapi.yml
  format: yaml
  label: iSpring Learn Jobtraining API
  slug: ispring-jobtraining-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-jobtraining-api-openapi.yml
- filename: ispring-learning-track-api-openapi.yml
  format: yaml
  label: iSpring Learn Learning Track API
  slug: ispring-learning-track-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-learning-track-api-openapi.yml
- filename: ispring-performance-management-api-openapi.yml
  format: yaml
  label: iSpring Learn Performance Management API
  slug: ispring-performance-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-performance-management-api-openapi.yml
- filename: ispring-quizzes-api-openapi.yml
  format: yaml
  label: iSpring Learn Quizzes API
  slug: ispring-quizzes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-quizzes-api-openapi.yml
- filename: ispring-report-api-openapi.yml
  format: yaml
  label: iSpring Learn Report API
  slug: ispring-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-report-api-openapi.yml
- filename: ispring-results-api-openapi.yml
  format: yaml
  label: iSpring Learn Results API
  slug: ispring-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-results-api-openapi.yml
- filename: ispring-statistics-api-openapi.yml
  format: yaml
  label: iSpring Learn Statistics API
  slug: ispring-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-statistics-api-openapi.yml
- filename: ispring-task-api-openapi.yml
  format: yaml
  label: iSpring Learn Task API
  slug: ispring-task-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-task-api-openapi.yml
- filename: ispring-token-api-openapi.yml
  format: yaml
  label: iSpring Learn Token API
  slug: ispring-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-token-api-openapi.yml
- filename: ispring-training-api-openapi.yml
  format: yaml
  label: iSpring Learn Training API
  slug: ispring-training-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-training-api-openapi.yml
- filename: ispring-user-api-openapi.yml
  format: yaml
  label: iSpring Learn User API
  slug: ispring-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-user-api-openapi.yml
- filename: ispring-webhook-api-openapi.yml
  format: yaml
  label: iSpring Learn Webhook API
  slug: ispring-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/openapi/ispring-webhook-api-openapi.yml
consequence_counts:
  physical: 3
  read: 61
  safety-critical: 3
  write: 75
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Ispring Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /statistics/module
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /users/terminate
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /webhook/disable
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /gamification/points/withdraw
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /performance-management/appraisal/session/{sessionId}/question/change-order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /webhook/code/send
operation_count: 142
overview: 'iSpring Learn exposes 142 API operations that an AI agent could call, of which 81 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 61 read, 75 write, 3 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: iSpring Learn
provider_slug: ispring
slug: ispring-agentic-access
source_filename: ispring-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/ispring-assignments-api-openapi.yml, openapi/ispring-certificate-api-openapi.yml,\n  openapi/ispring-content-api-openapi.yml, openapi/ispring-department-api-openapi.yml, openapi/ispring-departments-api-openapi.yml,\n  openapi/ispring-enrollment-api-openapi.yml, openapi/ispring-gamification-api-openapi.yml,\n  openapi/ispring-group-api-openapi.yml, openapi/ispring-jobtraining-api-openapi.yml, openapi/ispring-learning-track-api-openapi.yml,\n  openapi/ispring-performance-management-api-openapi.yml, openapi/ispring-quizzes-api-openapi.yml,\n  openapi/ispring-report-api-openapi.yml, openapi/ispring-results-api-openapi.yml, openapi/ispring-statistics-api-openapi.yml,\n  openapi/ispring-task-api-openapi.yml, openapi/ispring-token-api-openapi.yml, openapi/ispring-training-api-openapi.yml,\n  openapi/ispring-user-api-openapi.yml, openapi/ispring-webhook-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts,\
  \ classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 142\n  by_action_class:\n    connected: 61\n    acting: 81\n  by_consequence:\n    read: 61\n    write: 75\n    physical: 3\n    safety-critical: 3\n  human_in_the_loop_required: 3\noperations:\n- path: /assignments\n  method: get\n  operationId: ListAssignments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assignment/{assignmentId}/attempts/ungraded\n  method: get\n  operationId: ListAssignmentAttempts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assignments/attempts/grade\n  method: post\n  operationId: GradeAssignments\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /certificate/{issuedCertificateId}\n  method: get\n  operationId: GetIssuedCertificate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /content\n  method: get\n  operationId: GetContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contents\n  method: get\n  operationId: ListContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contents\n  method: post\n  operationId: ListContentByPost\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /content/{contentId}\n  method: get\n  operationId: GetContentItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /content/{contentId}/final_statuses\n  method: get\n  operationId: GetContentItemFinalStatuses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /courses/modules\n  method: get\n  operationId: ListCoursesModules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /course_fields\n  method: get\n  operationId: ListCourseFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /content/create/{contentType}\n  method: post\n  operationId: CreateContent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /course/{courseId}/modules\n  method: get\n  operationId: ListCourseModules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /courses_tree\n  method: get\n  operationId: GetCoursesTree\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /department\n  method: get\n  operationId: GetDepartments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /department\n  method: post\n  operationId: AddDepartment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /department/{departmentId}\n  method: get\n  operationId: GetDepartment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /department/{departmentId}\n  method: post\n  operationId: UpdateDepartment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /department/{departmentId}\n\
  \  method: delete\n  operationId: RemoveDepartment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /department/{departmentId}/subordination\n  method: post\n  operationId: ChangeDepartmentSubordination\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /department/{departmentId}/user/move\n  method: post\n  operationId: MoveUsersToDepartment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /department/{parentId}/department/move\n  method: post\n  operationId: MoveDepartments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /departments\n  method: get\n  operationId: ListDepartments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /enrollment\n  method: get\n  operationId: GetEnrollments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /enrollment\n  method: post\n  operationId: EnrollLearnersInCourses\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /enrollments\n  method: get\n  operationId: ListEnrollments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /enrollments\n  method: post\n  operationId: ListEnrollmentsByPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /enrollment/{enrollmentId}\n  method: get\n  operationId: GetEnrollment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /enrollment/{enrollmentId}\n  method: post\n  operationId: ChangeEnrollment\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /enrollment/{enrollmentId}/reenroll\n  method: post\n  operationId: Reenroll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /enrollment/delete\n  method: post\n  operationId: Unenroll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gamification/points\n  method:\
  \ get\n  operationId: GetGamificationPoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gamification/points/award\n  method: post\n  operationId: AwardGamificationPoints\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gamification/points/withdraw\n  method: post\n  operationId: WithdrawGamificationPoints\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /group\n\
  \  method: get\n  operationId: GetGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /group\n  method: post\n  operationId: AddGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /group/smart\n  method: post\n  operationId: AddSmartGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /group/smart/{groupId}\n  method: post\n  operationId: EditSmartGroup\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /group/smart/{groupId}/rules\n  method: get\n  operationId: GetSmartGroupRules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /group/{groupId}\n  method: get\n  operationId: GetGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /group/{groupId}\n  method: post\n  operationId: UpdateGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /group/{groupId}\n  method: delete\n  operationId: RemoveGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /group/{groupId}/members\n  method: post\n  operationId: UpdateGroupMembers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups\n  method: get\n  operationId: ListGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /job-training/checklist/sessions/list\n  method: post\n  operationId: listChecklistSessions\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /job-training/sessions/result/list\n  method: post\n  operationId: listSessionsResult\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /job-training/completed-session/criterion-group/result/list\n  method: post\n  operationId: listCriterionGroupsResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /job-training/completed-session/criterion/result/list\n  method: post\n\
  \  operationId: listCriterionResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /learning_track/courses\n  method: get\n  operationId: ListLearningTracksCourses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /performance-management/competencies/scale/list\n  method: get\n  operationId: ListCompetencyScales\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /performance-management/competencies/scale/create\n  method: post\n  operationId: CreateCompetencyScale\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /performance-management/competencies/scale/{scaleId}/change\n  method: post\n  operationId: ChangeCompetencyScale\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /performance-management/competencies/group/create\n  method: post\n  operationId: CreateCompetencyGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /performance-management/competencies/group/{groupId}/rename\n  method: post\n  operationId: ChangeCompetencyGroupName\n  x-agentic-access:\n \
  \   action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /performance-management/competencies/group/batch-move\n  method: post\n  operationId: MoveCompetencyGroups\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /performance-management/competencies/competency/batch-move\n  method: post\n  operationId: MoveCompetenciesToGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /performance-management/competencies/group/list\n  method: get\n  operationId: ListCompetencyGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /performance-management/competencies/competency/list\n  method: post\n  operationId: ListCompetencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /performance-management/competencies/competency/create\n  method: post\n  operationId: CreateCompetency\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /performance-management/competencies/competency/{competencyId}/change\n\
  \  method: post\n  operationId: ChangeCompetency\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /performance-management/competencies/competency/{competencyId}/indicator/create\n  method: post\n  operationId: CreateCompetencyIndicator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /performance-management/competencies/competency/{competencyId}/indicator/{indicatorId}/change\n  method: post\n  operationId: ChangeCompetencyIndicator\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /performance-management/competencies/profile/list\n  method: post\n  operationId: ListCompetencyProfiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /performance-management/appraisal/session/list\n  method: post\n  operationId: ListAppraisalSessions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /performance-management/appraisal/session/{sessionId}/employee-card/list\n  method: get\n  operationId: ListAppraisalSessionEmployeeCards\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /performance-management/appraisal/session/{sessionId}/review/list\n  method: get\n  operationId: ListAppraisalSessionReviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /performance-management/appraisal/session/{sessionId}/results\n  method: get\n  operationId: GetAppraisalSessionResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /performance-management/appraisal/session/{sessionId}/content/competencies\n  method: get\n  operationId: GetAppraisalSessionContentCompetencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /performance-management/appraisal/session/{sessionId}/user/attributes/list\n\
  \  method: post\n  operationId: ListAppraisalSessionUserAttributes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /performance-management/appraisal/session/{sessionId}/start\n  method: post\n  operationId: StartAppraisalSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /performance-management/appraisal/session/{sessionId}/restart\n  method: post\n  operationId: RestartAppraisalSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /performance-management/appraisal/session/{sessionId}/complete\n  method: post\n  operationId: CompleteAppraisalSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /performance-management/appraisal/session/{sessionId}/update\n  method: post\n  operationId: UpdateAppraisalSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /performance-management/appraisal/session/create\n\
  \  method: post\n  operationId: CreateAppraisalSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /performance-management/appraisal/session/{sessionId}/employee-card/add\n  method: post\n  operationId: AddAppraisalSessionEmployeeCards\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /performance-management/appraisal/session/{sessionId}/employee-card/reviewer/replace\n  method: post\n  operationId: ReplaceAppraisalSessionEmployeeReviewers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /performance-management/appraisal/session/{sessionId}/employee-card/remove\n  method: post\n  operationId: RemoveAppraisalSessionEmployeeCards\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /performance-management/appraisal/session/{sessionId}/employee-card/reviewer/remove\n  method: post\n  operationId: RemoveAppraisalSessionReviewers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /performance-management/appraisal/session/{sessionId}/question/add\n  method: post\n  operationId: AddAppraisalQuestion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /performance-management/appraisal/session/{sessionId}/question/{questionId}/update\n  method: post\n  operationId: UpdateAppraisalQuestion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /performance-management/appraisal/session/{sessionId}/question/change-order\n  method: post\n  operationId:\
  \ ChangeAppraisalQuestionOrders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /performance-management/appraisal/session/{sessionId}/question/{questionId}/remove\n  method: post\n  operationId: RemoveAppraisalQuestion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /performance-management/appraisal/session/{sessionId}/permissions/add\n  method: post\n  operationId: AddAppraisalSessionPermissions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /performance-management/appraisal/session/{sessionId}/permissions/remove\n  method: post\n  operationId: RemoveAppraisalSessionPermissions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /performance-management/appraisal/session/{sessionId}/info\n  method: get\n  operationId: GetAppraisalSessionInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /performance-management/appraisal/session/{sessionId}/notification/change\n  method: post\n\
  \  operationId: ChangeAppraisalSessionNotificationSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /quizzes\n  method: get\n  operationId: ListQuizzes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /report/answer-breakdown\n  method: get\n  operationId: ListAnswerBreakdownResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /report/active-users-by-period\n  method: get\n  operationId: GetUsersWithActivity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /report/answer-breakdown\n  method: get\n  operationId: ListAnswerBreakdownResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /learners/results\n  method: get\n  operationId: ListLearnerResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /learners/modules/results\n  method: get\n  operationId: ListLearnerModulesResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /statistics/course\n  method: post\n  operationId: UpdateCourseStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n  \
  \    triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /statistics/module\n  method: post\n  operationId: UpdateModuleStatuses\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /statistics/module\n  method: delete\n  operationId: ResetModuleStatistics\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /task/{taskId}/status\n  method: get\n  operationId: GetTaskStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/token\n  method: post\n  operationId: AccessRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /training/{trainingId}\n  method: get\n  operationId: GetTrainingById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /training/session/{trainingSessionId}\n  method: get\n  operationId: GetTrainingSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /training/{trainingId}/sessions\n  method: get\n  operationId: ListSessionsByTrainingId\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /training/day/{dayId}\n  method: get\n  operationId: GetDay\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /training/day/{dayId}\n  method: post\n  operationId: UpdateDay\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /training/session/participants/{sessionId}\n  method: get\n  operationId: ListSessionParticipants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\n\n# --- truncated at 32 KB (43 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/agentic-access/ispring-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ispring/refs/heads/main/agentic-access/ispring-agentic-access.yml
summary_line: 142 operations · 81 acting · 3 human-in-the-loop
tags:
- E-Learning
- LMS
- Learning Management System
- Training
- Courses
- Enrollment
- User
- Group
- Reporting
- Webhook
- SCORM
- Corporate Training
---
