# GADS-cloud

##### 1. Getting Started With Computed Engines

- [x] Get list of zones in the <b>Region</b>
  `gcloud compute zones list | grep us-central1`
  <br/>

- [x] Set zones
  `gcloud config set compute/zone us-central1-b`
  <br/>
  
- [x] Create virtual machine on compute engine
  ```
    gcloud compute instance create "my-vm-1"  \
    --machine-type "n1-standard-1" \
    --image-project "debian-cloud" \
    --image "debian-9-stretch-v20190213" \
    --subnet "default"
  ```

- [x] Test the vm by pinging it through ssh


##### 2. Getting started with market place

- [x] deploy a LAMP stack
  `gcloud deployment-manager deployments create my-dep --config lampstack.jinja`
  
 - [x] verify deployment by checking into the directory
  `cd /opt/bitnami`
 - [x] expose the phpinfo file
  `sudo sh -c 'echo "<?php phpinfo(); ?>" > apache2/htdocs/phpinfo.php'`
  - [x] visit the phpinfo rule -> `http://[SITE_ADDRESS]/phpinfo.php`
