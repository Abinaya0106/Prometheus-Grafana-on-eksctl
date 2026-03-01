# IRSA Setup (IAM Roles for Service Accounts)

## Why IRSA?

Secure way for pods to access AWS services without static credentials.

## Steps

1.  Extract OIDC ID
2.  Associate IAM OIDC provider
3.  Create IAM Service Account
4.  Attach AmazonEBSCSIDriverPolicy
5.  Install EBS CSI Addon

This enables dynamic EBS volume provisioning securely.
