# 3.1 Cloud Infrastructure

Created time: 14 mars 2025 16:46
Last edited by: OLB_
Last edited time: 5 avril 2025 14:07

- responsability matrix

![image.png](image%2031.png)

- Hybrid cloud
    - complexity
    - authentication across platform
    - logs are diverse
    - data leak risk (lot of data in transit)
- Cloud Vendors - Third parties
    - vendor risk management policy is necessary
    - do vendor risk assessment
        - due diligence
        - vendor audits / right to audit
    - include them in incident response
    - constant monitoring
- Infra as code IAC
    - describe infrastructure in a code
    - manage version of infrastructure like code version (modifications stored with GIT)
    - buid always the same infrastructure (like it is in the code)
- Serverless Architecture
    - FAAS - function as a service
    - code runs in a stateless container
    - easy to scale
- Microservices
    - replace monolithic app
    - use APIs
    - more scalable
    - more resilient
    - more secure (containment)
- MSP : Managed Service Provider are service organizations that provide
information technology as a service to their customers.
- When MSPs offer security services, they are commonly referred to
as managed security service providers (MSSPs)
- Cloud Security Alliance (CSA) is an industry organization focused
on developing and promoting best practices in cloud security
    - They developed the Cloud Controls Matrix (CCM) as a reference document
    designed to help organizations understand the appropriate use of
    cloud security controls
- **Edge computing** approaches seek to address this issue by placing
some processing power on the remote sensors, allowing them to
preprocess data before shipping it back to the cloud
- **Fog computing** is a related concept that uses IoT gateway devices
that are located in close physical proximity to the sensors. The
sensors themselves don't necessarily have processing power, but
they send data to their local gateway that performs preprocessing
before sending the results to the cloud.
- AWS Security groups
    - set of rules for network traffic that are substantially the same as a firewall ruleset
    - kind of firewall settings for virtual servers
- Virtual Private Cloud (VPC)
    - Similar to VLAN to create subnets in cloud environment
- **Cloud transit gateways** extend this model even further, allowing the direct interconnection of
cloud VPCs with on-premises VLANs for hybrid cloud operations

<aside>
👉

**Auditability i**s an important component of cloud governance. Cloud
computing contracts should include language guaranteeing the right of
the customer to audit cloud service providers. They may choose to
perform these audits themselves or engage a third party to perform an
independent audit. The use of auditing is essential to providing
customers with the assurance that the provider is operating in a secure
manner and meeting its contractual data protection obligations.

</aside>

### Resource Policies

Cloud providers offer resource policies that customers may use to limit
the actions that users of their accounts may take

- **IAM Policies** sont principalement utilisées pour gérer les permissions des utilisateurs et des rôles.
- **Service Quotas** limitent le nombre de ressources que vous pouvez utiliser dans votre compte AWS.
- **Resource Policies** contrôlent l'accès à des ressources spécifiques.
- **AWS Security groups** : règles de type firewall d’accès aux protocoles,services et aux ports
- **SCPs** : Les Service Control Policies pour limiter le nombre d'instances EC2 qu'un compte peut lancer.

L**es SCPs et les Resource Policies sont complémentaires** et peuvent être utilisées ensemble pour mettre en place une stratégie de sécurité robuste sur AWS. Les SCPs permettent de définir des limites globales sur ce que les comptes peuvent faire, tandis que les Resource Policies permettent de contrôler l'accès à des ressources spécifiques

**IAM Policies**

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Effect": "Allow",
      "Action": [
        "s3:ListBucket",
        "s3:GetObject",
        "s3:PutObject"
      ],
      "Resource": [
        "arn:aws:s3:::example-bucket",
        "arn:aws:s3:::example-bucket/*"
      ]
    }
  ]
}
```

**SCP Service Control Policies**

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Effect": "Deny",
      "Action": [
        "ec2:TerminateInstances",
        "rds:DeleteDBInstance"
      ],
      "Resource": "*"
    }
  ]
}
```

**Security groups**

```json
{
  "AWSTemplateFormatVersion": "2010-09-09",
  "Resources": {
    "MySecurityGroup": {
      "Type": "AWS::EC2::SecurityGroup",
      "Properties": {
        "GroupName": "MySecurityGroup",
        "GroupDescription": "Security group allowing HTTP and SSH access",
        "SecurityGroupIngress": [
          {
            "IpProtocol": "tcp",
            "FromPort": 80,
            "ToPort": 80,
            "CidrIp": "0.0.0.0/0"
          },
          {
            "IpProtocol": "tcp",
            "FromPort": 22,
            "ToPort": 22,
            "CidrIp": "0.0.0.0/0"
          }
        ],
        "SecurityGroupEgress": [
          {
            "IpProtocol": "-1",
            "CidrIp": "0.0.0.0/0"
          }
        ],
        "VpcId": "vpc-12345678"
      }
    }
  }
}
```

**Ressources policies**

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Effect": "Allow",
      "Action": [
        "s3:ListBucket",
        "s3:GetObject",
        "s3:PutObject"
      ],
      "Resource": [
        "arn:aws:s3:::example-bucket",
        "arn:aws:s3:::example-bucket/*"
      ]
    }
  ]
}
```