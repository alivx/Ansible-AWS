In this repo, you will find out how to create production secure AWS VPC using ansible.

This VPC will include:

* VPC.
* Subnet [Private, Public].
* Internet Gateway (IGW).
* Elastic IP (For nat gateway ).
* nat gateway.
* Route Table.
* AWS Service endpoint.
* Security Groups.
* SSH nat server.


Details

In this topology we will create:
1. Public subnet for public application such as "Nginx".
2. Public subnet for public NAT server that we need to access internal VPC EC2 instance.
3. Private subnet for Application such as API server.
4. Private subnet for Databases such as MySQL or any database.
5. Private subnet for serverless application such as AWS lambdas.
6. AWS endpoint that enables a private connection between your VPC and another AWS service without requiring access over the Internet.
7. Internet Gateway.
8. Elastic IP.
9. nat gateway.
10. route tables.
11. Security Groups.
  * Public SSH NAT #To access nat server via port 22
  * Private Security Group #For internal usages.
  * Public Security group (HTTP/HTTPS).
12. EC2 ssh nat instance.

