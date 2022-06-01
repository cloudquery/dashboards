# Grafana Dashboards for CloudQuery

[CloudQuery](https://github.com/cloudquery/cloudquery) is an open-source cloud asset inventory powered by SQL.

You can connect your CloudQuery PostgreSQL database to Grafana to create a cloud asset inventory that you can visualization, monitoring and alert on.

Also, Checkout our blog about [Building an Open Source Cloud Asset Inventory with CloudQuery and Grafana](https://www.cloudquery.io/blog/open-source-cloud-asset-inventory-with-cloudquery-and-grafana)

## What's inside?

Currently we have basic asset inventory dashboards for AWS, GCP filterable by account_ids, regions and tables (project_id for GCP) (more is coming).

### AWS

All AWS dashboards are coming with account_ids and regions filter.

Located under [./dashboards/aws](./dashboards/aws)

**Note**: aws_asset_inventory.json will require to execute the following [view](https://github.com/cloudquery/cq-provider-aws/blob/main/views/resources.sql) before importing the dashboard.

### GCP

All GCP dashboards are comming with project_ids filter

Located under [./dashboards/gcp](./dashboards/gcp)

**Note**: aws_asset_inventory.json will require to execute the following [view](https://github.com/cloudquery/cq-provider-gcp/blob/main/views/resource.sql) before importing the dashboard.

### Examples

Here is an example of AWS asset inventory Grafana dashboard:

![AWS Asset Inventory](./dashboards/aws/aws_asset_inventory.png)

Here is an example of AWS EC2 Public and Private Instances Grafana dashboard:

![AWS EC2 Public/Private Instances](./dashboards/aws/aws_ec2_public_private.png)

## Contributions

PRs are welcome with news dashboards, also feel free to ask for new dashboards via [GitHub Issues](https://github.com/cloudquery/grafana-dashboards) or hop on [discord](https://cloudquery.io/discord)

