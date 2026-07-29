# AWS Cost Optimization Checklist

A practical checklist for reducing your AWS bill without breaking production.
Based on real patterns seen across startup and SMB AWS accounts.

## Compute
- [ ] Right-size EC2 instances based on actual CPU/memory utilization (not guesswork)
- [ ] Use Savings Plans or Reserved Instances for steady-state workloads
- [ ] Move dev/staging environments to smaller instance types or scheduled shutdown
- [ ] Check for idle/unattached EBS volumes and unused Elastic IPs

## Storage
- [ ] Set S3 lifecycle policies to move cold data to Glacier/Infrequent Access
- [ ] Audit S3 buckets for orphaned or duplicate data
- [ ] Review RDS storage type — gp3 vs gp2 pricing differences

## Networking
- [ ] Check NAT Gateway data processing costs — often a hidden bill driver
- [ ] Review data transfer costs between regions/AZs
- [ ] Use CloudFront to reduce origin data transfer costs where applicable

## Monitoring & Governance
- [ ] Enable AWS Cost Explorer and set budget alerts
- [ ] Tag resources consistently for cost allocation visibility
- [ ] Review Trusted Advisor cost recommendations monthly

## Further reading
Full guide: [How to Reduce Your AWS Monthly Bill](https://cloudsyncpk.com/blog/how-to-reduce-your-aws-monthly-bill)

---
Maintained by [CloudSync](https://cloudsyncpk.com) — AWS cloud infrastructure and cost optimization consulting.
