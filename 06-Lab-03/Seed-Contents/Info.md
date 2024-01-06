
# Contents / Commands

- CIDR to IP Range Conversion
    - https://www.ipaddressguide.com/cidr


- Upload the file
    - Change Permission
        - chmod 400 ./gl-lab-03.pem
    - Using SCP to upload the files
        - scp -i ./gl-lab-03.pem -r ./GL-AWS-Lab-03.zip ec2-user@3.93.188.2:~

- Verify the Upload Operation
    - SSH Connect to EC2
        - ssh -i ./gl-lab-03.pem ec2-user@3.93.188.2
- Unzip the uploaded Zip file
    - unzip ./GL-AWS-Lab-03.zip
- Supply permission to EC2 instance
    - aws configure

- Execute the CF files
    - CF1.json
        - aws cloudformation create-stack --stack-name gl-lab-03-stack --template-body file://./CF-Template-Files/v2-Work/CF1.json
    - CF2.json
        - aws cloudformation create-stack --stack-name gl-lab-03-stack --template-body file://./CF-Template-Files/v2-Work/CF2.json



