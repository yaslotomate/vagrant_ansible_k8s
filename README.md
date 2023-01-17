# vagrant_ansible_k8s
vagrant cluster k8s version 1.25 | cni = cilium 1.12.4| container runtime = containerd 1.5.9|
prerequis: install virtualbox openssh-server ansible vagrant 
puis install plugin kubernetes.core
#ansible-galaxy collection install kubernetes.core |

vagrant up |
vagrant ssh master 


si vous voulez envoyer doc,fichier ==>
vagrant plugin install vagrant-scp |
vagrant scp [nom_vm]:<remote_path>  <local_path> |
vagrant scp <local_path> [nom_vm]:<remote_path>


si vous voulez configuré dns ===>  sudo apt-get install ruby-full rubygems | vagrant plugin install vagrant-dns 



vm.dns.tld: définissez le tld pour la machine virtuelle donnée. Aucun défaut.
vm.dns.tlds: Définissez plusieurs tlds. Défaut:[tld]
vm.dns.patterns: une liste de modèles de domaine à faire correspondre. Par défaut à[/^.*{host_name}.{tld}$/]
