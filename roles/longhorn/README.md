# `dannixon.k8s.longhorn`

Installs [Longhorn](https://longhorn.io/) via the [helm chart](https://github.com/longhorn/charts/tree/master/charts/longhorn) and optionally configures S3 backup.

Note that once Longhorn is deployed, changes to the S3 backup target will do nothing.
Any changes needed should be made via the web dashboard.

## Variables

- `longhorn_chart_version` (string): Chart version to install, so far this has directly mapped onto the Longhorn version.
- `longhorn_generate_iscsi_iname` (bool): If new iSCSI names should be generated.
- `longhorn_s3_backup_enabled` (bool): If S3 backup should be configured and enabled.
- `longhorn_s3_backup_secret_name` (string): Name of the Secret used to store S3 backup target.
- `longhorn_s3_backup_bucket` (string): S3 bucket name.
- `longhorn_s3_backup_region` (string): S3 region.
- `longhorn_s3_backup_path` (string): Path within bucket.
- `longhorn_s3_backup_key_id` (string): S3 key ID.
- `longhorn_s3_backup_key_secret` (string): S3 key secret.
- `longhorn_s3_backup_endpoint` (string): S3 endpoint URL.
