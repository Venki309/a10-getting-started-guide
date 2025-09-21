**A10 Control Licensing**

Deploying A10 Control and managing devices requires the right licenses. There are two broad categories of licenses:
- **A10 Control licenses (Controller License)**: It is used to connect and manage devices. A trial license is available by default when you install A10 Control.  
- **Thunder device licenses (FlexPool License)**: It is used to run and manage Thunder devices. These licenses can be configured from A10 Control or through the device CLI.  

The A10 Control portal displays warning messages three months before expiry of the license in the **License** page. Four weeks before expiry, warnings are displayed across all pages. Users should renew licenses promptly to ensure applications continue to function as expected.

**A10 Control Licenses**

A10 Control licenses are available as a pool of Managed Bandwidth Units (MBUs). These MBUs can be shared among multiple organization admin accounts across deployments. Organization Admins can request more capacity from the license manager or return unused MBUs.

Each Thunder device has a fixed MBU value. When a Thunder device connects to A10 Control, it consumes the license in the equal amount of its MBU value. If MBUs are unavailable, the device registration fails. When a device deregisters from A10 Control, its MBUs return to the pool.

Most MBU licenses support unlimited devices, with restrictions only on bandwidth units. In some cases, the license may also limit the number of devices. The available device slots are shared across all organization admins using the same license pool. For example, if the license allows 10 devices, Org A could register 6 devices and Org B could register 4 devices. Once the 10-device limit is reached, no additional devices can be registered until one is deregistered.

License types under A10 Control:

A10 Control SW MBU – A pool of MBUs for multiple deployments.

A10 Control SaaS MBU – A pool of MBUs for A10 Control deployed as SaaS.

A10 Control SaaS Trial – Trial MBUs for SaaS deployments.

**Device Licenses**

A device license is required to configure and manage Thunder devices from A10 Control. FlexPool licenses can be managed directly in A10 Control. Other license platforms must be managed through the device CLI.

When a Thunder device is added, its installed license is automatically shown in A10 Control. If a license is missing, it can be assigned from the license pools available in A10 Control. Devices orchestrated by A10 Control can also receive licenses during the orchestration workflow.

Supported device license platforms:

Capacity FlexPool – A pool of capacity for multiple devices.

Instance FlexPool – A pool of ADC application capacity.

Subscriber FlexPool – Licenses for a specific number of subscribers, applicable for CGN services on unlimited devices with unlimited bandwidth. Managed through GLM.

For information about managing license, see Manage Licenses.
