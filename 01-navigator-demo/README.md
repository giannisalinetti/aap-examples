# K8S Collections Lab

Demo project to demonstrate Ansible community collections for Kubernetes and OpenShift

Requirements
------------


Role Variables
--------------
**api_url**: API endpoint of the managed server
**cluster_auth_user**: login user
**cluster_auth_password**: login password
**app_name**: Application name
**ns_name**: Target namespace (create if absent)
**app_image**: Application image
**app_replicas**: Final desired replicas
**service_name**: K8s service name
**route_hostname**: Application route name (works in OpenShift only)

Demo
----

Playbook execution:
```
$ ansible-navigator --eei quay.io/gbsalinetti/custom-ee:latest run playbook.yaml -e 'cluster_auth_user=<username>' -e 'cluster_auth_password=<password>'

```

