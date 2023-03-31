# filer
Customized Templates for File Sharing. No no I mean pyinnyarbase 

This template is to update UI in filesharing pyin nyar base project in our aws ec2 instance

Please Follow the instruction 
-----------------------------

1. Connect to File Sharing (Pyinnyar Base) Running Instance

2. after ssh login, please go to this path.
  cd /home/ubuntu/env/lib/python3.8/site-packages/filer/templates/admin/
  
3. Remoe filer/ folder 
  rm -rf filer
  
4. Update This Plugin 
  git clone https://github.com/wwsict/filer.git
  
5. Restart Your Instance
  sudo service nginx restart
  sudo systemctl reload nginx 
  sudo supervisorctl reload 
  wait 10 seconds and type this below
  sudo supervisorctl status
  
When Supervisorctl status show our instance is up in running, we have successfully updated with this customized UI.
Thank you. zwelinux_15_10_2022_11_20_PM
