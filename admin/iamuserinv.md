---

copyright:

  years: 2015, 2017
lastupdated: "2017-04-27"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}

# Inviting users and assigning access
{: #iamuserinv}

You can invite users across {{site.data.keyword.Bluemix_notm}} services, applications, and {{site.data.keyword.Bluemix_notm}} infrastructure from a single location. You assign access for the users as you invite them, assigning roles, policies, and the accounts or organizations, or both, that they can access. Depending on the access options that you are authorized to manage, you can invite and provide access for users across the account or organization. As an account owner, you can assign access options to your account for a user when you and the user are both members, regardless of the role. 
{:shortdesc}

## Inviting users

To invite users and manage outstanding invitations, you must be either an account owner, an organization manager, or you must have infrastructure permissions to add users. You can invite users, cancel invitations, and resend a pending invitation to an invited user. You can invite a single user or, if you are providing the same access for all members in a group of users, you can invite multiple users at once.

To invite users or manage user invitations in your account, complete the following steps:

1. From the menu bar, click **Manage** &gt; **Account** &gt; **Users**. The Users window displays a list of users with their email addresses and current status in the accounts that you manage. 
2. Click **Invite users**. 
3. Specify the email address or IBMid of the user. If you are providing multiple users the same access, you can select **Invite multiple users** to enter a list of users to invite. Separate the user ID entries with commas. 
4. Add one or more of the access options that you manage. You must assign at least one access option and configure the settings for the user in each access option that you assign. For any additional access options that you don't add and configure, the default value of *no access* is assigned. You might see one or all of the following access options, depending on the options that you are authorized to manage: **Identity and access enabled services**, **Cloud Foundry access**, **Infrastructure access**.

If you determine that a user does not need access, you can cancel an invitation for any users that are shown in a **Processing** or **Pending** state in the **Status** column. If an invited user did not receive an invitation, you can resend the invitation to any user in a **Pending** state.

## Assigning access

### Identity and access enabled services

Select to assign the services, regions, service instances, and roles for the users you invite.

**Note**:  If you select the **Automatically grant access when new services are added** option, you are not notified to deselect each new {{site.data.keyword.Bluemix_notm}} service for that user when services are added later.

### Cloud Foundry access

Select to assign the organization, regions, spaces, and space roles for the users you invite. See [User roles](/docs/admin/users_roles.html#userrolesinfo) for more specific information about these settings. You can add multiple space roles, one at a time. All users granted the auditor organization role by default. You can update this role to billing manager or organization manager after the user accepts the invitation.

### Infrastructure access

You can assign the following infrastructure permissions to the user: 

<dl>
<dt>View Only</dt>
<dd>Users with this permission can only view items within the system.</dd>
<dt>Basic User</dt>
<dd>Users with this permission can perform basic actions within the system, such as adding a ticket and managing devices.</dd>
<dt>Super User</dt>
<dd>Users with this permission can perform all actions available in the system.</dd>
</dl>

**Note**: The actual permissions assigned are automatically limited to the subset of permissions that you have.

For information about configuring access for users after they have been added to your account, see [Managing user accounts and access](/docs/admin/iamusermanage.html).
