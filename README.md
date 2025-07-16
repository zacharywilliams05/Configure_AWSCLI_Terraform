<img width="442" height="24" alt="image" src="https://github.com/user-attachments/assets/10d1a359-973d-4efe-93b0-adc51053c3e6" /><img width="442" height="24" alt="image" src="https://github.com/user-attachments/assets/197aa308-8c9b-48f2-96e2-c9042b99cc25" /># Configure AWS CLI for Terraform

<img width="870" height="149" alt="image" src="https://github.com/user-attachments/assets/57b4b62d-0ed2-4f6c-94be-fbccb069a929" />

## How to Configure AWS CLI for Use with Terraform

Our goal is to have a configured AWS CLI ready to accept commands from Terraform. This process is straightforward and requires five steps:

## Step 1: Create a Free AWS Account
1. Navigate to [AWS Free Tier](https://aws.amazon.com/free/).
2. Follow the on-screen instructions to sign up for a free account.

<img width="415" height="505" alt="image" src="https://github.com/user-attachments/assets/a0262d0d-3190-40bf-8ff1-bd34fc7c5251" />

You should see a home console page like this one:

<img width="425" height="86" alt="image" src="https://github.com/user-attachments/assets/a061660b-4e7d-43d3-a8ce-99706de42e3d" />

## Step 2: Install Terraform CLI for macOS
1. Open your Terminal.
2. If you have Homebrew installed, run the following command:
   ```bash
   brew tap hashicorp/tap
   ```
<img width="425" height="111" alt="image" src="https://github.com/user-attachments/assets/2341808e-e3b0-4303-8f1c-4dcb6ac16731" />

3. Install the Terraform CLI
   ```bash
   brew install hashicorp/tap/terraform
   ```
<img width="425" height="137" alt="image" src="https://github.com/user-attachments/assets/a7848024-4e58-4bf1-b8fa-e73fd902d801" />

4. Confirm installation
     ```bash
   terraform version
   ```
   <img width="214" height="50" alt="image" src="https://github.com/user-attachments/assets/2be42334-6fd8-4d05-9cb1-5b3f582878aa" />

## Step 3 : Install AWS cli
1. Install using the brew command
     ```bash
     brew install awscli
      ```

## Step 4 : Create an AWS user
1. In the AWS console search for IAM
<img width="425" height="86" alt="image" src="https://github.com/user-attachments/assets/502b6922-3653-497d-b059-0137c25754f7" />

2. Click on users in the left menu
<img width="317" height="240" alt="image" src="https://github.com/user-attachments/assets/6aa7ff0c-3b3f-4f49-9c7b-a683a68507f8" />

3. Click create user in the upper right
<img width="284" height="124" alt="image" src="https://github.com/user-attachments/assets/fe8daf43-592a-4413-81bb-61aa87afd765" />

4. Enter a user name
<img width="425" height="104" alt="image" src="https://github.com/user-attachments/assets/f0e7541f-211c-44e3-a05e-19fcbdba3ac2" />

5. Use the default option of add user and group, click next
<img width="255" height="186" alt="image" src="https://github.com/user-attachments/assets/038f660a-f2ff-4ead-ad6c-061797ed15a1" />

6. Click create user in the lower right
<img width="327" height="187" alt="image" src="https://github.com/user-attachments/assets/b26b0ecb-4070-41b6-9488-a78b3eeca1be" />

7. After the user is successfully created click on the user name and click create access key
<img width="425" height="111" alt="image" src="https://github.com/user-attachments/assets/7f639454-ce9e-4079-97f4-bd556b3c025c" />

8. Select the radio button for command line interface (CLI)
<img width="425" height="327" alt="image" src="https://github.com/user-attachments/assets/7a51f424-a732-49e9-b600-b3f2156a862d" />

## Step 5 : Configure awscli to use the access keys
1. Enter the command
     ```bash
     aws configure
      ```
2. Enter the AWS Access Key ID and press enter
3. Enter the AWS Secret Access Key and press enter
4. Enter the region (shown on your AWS console home, for me it is us-east-2)
5. For output format do not enter anything and press enter.
6. That is it! Terraform and AWSCLI are installed and configured for use!
   

9. Enter a tag value if you like and click generate access keys.
You should be presented with access keys for the user account.

