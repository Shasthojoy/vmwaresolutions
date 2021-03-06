---

copyright:

  years:  2016, 2017

lastupdated: "2017-11-13"

---

# Viewing Cloud Foundation instances

Use this procedure to view the VMware Cloud Foundation instances that you ordered and detailed information about them.

## Procedure

1. Click **Deployed Instances** from the left navigation pane. In the **Cloud Foundation Instances** table, view the summary about the ordered instances:

  * **Name**:The name of the instance.
  * **Version**: The release version that the instance was deployed in or upgraded to.
  * **Location**: The data center where the instance is hosted.
  * **Creation Time**: The date and time that the instance was created.
  * **Status**: The status of the instance. The status can have one of the following values:
    <dl class="dl">
    <dt class="dt dlterm">Creating</dt>
    <dd class="dd">The instance is being created.</dd>
    <dt class="dt dlterm">Building</dt>
    <dd class="dd">The instance is being configured.</dd>
    <dt class="dt dlterm">Ready to Use</dt>
    <dd class="dd">The instance is ready to use.</dd>
    <dt class="dt dlterm">Modifying </dt>
    <dd class="dd">The instance is being modified.</dd>
    <dt class="dt dlterm">Updating</dt>
    <dd class="dd">Updates and patches are being applied to the instance.</dd>
    <dt class="dt dlterm">Failed</dt>
    <dd class="dd">The creation, configuration, or modification process failed.</dd>
    <dt class="dt dlterm">Deleting</dt>
    <dd class="dd">The instance is being deleted.</dd>
    <dt class="dt dlterm">Deletion Error</dt>
    <dd class="dd">An error occurred when the instance was being deleted.</dd>
    <dt class="dt dlterm">Deleted</dt>
    <dd class="dd">The instance is deleted.</dd>
    </dl>
  * **Actions**: Take the following actions on the instance:
    <dl class="dl">
    <dt class="dt dlterm">Delete</dt>
    <dd class="dd">Delete the instance.</dd>
    </dl>

2. Click an instance to see the property details. Ensure that you are on the **Summary** tab.

  * **ID**: The ID of the instance.
  * **Name**: The name of the instance.
  * **Location**: The data center where the instance is hosted.
  * **Current version**: The current version of {{site.data.keyword.vmwaresolutions_full}}.
  * **vCenter version**: The version of VMware vCenter Server. There is a slight variation between the vCenter Server version displayed on the {{site.data.keyword.vmwaresolutions_short}} console and the VMware vSphere Web Client. Both are correct.
  * **NSX for vSphere**: The VMware NSX for vSphere product version.
  * _**VMware component**_ **License**: If you selected to use your own VMware license for any of the VMware components on the **Licensing** page when you were ordering the instance, the VMware component name and the license key string you entered for the component are displayed.

    Examples of VMware component licenses can include **NSX License**, **vCenter Server License**, and **vSAN License**.

  * **DNS**:
    <dl class="dl">
           <dt class="dt dlterm">Root Domain</dt>
    <dd class="dd">The root domain name is the DNS (Domain Name System) domain name and the Microsoft Active Directory (AD) forest root name for a
    primary (single) or secondary set of <span class="ph">Cloud Foundation instances</span>.</dd>
    <dt class="dt dlterm">SSO Domain</dt>
    <dd class="dd">The SSO domain is the vSphere Single Sign-On domain. The SSO domain name is fixed for all deployed  <span
    class="ph">Cloud Foundation instances</span> (primary or secondary) with a value of <samp class="ph codeph">vsphere.local</samp>.</dd>
    <dt class="dt dlterm">Subdomain</dt>
    <dd class="dd">The subdomain is the DNS subdomain name of the root domain name where the local <span class="ph">Cloud Foundation
    instance</span> host names reside. The subdomain name is in the format <samp class="ph codeph"><var class="keyword
    varname">cloud_foundation_instance_name</var>.<var class="keyword varname">root.domain_name</var></samp>.</dd>
    </dl>

  * **SDDC Manager version**: The version of the SDDC Manager of the instance.
  * **Status**: The detailed status of the instance.

    The information that is displayed provides an update on the progress of the deployment or the action that is taken on the instance.
    If there are issues, a message might be displayed to help you investigate and resolve the problem.

3. View the access information for the instance-related components. These passwords are initial passwords that are generated by the system. If you change them outside of the {{site.data.keyword.vmwaresolutions_short}} console, they are not updated on the instance details page.

  * **AD/DNS server IP**: The IP address of the AD server.
  * **AD/DNS server FQDN**: The AD/DNS server fully qualified domain name.
  * **AD/DNS server (Remote desktop)**: The user name and password that you can use to access the AD server via a remote desktop connection.
  * **NSX Manager IP**: The IP address of the NSX Manager.
  * **NSX Manager FQDN**: The NSX Manager fully qualified domain name (FQDN).
  * **NSX Manager (HTTP)**: The user name and password that you can use to access the NSX Manager web console.
  * **NSX Manager (SSH)**: The user name and password that you can use to access the NSX Manager VM via SSH connection.
  * **PSC IP**: The IP address of the Platform Services Controller (PSC).
  * **PSC FQDN**: The PSC fully qualified domain name (FQDN).
  * **PSC (SSH)**: The user name and password that you can use to access the PSC VM via SSH connection.
  * **PSC (ADMIN)**: The VMware vCenter Single Sign-On user name and password that you can use to access the PSC web console.
  * **vCenter IP**: The IP address of the vCenter Server.
  * **vCenter FQDN**: The vCenter Server fully qualified domain name (FQDN).
  * **vCenter (SSH)**: The user name and password that you can use to access the vCenter Server VM via SSH connection.
  * **vCenter (ADMIN)**: The VMware vCenter Single Sign-On user name and password that you can use to log in to the vCenter Server by
  using the vSphere Web Client.

4. View the deployment history for the instance.

  * **Date**: The date and time when the instance status is changed.
  * **Summary**: The details of the change.

    If errors occur during instance deployment or instance deletion, an {{site.data.keyword.cloud}} Support ticket is created automatically on your behalf. You can click the ticket link to check its status and progress.

## What to do next

Manage your instances from the {{site.data.keyword.vmwaresolutions_short}} console or the vSphere Web Client.

**Important**: Before you click **vCenter console** on the instance details page to go to the vSphere Web Client and start managing your ESXi servers, you must log in to the VPN portal of the {{site.data.keyword.CloudDataCent}}. Hover over the vCenter console button and follow the instructions to ensure that you meet all requirements and you completed the necessary steps before you access the vSphere Web Client.

Review the following topics for information to help you complete the login instructions:

* For the requirements and necessary steps before you access the vSphere Web Client, see [Timeout reached while connecting to the vSphere Web Client](../vmonic/trbl_timeout_vc_console.html).
* For a list of access points to log in to the {{site.data.keyword.cloud}} Private Network using VPN, see [VPN Access](http://www.softlayer.com/vpn-access){:new_window}.
* If you have problems when you deploy an OVF (Open Virtualization Format) file using the vSphere Web Client, see [Deploying an OVF file using the vSphere Web Client](../vmonic/trbl_deploy_ovf.html).

## Related links

* [Ordering Cloud Foundation instances](sd_orderinginstance.html)
* [Expanding and contracting capacity for Cloud Foundation instances](sd_addingremovingservers.html)
* [Deleting Cloud Foundation instances](sd_deletinginstance.html)
