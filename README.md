# Ansible_playbook_and_roles_for_DOCKER

Installation de docker et d'un conteneur nginx via Ansible

1) Création de l'inventaire qui contiendra l'hote, les alias + insérer IP_cible dans le fichier /etc/ansible/hosts
2) Dossier "roles" contenant les arborescences des rôles souhaités obtenus grâce à la commande "ansible-galaxy init <nom_du_role>
3) /roles/docker/tasks/main.yml, édition des tâches à effectuer pour les applicatifs en question
4) /roles/docker/vars/main.yaml, paramétrage des variables de nos tasks
5) Création du playbook.yml qui orchestrera l'injection des applicatifs en fonction des machine cibles (alias)
6) Executer le playbook "ansible-playbook playbook.yml -i inventaire.ini" ((-vvv) pour le mode debug)
