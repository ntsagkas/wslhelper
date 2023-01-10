# wslhelper

cp config/template config/mysite.json
sudo ansible-playbook localSiteCreate.yaml --extra-vars "@config/mysite.json"