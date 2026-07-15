---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 17
api_specs:
- filename: workday-tracking-system-time-tracking-openapi.yml
  format: yaml
  label: Workday Time Tracking API
  slug: workday-time-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-tracking-system/refs/heads/main/openapi/workday-tracking-system-time-tracking-openapi.yml
- filename: workday-tracking-system-absence-management-openapi.yml
  format: yaml
  label: Workday Absence Management API
  slug: workday-absence-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-tracking-system/refs/heads/main/openapi/workday-tracking-system-absence-management-openapi.yml
- filename: workday-tracking-system-scheduling-openapi.yml
  format: yaml
  label: Workday Scheduling API
  slug: workday-scheduling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-tracking-system/refs/heads/main/openapi/workday-tracking-system-scheduling-openapi.yml
consequence_counts:
  read: 17
  safety-critical: 1
  write: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Workday Tracking System Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /workers/{workerId}/accrualOverrides
operation_count: 35
overview: 'Workday Tracking System exposes 35 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read, 17 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Workday Tracking System
provider_slug: workday-tracking-system
slug: workday-tracking-system-agentic-access
source_filename: workday-tracking-system-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/workday-tracking-system-absence-management-openapi.yml, openapi/workday-tracking-system-scheduling-openapi.yml,\n  openapi/workday-tracking-system-time-tracking-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 35\n  by_action_class:\n    connected: 17\n    acting: 18\n  by_consequence:\n    read: 17\n    write: 17\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /workers/{workerId}/timeOff\n  method: get\n  operationId: listTimeOff\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workers/{workerId}/timeOff\n  method: post\n  operationId:\
  \ requestTimeOff\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workers/{workerId}/timeOff/{timeOffId}\n  method: get\n  operationId: getTimeOff\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workers/{workerId}/timeOff/{timeOffId}\n  method: put\n  operationId: adjustTimeOff\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workers/{workerId}/leaveOfAbsence\n  method: get\n  operationId: listLeavesOfAbsence\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workers/{workerId}/leaveOfAbsence\n  method: post\n  operationId: requestLeaveOfAbsence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workers/{workerId}/leaveOfAbsence/{leaveId}/return\n  method: post\n  operationId: returnFromLeaveOfAbsence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workers/{workerId}/timeOffBalances\n  method: get\n  operationId: listTimeOffBalances\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workers/{workerId}/accrualOverrides\n  method: get\n  operationId: listAccrualOverrides\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workers/{workerId}/accrualOverrides\n  method: post\n  operationId: createAccrualOverride\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /scheduleShifts\n  method: get\n  operationId: listScheduleShifts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /scheduleShifts\n  method: post\n  operationId: createScheduleShift\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scheduleShifts/{shiftId}\n  method: get\n  operationId: getScheduleShift\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scheduleShifts/{shiftId}\n  method: put\n  operationId: updateScheduleShift\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /scheduleShifts/{shiftId}\n\
  \  method: delete\n  operationId: deleteScheduleShift\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /schedulingOrganizations\n  method: get\n  operationId: listSchedulingOrganizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schedulingOrganizations\n  method: post\n  operationId: createSchedulingOrganization\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /schedulingOrganizations/{orgId}\n  method: get\n\
  \  operationId: getSchedulingOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /laborDemand\n  method: get\n  operationId: listLaborDemand\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /laborDemand\n  method: post\n  operationId: createLaborDemand\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workers/{workerId}/schedulingPreferences\n  method: get\n  operationId: getWorkerSchedulingPreferences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /workers/{workerId}/schedulingPreferences\n  method: put\n  operationId: updateWorkerSchedulingPreferences\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workers/{workerId}/timeBlocks\n  method: get\n  operationId: listTimeBlocks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workers/{workerId}/timeBlocks\n  method: post\n  operationId: createTimeBlock\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /workers/{workerId}/timeBlocks/{timeBlockId}\n  method: get\n  operationId: getTimeBlock\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workers/{workerId}/timeBlocks/{timeBlockId}\n  method: put\n  operationId: updateTimeBlock\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workers/{workerId}/timeBlocks/{timeBlockId}\n  method: delete\n  operationId: deleteTimeBlock\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /workers/{workerId}/timeClockEvents\n  method: get\n  operationId: listTimeClockEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workers/{workerId}/timeClockEvents\n  method: post\n  operationId: createTimeClockEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workers/{workerId}/workSchedule\n  method: get\n  operationId: getWorkSchedule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workers/{workerId}/workSchedule\n  method: put\n  operationId: assignWorkSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workers/{workerId}/timeRequests\n  method: get\n  operationId: listTimeRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workers/{workerId}/timeRequests\n  method: post\n  operationId: createTimeRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workers/{workerId}/timesheets\n  method: get\n  operationId: listTimesheets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /workers/{workerId}/timesheets/{timesheetId}/submit\n  method: post\n  operationId: submitTimesheet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-tracking-system/refs/heads/main/agentic-access/workday-tracking-system-agentic-access.yml
summary_line: 35 operations · 18 acting · 1 human-in-the-loop
tags:
- Absence Management
- Attendance
- Enterprise
- HCM
- Human Capital Management
- Payroll
- Scheduling
- Time Tracking
- Timesheets
- Workforce Management
---
