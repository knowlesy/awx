# Getting to grips with AWX 
## AWX Testing

Study Material 

K8s / Kubernetes 

-[Gitlab Docs](https://about.gitlab.com/install/#ubuntu)

-[Gitlab Autoboot](https://stackoverflow.com/questions/27983295/gitlab-autostart-on-boot)

-[Connecting Gitlab to AWX](https://baptiste.bouchereau.pro/tutorial/setup-awx-with-gitlab/)

-[Resolving the self signed cert issue when creating a project](https://github.com/ansible/awx/issues/490)

Note you may need to set a custom dns record in your hosts file or if you have your own local dns servers there for Gitlab

-[Resolving Git Cloning with self signed cert](https://confluence.atlassian.com/fishkb/unable-to-clone-git-repository-due-to-self-signed-certificate-376838977.html)

    git -c http.sslVerify=false clone <repository-name>

or for the entire env

    git config --global http.sslVerify false


Dont forget to setup your details in VSCode!!!
      
      git config --global user.email "you@example.com"
      git config --global user.name "Your Name"

