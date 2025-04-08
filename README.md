# IaC - Criação de Estrutura de Usuários, Diretórios e Permissões

## 📄 Descrição

Este projeto foi desenvolvido como parte do **Desafio do Bootcamp Santander - Linux para Iniciantes**, com o objetivo de aplicar os conceitos de administração de sistemas Linux por meio de um script que automatiza a criação de usuários, grupos, diretórios e permissões.

## 🚀 Funcionalidades do Script

- **Criação de Diretórios:**
  - `/publico`
  - `/adm`
  - `/ven`
  - `/sec`

- **Criação de Grupos de Usuários:**
  - `GRP_ADM`
  - `GRP_VEN`
  - `GRP_SEC`

- **Criação de Usuários e Associação aos Grupos:**
  - `GRP_ADM`: `carlos`, `maria`, `joao`
  - `GRP_VEN`: `debora`, `sebastiana`, `roberto`
  - `GRP_SEC`: `josefina`, `amanda`, `rogerio`

> Todos os usuários são criados com shell `/bin/bash`, diretório home, senha criptografada `@Mudar123`, e obrigatoriedade de trocar a senha no primeiro login.

- **Permissões Aplicadas aos Diretórios:**
  - Diretórios dos grupos (`/adm`, `/ven`, `/sec`): acesso exclusivo dos respectivos grupos (permissões `770`)
  - Diretório `/publico`: acesso liberado para todos os usuários (permissão `777`)
  - Propriedade dos diretórios atribuída ao `root` e ao grupo correspondente

## 🛠️ Tecnologias Utilizadas

- Shell Script (Bash)
- Linux (testado em distribuições baseadas em Debian/Ubuntu)

## 📦 Como Executar

1. Clone este repositório:
   ```bash
   git clone https://github.com/srthaiso/automacao_linux.git
   cd automacao_linux
   ```

2. Dê permissão de execução ao script:
   ```bash
   chmod +x iac1.sh
   ```

3. Execute o script como **root** ou com **sudo**:
   ```bash
   sudo ./iac1.sh
   ```

> ⚠️ **Importante**: Execute o script em um ambiente de testes para garantir que atende às necessidades antes de usar em produção.

## 👤 Autor

- **Ismael Nascimento**  
- Bootcamp Santander - Linux para Iniciantes  
- [Linkedin](https://www.linkedin.com/in/inascimento/)
