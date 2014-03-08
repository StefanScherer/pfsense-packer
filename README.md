# pfSense packer box
Create a pfSense box with Packer

# Download ISO manually
As packer is not able to download gzipped ISO files directly, you have to download
it manually and extract it. Then customize the pfsense.json file so packer could
find the ISO file locally.

http://fleximus.org/mirror/pfsense/downloads/pfSense-LiveCD-2.1-RELEASE-i386.iso.gz

# Create box

```
packer build -only=virtualbox-iso pfsense.json
```

