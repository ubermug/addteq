Please find attached the playbook that sets up, locally, an instance of postgresql, jira and java.

The account that is being connected too has the username of "eric" but this can be changed in the inventory file

As the instructions stated that the UI could be used to finish setting up jira, I opted to do that for the config.sh file to 
connect to the postgresql databse and then started Jira using the init service.  I could have setup an x11 forwarding 
scheme to bring that setup screen back to the user running ansible, or saved the xml as a file ot import, 
but this seemed out of the scope for this demo.

This deployment scenario used Ubuntu 18.04 desktop so there was a local browser to test with pre-installed.

Had to pre-install ansible, sshpass and openssh-server for deployment connection processes that are not included in the playbook.

In order to stay with the free GitHub account (due to file size contraints), I needed to download the jira software to the instance as part of the playbook, so
internet connectivity is assumed.

After the playbook was run, and the config.sh file was run, and the service started, the Jira UI was available at 127.0.0.1:8080