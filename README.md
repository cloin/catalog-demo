# catalog-demo
A playbook to configure a basic demo of Automation Services Catalog, a component of the Ansible Automation Platform


files are named after the API documented at https://cloud.redhat.com/docs/api/

`rbac` configures a Catalog admin group and adds the passed in user to that group


`sources` configures a Platform from specified Tower


`portfolios` creates a new portfolio and adds a job template from the Tower as a portfolio item

This playbook relies on a harder to find API documented [here](https://cloud.redhat.com/api/topological-inventory/v3.0/openapi.json). I also check to see if the Platform created has an Templates yet in `sources.yml` by using `/sources/{id}/service_offerings` before trying to create a Portfolio
