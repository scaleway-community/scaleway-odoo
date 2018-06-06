# Scaleway odoo packer template

## Requirements

- Having [packer](https://packer.io) installed
- Having your Scaleway keys defined in your environment.

We suppose that in your environment, `$(SCW_ACCESS_KEY)` and `$(SCW_TOKEN)` are defined.
Use the following command to create your odoo image.

    packer --api_access_key $SCW_ACCESS_KEY --api_token $SCW_TOKEN build scaleway-odoo-template.json 

Go to <YOURIP>:8069 and you should see a odoo installation wizard.
