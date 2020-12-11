# Logging with fluentd - works when cluster is deployed

1) Clone or create deploylogging.yaml file
2) Edit file 6th line, change to your cluster region (eu-west-1 - Ireland by default)
3) Run kubectl -f deploylogging.yaml
4) Open aws console IAM > Roles > open your AWS service: ec2 role > press Attach policies > search and check CloudWatchAgentServerPolicy > Attach policy
5) Test by opening CloudWatch > Logs, should show you three log groups - application, host, dataplane
