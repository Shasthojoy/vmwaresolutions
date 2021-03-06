---

copyright:

  years:  2016, 2017

lastupdated: "2017-11-10"

---

# Scaling clusters created outside of the console

You can use the VMware vSphere Cluster offering to scale existing clusters, which are created outside of the {{site.data.keyword.vmwaresolutions_full}} console, by adding ESXi servers to them.

## Requirements

Ensure that you completed the following tasks:
*  You configured the {{site.data.keyword.cloud}} infrastructure credentials on the **Settings** page. For more information, see [User accounts and settings](../vmonic/useraccount.html).
*  You meet the requirements and you reviewed the considerations in [Requirements and planning for vSphere clusters](vs_planning.html).

## Procedure

1. Click **Getting Started** or **Order Instance** from the left navigation pane.
2. On the **vSphere Cluster** card, click **Order Instance**. Ensure that you are on the **Create new cluster** tab and that **New
cluster** is displayed in the **Cluster Configurations** list.
3. Configure a new cluster with the same settings as your existing cluster, which was created outside of the {{site.data.keyword.vmwaresolutions_short}} console. For more information, see [Ordering new vSphere clusters](vs_orderinginstances.html).

   **Note**: You must click **Select Existing Public and Private VLANs** under **Network Details** to specify the VLANs information,
   which is required for scaling the cluster you created outside of the {{site.data.keyword.vmwaresolutions_short}} console.
4. Click **Next**.
5. On the **Summary** page, review the cluster settings and click **Save Configuration**.
6. Go back to the **Order Instance** page by clicking **Order Instance** from the left navigation pane. Then click **Order Instance** on the **vSphere Cluster** card.
7. On the **Basics** page, click the **Scaling existing cluster** tab.
8. Select the cluster you just created from the **Cluster Configurations** list.
9. Under **Bare Metal Servers**, select the number of bare metal servers that you want to add to the cluster.
11. If the cluster does not include the HA-pair of FortiGate 300 series Security Appliance on its public VLAN, you can order one for it by selecting **Include with purchase** under **FortiGate Physical Appliance 300 Series HA Pair**.
12. Click **Next**.
13. On the **Summary** page, verify the cluster configuration before you place the order.
   1. Review the settings for the cluster.
   2. Click the link or links of the terms that apply to your order, and ensure that you agree with these terms before you continue.
   3. Review the estimated cost of the cluster by clicking the price link under **Estimated Cost**. To save or print your order
   summary, click the **Print** or **Download** icon on the upper right of the PDF window.
   4. Click **Place Order**.

## Results

The deployment of the cluster starts automatically, and you receive an email confirmation that the order is being processed. When the cluster is ready to use, you are notified by email.

## Related links

* [Ordering new vSphere clusters](vs_orderinginstances.html)
* [Ordering vSphere clusters based on existing configurations](vs_orderingbasedonexistingconfig.html)
* [Scaling existing vSphere clusters](vs_scalingexistingclusters.html)
