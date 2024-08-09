![Ansible](https://img.shields.io/badge/ansible-%231A1918.svg?style=for-the-badge&logo=ansible&logoColor=white)
![ChatGPT](https://img.shields.io/badge/chatGPT-74aa9c?style=for-the-badge&logo=openai&logoColor=white)
[![Linkedin](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/fernando-dias-da-silva/)

---

# Ansible Playbook: Configuração de Servidor Web

Este playbook do Ansible automatiza a configuração de um servidor web com PHP, MySQL (Percona), HTTPD, e outras dependências essenciais.

## Pré-requisitos

- **Sistema Operacional:** CentOS/RHEL 9 ou equivalente.
- **Permissões:** Acesso root ou permissões `sudo`.
- **Ansible:** Instalado na máquina de controle.
- **Variáveis de Ambiente:** Definidas no arquivo `vars/env.yml`.

## Uso

1. **Clone este repositório:**
   ```bash
   git clone <URL-do-seu-repositorio>
   cd <nome-do-repositorio>
   ```

2. **Defina as variáveis no arquivo `vars/env.yml`.**

3. **Execute o playbook:**
   ```bash
   ansible-playbook -i <arquivo-de-inventario> playbook.yml
   ```

## Principais Funcionalidades

- Instalação e configuração dos repositórios EPEL, Remi, e Percona.
- Instalação do PHP 8.2 e suas extensões.
- Instalação do servidor HTTPD e dependências adicionais.
- Configuração inicial do MySQL com Percona.
- Desativação do SELinux.
- Ajustes de configuração do PHP.

## Observações

Certifique-se de que as variáveis de ambiente estejam corretamente definidas no arquivo `vars/env.yml`, especialmente `MYSQL_ROOT_PASSWORD`.

---

Esse README foi criado com a ajuda de Inteligencia Artificial
