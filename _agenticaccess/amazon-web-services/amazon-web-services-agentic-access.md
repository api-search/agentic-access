---
acting_count: 3518
action_class_counts:
  acting: 3518
  connected: 1663
consequence_counts:
  physical: 123
  read: 1663
  safety-critical: 147
  write: 3248
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 147
kind: agentic-access
layout: agentic-access
method: generated
name: Amazon Web Services Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /2013-04-01/hostedzone/{Id}/disable-dnssec
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /2015-01-01/es/domain/{DomainName}/revokeVpcEndpointAccess
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /2017-08-29/presets/{name}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /2020-05-31/origin-access-control/{Id}/config
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /2020-08-01/studios/{studioId}/streaming-sessions/{sessionId}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /2020-11-20/projects/{projectName}/models/{modelVersion}/stop
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /2021-01-01/opensearch/domain/{DomainName}/revokeVpcEndpointAccess
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /2022-01-01/osis/stopPipeline/{PipelineName}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /BatchRevokePermissions
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /RevokePermissions
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /StopComposition
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /StopFailback
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /StopReplication
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /StopReplication
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /StopSourceNetworkReplication
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /StopStream
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /TerminateRecoveryInstances
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /TerminateTargetInstances
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /accounts/{accountId}/users/{userId}?operation=reset-personal-pin
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /admin/disable
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /alarms/disable
operation_count: 5181
overview: 'Amazon Web Services exposes 5181 API operations that an AI agent could call, of which 3518 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1663 read, 3248 write, 123 physical, and 147 safety-critical.


  147 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amazon Web Services
provider_slug: amazon-web-services
slug: amazon-web-services-agentic-access
source_filename: amazon-web-services-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/accessanalyzer-openapi-original.yml, openapi/account-openapi-original.yml, openapi/acm-openapi-original.yml,\n  openapi/acm-pca-openapi-original.yml, openapi/amp-openapi-original.yml, openapi/amplify-openapi-original.yml,\n  openapi/amplifybackend-openapi-original.yml, openapi/amplifyuibuilder-openapi-original.yml,\n  openapi/apigateway-openapi-original.yml, openapi/apigatewaymanagementapi-openapi-original.yml,\n  openapi/apigatewayv2-openapi-original.yml, openapi/appconfig-openapi-original.yml, openapi/appconfigdata-openapi-original.yml,\n  openapi/appfabric-openapi-original.yml, openapi/appflow-openapi-original.yml, openapi/appintegrations-openapi-original.yml,\n  openapi/application-autoscaling-openapi-original.yml, openapi/application-insights-openapi-original.yml,\n  openapi/applicationcostprofiler-openapi-original.yml, openapi/appmesh-openapi-original.yml,\n  openapi/apprunner-openapi-original.yml, openapi/appstream-openapi-original.yml,\
  \ openapi/appsync-openapi-original.yml,\n  openapi/arc-zonal-shift-openapi-original.yml, openapi/athena-openapi-original.yml, openapi/auditmanager-openapi-original.yml,\n  openapi/autoscaling-openapi-original.yml, openapi/autoscaling-plans-openapi-original.yml,\n  openapi/awsmigrationhub-openapi-original.yml, openapi/b2bi-openapi-original.yml, openapi/backup-gateway-openapi-original.yml,\n  openapi/backup-openapi-original.yml, openapi/backupstorage-openapi-original.yml, openapi/batch-openapi-original.yml,\n  openapi/bcm-data-exports-openapi-original.yml, openapi/bedrock-agent-openapi-original.yml,\n  openapi/bedrock-agent-runtime-openapi-original.yml, openapi/bedrock-openapi-original.yml,\n  openapi/bedrock-runtime-openapi-original.yml, openapi/billingconductor-openapi-original.yml,\n  openapi/braket-openapi-original.yml, openapi/budgets-openapi-original.yml, openapi/ce-openapi-original.yml,\n  openapi/chime-openapi-original.yml, openapi/chime-sdk-identity-openapi-original.yml, openapi/chime-sdk-media-pipelines-openapi-original.yml,\n\
  \  openapi/chime-sdk-meetings-openapi-original.yml, openapi/chime-sdk-messaging-openapi-original.yml,\n  openapi/chime-sdk-voice-openapi-original.yml, openapi/cleanrooms-openapi-original.yml, openapi/cleanroomsml-openapi-original.yml,\n  openapi/cloud9-openapi-original.yml, openapi/cloudcontrol-openapi-original.yml, openapi/clouddirectory-openapi-original.yml,\n  openapi/cloudformation-openapi-original.yml, openapi/cloudfront-keyvaluestore-openapi-original.yml,\n  openapi/cloudfront-openapi-original.yml, openapi/cloudhsm-openapi-original.yml, openapi/cloudhsmv2-openapi-original.yml,\n  openapi/cloudsearch-openapi-original.yml, openapi/cloudsearchdomain-openapi-original.yml,\n  openapi/cloudtrail-data-openapi-original.yml, openapi/cloudtrail-openapi-original.yml, openapi/codeartifact-openapi-original.yml,\n  openapi/codebuild-openapi-original.yml, openapi/codecatalyst-openapi-original.yml, openapi/codecommit-openapi-original.yml,\n  openapi/codedeploy-openapi-original.yml, openapi/codeguru-reviewer-openapi-original.yml,\
  \ openapi/codeguru-security-openapi-original.yml,\n  openapi/codeguruprofiler-openapi-original.yml, openapi/codepipeline-openapi-original.yml,\n  openapi/codestar-connections-openapi-original.yml, openapi/codestar-notifications-openapi-original.yml,\n  openapi/codestar-openapi-original.yml, openapi/cognito-identity-openapi-original.yml, openapi/cognito-idp-openapi-original.yml,\n  openapi/cognito-sync-openapi-original.yml, openapi/comprehend-openapi-original.yml, openapi/comprehendmedical-openapi-original.yml,\n  openapi/compute-optimizer-openapi-original.yml, openapi/config-openapi-original.yml, openapi/connect-contact-lens-openapi-original.yml,\n  openapi/connect-openapi-original.yml, openapi/connectcampaigns-openapi-original.yml, openapi/connectcases-openapi-original.yml,\n  openapi/connectparticipant-openapi-original.yml, openapi/controltower-openapi-original.yml,\n  openapi/cost-optimization-hub-openapi-original.yml, openapi/cur-openapi-original.yml, openapi/customer-profiles-openapi-original.yml,\n\
  \  openapi/databrew-openapi-original.yml, openapi/dataexchange-openapi-original.yml, openapi/datapipeline-openapi-original.yml,\n  openapi/datasync-openapi-original.yml, openapi/datazone-openapi-original.yml, openapi/dax-openapi-original.yml,\n  openapi/detective-openapi-original.yml, openapi/devicefarm-openapi-original.yml, openapi/devops-guru-openapi-original.yml,\n  openapi/directconnect-openapi-original.yml, openapi/discovery-openapi-original.yml, openapi/dlm-openapi-original.yml,\n  openapi/dms-openapi-original.yml, openapi/docdb-elastic-openapi-original.yml, openapi/docdb-openapi-original.yml,\n  openapi/drs-openapi-original.yml, openapi/ds-openapi-original.yml, openapi/dynamodb-openapi-original.yml,\n  openapi/ebs-openapi-original.yml, openapi/ec2-instance-connect-openapi-original.yml, openapi/ec2-openapi-original.yml,\n  openapi/ecr-openapi-original.yml, openapi/ecr-public-openapi-original.yml, openapi/ecs-openapi-original.yml,\n  openapi/eks-auth-openapi-original.yml, openapi/eks-openapi-original.yml,\
  \ openapi/elastic-inference-openapi-original.yml,\n  openapi/elasticache-openapi-original.yml, openapi/elasticbeanstalk-openapi-original.yml, openapi/elasticfilesystem-openapi-original.yml,\n  openapi/elasticloadbalancing-openapi-original.yml, openapi/elasticloadbalancingv2-openapi-original.yml,\n  openapi/elasticmapreduce-openapi-original.yml, openapi/elastictranscoder-openapi-original.yml,\n  openapi/email-openapi-original.yml, openapi/emr-containers-openapi-original.yml, openapi/emr-serverless-openapi-original.yml,\n  openapi/entitlementmarketplace-openapi-original.yml, openapi/entityresolution-openapi-original.yml,\n  openapi/es-openapi-original.yml, openapi/eventbridge-openapi-original.yml, openapi/events-openapi-original.yml,\n  openapi/evidently-openapi-original.yml, openapi/finspace-data-openapi-original.yml, openapi/finspace-openapi-original.yml,\n  openapi/firehose-openapi-original.yml, openapi/fis-openapi-original.yml, openapi/fms-openapi-original.yml,\n  openapi/forecast-openapi-original.yml,\
  \ openapi/forecastquery-openapi-original.yml, openapi/frauddetector-openapi-original.yml,\n  openapi/freetier-openapi-original.yml, openapi/fsx-openapi-original.yml, openapi/gamelift-openapi-original.yml,\n  openapi/glacier-openapi-original.yml, openapi/globalaccelerator-openapi-original.yml, openapi/glue-openapi-original.yml,\n  openapi/grafana-openapi-original.yml, openapi/greengrass-openapi-original.yml, openapi/greengrassv2-openapi-original.yml,\n  openapi/groundstation-openapi-original.yml, openapi/guardduty-openapi-original.yml, openapi/health-openapi-original.yml,\n  openapi/healthlake-openapi-original.yml, openapi/honeycode-openapi-original.yml, openapi/iam-openapi-original.yml,\n  openapi/identitystore-openapi-original.yml, openapi/imagebuilder-openapi-original.yml, openapi/importexport-openapi-original.yml,\n  openapi/inspector-openapi-original.yml, openapi/inspector-scan-openapi-original.yml, openapi/inspector2-openapi-original.yml,\n  openapi/internetmonitor-openapi-original.yml,\
  \ openapi/iot-data-openapi-original.yml, openapi/iot-jobs-data-openapi-original.yml,\n  openapi/iot-openapi-original.yml, openapi/iot-roborunner-openapi-original.yml, openapi/iot1click-devices-openapi-original.yml,\n  openapi/iot1click-projects-openapi-original.yml, openapi/iotanalytics-openapi-original.yml,\n  openapi/iotdeviceadvisor-openapi-original.yml, openapi/iotevents-data-openapi-original.yml,\n  openapi/iotevents-openapi-original.yml, openapi/iotfleethub-openapi-original.yml, openapi/iotfleetwise-openapi-original.yml,\n  openapi/iotsecuretunneling-openapi-original.yml, openapi/iotsitewise-openapi-original.yml,\n  openapi/iotthingsgraph-openapi-original.yml, openapi/iottwinmaker-openapi-original.yml, openapi/iotwireless-openapi-original.yml,\n  openapi/ivs-openapi-original.yml, openapi/ivs-realtime-openapi-original.yml, openapi/ivschat-openapi-original.yml,\n  openapi/kafka-openapi-original.yml, openapi/kafkaconnect-openapi-original.yml, openapi/kendra-openapi-original.yml,\n \
  \ openapi/kendra-ranking-openapi-original.yml, openapi/keyspaces-openapi-original.yml, openapi/kinesis-openapi-original.yml,\n  openapi/kinesis-video-archived-media-openapi-original.yml, openapi/kinesis-video-media-openapi-original.yml,\n  openapi/kinesis-video-signaling-openapi-original.yml, openapi/kinesis-video-webrtc-storage-openapi-original.yml,\n  openapi/kinesisanalytics-openapi-original.yml, openapi/kinesisanalyticsv2-openapi-original.yml,\n  openapi/kinesisvideo-openapi-original.yml, openapi/kms-openapi-original.yml, openapi/lakeformation-openapi-original.yml,\n  openapi/lambda-openapi-original.yml, openapi/launch-wizard-openapi-original.yml, openapi/lex-models-openapi-original.yml,\n  openapi/license-manager-linux-subscriptions-openapi-original.yml, openapi/license-manager-openapi-original.yml,\n  openapi/license-manager-user-subscriptions-openapi-original.yml, openapi/lightsail-openapi-original.yml,\n  openapi/location-openapi-original.yml, openapi/logs-openapi-original.yml,\
  \ openapi/lookoutequipment-openapi-original.yml,\n  openapi/lookoutmetrics-openapi-original.yml, openapi/lookoutvision-openapi-original.yml, openapi/m2-openapi-original.yml,\n  openapi/machinelearning-openapi-original.yml, openapi/macie2-openapi-original.yml, openapi/managedblockchain-openapi-original.yml,\n  openapi/managedblockchain-query-openapi-original.yml, openapi/marketplace-agreement-openapi-original.yml,\n  openapi/marketplace-catalog-openapi-original.yml, openapi/marketplace-deployment-openapi-original.yml,\n  openapi/marketplacecommerceanalytics-openapi-original.yml, openapi/mediaconnect-openapi-original.yml,\n  openapi/mediaconvert-openapi-original.yml, openapi/medialive-openapi-original.yml, openapi/mediapackage-openapi-original.yml,\n  openapi/mediapackage-vod-openapi-original.yml, openapi/mediapackagev2-openapi-original.yml,\n  openapi/mediastore-data-openapi-original.yml, openapi/mediastore-openapi-original.yml, openapi/mediatailor-openapi-original.yml,\n  openapi/medical-imaging-openapi-original.yml,\
  \ openapi/memorydb-openapi-original.yml, openapi/meteringmarketplace-openapi-original.yml,\n  openapi/mgn-openapi-original.yml, openapi/migration-hub-refactor-spaces-openapi-original.yml,\n  openapi/migrationhub-config-openapi-original.yml, openapi/migrationhuborchestrator-openapi-original.yml,\n  openapi/migrationhubstrategy-openapi-original.yml, openapi/mobile-openapi-original.yml, openapi/modelslexv2-openapi-original.yml,\n  openapi/monitoring-openapi-original.yml, openapi/mq-openapi-original.yml, openapi/mturk-requester-openapi-original.yml,\n  openapi/mwaa-openapi-original.yml, openapi/neptune-graph-openapi-original.yml, openapi/neptune-openapi-original.yml,\n  openapi/neptunedata-openapi-original.yml, openapi/network-firewall-openapi-original.yml, openapi/networkmanager-openapi-original.yml,\n  openapi/networkmonitor-openapi-original.yml, openapi/nimble-openapi-original.yml, openapi/oam-openapi-original.yml,\n  openapi/omics-openapi-original.yml, openapi/opensearch-openapi-original.yml,\
  \ openapi/opensearchserverless-openapi-original.yml,\n  openapi/opsworks-openapi-original.yml, openapi/opsworkscm-openapi-original.yml, openapi/organizations-openapi-original.yml,\n  openapi/osis-openapi-original.yml, openapi/outposts-openapi-original.yml, openapi/panorama-openapi-original.yml,\n  openapi/payment-cryptography-data-openapi-original.yml, openapi/payment-cryptography-openapi-original.yml,\n  openapi/pca-connector-ad-openapi-original.yml, openapi/personalize-events-openapi-original.yml,\n  openapi/personalize-openapi-original.yml, openapi/personalize-runtime-openapi-original.yml,\n  openapi/pi-openapi-original.yml, openapi/pinpoint-email-openapi-original.yml, openapi/pinpoint-openapi-original.yml,\n  openapi/pinpoint-sms-voice-v2-openapi-original.yml, openapi/pipes-openapi-original.yml, openapi/polly-openapi-original.yml,\n  openapi/pricing-openapi-original.yml, openapi/privatenetworks-openapi-original.yml, openapi/proton-openapi-original.yml,\n  openapi/qbusiness-openapi-original.yml,\
  \ openapi/qconnect-openapi-original.yml, openapi/qldb-openapi-original.yml,\n  openapi/qldb-session-openapi-original.yml, openapi/quicksight-openapi-original.yml, openapi/ram-openapi-original.yml,\n  openapi/rbin-openapi-original.yml, openapi/rds-data-openapi-original.yml, openapi/rds-openapi-original.yml,\n  openapi/redshift-data-openapi-original.yml, openapi/redshift-openapi-original.yml, openapi/redshift-serverless-openapi-original.yml,\n  openapi/rekognition-openapi-original.yml, openapi/repostspace-openapi-original.yml, openapi/resiliencehub-openapi-original.yml,\n  openapi/resource-explorer-2-openapi-original.yml, openapi/resource-groups-openapi-original.yml,\n  openapi/resourcegroupstaggingapi-openapi-original.yml, openapi/robomaker-openapi-original.yml,\n  openapi/rolesanywhere-openapi-original.yml, openapi/route53-openapi-original.yml, openapi/route53-recovery-cluster-openapi-original.yml,\n  openapi/route53-recovery-control-config-openapi-original.yml, openapi/route53-recovery-readiness-openapi-original.yml,\n\
  \  openapi/route53domains-openapi-original.yml, openapi/route53resolver-openapi-original.yml,\n  openapi/rum-openapi-original.yml, openapi/runtimelex-openapi-original.yml, openapi/runtimelexv2-openapi-original.yml,\n  openapi/runtimesagemaker-openapi-original.yml, openapi/s3-openapi-original.yml, openapi/s3control-openapi-original.yml,\n  openapi/s3outposts-openapi-original.yml, openapi/sagemaker-a2i-runtime-openapi-original.yml,\n  openapi/sagemaker-edge-openapi-original.yml, openapi/sagemaker-featurestore-runtime-openapi-original.yml,\n  openapi/sagemaker-geospatial-openapi-original.yml, openapi/sagemaker-metrics-openapi-original.yml,\n  openapi/sagemaker-openapi-original.yml, openapi/savingsplans-openapi-original.yml, openapi/scheduler-openapi-original.yml,\n  openapi/schemas-openapi-original.yml, openapi/sdb-openapi-original.yml, openapi/secretsmanager-openapi-original.yml,\n  openapi/securityhub-openapi-original.yml, openapi/securitylake-openapi-original.yml, openapi/serverlessrepo-openapi-original.yml,\n\
  \  openapi/service-quotas-openapi-original.yml, openapi/servicecatalog-appregistry-openapi-original.yml,\n  openapi/servicecatalog-openapi-original.yml, openapi/servicediscovery-openapi-original.yml,\n  openapi/sesv2-openapi-original.yml, openapi/shield-openapi-original.yml, openapi/signer-openapi-original.yml,\n  openapi/simspaceweaver-openapi-original.yml, openapi/sms-openapi-original.yml, openapi/sms-voice-openapi-original.yml,\n  openapi/snow-device-management-openapi-original.yml, openapi/snowball-openapi-original.yml,\n  openapi/sns-openapi-original.yml, openapi/sqs-openapi-original.yml, openapi/ssm-contacts-openapi-original.yml,\n  openapi/ssm-incidents-openapi-original.yml, openapi/ssm-openapi-original.yml, openapi/ssm-sap-openapi-original.yml,\n  openapi/sso-admin-openapi-original.yml, openapi/sso-oidc-openapi-original.yml, openapi/sso-openapi-original.yml,\n  openapi/states-openapi-original.yml, openapi/storagegateway-openapi-original.yml, openapi/streamsdynamodb-openapi-original.yml,\n\
  \  openapi/sts-openapi-original.yml, openapi/supplychain-openapi-original.yml, openapi/support-app-openapi-original.yml,\n  openapi/support-openapi-original.yml, openapi/swf-openapi-original.yml, openapi/synthetics-openapi-original.yml,\n  openapi/textract-openapi-original.yml, openapi/timestream-query-openapi-original.yml, openapi/timestream-write-openapi-original.yml,\n  openapi/tnb-openapi-original.yml, openapi/transcribe-openapi-original.yml, openapi/transcribe-streaming-openapi-original.yml,\n  openapi/transfer-openapi-original.yml, openapi/translate-openapi-original.yml, openapi/trustedadvisor-openapi-original.yml,\n  openapi/verifiedpermissions-openapi-original.yml, openapi/voice-id-openapi-original.yml, openapi/vpc-lattice-openapi-original.yml,\n  openapi/waf-openapi-original.yml, openapi/waf-regional-openapi-original.yml, openapi/wafv2-openapi-original.yml,\n  openapi/wellarchitected-openapi-original.yml, openapi/wisdom-openapi-original.yml, openapi/workdocs-openapi-original.yml,\n\
  \  openapi/worklink-openapi-original.yml, openapi/workmail-openapi-original.yml, openapi/workmailmessageflow-openapi-original.yml,\n  openapi/workspaces-openapi-original.yml, openapi/workspaces-thin-client-openapi-original.yml,\n  openapi/workspaces-web-openapi-original.yml, openapi/xray-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5181\n  by_action_class:\n    acting: 3518\n    connected: 1663\n  by_consequence:\n    write: 3248\n    read: 1663\n    safety-critical: 147\n    physical: 123\n  human_in_the_loop_required: 147\noperations:\n- path: /archive-rule\n  method: put\n  operationId: amazonWebServicesApplyArchiveRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /policy/generation/{jobId}\n  method: get\n  operationId: amazonWebServicesGetGeneratedPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /policy/check-access-not-granted\n  method: post\n  operationId: amazonWebServicesCheckAccessNotGranted\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /policy/check-no-new-access\n  method: post\n  operationId: amazonWebServicesCheckNoNewAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access-preview\n  method: get\n  operationId: amazonWebServicesListAccessPreviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analyzer\n  method: get\n  operationId: amazonWebServicesListAnalyzers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analyzer/{analyzerName}/archive-rule\n  method: get\n  operationId: amazonWebServicesListArchiveRules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analyzer/{analyzerName}\n  method: get\n  operationId: amazonWebServicesGetAnalyzer\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /analyzer/{analyzerName}/archive-rule/{ruleName}\n  method: put\n  operationId: amazonWebServicesUpdateArchiveRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /access-preview/{accessPreviewId}\n  method: post\n  operationId: amazonWebServicesListAccessPreviewFindings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /analyzed-resource\n  method: post\n  operationId:\
  \ amazonWebServicesListAnalyzedResources\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /finding/{id}\n  method: get\n  operationId: amazonWebServicesGetFinding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /findingv2/{id}\n  method: get\n  operationId: amazonWebServicesGetFindingV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /finding\n  method: put\n  operationId: amazonWebServicesUpdateFindings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /findingv2\n  method: post\n  operationId: amazonWebServicesListFindingsV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /policy/generation\n  method: put\n  operationId: amazonWebServicesStartPolicyGeneration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tags/{resourceArn}\n  method: delete\n  operationId: amazonWebServicesUntagResource\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /resource/scan\n  method: post\n  operationId: amazonWebServicesStartResourceScan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /policy/validation\n  method: post\n  operationId: amazonWebServicesValidatePolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deleteAlternateContact\n\
  \  method: post\n  operationId: amazonWebServicesDeleteAlternateContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /disableRegion\n  method: post\n  operationId: amazonWebServicesDisableRegion\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /enableRegion\n  method: post\n  operationId: amazonWebServicesEnableRegion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getAlternateContact\n  method: post\n  operationId: amazonWebServicesGetAlternateContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getContactInformation\n  method: post\n  operationId: amazonWebServicesGetContactInformation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getRegionOptStatus\n  method: post\n  operationId: amazonWebServicesGetRegionOptStatus\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listRegions\n  method: post\n  operationId: amazonWebServicesListRegions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /putAlternateContact\n  method: post\n  operationId: amazonWebServicesPutAlternateContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /putContactInformation\n\
  \  method: post\n  operationId: amazonWebServicesPutContactInformation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /\n  method: post\n  operationId: amazonWebServicesUpdateCertificateOptions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /\n  method: post\n  operationId: amazonWebServicesUpdateCertificateAuthority\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/alertmanager/definition\n  method: put\n  operationId: amazonWebServicesPutAlertManagerDefinition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/logging\n  method: put\n  operationId: amazonWebServicesUpdateLoggingConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/rulegroupsnamespaces\n  method: get\n  operationId: amazonWebServicesListRuleGroupsNamespaces\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scrapers\n  method: get\n  operationId: amazonWebServicesListScrapers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces\n  method: get\n  operationId: amazonWebServicesListWorkspaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}/rulegroupsnamespaces/{name}\n  method: put\n  operationId: amazonWebServicesPutRuleGroupsNamespace\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /scrapers/{scraperId}\n  method: get\n  operationId: amazonWebServicesDescribeScraper\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /workspaces/{workspaceId}\n  method: get\n  operationId: amazonWebServicesDescribeWorkspace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /scraperconfiguration\n  method: get\n  operationId: amazonWebServicesGetDefaultScraperConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tags/{resourceArn}\n  method: delete\n  operationId: amazonWebServicesUntagResource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n   \
  \ escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workspaces/{workspaceId}/alias\n  method: post\n  operationId: amazonWebServicesUpdateWorkspaceAlias\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps\n  method: get\n  operationId: amazonWebServicesListApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/{appId}/backendenvironments\n  method: get\n  operationId: amazonWebServicesListBackendEnvironments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /apps/{appId}/branches\n  method: get\n  operationId: amazonWebServicesListBranches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/{appId}/branches/{branchName}/deployments\n  method: post\n  operationId: amazonWebServicesCreateDeployment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/{appId}/domains\n  method: get\n  operationId: amazonWebServicesListDomainAssociations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/{appId}/webhooks\n  method: get\n  operationId: amazonWebServicesListWebhooks\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/{appId}\n  method: post\n  operationId: amazonWebServicesUpdateApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/{appId}/backendenvironments/{environmentName}\n  method: get\n  operationId: amazonWebServicesGetBackendEnvironment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/{appId}/branches/{branchName}\n  method: post\n  operationId: amazonWebServicesUpdateBranch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/{appId}/domains/{domainName}\n  method: post\n  operationId: amazonWebServicesUpdateDo\n\n# --- truncated at 32 KB (1711 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/amazon-web-services/refs/heads/main/agentic-access/amazon-web-services-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-web-services/refs/heads/main/agentic-access/amazon-web-services-agentic-access.yml
summary_line: 5181 operations · 3518 acting · 147 human-in-the-loop
tags:
- Amazon
- Cloud
- Network
- Index
---
