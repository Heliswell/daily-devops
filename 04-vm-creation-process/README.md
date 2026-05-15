# Day 04 - AWS EC2 & Automation Basics

## Topics Covered

- What does the EC2 instance creation process look like?
- How is scripting/automation used in AWS?
- Different ways to automate EC2 instance creation

---

# Concepts

## EC2 Instance Creation Flow

The EC2 instance creation process follows this workflow:

```text
User / CLI / SDK
        ↓
AWS API Request
        ↓
Authentication Check
        ↓
IAM Permission Check
        ↓
Parameter Validation
        ↓
Resource Availability Check
        ↓
EC2 Service Creates Instance
        ↓
Response Returned
```

This process ensures:
- authentication
- authorization
- valid configuration
- available infrastructure resources

before the EC2 instance is launched.

---

## How is Scripting/Automation Used in AWS?

If you only need to create 1–2 EC2 instances, using the AWS Console manually is manageable.

However, in real-world environments, engineers may need to create:
- hundreds of EC2 instances
- storage resources
- networking configurations
- monitoring setups

Automation helps engineers:
- reduce manual work
- improve consistency
- deploy infrastructure faster
- manage cloud resources efficiently

Using scripts and Infrastructure as Code (IaC), large-scale infrastructure can be created using just a few configuration files.

---

## Different Ways to Automate EC2 Instance Creation

### AWS CLI
Command-line interface used to manage AWS services directly from the terminal.

### AWS CDK
AWS Cloud Development Kit allows infrastructure creation using programming languages.

### AWS CloudFormation (CFT)
Infrastructure as Code service used to provision AWS resources through YAML or JSON templates.

### AWS API
AWS services can be controlled programmatically through API requests.

### Terraform
Popular Infrastructure as Code tool used for cloud automation across multiple cloud providers.


---

# Key Takeaways

- AWS services are heavily automation-driven.
- APIs are the foundation of cloud automation.
- Infrastructure can be managed efficiently using scripting and IaC tools.
- AWS CLI provides direct terminal-based control over AWS resources.

---

# Resources

[AWS EC2 Documentation] https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/concepts.html

DATE DevOps Playlist

---

# Conclusion

Automation is an important part of DevOps and cloud computing. It helps create infrastructure faster, reduces manual work, and improves efficiency.

