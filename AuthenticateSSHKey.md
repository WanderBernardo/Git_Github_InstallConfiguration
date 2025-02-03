
Documents:

- https://docs.github.com/en/authentication/connecting-to-github-with-ssh


### Configuration:

1 - Let's check if exist a SSH Key. Open Command sreen (bash)

- Use command:  ``` ls -al ~/.ssh ```

  ![image](https://github.com/user-attachments/assets/49181b31-9abe-4672-85e7-589b385f1c53)

If show the mensage below, it want to show: "No exist SSH Key"
![image](https://github.com/user-attachments/assets/52d048cb-ab79-463e-82e1-311be46cad4f)

2 - Create SSH Key:

- Use command: ``` ssh-keygen -t ed25519 -C "your_email@example.com" ```

  ![image](https://github.com/user-attachments/assets/96b7b490-b7a9-467f-b4a9-daea471e424e)

3 - Now, go to ask where do you want to salve your Key. Suggestion: maintaim standard. Click in the "enter botton":
![image](https://github.com/user-attachments/assets/59a9b960-8e48-455a-bd4c-7a843c6c103d)

4 - After go to request to salve a "passphase"(as if it were a password):
![image](https://github.com/user-attachments/assets/e160c744-8d8d-4cf6-8d37-f31cf1cd9a6d)

Key Okay: 

![image](https://github.com/user-attachments/assets/63211505-90cd-4152-b07b-555f39cf86c6)


5 - We're going to salve Key of security:

- Use command: ``` eval "$(ssh-agent -s)" ```

  ![image](https://github.com/user-attachments/assets/a1c9336f-13ec-43b8-bb19-bcc995b91f16)

- Use command: ```ssh-add ~/.ssh/id_ed25519 ``` and it go request passphare:

  ![image](https://github.com/user-attachments/assets/c6e63e93-8b55-4ee8-823c-39cff2f26afe)

When show message below it's okay:

![image](https://github.com/user-attachments/assets/77805d59-768d-4769-8ddd-d3aa21824ae0)

6 - Open Github: https://github.com/ and clik "Settings" in your photo:
![image](https://github.com/user-attachments/assets/342db8f4-a965-4ae6-902e-e2882de9196a)

7 - left side, select item:``` SSH and GPG keys ```: 
![image](https://github.com/user-attachments/assets/cc0706e7-1648-4b82-a58d-5ac11b3651e9)

8 - Now, select option:``` SSH and GPG keys ```:
![image](https://github.com/user-attachments/assets/e71c596d-bb41-4265-aeaf-0f0a265b6fc7)

9 - Fill out fields below:
![image](https://github.com/user-attachments/assets/b1f938c2-ec96-44ae-8692-00636208cea0)

10 - Return in the command screem (bash) and copy public key:

- Use command: ``` cd ~/.ssh ``` after ``` ls ```

  ![image](https://github.com/user-attachments/assets/13634c6d-3af4-49ad-baa0-f824077c5900)

- Use command: ``` cat id_ed25519.pub ```. Copy key - begin: shh and finish: after email.
 
  ![image](https://github.com/user-attachments/assets/d545ccf8-a99b-46da-a9fc-0b371b60bf2d)
 
11 -  Return in the portal: GitHub, and paste Public Key:
![image](https://github.com/user-attachments/assets/6dc7cc6b-54e6-4cec-8080-44238087e9fa)

12 - After of click in "Add SSH key", confirm again your password and Done.


### Configuration Test 

13 - To Execuse again command: ``` git clone https://github.com/WanderBernardo/TestCloneGitDesktop ```.



