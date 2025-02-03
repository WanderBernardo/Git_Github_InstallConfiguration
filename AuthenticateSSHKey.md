
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

### return in the portal: GitHub

6 - 
