An image is the state of the files in a [[Persistent Disks]] at a given time. This allows you to quickly start [[Virtual Machines]] from that file state instead of running scripts to get it to that file state. 

There are images that you can use straight away. These are called public images. You can also modify these images to create custom images. 

## Custom Images
In order to create a custom image you need one of:
- [[Persistent Disk]]
- Running [[Virtual Machines]] in GCE
- Snapshot
- Another Image
- File in Google Cloud Storage. 

## Image encryption
While the image is at rest it is encrypted. Like most things encryption wise in google. You can choose how the key that encrypts it is managed. 

## Resources
- https://cloud.google.com/compute/docs/images
- https://cloud.google.com/compute/docs/images/create-custom