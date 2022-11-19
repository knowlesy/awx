# Getting to grips with AWX 
## AWX Testing

Connecting Gitlab To AWX

-[baptiste.bouchereau.pro Guide](https://baptiste.bouchereau.pro/tutorial/setup-awx-with-gitlab/)

on the Linux AWX Box
    
    ssh-keygen -f awx_ssh_key

Enter pass 


     cat awx_ssh_key.pub

Add the key to your user > SSH Keys 

Run the following on the box 

    cat awx_ssh_key

Add this as a source control cred in creds in AWX along with your priv key

Create a project in git if you havent already and grab the clone ssh url 

Head into AWX and create a project specify git type and paste in your url and specify the creds

    git@gitlab.example.com:gitlabuser/test.git

Save and this should be successful 