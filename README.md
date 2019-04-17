1. Install Terraform on the local machine
2. Use test_aws.tf to create new host on AWS (with security groups)
    # terraform apply
3. Install Ansible on the local machine
4. Place test_host.txt and test_aws.yml into the working directory
  a. after successfully terraform deploying into AWS, edit file host.txt (place new server public IP)
5. Run playbook
   # ansible-playbook test_aws.yml
After successfully deploy? check the results on page "http://AWS_PUBLIC_INSTANCE_IP:9000/ping"
