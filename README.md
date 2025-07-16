# Configure AWS CLI for Terraform

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
