# catalog-demo
files are named after the API documented at https://cloud.redhat.com/docs/api/

`rbac` configures a Catalog admin group and adds the passed in user to that group


`sources` configures a Platform from specified Tower


`portfolios` creates a new portfolio and adds a job template from the Tower as a portfolio item

This playbook relies on a harder to find API documented [here](https://cloud.redhat.com/api/topological-inventory/v3.0/openapi.json). We can probably reuse this to check progress of the collector populated job templates on the platform created in `sources.yml`
