
### Documents:

- https://github.blog/security/application-security/token-authentication-requirements-for-git-operations/


### Create Repository in the GitHub

- Repository name: TestCloneGitDesktop
- "Private"

Link: https://github.com/WanderBernardo/TestCloneGitDesktop

This repository can be canceled in the finish configuration of the token.

### Configuration: Authenticate Token

1 - Open Github: https://github.com/ and clik "Settings" in your photo:
![image](https://github.com/user-attachments/assets/342db8f4-a965-4ae6-902e-e2882de9196a)

2 - Scroll down to the option: "Developer settings", left side.
![image](https://github.com/user-attachments/assets/8e5f3169-691e-4034-a39f-ae8239a2a75b)

3 - Now, select item: "Personal access Tokens" and "Token (classic)":
![image](https://github.com/user-attachments/assets/a3afab22-9a13-4300-8b60-37b97550e2cf)

4 - click in "Generate new token" and "Generate new token (classic)", after the github going to request confirm your password:
![image](https://github.com/user-attachments/assets/119574cb-390d-4e36-8080-3ae094189002)

5 - After confirm again your password so, it going to open screen where you need configurate the permission this token:
![image](https://github.com/user-attachments/assets/dc9096eb-1170-4c30-8eac-5e518ee7949b)

At this case, I'm going to configurate:
   * Note: Use in my notebook personal.
   * Expiration: 30 days
   * Select scopes:
        * Repo: Full
     Other items: I don't mark 
![image](https://github.com/user-attachments/assets/a00b0871-ecae-49f2-8694-7a680001185e)

6 - At the end page, click in the botton "Generate token":
![image](https://github.com/user-attachments/assets/f23f855b-4a89-448f-9ff7-18405b754d99)

Don't leave the screen until you complete the configuration in Git and verify that it worked
![image](https://github.com/user-attachments/assets/a1d70cd2-6390-43c1-b469-ee87a4cab9c8)

7 - Open in the command screen(Bash) and make command according below (in the same sequence):
- Use command: ``` git config --global credencial.helper store ```
![image](https://github.com/user-attachments/assets/7d18f775-b6ac-4605-840e-745db23e3dce)

- Use command: ``` git clone https://github.com/WanderBernardo/TestCloneGitDesktop ```
![image](https://github.com/user-attachments/assets/8a26a276-32ef-4acf-857d-420d87a6fb3c)

8 - When typing the above command and not will be opened portal of the "Github", it will show screen below:
![image](https://github.com/user-attachments/assets/f0a1bd44-3f41-4dae-a3c3-5031f4a7ff6f)

Then, Select "Browser/Device" or "Token". In this case, I selected: "Token" and paste Token previously created.

After, if will go to show mensage:
![image](https://github.com/user-attachments/assets/337ae585-938d-4cd8-b86a-272ac4f8cffd)


### Configuration Test 

9 - Delete clone foulder created in the your device:
![image](https://github.com/user-attachments/assets/f44a8de9-2b36-4051-b70a-197438aeba1e)

10 - To Execuse again command: ``` git clone https://github.com/WanderBernardo/TestCloneGitDesktop ```.

If it don't request again for token. Configuration finished correctly!

## Consult or Delete token

Go to step 01, 02, 03 and 04.
![image](https://github.com/user-attachments/assets/8dd95ec6-37d8-4434-b456-b26fb8e0e82c)




