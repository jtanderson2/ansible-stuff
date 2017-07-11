# config-generator
No configuration of devices, simply a method of creating device ios configuration files from jinja2 templates with variables. Paste configs into devices at your leisure :)

* Edit ./hosts file to suit you environment
* Common configuration variables and ssh login details set in ./group_vars/all.yml (should use a vault for the ssh stuff or public key auth in the real world!)
* Device specific configuration variables set in files in ./host_vars/
* Create a 'compiled' directory in ./ to take your generated configs
* Roles used in this project so the build task and jinja2 templates can be found in ./roles/base
* It would be fun to add advanced configuration, such as OSPF or BGP, using additional roles as opposed to the base role and template...
* Probably needs a more efficient way of getting host variables in, such as a single file that could be created from a spreadhseet/csv..
