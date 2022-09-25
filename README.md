# ami-enhanced-debian
Build AMI from arm64 debian 11 add aws tools and other features

## debian enhanced ?

The goal of this image is enhancing the debian AMI (arm64) with tools including aws one like ssm or nvme ('https://github.com/amazonlinux/amazon-ec2-utils'), it sets french tz and features (should be set as variable...)

* contrib debian repo 
* python libs: pip, boto3
* aws cli
* ...

## Build

Run the following commands to build enhanced debian image:

* export PKR_VAR_AWS_ACCOUNT="<account number>"
* packer init ami.pkr.hcl
* packer build ami.pkr.hcl