# Evaluate a regulatory compliance strategy

Learn how to evaluate a regulatory compliance strategy for your
organization and leverage the right set of tools to measure progress.

**Learning Objectives**

In this module, you will learn how to:

- Interpret compliance requirements and their technical capabilities

- Evaluate infrastructure compliance by using Microsoft Defender for
    Cloud

- Interpret compliance scores and recommend actions to resolve issues
    or improve security

- Design and validate implementation of Azure Policy

- Design for data residency Requirements

- Translate privacy requirements into requirements for security
    solutions

## 2.1.1 Interpret compliance requirements and their technical capabilities

Cloud governance is the product of an ongoing adoption effort over time,
as a true lasting transformation doesn\'t happen overnight. It becomes
critical to evaluate risk tolerance to inform minimally invasive
policies that govern cloud adoption and manage risks. In some
industries, third-party compliance affects initial policy creation.

Regulatory organizations frequently publish standards and updates to
help define good security practices so that organizations can avoid
negligence. The purpose and scope of these standards, and regulations
vary. The security requirements, however, can influence the design for
data protection and retention, network access, and system security.

Once the business risks are mapped and converted into decisions to
policy statements, the cybersecurity architect will be able to establish
the regulatory compliance strategy. This strategy also takes into
consideration the industry in which the organization belongs or the type
of transactions that the organization performs. A good compliance
strategy needs to ensure that security controls are implemented to
directly map regulatory compliance requirements, that's why is important
to have full visibility of the type of business, transactions, and
overall business requirements before establishing a regulatory
compliance strategy.

Noncompliance can lead to fines or other business impact. Work with your
regulators and carefully review the standard to understand both the
intent and the literal wording of each requirement. Here are some
questions that may help you understand each requirement.

- How is compliance measured?

- Who approves if the workload meets the requirements?

- Are there processes for obtaining attestations?

- What are the documentation requirements?

In traditional governance and incremental governance, corporate policy
creates the working definition of governance. Most IT governance actions
seek to implement technology to monitor, enforce, operate, and automate
those corporate policies. Cloud governance is built on similar concepts.

![Corporate governance and governance
disciplines](media\DefineCorporatePolicy.png)

*Figure 1: Corporate governance and governance disciplines.*

The image above demonstrates the interactions between business risk,
policy and compliance, and monitoring and enforcement to create a
governance strategy. During the corporate policy definition you will
need to first evaluate the business risk, which includes the
investigation of current cloud adoption plans and data classification.
In this phase you will work with the business to balance risk tolerance
and mitigation costs.

Once you establish the business risk, you will evaluate risk tolerance
to inform minimally invasive policies that govern cloud adoption and
manage risks. Keep in mind that in some industries, third-party
compliance affects initial policy creation. The final stage is comprised
by the pace of adoption and innovation activities that will naturally
create policy violations. Executing relevant processes will aid in
monitoring and enforcing adherence to policies.

After defining your corporate policy strategy, which includes regulatory
compliance requirements, you will need to ensure that you have proper
governance in place to stay compliant over time as new workloads are
provisioned. You can use the five disciplines of cloud governance shown
in the diagram as the main pillars for your cloud governance strategy.

### Compliance considerations

Organizations may need to be compliant with one or more industry
standards. Compliance is based on various types of assurances, including
formal certifications, attestations, validations, authorizations, and
assessments produced by independent third-party auditing firms, as well
as contractual amendments, self-assessments, and customer guidance
documents.

Compliance can also be distinguished according to the type of risk,
regulatory or operational. According to Federal US regulators,
*Operational Risk* is the failure to establish a system of internal
controls and an independent assurance function and exposes the
organization to the risk of signification fraud, defalcation, and other
operational losses. While *Compliance Risk* is the risk of legal or
regulatory sanctions, financial loss, or damage to reputation resulting
from failure to comply with laws, regulations, rules, other regulatory
requirements, or codes of conduct. When planning your compliance
strategy, you should take into consideration operational compliance that
will support your regulatory compliance.

If your organization uses vendors or other trusted business partners,
one of the biggest business risks to consider may be a lack of adherence
to **regulatory compliance** by these external organizations. This risk
often cannot be remediated, and instead may require a strict adherence
to requirements by all parties. Make sure you\'ve identified and
understand any third-party compliance requirements before beginning a
policy review.

Improving **operational compliance** reduces the likelihood of an outage related to configuration drift or vulnerabilities related to systems being improperly patched. The following table gives some examples of operational compliance processes along with the tools that can perform them and their purpose.

| Process         | Tool     | Purpose |
|--------------|-----------|------------|
| Patch Management | Azure Automation Update Management      | Management and scheduling of updates         |
| Policy enforcement       | Azure Policy   | Policy enforcement to ensure environment and guest compliance       |
| Environment configuration  | Azure Blueprints       | Automated compliance for core services         |
| Resource configuration        | Desired State Configuration    | Automated configuration on guest OS and some aspects of the environment       |

The compliance requirements that an organization must follow will vary
according to the organization's industry and type of service. Consider a
health organization, which could be a doctors' offices, hospitals,
health insurers, and other healthcare companies---that create, receive,
maintain, transmit, or access protected health information (PHI)---this
organization will need to be compliant with the Health Insurance
Portability and Accountability Act of 1996 (HIPAA). The regulations
issued under HIPAA are a set of US healthcare laws that, among other
provisions, establish requirements for the use, disclosure, and
safeguarding of PHI. Azure Policy Regulatory Compliance built-in
initiative definition maps to compliance domains and controls in HIPAA
HITRUST 9.2.

Azure Policy Regulatory Compliance built-in initiative definition maps
to compliance domains and controls in Azure Security Benchmark. Each
control is associated with one or more Azure Policy definitions. These
policies may help you assess compliance with the control; however, there
often is not a one-to-one or complete match between a control and one or
more policies. As such, Compliant in Azure Policy refers only to the
policy definitions themselves; this doesn\'t ensure you\'re fully
compliant with all requirements of a control. In addition, the
compliance standard includes controls that aren\'t addressed by any
Azure Policy definitions at this time. Therefore, compliance in Azure
Policy is only a partial view of your overall compliance status. The
associations between compliance domains, controls, and Azure Policy
definitions for this compliance standard may change over time.

By default, every subscription has the Azure Security Benchmark
assigned. This is the Microsoft-authored, Azure-specific guidelines for
security and compliance best practices based on common compliance
frameworks. Learn more about Azure Security Benchmark. Available
regulatory standards:

- PCI-DSS v3.2.1:2018

- SOC TSP

- NIST SP 800-53 R4

- NIST SP 800 171 R2

- UK OFFICIAL and UK NHS

- Canada Federal PBMM

- Azure CIS 1.1.0

- HIPAA/HITRUST

- SWIFT CSP CSCF v2020

- ISO 27001:2013

- New Zealand ISM Restricted

- CMMC Level 3

- Azure CIS 1.3.0

- NIST SP 800-53 R5

- FedRAMP H

- FedRAMP M

## 2.1.2 Evaluate infrastructure compliance by using Microsoft Defender for Cloud

As you establish corporate policy and plan your governance strategies,
you can use tools and services like Azure Policy, Azure Blueprints, and
Microsoft Defender for Cloud to enforce and automate your
organization\'s governance decisions.

Microsoft Defender for Cloud plays an important part in your governance
strategy. It helps you stay on top of security because it:

- Provides a unified view of security across your workloads.

- Collects, searches, and analyzes security data from a variety of
    sources, which includes firewalls and other partner solutions.

- Provides actionable security recommendations to fix issues before
    they can be exploited.

- Can be used to apply security policies across your hybrid cloud
    workloads to ensure compliance with security standards.

Many security features, like security policy and recommendations, are
available for free. Some of the more advanced features, like
just-in-time VM access and hybrid workload support, are available under
the Defender for Cloud Standard tier. Just-in-time VM access can help
reduce the network attack surface by controlling access to management
ports on Azure VMs.

The regulatory compliance dashboard in Microsoft Defender for Cloud
shows your selected compliance standards with all their requirements,
where supported requirements are mapped to applicable security
assessments. The status of these assessments reflects your compliance
with the standard. Below you have an example of the Regulatory
Compliance Dashboard in Microsoft Defender for Cloud:

![Graphical user interface, text, application, email Description
automatically
generated](media\MicrosoftDefenderforCloudRegulatoryPolicy.png)

The regulatory compliance dashboard shows the status of all the
assessments within your environment for your chosen standards and
regulations. As you act on the recommendations and reduce risk factors
in your environment, your compliance posture improves.

Using the information in the regulatory compliance dashboard, you can
improve your compliance posture by resolving recommendations directly
within the dashboard. You can select any of the failing assessments that
appear in the dashboard to view the details for that recommendation.
Each recommendation includes a set of remediation steps to resolve the
issue. From there you can select any of the failing assessments that
appear in the dashboard to view the details for that recommendation.
Each recommendation includes a set of remediation steps to resolve the
issue.

## 2.1.3 Interpret compliance scores and recommend actions to resolve issues or improve security

When reviewing the assessments, you can select a tab for a compliance
standard that is relevant to you (1). You\'ll see which subscriptions
the standard is applied on (2), and the list of all controls for that
standard (3). For the applicable controls, you can view the details of
passing and failing assessments associated with that control (4), and
the number of affected resources (5). Some controls are greyed out.
These controls don\'t have any Defender for Cloud assessments associated
with them. Check their requirements and assess them in your environment.
Some of these might be process-related and not technical.

![Graphical user interface, text, application, email Description
automatically
generated](media\AzureSecurityBenchmark.png)

Use the regulatory compliance dashboard to help focus your attention on
the gaps in compliance with your chosen standards and regulations.

Let's consider a scenario where Contoso Security Admin needs to ensure
their SQL Databases workloads are compliant with PCI DSS 3.2.1. When
reviewing the dashboard, he noticed the following item was not
compliant:

![Graphical user interface, text, application, email Description
automatically
generated](media\AzureSecurityBenchmarkV3.png)

To address this issue, the Security Admin needs to click on the *SQL
servers should have an Azure Active Directory administrator provisioned*
recommendation and remediate it.

To track your progress over time you can use the *Compliance Over Time
Workbook*. This workbook tracks your compliance status over time with
the various standards you\'ve added to your dashboard.

![Graphical user interface, table Description automatically
generated](media\MDCWorkbooksComplianceoverTime.png)

## 2.1.4 Design and validate implementation of Azure Policy

When designing your Azure Policy, you need to take into consideration
the organization's needs from the infrastructure perspective as well as
compliance. By designing a tailored policy, you can help to reduce the
time necessary to audit your environment by having all your compliance
data in a single place.

Azure Policy can also help to set guardrails throughout your resources
to help ensure cloud compliance, avoid misconfigurations, and practice
consistent resource governance. Consider also using Azure Policy to
reduce the number of external approval processes by implementing
policies at the core of the Azure platform for increased developer
productivity and control optimization of your cloud spend. Azure Policy
will help you govern your Azure resources with simplicity, enforce
policies and audit compliance, and monitor compliance continuously.
Azure Policy establishes conventions for resources. Policy definitions
describe resource compliance conditions and the effect to take if a
condition is met. A condition compares a resource property field or a
value to a required value. Resource property fields are accessed by
using aliases. When a resource property field is an array, a special
array alias can be used to select values from all array members and
apply a condition to each one.

By defining conventions, you can control costs and more easily manage
your resources. For example, you can specify that only certain types of
virtual machines are allowed. Or, you can require that resources have a
particular tag. Policy assignments are inherited by child resources. If
a policy assignment is applied to a resource group, it\'s applicable to
all the resources in that resource group.

When designing your Azure Policy, you need to take into account how the
policies will affect your Azure resources to business standards and meet
compliance needs. When people, processes, or pipelines create or update
resources, Azure Policy reviews the request. When the policy definition
effect is *Modify*, *Append*, or *DeployIfNotExists*, Policy alters the
request or adds to it. When the policy definition effect is *Audit* or
*AuditIfNotExists*, Policy causes an activity log entry to be created
for new and updated resources. And when the policy definition effect is
*Deny*, Policy stops the creation or alteration of the request.

The recommended approach to validating a new policy definition is by
following these steps:

- Tightly define your policy

- Audit your existing resources

- Audit new or updated resource requests

- Deploy your policy to resources

- Continuous monitoring

### Tightly define your policy

It\'s important to understand how the business policy is implemented as
a policy definition and the relationship of Azure resources with other
Azure services. This step is accomplished by identifying the
requirements and determining the resource properties. But it\'s also
important to see beyond the narrow definition of your business policy.
Does your policy state for example \"All Virtual Machines must\...\"?
What about other Azure services that make use of VMs, such as HDInsight
or AKS? When defining a policy, we must consider how this policy impacts
resources that are used by other services.

For this reason, your policy definitions should be as tightly defined
and focused on the resources and the properties you need to evaluate for
compliance as possible.

### Audit existing resources

Before looking to manage new or updated resources with your new policy
definition, it\'s best to see how it evaluates a limited subset of
existing resources, such as a test resource group. Use the enforcement
mode Disabled (*DoNotEnforce*) on your policy assignment to prevent the
effect from triggering or activity log entries from being created.

This step gives you a chance to evaluate the compliance results of the
new policy on existing resources without impacting workflow. Check that
no compliant resources are marked as non-compliant (false positive) and
that all the resources you expect to be non-compliant are marked
correctly. After the initial subset of resources validates as expected,
slowly expand the evaluation to all existing resources.

Evaluating existing resources in this way also provides an opportunity
to remediate non-compliant resources before full implementation of the
new policy. This cleanup can be done manually or through a remediation
task if the policy definition effect is *DeployIfNotExists*.

### Audit new or updated resources

Once you\'ve validated your new policy definition is reporting correctly
on existing resources, it\'s time to look at the impact of the policy
when resources get created or updated. If the policy definition supports
effect parameterization, use Audit. This configuration allows you to
monitor the creation and updating of resources to see whether the new
policy definition triggers an entry in Azure Activity log for a resource
that is non-compliant without impacting existing work or requests.

It\'s recommended to both update and create new resources that match
your policy definition to see that the Audit effect is correctly being
triggered when expected. Be on the lookout for resource requests that
shouldn\'t be affected by the new policy definition that trigger the
Audit effect. These affected resources are another example of false
positives and must be fixed in the policy definition before full
implementation.

In the event the policy definition is changed at this stage of testing,
it\'s recommended to begin the validation process over with the auditing
of existing resources. A change to the policy definition for a false
positive on new or updated resources is likely to also have an impact on
existing resources.

### Deploy your policy to resources

After completing validation of your new policy definition with both
existing resources and new or updated resource requests, you begin the
process of implementing the policy. It\'s recommended to create the
policy assignment for the new policy definition to a subset of all
resources first, such as a resource group. After validating initial
deployment, extend the scope of the policy to broader and broader
levels, such as subscriptions and management groups. This expansion is
achieved by removing the assignment and creating a new one at the target
scopes until it\'s assigned to the full scope of resources intended to
be covered by your new policy definition.

During rollout, if resources are located that should be exempt from your
new policy definition, address them in one of the following ways:

- Update the policy definition to be more explicit to reduce
    unintended impact

- Change the scope of the policy assignment (by removing and creating
    a new assignment)

- Add the group of resources to the exclusion list for the policy
    assignment

Any changes to the scope (level or exclusions) should be fully validated
and communicated with your security and compliance organizations to
ensure there are no gaps in coverage.

### Monitor your policy and compliance

Implementing and assigning your policy definition isn\'t the final step.
Continuously monitor the compliance level of resources to your new
policy definition and set up appropriate Azure Monitor alerts and
notifications for when non-compliant devices are identified. It\'s also
recommended to evaluate the policy definition and related assignments on
a scheduled basis to validate the policy definition is meeting business
policy and compliance needs. Policies should be removed if no longer
needed. Policies also need updating from time to time as the underlying
Azure resources evolve and add new properties and capabilities.

## 2.1.5 Design for data residency requirements

For regulatory compliance considerations, data residency considerations
may support or even mandate the physical locations where data can be
stored, and how and when it can be transferred internationally. These
regulations can differ significantly depending on jurisdiction. Azure's
regions and service features provide customers with different avenues so
they can select and limit data residency and data access. This enables
customers in regulated industries to successfully run mission-critical
workloads in the cloud and leverage all the advantages of the Microsoft
hyperscale cloud.

When designing your data residency solution, one common requirement is
regarding data sovereignty. While it implies data residency; it also
introduces rules and requirements that define who has control over and
access the data stored in the cloud. In many cases, data sovereignty
mandates that customer data be subject to the laws and legal
jurisdiction of the country or region in which data resides. These laws
can have direct implications on data access even for platform
maintenance or customer-initiated support requests. You can use Azure
public multi-tenant cloud in combination with Azure Stack products for
on-premises and edge solutions to meet your data sovereignty
requirements, as described later in this article. These other products
can be deployed to put you solely in control of your data, including
storage, processing, transmission, and remote access.

As a customer, you retain all rights, titles, and interest in and to
customer data---personal data and other content---that you provide for
storing and hosting in Azure services. Microsoft will not store or
process customer data outside the geography you specify, except for
certain services and scenarios. You are also in control of any
additional geographies where you decide to deploy your solutions or
replicate your data. In addition, you and your users may move, copy, or
access your customer data from any location globally. Most Azure
services are deployed regionally and enable you to specify where your
customer data will be stored and processed. Examples of such regional
services include VMs, storage, and SQL Database. To maintain resiliency,
Microsoft uses variable network paths that sometimes cross geo
boundaries; however, replication of customer data between regions is
always transmitted over encrypted network connections.

When designing your data resident solution, take into consideration the
use of Azure Policy. You can use Azure Policy to implement governance
over cloud infrastructure and data, including but not limited to regions
in which resources can be deployed, which services can be deployed, and
resource monitoring requirements. To restrict the data and resources to
certain Azure regions, such as for data residency, customers can use the
*Allowed Locations* policy. Once policies are established, not only will
new resources that are deployed be checked against the policies, but all
resources will be periodically scanned to help ensure ongoing
compliance.

Another option to take into consideration is the use of Azure
Blueprints. Blueprints can be used to help manage data residency for
specific compliance needs by specifying both allowed locations and
allowed locations for resource groups. The typical scenario to use Azure
Blueprints is when you need to create scale deployments by supplying
templates to create, deploy, and update fully governed cloud
environments to consistent standards, which helps customers comply with
regulatory requirements. It differs from Azure Resource Manager (ARM)
and Azure Policy in that Blueprints is a package that contains different
types of artifacts---including ARM templates, resource groups, policy
assignments, and role assignments---all in one container, so you can
quickly and easily deploy all these components in a repeatable
configuration. Blueprints help to simplify large-scale Azure deployments
by packaging policies in a single blueprint definition.

If you want to ensure your data is stored only in your chosen Geography,
you should select from the options below:

- Data storage for regional services: Most Azure services are deployed
    regionally and enable you to specify the region into which the
    service will be deployed. Microsoft won\'t store your data outside
    the Geography you specified except for a few regional services and
    Preview services as described on the Azure data location page. This
    commitment helps ensure that your data stored in a given region will
    remain in the corresponding Geography, and won\'t be moved to
    another Geography for most regional services. For service
    availability, see Products available by region.

- Data storage for non-regional services: Certain Azure services
    don\'t enable you to specify the region where the services will be
    deployed as described on the data location page. For a complete list
    of non-regional services, see Products available by region.

Your data in an Azure Storage account is always replicated to help
ensure durability and high availability. Azure Storage copies your data
to protect it from transient hardware failures, network or power
outages, and even massive natural disasters. You can typically choose to
replicate your data within the same data center, across availability
zones within the same region, or across geographically separated
regions.

One example of a non-regional service is Azure Active Directory (Azure
AD). In other words, Azure AD may store identity data globally, except
for Azure AD deployments in:

- The United States, where identity data is stored solely in the
    United States.

- Europe, where Azure AD keeps most of the identity data within
    European datacenters except as noted in Identity data storage for
    European customers in Azure Active Directory.

- Australia and New Zealand, where identity data is stored in
    Australia except as noted in Customer data storage for Australian
    and New Zealand customers in Azure Active Directory.

*Note: Customers can configure certain Azure services, tiers, or plans
to store customer data only in a single region, with certain exceptions.
These include Azure Backup, Azure Data Factory, Azure Site Recovery,
Azure Stream Analytics, and locally redundant storage (LRS).

## 2.1.6 Translate privacy requirements into requirements for security solutions

Microsoft has an enduring commitment to protect data privacy, not as an
afterthought, but built into Microsoft Azure from the ground up.
Microsoft designed Azure with industry-leading security controls,
compliance tools, and privacy policies to safeguard your data in the
cloud, including the categories of personal data identified by the GDPR.
These also help you comply with other important global and regional
privacy standards such as ISO/IEC 27018, EU-U.S. Privacy Shield, EU
Model Clauses, HIPAA/HITECH, and HITRUST.

Consider also leveraging Azure Policy to enforce your privacy
requirements. Azure Policy is deeply integrated into Azure Resource
Manager, which helps your organization to enforce policy across
resources. With Azure Policy you can define policies at an
organizational level to manage resources and prevent developers from
accidentally allocating resources in violation of those policies. You
can use Azure Policy in a wide range of compliance scenarios, such as
ensuring that your data is encrypted or remains in a specific region to
comply with the GDPR.

When you build on Azure's secure foundation, you accelerate your move to
the cloud by achieving compliance more readily, allowing you to enable
privacy-sensitive cloud scenarios, such as financial and health service,
with confidence. Different organizations will need different levels of
privacy requirements based on the industry and compliance standards that
are required to follow. Azure provides customers with strong data
security, both by default on its own infrastructure, as well as for
customer-enabled services.

When designing your solution to fulfil the privacy requirements, take
into consideration the state of the data at a certain point of time. For
example, for some scenarios it may not be enough to protect the data
only when the data is at rest, you may also need to protect it while
in-transit. For example, the PCI DSS requirement 4 is about *Encrypt
transmission of cardholder data across open, public networks.* To
fulfill this requirement your solution must encrypt data in-transit.
Below you have some examples of ta protection according to the data
stage:

- **At-rest data protection:** Encryption at rest provides data
    protection for stored data (at rest). Attacks against data at-rest
    include attempts to obtain physical access to the hardware on which
    the data is stored, and then compromise the contained data. In such
    an attack, a server\'s hard drive may have been mishandled during
    maintenance allowing an attacker to remove the hard drive. Later the
    attacker would put the hard drive into a computer under their
    control to attempt to access the data. Customers are responsible for
    ensuring that data stored in Azure is encrypted in accordance with
    their standards. Azure offers a wide range of encryption
    capabilities, giving customers the flexibility to choose the
    solution that best meets their needs. Azure Key Vault helps
    customers easily maintain control of keys that are used by cloud
    applications and services to encrypt data. Azure Disk Encryption
    enables customers to encrypt VMs. Azure Storage Service Encryption
    makes it possible to encrypt all data placed into a customer\'s
    storage account.

- **In-transit data protection:** Protecting data in transit should be
    an essential part of your data protection strategy. Because data is
    moving back and forth from many locations, we generally recommend
    that you always use SSL/TLS protocols to exchange data across
    different locations. In some circumstances, you might want to
    isolate the entire communication channel between your on-premises
    and cloud infrastructures by using a VPN. Microsoft provides a
    number of options that can be utilized by customers for securing
    data in transit internally within the Azure network and externally
    across the Internet to the end user. These include communication
    through Virtual Private Networks (utilizing IPsec/IKE encryption),
    Transport Layer Security (TLS) 1.2 or later (via Azure components
    such as Application Gateway or Azure Front Door), protocols directly
    on the Azure virtual machines (such as Windows IPsec or SMB), and
    more.

### Azure resource providers encryption model support

Microsoft Azure Services each support one or more of the encryptions at
rest models. For some services, however, one or more of the encryption
models may not be applicable. For services that support customer-managed
key scenarios, they may support only a subset of the key types that
Azure Key Vault supports for key encryption keys. Additionally, services
may release support for these scenarios and key types at different
schedules. This section describes the encryption at rest support at the
time of this writing for each of the major Azure data storage services.

#### Azure disk encryption

Any customer using Azure Infrastructure as a Service (IaaS) features can
achieve encryption at rest for their IaaS VMs and disks through Azure
Disk Encryption. For more information on Azure Disk encryption, see the
Azure Disk Encryption documentation.

#### Azure storage

All Azure Storage services (Blob storage, Queue storage, Table storage,
and Azure Files) support server-side encryption at rest; some services
additionally support customer-managed keys and client-side encryption.

#### Azure SQL Database

Azure SQL Database currently supports encryption at rest for
Microsoft-managed service side and client-side encryption scenarios.
Support for server encryption is currently provided through the SQL
feature called Transparent Data Encryption. Once an Azure SQL Database
customer enables TDE key are automatically created and managed for them.
Encryption at rest can be enabled at the database and server levels. As
of June 2017, Transparent Data Encryption (TDE) is enabled by default on
newly created databases. Azure SQL Database supports RSA 2048-bit
customer-managed keys in Azure Key Vault. For more information, see
Transparent Data Encryption with Bring Your Own Key support for Azure
SQL Database and Data Warehouse.

Client-side encryption of Azure SQL Database data is supported through
the Always Encrypted feature. Always Encrypted uses a key that is
created and stored by the client. Customers can store the master key in
a Windows certificate store, Azure Key Vault, or a local Hardware
Security Module. Using SQL Server Management Studio, SQL users choose
what key they\'d like to use to encrypt which column.

### Data classification

The security controls that will be applied to the data will vary also
according to the level of privacy required by the data and to ensure
that you are prioritizing the data that it is important to be secure you
will need to classify your data. Data classification is a way of
categorizing data assets by assigning unique logical labels or classes
to the data assets. Classification is based on the business context of
the data. For example, you might classify assets by Passport Number,
Driver\'s License Number, Credit Card Number, SWIFT Code, Person's Name,
and so on.

One solution for data classification in Azure is Azure Purview. Azure
Purview is a unified data governance service that helps you manage and
govern your on-premises, multi-cloud, and Software as a Service (SaaS)
data. Create a holistic, up-to-date map of your data landscape with
automated data discovery, sensitive data classification, and end-to-end
data lineage. Enable data curators to manage and secure your data
estate. Empower data consumers to find valuable, trustworthy data.

![Graphical user interface, application Description automatically
generated](media\AzurePurview.png)

### Identity Protection

One important aspect of privacy is to ensure that you have a system to
protect the user's identity. A compromised identity could lead to data
compromise and directly affect the privacy requirements for your
project. Consider using Azure AD Identity Protection to enhance your
identity protection strategy to ensure you are fulfilling the privacy
requirements.

Identity Protection uses the learnings Microsoft has acquired from their
position in organizations with Azure AD, the consumer space with
Microsoft Accounts, and in gaming with Xbox to protect your users.
Microsoft analyzes 6.5 trillion signals per day to identify and protect
customers from threats. The signals generated by and fed to Identity
Protection, can be further fed into tools like Conditional Access to
make access decisions, or fed back to a security information and event
management (SIEM) tool for further investigation based on your
organization\'s enforced policies.

## Check your knowledge

Choose the best response for each of the questions below. Then select Check your answers.

1. When evaluating your organization's security posture, which pillar represents proactive measures that needs to be done to enhance the security hygiene of your workloads? 
 (a. Detect ).{{That’s incorrect. This pillar is focused on reactive measures.}} (b. Protect ){{That’s correct. Protection is focused on proactive measures.}} (c. Respond )That’s incorrect. This pillar is focused on reactive measures that are triggered by the detection pillar. (d. Detection and Response ){{That’s incorrect. Both are reactive measures.}}
 
Multiple Choice
Insert the question text in this cell. ()Insert the second incorrect answer text in this cell.{{Insert the second incorrect answer feedback in this cell.}} (x)Insert the correct answer text in this cell.{{Insert the correct answer feedback in this cell.}} ()Insert the first incorrect answer text in this cell.{{Insert the first incorrect answer feedback in this cell.}}

Lab-Sandbox-t
tasks:
- action: exists
  environment: azure
  azure:
    resource:
      type: "Microsoft.ContainerInstance/containerGroups"
      name: aci-demo
  hint: ""
  

1\. Which tool should you use to automate compliance for core Azure
Services and set a standard in the environment\'s settings?

a\. Azure Automation Update Management

b\. Azure Policy

c\. Azure Blueprints

d\. All the above

2\. Which solution should you utilize if the requirements for your
project include cloud security posture management from a centralized
location?

a\. Microsoft Defender for Cloud

b\. Azure Purview

c\. Azure AD

d\. Azure AD Identity Protection

3\. Which steps below are not part of the recommended approach to
validate a new Azure Policy that was customized for your organization\'s
compliance requirements?

a\. Audit your existing resources

b\. Audit new or updated resource requests

c\. Deploy your policy to resources

d\. Duplicate your Azure Policy

4\. When designing your data residency strategy, which tool should be
used to ensure you are limiting to which regions resources can be
deployed?

a\. Azure Policy

b\. Azure AD

c\. Azure Identity Protection

d\. Microsoft Defender for Cloud

5\. To which scenario is the use of SSL/TLS protocols to exchange data
across different locations relevant?

a\. Data at-rest in the datacenter

b\. Data in-transit

c\. Data at-rest in the user\'s device

d\. It is relevant to all scenarios above


## Case Study

**Scenario**

Contoso Pharma is an international pharmaceutical industry with a
presence in North America and Europe. Contoso Pharma has workloads
on-premises and in Azure. The goal is that in the next two years, all
workloads will be fully in Azure and there will be minimum workloads
on-premises. Below is a list of their major workloads:

- VMs (Windows and Linux)

- Storage accounts

- Key Vault

- SQL PaaS and SQL on VMs

Contoso Pharma also has a Site-to-Site VPN between the headquarters in
Redmond and the main office in London. This VPN is used to allow
resources on-premises to communicate.

Contoso Pharma has a legacy environment in Redmond composed by a couple
of Windows Server 2012 running a Web Server that is leveraged by the
application that queries the database to check for customer's
information. Upon investigation it was noted that the communication of
the legacy web server with the database is done via HTTP.

**Design Requirements**

Contoso Pharma has different compliance needs according to their
workloads, as shown in the table below:
| **Workload**         | **Type of Data**  | **Compliance Standard** |
|--------------|:-----:|-----------:|
| Windows VMs |  Credit card holder information |        PCI DSS |
| SQL PaaS      |  Patient health information  |          HIPAA |
| Storage Accounts     |  Credit card holder information  |          PCI DSS accounts |

To be compliant with these standards, Contoso Pharma must be able to:

- Monitor compliance progress over time

- Prohibit workload owners to provision resources that are not
    compliant with those standards

- Ensure that new subscriptions that are deployed in the environment
    are using required standards by default

- Ensure resources that are provisioned on each geo-location keep the
    data in the source region for data sovereignty purposes

**Questions**

1\) To ensure that Contoso Pharma can analyze their compliance status
over time, which tool should be utilized? Select the most appropriate
option.

a\. Azure Policy

b\. Azure Security Benchmark

c\. Microsoft Defender for Cloud

d\. Microsoft Defender for Cloud/Compliance Overtime Workbook

2\) Which service in Azure should be used to enforce workload owners to
create only resources that are following the required standards?

a\. Microsoft Defender for Cloud

b\. Azure Policy

c\. Azure Purview

d\. Regulatory Compliance Dashboard

3\) Which option should be utilized to ensure that when workload owners
create resources, they are keeping the data in the correct geo-location?

a\. Use the Allowed Location policy feature

b\. Create a Deny policy

c\. Use Microsoft Defender for Cloud to gain visibility of
misconfiguration

d\. No additional configuration is required as Azure will create based
on region by default

4\) How can Contoso Pharma validate if the VMs that were provisioned are
compliant with PCI DSS and if they are not what needs to be done to
remediate? Select the most appropriate answer.

a\. Utilize the Azure Security Benchmark

b\. Use the Compliance Overtime Workbook

c\. Use the Regulatory Compliance dashboard in Microsoft Defender for
Cloud to review the recommendation and implement the remediation steps

d\. Use Azure Policy and review the compliance chart

5\) Privacy requirements

- Data encryption is an imperative component to address your privacy
    requirements. What are the data stages that you must apply
    encryption?

- Which Azure service can you use to enforce data encryption across
    workloads?

## Summary

In this module you learned that business risk is the starting point to
establishing a compliance strategy, since it is during the business's
risk assessment that you will identify the regulatory compliance needs
based on the industry's requirements. You learned that operational
compliance should be in place to support the regulatory compliance needs
and the options available in Azure to help you be compliant with the
major regulatory standards. You also learned how to interpret compliance
scores using Microsoft Defender for cloud and how to recommend actions
to improve your compliance over time.

In addition, you learned how to design and validate your Azure Policy to
enforce compliance requirements and continuously monitor your
environment. As part of the compliance strategy, you also learned to
design data residency requirements and translate privacy requirements
into security solutions with proper data classification and identity
protection.

Visit the links below for more information about the topics covered in
this module:

- [Define cloud governance corporate policy - Cloud Adoption Framework
    \| Microsoft
    Docs](https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/govern/policy-compliance/policy-definition)

- [Operational compliance in Azure - Cloud Adoption Framework \|
    Microsoft
    Docs](https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/manage/azure-management-guide/operational-compliance?tabs=UpdateManagement%2CAzurePolicy%2CAzureBlueprints)

- [Azure and other Microsoft cloud services compliance offerings -
    Azure Compliance \| Microsoft
    Docs](https://docs.microsoft.com/en-us/azure/compliance/offerings/)

- [Operational compliance in Azure - Cloud Adoption Framework \|
    Microsoft
    Docs](https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/manage/azure-management-guide/operational-compliance?tabs=UpdateManagement%2CAzurePolicy%2CAzureBlueprints)

- [Evaluate and define corporate policy - Cloud Adoption Framework \|
    Microsoft
    Docs](https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/govern/corporate-policy)

- [Regulatory compliance - Microsoft Azure Well-Architected Framework
    \| Microsoft
    Docs](https://docs.microsoft.com/en-us/azure/architecture/framework/security/design-regulatory-compliance)

[HIPAA HITRUST
9.2](https://docs.microsoft.com/en-us/azure/governance/policy/samples/hipaa-hitrust-9-2)

*Visit Azure Compliance offerings to learn more about the industries
that are covered by Azure from the compliance perspective: [Azure and
other Microsoft cloud services compliance offerings - Azure Compliance
\| Microsoft
Docs](https://docs.microsoft.com/en-us/azure/compliance/offerings/)*

*Note: Watch [this webinar](https://youtu.be/tD8JnqzNOPc) for more
information on how to track your regulatory compliance. Although this
webinar was delivered when Microsoft Defender for Cloud was called Azure
Security Center, the content and rationale are still applicable for this
topic.*

*Note: Watch [this video](https://youtu.be/S_zJ2QBkk-0) more information
on how to use the Compliance Over Time Workbook workbook. Although this
video was recorded when Microsoft Defender for Cloud was called Azure
Security Center, the content and rationale are still applicable for this
topic.*

*Note: watch [this video](https://youtu.be/n469bC2V2Wo) for a quick demo
on Allowed Locations policy*

*For more information, visit [Data Residency in
Azure](https://azure.microsoft.com/en-us/global-infrastructure/data-residency/)*

*Note: Watch [this video](https://youtu.be/W2bsj3ULw0Y) for more
information about Azure Purview.*

*Note: Watch [this video](https://youtu.be/1REQYdZ6364) for more
information on Azure AD Identity Protection.*
