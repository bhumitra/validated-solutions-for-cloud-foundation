# Cloud Maturity Model Dashboards in VMware Aria Operations

## Table of Contents

- [CMM Dashboards in VMware Aria Operations](#cmm-dashboards-in-vmware-aria-operations)
  - [Table of Contents](#table-of-contents)
  - [Introduction](#introduction)
  - [Requirements](#requirements)
    - [Platforms](#platforms)
  - [Implementation](#implementation)
  - [VMware Aria Operations Dashboards Preview](#vmware-aria-operations-dashboards-preview)
  - [Known Issues](#known-issues)
  - [Support](#support)
  - [License](#license)

## Introduction

This content supports the [Health Reporting and Monitoring for VMware Cloud Foundation](https://core.vmware.com/health-reporting-and-monitoring-vmware-cloud-foundation) validated solution which enables the user to monitor the operational state of your [VMware Cloud Foundation](https://docs.vmware.com/en/VMware-Cloud-Foundation) environment through custom dashboards, alerts, and notifications. These custom dashboards are intended to serve as an extension to native VMware Aria Operations dashboards and dashboards that are enabled using the respective management packs.

## Requirements

### Platforms
- VMware Cloud Foundation 5.2
- VMware Cloud Foundation 5.1
- VMware Cloud Foundation 5.0
- VMware Cloud Foundation 4.5

## Implementation

1. Import Dashboards
2. Import Super Metrics
3. Import Alerts

Procedure
1. Log in to the VMware Aria Operations interface at https://<aria_operations_fqdn> with a user assigned the Administrator role.

2. Import the pre-defined super metrics.
- In the left pane, navigate to Operations > Configurations.
- On the Configuration page, click Super metrics
- From the ellipsis drop-down menu, select Import.
- In the Import super metric dialog box, click Browse, navigate to the Supermetrics.json file, click Open, click - Import, and click Done.
- Configure the default policy to enable the super metrics.
- In the left pane, navigate to Operations > Configurations.
- On the Configuration page, click Policy definitions.
- On the Policy definition page, select the Default policy and, from the ellipsis drop-down menu, select Edit.
- On the Default policy page, click the Metrics and properties card.
- From the Select object type drop-down menu, select vCenter > Cluster compute resource.
- Expand Super metrics and select all super metrics beginning with SM.
- From the Actions drop-down menu, select State > Activate.
- On the Metrics and properties page, click Save.
- Repeat this step to activate these Object Types: Cluster computer resource, CAS Adapter Instance, Universe, LoginSight Adapter Instance


3. Import the pre-defined dashboards.
- In the left pane, navigate to Operations > Dashboards.
- In the Dashboards pane, click Manage.
- From the ellipsis drop-down menu, select Import.
- In the Import dashboard dialog box, click Browse, navigate to the Dashboards.zip file, click Open, click Import, and click Done.


## Support

CMM Dashboards are not supported by VMware Support Services.

We welcome you to use the [GitHub Issues](https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/issues) to report bugs or suggest enhancements.

In order to have a good experience with our community, we recommend that you read the [contributing guidelines](../CONTRIBUTING.md).

When filing an issue, please check existing open, or recently closed, issues to make sure someone else hasn't already
reported the issue.

Please try to include as much information as you can. Details like these are incredibly useful:

- A reproducible test case or series of steps.
- Any modifications you've made relevant to the bug.
- Anything unusual about your environment or deployment.

## License

Copyright 2024 Broadcom. All Rights Reserved.

Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:

1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.

2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.

[//]: Links

[changelog]: CHANGELOG.md
