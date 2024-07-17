install ssh client https://www.cyberciti.biz/faq/how-to-install-ssh-on-ubuntu-linux-using-apt-get/
ssh-copy-id -f "-o IdentityFile /home/emmalinux/Downloads/kk.pem" ubuntu@3.137.218.102

ssh-copy-id -f "-o IdentityFile /home/emmalinux/Downloads/kk.pem" ubuntu@3.15.202.78

ssh-copy-id  ubuntu@18.118.137.74
ssh  ubuntu@18.118.137.74
ssh -o PubkeyAuthentication=no ubuntu@18.118.137.74


sudo vim /etc/ssh/sshd_config.d/60-cloudimg-settings.conf

sudo vim /etc/ssh/sshd_config
sudo systemctl restart ssh
sudo passwd ubuntu

ssh -o PubkeyAuthentication=no ubuntu@3.133.151.64
ssh-copy-id -o PubkeyAuthentication=no ubuntu@18.118.137.74
#####################################################################################################
sudo nano /etc/ansible/hosts    ----------def host s
ansible -i /home/emmalinux/Desktop/CI_CD/ansible/inventory.ini -m ping all
###############################################################################################################################3
ansible -i /home/emmalinux/Desktop/CI_CD/ansible/inventory.ini -m shell -a "sudo apt-get update && sudo apt-get install -y openjdk-17-jdk" all

ansible -i /home/emmalinux/Desktop/CI_CD/ansible/inventory.ini -m shell -a "sudo apt-get remove --purge -y openjdk-17-jdk && sudo apt-get autoremove -y && sudo apt-get clean" all

ansible-playbook -i inventory.ini myplaybook.yaml

 ansible-playbook -i inventory.ini docplaybook.yml 
 ansible-galaxy role install iam-surya369.java-jenkins-docker