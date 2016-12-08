# ec2_anurag
## Prereqs:

* aws-cli

'''
yum install unzip -y
curl "https://s3.amazonaws.com/aws-cli/awscli-bundle.zip" -o "awscli-bundle.zip"
unzip awscli-bundle.zip
sudo ./awscli-bundle/install -i /usr/local/aws -b /usr/local/bin/aws
ln /usr/local/bin/aws /bin/aws
aws configure
'''

* boto

'''
git clone git://github.com/boto/boto.git
cd boto
python setup.py install
'''

* boto-config

Configure BOTO
touch ~/.boto
Add the following lines to the file
```
[Credentials]
aws_access_key_id = REDACTED
aws_secret_access_key = REDACTED
```
