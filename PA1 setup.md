# Amazon AWS
EC2
<Launch Instance>
FREE TIER
1. Choose AMI -> SUSE Linux 
2. Choose Instance Type -> t2.micro
3. Configure Instance -> Enable CloudWatch
4. Add Storage (nothing)
5. Tag Instance (nothing)
6. Configure Security Group
	Create a new security group
		Rules
		SSH - TCP - 22 - My IP
		HTTP - TCP - 80 - Anywhere
7. Review
	<Launch>

	Create a new key pair
		Key pair name: nicole
		<Download Key Pair> → SAVE IT!!
		<Launch Instance>
		<View Instances>

		Copy your "Public DNS" 
>> ex: ec2-52-10-28-171.us-west-2.compute.amazonaws.com

# FileZilla
	FileZilla > Settings > SFTP > Add keyfile > *.pem > Open > Yes > Save > Ok
	File > Site Manager > New Site
		Host: [paste your Public DNS]
			ex: ec2-52-10-28-171.us-west-2.compute.amazonaws.com
		Protocol: SFTP
		Logon Type: Interactive
		User: ec2-user
		<Connect>
			Unknown host key dialog >> <Ok>
