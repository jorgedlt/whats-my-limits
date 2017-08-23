# whats-my-limits
discover your service limits from the command line - whats-my-limits

# discover your service limits from the command line
aws support describe-trusted-advisor-check-result \
  --check-id eW7HH0l7J9 \
  --query 'result.sort_by(flaggedResources[?status!="ok"],&metadata[2])[].metadata' \
  --region us-east-1 \
    --output text
#

# also see 
https://awslimitchecker.readthedocs.io/en/latest/getting_started.html
