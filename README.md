# Ansible Role: Elasticsearch

This role installs and configures Elasticsearch on both Debian-based and RedHat-based systems.

## Role Variables

- `elasticsearch_version` (default: `"8.9.0"`): The version of Elasticsearch to install.
- `elasticsearch_network_host` (default: `"0.0.0.0"`): The network host for Elasticsearch.
- `elasticsearch_http_port` (default: `9200`): The HTTP port for Elasticsearch.
- `elasticsearch_cluster_name` (default: `"my-cluster"`): The cluster name for Elasticsearch.
- `elasticsearch_node_name` (default: `"node-1"`): The node name for Elasticsearch.

## Tags

- `packages`: Install required packages.
- `repo`: Set up the Elasticsearch repository.
- `elasticsearch`: Install Elasticsearch.
- `config`: Configure Elasticsearch.
- `service`: Manage the Elasticsearch service.

## Usage

Include this role in your playbook:

```yaml
- hosts: all
  roles:
    - elasticsearch

