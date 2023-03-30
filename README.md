# shell-snap

snapcraft init
snapcraft
sudo snap install shell_0.1_all.snap --dangerous --devmode


error - 
launch failed: cannot connect to the multipass socket/                           
Please ensure multipassd is running and '/var/snap/multipass/common/multipass_socket' is accessible
An error occurred with the instance when trying to launch with 'multipass': returned exit code 2.
Ensure that 'multipass' is setup correctly and try again.


sudo chmod a+w /var/snap/multipass/common/multipass_socket
sudo snap restart multipass.multipassd
