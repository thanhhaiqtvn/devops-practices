kops create cluster --name=kube.oladev.info \ 
--state=s3://leoaws-vprofile-kops-state --zones=us-west-2a,us-west-2b \ 
--node-count=2 --node-size=t3.small --master-size=t3.medium --dns-zone=kube.oladev.info \ 
--node-volume-size=8 --master-volume-size=8

kops update cluster --name kube.oladev.info --state=s3://leoaws-vprofile-kops-state --yes --admin

kops delete cluster --name kube.oladev.info --state=s3://leoaws-vprofile-kops-state --yes --admin

kops create cluster --name=kube.oladev.info --state=s3://leoaws-vprofile-kops-state --zones=us-east-1a,us-east-1b --node-count=2 --node-size=t3.small --master-size=t3.medium --dns-zone=kube.oladev.info --node-volume-size=8 --master-volume-size=8


kops create cluster --name=kube.oladev.info --state=s3://leoaws-vprofile-kops-state --zones=us-west-2a,us-west-2b --node-count=2 --node-size=t3.small --master-size=t3.medium --dns-zone=kube.oladev.info --node-volume-size=8 --master-volume-size=8

kops update cluster --name kube.oladev.info --state=s3://leoaws-vprofile-kops-state --yes --admin

kops validate cluster --state=s3://leoaws-vprofile-kops-state

kops delete cluster --name kube.oladev.info --state=s3://leoaws-vprofile-kops-state --yes


kops create cluster --name=kube.oladev.info \
--state=s3://leoaws-vprofile-kops-state \
--zones=us-west-2a,us-west-2b \
--node-count=2 --node-size=t3.small --master-size=t3.medium \
--dns-zone=kube.oladev.info \
--node-volume-size=8 --master-volume-size=8