# Amazon CloudWatch Permissions Reference<a name="permissions-reference-cw"></a>

When you are setting up [Access Control](auth-and-access-control-cw.md#access-control-cw) and writing permissions policies that you can attach to an IAM identity \(identity\-based policies\), you can use the following table as a reference\. The table lists each CloudWatch API operation and the corresponding actions for which you can grant permissions to perform the action\. You specify the actions in the policy's `Action` field, and you specify a wildcard character \(\*\) as the resource value in the policy's `Resource` field\.

You can use AWS\-wide condition keys in your CloudWatch policies to express conditions\. For a complete list of AWS\-wide keys, see [AWS Global and IAM Condition Context Keys](http://docs.aws.amazon.com/IAM/latest/UserGuide/reference_policies_condition-keys.html) in the *IAM User Guide*\.

**Note**  
To specify an action, use the `cloudwatch:` prefix followed by the API operation name\. For example: `cloudwatch:GetMetricStatistics`, `cloudwatch:ListMetrics`, or `cloudwatch:*` \(for all CloudWatch actions\)\.

**Tables**

+ [CloudWatch API Operations and Required Permissions](http://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/permissions-reference-cw.html#cw-permissions-table)

+ [CloudWatch Events API Operations and Required Permissions](http://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/permissions-reference-cw.html#cwe-permissions-table)

+ [CloudWatch Logs API Operations and Required Permissions](http://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/permissions-reference-cw.html#cwl-permissions-table)

+ [Amazon EC2 API Operations and Required Permissions](http://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/permissions-reference-cw.html#cw-ec2-permissions-table)

+ [Auto Scaling API Operations and Required Permissions](http://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/permissions-reference-cw.html#cw-as-permissions-table)


**CloudWatch API Operations and Required Permissions for Actions**  

| CloudWatch API Operations | Required Permissions \(API Actions\) | 
| --- | --- | 
|  [DeleteAlarms](http://docs.aws.amazon.com/AmazonCloudWatch/latest/APIReference/API_DeleteAlarms.html)  |  `cloudwatch:DeleteAlarms` Required to delete an alarm\.  | 
|  [DeleteDashboards](http://docs.aws.amazon.com/AmazonCloudWatch/latest/APIReference/API_DeleteDashboards.html)  |  `cloudwatch:DeleteDashboards` Required to delete a dashboard\.  | 
|  [DescribeAlarmHistory](http://docs.aws.amazon.com/AmazonCloudWatch/latest/APIReference/API_DescribeAlarmHistory.html)  |  `cloudwatch:DescribeAlarmHistory` Required to view alarm history\.  | 
|  [DescribeAlarms](http://docs.aws.amazon.com/AmazonCloudWatch/latest/APIReference/API_DescribeAlarms.html)  |  `cloudwatch:DescribeAlarms` Required to retrieve alarm information by name\.  | 
|  [DescribeAlarmsForMetric](http://docs.aws.amazon.com/AmazonCloudWatch/latest/APIReference/API_DescribeAlarmsForMetric.html)  |  `cloudwatch:DescribeAlarmsForMetric` Required to view alarms for a metric\.  | 
|  [DisableAlarmActions](http://docs.aws.amazon.com/AmazonCloudWatch/latest/APIReference/API_DisableAlarmActions.html)  |  `cloudwatch:DisableAlarmActions` Required to disable an alarm action\.  | 
|  [EnableAlarmActions](http://docs.aws.amazon.com/AmazonCloudWatch/latest/APIReference/API_EnableAlarmActions.html)  |  `cloudwatch:EnableAlarmActions` Required to enable an alarm action\.  | 
|  [GetDashboard](http://docs.aws.amazon.com/AmazonCloudWatch/latest/APIReference/API_GetDashboard.html)  |  `cloudwatch:GetDashboard` Required to display data about existing dashboards\.  | 
|  [GetMetricData](http://docs.aws.amazon.com/AmazonCloudWatch/latest/APIReference/API_GetMetricData.html)  |  `cloudwatch:GetMetricData` Required to retrieve large batches of metric data and perform metric math on that data\.  | 
|  [GetMetricStatistics](http://docs.aws.amazon.com/AmazonCloudWatch/latest/APIReference/API_GetMetricStatistics.html)  |  `cloudwatch:GetMetricStatistics` Required to view graphs in other parts of the CloudWatch console and in dashboard widgets\.  | 
|  [ListDashboards](http://docs.aws.amazon.com/AmazonCloudWatch/latest/APIReference/API_ListDashboards.html)  |  `cloudwatch:ListDashboards` Required to view the list of CloudWatch dashboards in your account\.  | 
|  [ListMetrics](http://docs.aws.amazon.com/AmazonCloudWatch/latest/APIReference/API_ListMetrics.html)  |  `cloudwatch:ListMetrics` Required to view or search metric names within the CloudWatch console and in the CLI\. Required to select metrics on dashboard widgets\.  | 
|  [PutDashboard](http://docs.aws.amazon.com/AmazonCloudWatch/latest/APIReference/API_PutDashboard.html)  |  `cloudwatch:PutDashboard` Required to create a dashboard or update an existing dashboard\.  | 
|  [PutMetricAlarm](http://docs.aws.amazon.com/AmazonCloudWatch/latest/APIReference/API_PutMetricAlarm.html)  |  `cloudwatch:PutMetricAlarm` Required to create or update an alarm\.  | 
|  [PutMetricData](http://docs.aws.amazon.com/AmazonCloudWatch/latest/APIReference/API_PutMetricData.html)  |  `cloudwatch:PutMetricData` Required to create metrics\.  | 
|  [SetAlarmState](http://docs.aws.amazon.com/AmazonCloudWatch/latest/APIReference/API_SetAlarmState.html)  |  `cloudwatch:SetAlarmState` Required to manually set an alarm's state\.  | 


**CloudWatch Events API Operations and Required Permissions for Actions**  

| CloudWatch Events API Operations | Required Permissions \(API Actions\) | 
| --- | --- | 
|  [DeleteRule](http://docs.aws.amazon.com/AmazonCloudWatchEvents/latest/APIReference/API_DeleteRule.html)  |  `events:DeleteRule` Required to delete a rule\.  | 
|  [DescribeRule](http://docs.aws.amazon.com/AmazonCloudWatchEvents/latest/APIReference/API_DescribeRule.html)  |  `events:DescribeRule` Required to list the details about a rule\.  | 
|  [DisableRule](http://docs.aws.amazon.com/AmazonCloudWatchEvents/latest/APIReference/API_DisableRule.html)  |  `events:DisableRule` Required to disable a rule\.  | 
|  [EnableRule](http://docs.aws.amazon.com/AmazonCloudWatchEvents/latest/APIReference/API_EnableRule.html)  |  `events:EnableRule` Required to enable a rule\.  | 
|  [ListRuleNamesByTarget](http://docs.aws.amazon.com/AmazonCloudWatchEvents/latest/APIReference/API_ListRuleNamesByTarget.html)  |  `events:ListRuleNamesByTarget` Required to list rules associated with a target\.  | 
|  [ListRules](http://docs.aws.amazon.com/AmazonCloudWatchEvents/latest/APIReference/API_ListRules.html)  |  `events:ListRules` Required to list all rules in your account\.  | 
|  [ListTargetsByRule](http://docs.aws.amazon.com/AmazonCloudWatchEvents/latest/APIReference/API_ListTargetsByRule.html)  |  `events:ListTargetsByRule` Required to list all targets associated with a rule\.  | 
|  [PutEvents](http://docs.aws.amazon.com/AmazonCloudWatchEvents/latest/APIReference/API_PutEvents.html)  |  `events:PutEvents` Required to add custom events that can be matched to rules\.  | 
|  [PutRule](http://docs.aws.amazon.com/AmazonCloudWatchEvents/latest/APIReference/API_PutRule.html)  |  `events:PutRule` Required to create or update a rule\.  | 
|  [PutTargets](http://docs.aws.amazon.com/AmazonCloudWatchEvents/latest/APIReference/API_PutTargets.html)  |  `events:PutTargets` Required to add targets to a rule\.  | 
|  [RemoveTargets](http://docs.aws.amazon.com/AmazonCloudWatchEvents/latest/APIReference/API_RemoveTargets.html)  |  `events:RemoveTargets` Required to remove a target from a rule\.  | 
|  [TestEventPattern](http://docs.aws.amazon.com/AmazonCloudWatchEvents/latest/APIReference/API_TestEventPattern.html)  |  `events:TestEventPattern` Required to test an event pattern against a given event\.  | 


**CloudWatch Logs API Operations and Required Permissions for Actions**  

| CloudWatch Logs API Operations | Required Permissions \(API Actions\) | 
| --- | --- | 
|  [CancelExportTask](http://docs.aws.amazon.com/AmazonCloudWatchLogs/latest/APIReference/API_CancelExportTask.html)  |  `logs:CancelExportTask` Required to cancel a pending or running export task\.  | 
|  [CreateExportTask](http://docs.aws.amazon.com/AmazonCloudWatchLogs/latest/APIReference/API_CreateExportTask.html)  |  `logs:CreateExportTask` Required to export data from a log group to an Amazon S3 bucket\.  | 
|  [CreateLogGroup](http://docs.aws.amazon.com/AmazonCloudWatchLogs/latest/APIReference/API_CreateLogGroup.html)  |  `logs:CreateLogGroup` Required to create a new log group\.  | 
|  [CreateLogStream](http://docs.aws.amazon.com/AmazonCloudWatchLogs/latest/APIReference/API_CreateLogStream.html)  |  `logs:CreateLogStream` Required to create a new log stream in a log group\.  | 
|  [DeleteDestination](http://docs.aws.amazon.com/AmazonCloudWatchLogs/latest/APIReference/API_DeleteDestination.html)  |  `logs:DeleteDestination` Required to delete a log destination and disables any subscription filters to it\.  | 
|  [DeleteLogGroup](http://docs.aws.amazon.com/AmazonCloudWatchLogs/latest/APIReference/API_DeleteLogGroup.html)  |  `logs:DeleteLogGroup` Required to delete a log group and any associated archived log events\.  | 
|  [DeleteLogStream](http://docs.aws.amazon.com/AmazonCloudWatchLogs/latest/APIReference/API_DeleteLogStream.html)  |  `logs:DeleteLogStream` Required to delete a log stream and any associated archived log events\.  | 
|  [DeleteMetricFilter](http://docs.aws.amazon.com/AmazonCloudWatchLogs/latest/APIReference/API_DeleteMetricFilter.html)  |  `logs:DeleteMetricFilter` Required to delete a metric filter associated with a log group\.  | 
|  [DeleteRetentionPolicy](http://docs.aws.amazon.com/AmazonCloudWatchLogs/latest/APIReference/API_DeleteRetentionPolicy.html)  |  `logs:DeleteRetentionPolicy` Required to delete a log group's retention policy\.  | 
|  [DeleteSubscriptionFilter](http://docs.aws.amazon.com/AmazonCloudWatchLogs/latest/APIReference/API_DeleteSubscriptionFilter.html)  |  `logs:DeleteSubscriptionFilter` Required to delete the subscription filter associated with a log group\.  | 
|  [DescribeDestinations](http://docs.aws.amazon.com/AmazonCloudWatchLogs/latest/APIReference/API_DescribeDestinations.html)  |  `logs:DescribeDestinations` Required to view all destinations associated with the account\.  | 
|  [DescribeExportTasks](http://docs.aws.amazon.com/AmazonCloudWatchLogs/latest/APIReference/API_DescribeExportTasks.html)  |  `logs:DescribeExportTasks` Required to view all export tasks associated with the account\.  | 
|  [DescribeLogGroups](http://docs.aws.amazon.com/AmazonCloudWatchLogs/latest/APIReference/API_DescribeLogGroups.html)  |  `logs:DescribeLogGroups` Required to view all log groups associated with the account\.  | 
|  [DescribeLogStreams](http://docs.aws.amazon.com/AmazonCloudWatchLogs/latest/APIReference/API_DescribeLogStreams.html)  |  `logs:DescribeLogStreams` Required to view all log streams associated with a log group\.  | 
|  [DescribeMetricFilters](http://docs.aws.amazon.com/AmazonCloudWatchLogs/latest/APIReference/API_DescribeMetricFilters.html)  |  `logs:DescribeMetricFilters` Required to view all metrics associated with a log group\.  | 
|  [DescribeSubscriptionFilters](http://docs.aws.amazon.com/AmazonCloudWatchLogs/latest/APIReference/API_DescribeSubscriptionFilters.html)  |  `logs:DescribeSubscriptionFilters` Required to view all subscription filters associated with a log group\.  | 
|  [FilterLogEvents](http://docs.aws.amazon.com/AmazonCloudWatchLogs/latest/APIReference/API_FilterLogEvents.html)  |  `logs:FilterLogEvents` Required to sort log events by log group filter pattern\.  | 
|  [GetLogEvents](http://docs.aws.amazon.com/AmazonCloudWatchLogs/latest/APIReference/API_GetLogEvents.html)  |  `logs:GetLogEvents` Required to retrieve log events from a log stream\.  | 
|  [ListTagsLogGroup](http://docs.aws.amazon.com/AmazonCloudWatchLogs/latest/APIReference/API_ListTagsLogGroup.html)  |  `logs:ListTagsLogGroup` Required to list the tags associated with a log group\.  | 
|  [PutDestination](http://docs.aws.amazon.com/AmazonCloudWatchLogs/latest/APIReference/API_PutDestination.html)  |  `logs:PutDestination` Required to create or update a destination log stream \(such as a Kinesis stream\)\.  | 
|  [PutDestinationPolicy](http://docs.aws.amazon.com/AmazonCloudWatchLogs/latest/APIReference/API_PutDestinationPolicy.html)  |  `logs:PutDestinationPolicy` Required to create or update an access policy associated with an existing log destination\.  | 
|  [PutLogEvents](http://docs.aws.amazon.com/AmazonCloudWatchLogs/latest/APIReference/API_PutLogEvents.html)  |  `logs:PutLogEvents` Required to upload a batch of log events to a log stream\.  | 
|  [PutMetricFilter](http://docs.aws.amazon.com/AmazonCloudWatchLogs/latest/APIReference/API_PutMetricFilter.html)  |  `logs:PutMetricFilter` Required to create or update a metric filter and associate it with a log group\.  | 
|  [PutRetentionPolicy](http://docs.aws.amazon.com/AmazonCloudWatchLogs/latest/APIReference/API_PutRetentionPolicy.html)  |  `logs:PutRetentionPolicy` Required to set the number of days to keep log events \(retention\) in a log group\.  | 
|  [PutSubscriptionFilter](http://docs.aws.amazon.com/AmazonCloudWatchLogs/latest/APIReference/API_PutSubscriptionFilter.html)  |  `logs:PutSubscriptionFilter` Required to create or update a subscription filter and associate it with a log group\.  | 
|  [TestMetricFilter](http://docs.aws.amazon.com/AmazonCloudWatchLogs/latest/APIReference/API_TestMetricFilter.html)  |  `logs:TestMetricFilter` Required to test a filter pattern against a sampling of log event messages\.  | 


**Amazon EC2 API Operations and Required Permissions for Actions**  

| Amazon EC2 API Operations | Required Permissions \(API Actions\) | 
| --- | --- | 
|  [DescribeInstanceStatus](http://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_DescribeInstanceStatus.html)  |  `ec2:DescribeInstanceStatus` Required to view EC2 instance status details\.  | 
|  [DescribeInstances](http://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_DescribeInstances.html)  |  `ec2:DescribeInstances` Required to view EC2 instance details\.  | 
|  [RebootInstances](http://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_RebootInstances.html)  |  `ec2:RebootInstances` Required to reboot an EC2 instance\.  | 
|  [StopInstances](http://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_StopInstances.html)  |  `ec2:StopInstances` Required to stop an EC2 instance\.  | 
|  [TerminateInstances](http://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_TerminateInstances.html)  |  `ec2:TerminateInstances` Required to terminate an EC2 instance\.  | 


**Auto Scaling API Operations and Required Permissions for Actions**  

| Auto Scaling API Operations | Required Permissions \(API Actions\) | 
| --- | --- | 
|  Scaling  |  `autoscaling:Scaling` Required to scale an Auto Scaling group\.  | 
|  Trigger  |  `autoscaling:Trigger` Required to trigger an Auto Scaling action\.  | 