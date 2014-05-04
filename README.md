# OpenShift Ant Cartridge

This is a cartidge that adds ant to the SSH path

This was created for use on a private OpenShift instance, where ant isn't available by default (unlike the Redhat Openshift server, where ant is on /usr/bin for free)

The ant distribution is in /usr/apache-ant-x.y.z

Ant is added to the path using the OPENSHIFT_ANT_PATH_ELEMENT.erb file in env

An alias is added to /app-root/data/.bash_profile for ant, this is required to stop the 'default' install of ant being used when avaialable. See the install script for more information