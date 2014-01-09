cloudify-openstack
==================

Cloudify 3.0 openstack CLI package
This Python project contains the code and configurations needed to bootstrap the Cloudify management netwrok &amp; manager VM on Openstack 

##Mandatory Configurations
In order to boostrap Cloudify manager on OpenStack you must edit the cloudify-config.yaml file and update the following propeties:

* `username`: The Openstack username you want to use vs. keystone authentication service

* `password`: The Openstack password you want to use vs. keystone authentication service

* `tenant_name`: The Openstack tenant name to which you want to use now.

##Cloudiofy OpenStack Configuration

The following configuration options are available in the cloudify-config.defaults.yaml file. You can edit this file if you need to change any of these defaults:

* Keystone configuration

  * `auth_url`: The URL to Keystone authentication service

* Networking configuration
* Security Configuration

* Management Server Configuration
 * `region`: The Openstack Region in which this VM will be provisioned. 
 * `user_on_management`: The username to use in order to SSH the manager VM
 * `userhome_on_management`: The home directory for this user
 * `instance`: VM configuration including:
  * `name` - the host name
  * `image` - the cloud image to use
  * `flavor` - the hardware flavor to use





