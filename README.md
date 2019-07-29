# Send AWS cloudwatch notifications to Slack channel
# AWS is now providing free service called AWS Chatbot to do the same thing.

1. Create s3 bucket and push zipped .py file
2. Run cloudformation with provided template to create a stack

aws cloudformation create-stack --stack-name cw-to-slack-notifications --template-body file://templates/cloud_watch_to_slack.yaml --parameters file://params.json --region eu-west-1 --profile default --capabilities CAPABILITY_IAM
