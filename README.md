# Webserver Role - Projeto Ansible

Este projeto contém uma **role Ansible** para configurar servidores web com Nginx. Ele foi criado como parte de um estudo prático de automação de infraestrutura usando Ansible.

---

## Conteúdo do projeto

- `hosts` – Arquivo de inventário com os endereços IP dos servidores.
- `playbooks/setup.yml` – Playbook principal que instala e configura o Nginx.
- `roles/` – Pasta onde futuras roles podem ser adicionadas.

---

## Pré-requisitos

- Servidores Linux com acesso via SSH.
- Ansible instalado na máquina de controle.
- Chave SSH configurada para login sem senha nos servidores.

---

## Como usar

1. **Editar o inventário** (`hosts`) com os IPs dos servidores que você quer gerenciar.
2. **Executar o playbook**:
   ```bash
   ansible-playbook -i hosts playbooks/setup.yml
