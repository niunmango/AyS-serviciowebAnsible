# Ejemplo de uso de Ansible
## Asignatura: Automatización y Scripting (CURZA) https://web.curza.uncoma.edu.ar/
Ejemplo de uso de la herramienta Ansible, son necesarios cuatro nodos, un controller, uno load balancer y dos nodos para servidores web. Los mismos deben tener los nombres detallados en 'servidores.txt' y utilizar Ubuntu Server o similar. También debe poderse resolver sus nombres por DNS (o bien incluirlos en '/etc/hosts' del nodo controller)
Para mayor facilidad es necesario generar claves en el nodo controller e intercambiar con los nodos controlados

Uso de ejemplo:

'$ ansible-playbook -v playbooks/uptime.yml'

Si el usuario no es root las tareas que incluyan 'become: true' deberán ejecutarse con el modificador -K