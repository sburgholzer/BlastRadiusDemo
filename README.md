# Blast Radius Demo

Demo repo showing [Blast Radius](https://github.com/sburgholzer/BlastRadius) in action as a GitHub Action.

## What This Demonstrates

1. A CDK stack is deployed (ECS Fargate + Aurora + ALB + Lambda)
2. A PR proposes a risky change (restrict security group + resize database)
3. Blast Radius automatically analyzes the change and comments on the PR with:
   - Risk scores for all affected resources
   - AI-powered deployment recommendation
   - Pass/fail verdict based on threshold + AI gate

## Try It

1. The `main` branch has the baseline infrastructure
2. Create a branch, make a risky change to `lib/baseline-stack.ts`
3. Open a PR → Blast Radius runs automatically and comments results
