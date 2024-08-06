Aqui está um README simplificado para o seu playbook:

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

Esse README fornece as informações essenciais para entender e usar o playbook.