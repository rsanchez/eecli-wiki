Create a member group.

```
eecli create:member_group <name>
```

## Arguments

### `name`

Member group name

## Options

### `--clone="1"`

Clone the specified member group id.

### `--description="Your description here."`

The member group description.

### `--is_locked="y"`

### `--can_view_online_system="y"`

### `--can_view_offline_system="n"`

### `--can_view_profiles="n"`

### `--can_email_from_profile="n"`

### `--can_edit_html_buttons="n"`

### `--include_in_authorlist="n"`

### `--include_in_memberlist="n"`

### `--include_in_mailinglists="n"`

### `--can_delete_self="n"`

### `--mbr_delete_notify_emails=""`

### `--can_post_comments="y"`

### `--exclude_from_moderation="n"`

### `--can_search="y"`

### `--search_flood_control="15"`

### `--can_send_private_messages="n"`

### `--prv_msg_send_limit="20"`

### `--prv_msg_storage_limit="60"`

### `--can_attach_in_private_messages="n"`

### `--can_send_bulletins="n"`

### `--can_access_cp="n"`

### `--can_access_content="n"`

### `--can_access_publish="n"`

### `--can_access_edit="n"`

### `--can_access_files="n"`

### `--can_access_design="n"`

### `--can_access_addons="n"`

### `--can_access_modules="n"`

### `--can_access_extensions="n"`

### `--can_access_accessories="n"`

### `--can_access_plugins="n"`

### `--can_access_fieldtypes="n"`

### `--can_access_members="n"`

### `--can_access_admin="n"`

### `--can_access_sys_prefs="n"`

### `--can_access_content_prefs="n"`

### `--can_access_tools="n"`

### `--can_access_comm="n"`

### `--can_access_utilities="n"`

### `--can_access_data="n"`

### `--can_access_logs="n"`

### `--can_admin_channels="n"`

### `--can_admin_upload_prefs="n"`

### `--can_admin_templates="n"`

### `--can_admin_design="n"`

### `--can_admin_members="n"`

### `--can_admin_mbr_groups="n"`

### `--can_admin_mbr_templates="n"`

### `--can_delete_members="n"`

### `--can_ban_users="n"`

### `--can_admin_modules="n"`

### `--can_send_email="n"`

### `--can_email_member_groups="n"`

### `--can_email_mailinglist="y"`

### `--can_send_cached_email="n"`

### `--can_view_other_entries="n"`

### `--can_delete_self_entries="n"`

### `--can_edit_other_entries="n"`

### `--can_delete_all_entries="n"`

### `--can_assign_post_authors="n"`

### `--can_edit_categories="n"`

### `--can_delete_categories="n"`

### `--can_moderate_comments="n"`

### `--can_view_other_comments="n"`

### `--can_edit_own_comments="n"`

### `--can_delete_own_comments="n"`

### `--can_edit_all_comments="n"`

### `--can_delete_all_comments="n"`

## Examples

Create a member group with default preferences

```
eecli create:member_group your_group_name
```

Create a member group using another group's preferences

```
eecli create:member_group --clone=1 your_group_name
```

Create a member group and with the specified preferences

```
eecli create:member_group --can_access_cp=y --can_access_content=y your_group_name
```

Show all possible preference options

```
eecli create:member_group create:member_group
```