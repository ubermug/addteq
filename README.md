Please find attached the playbook that sets up, locally, an instance of postgresql, jira and java.

The account that is being connected too has the username of "eric" but this can be changed in the inventory file

As the instructions stated that the UI could be used to finish setting up jira, I opted to do that for the config.sh file to 
connect to the postgresql databse and the first time startup using the startup.sh file.  I could have setup an x11 forwarding 
scheme to bring those screens back to the user running ansible, but this seemed out of the scope for this demo.

This deployment scenario used Ubuntu 18.04 desktop so there was a local browser to test with pre-installed.

Had to pre-install ansible, sshpass and openssh-server for deployment connection processes that are not included in the playbook.
