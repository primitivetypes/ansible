# Primitive Types DevOps

## openvpn-server

### vagrant
Bring up the vagrant instance:
`vagrant up`

Destroy the vagrant instance:
`vagrant destroy`

### docker
Bring up the docker container and provision it:
`ansible-playbook -i docker-inventory.yml docker-playbook.yml`

Destroy the docker container:
`ansible-playbook -i docker-inventory.yml docker-destroy.yml`

### TODO
Handle persistence by setting up common directory structure for both docker and vagrant instances so that
signed keys/cert and the CA keys/cert land in the persistent directory.