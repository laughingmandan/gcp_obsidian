These are the steps to debugging an issue with [[Virtual Machines]]

### Step One: Verify that your application is running
You can do this by SSHing into the instance via Google Cloud Console.

### Step Two: Access the System logs
Within the SSH connection you can run this command
`sudo journalctl -xe`
This will show you all the logs for that VM

### Step Three: Access the Application Logs
Locate where those are stored within the VM or Stack Driver

### Step Four: Check System Resources
Make sure that the VM specs are not at max capacity as this would cause crazy issues.

### Step Five: Check Networking 
Ping your machine from an external source to make sure that you can actually reach it. In either case make sure that your firewall rules allow for the connection you want to make.

### Step Six: External Dependencies
Make sure that any external dependencies are working as expected. This includes enabling and allowing API access to you specific VM.


## What to do if a VM is failing to boot or is inaccessible via SSH

Connect to the Serial console. This is feature is disable by default and needs to be manually turned on for each instance or a per project basis. Since it is a security risk make sure to turn it off again.

## Resources
- https://cloud.google.com/compute/docs/troubleshooting/troubleshooting-using-serial-console