# Getting to grips with AWX 
## AWX Testing

Installing Gitlab on AWX Box

-[Gitlab Docs](https://about.gitlab.com/install/#ubuntu)

    
    sudo apt-get update
    sudo apt-get install -y curl openssh-server ca-certificates tzdata perl
    sudo apt-get install -y postfix

I selected no config 


     curl https://packages.gitlab.com/install/repositories/gitlab/gitlab-ee/script.deb.sh | sudo bash

Configure your domain below (ideally add it to DNS or host file)

    sudo EXTERNAL_URL="https://gitlab.example.com" apt-get install gitlab-ee


Get the password 

    sudo nano /etc/gitlab/initial_root_password

    sudo systemctl enable gitlab-runsvdir

Open your browser to .... and accept the cert (username: root and password listed in file from before)

    https://gitlab.example.com