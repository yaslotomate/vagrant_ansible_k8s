# vagrant_ansible_k8s
vagrant cluster k8s version 1.23 | cni = cilium | container runtime = containerd | helm
prerequis: install virtualbox openssh-server ansible vagrant 
puis install plugin kubernetes.core
#ansible-galaxy collection install kubernetes.core

vagrant up 
vagrant ssh master 
