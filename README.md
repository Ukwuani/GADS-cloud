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
