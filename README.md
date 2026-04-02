# P1Marcelo

### Integrantes do Grupo

* YASMIN ALVES DA SILVA / RA 25000193
* KEVIN HENRIQUE BENEDITO / RA 25000492
* VITOR LEONCIO BARTALANI / RA 2500095

---

### Descrição do Projeto

Este projeto consiste no desenvolvimento de um aplicativo Flutter contendo navegação entre telas, formulários com validação e uso de dados mockados em memória.

O aplicativo simula um sistema simples de autenticação de usuários, sem utilização de banco de dados ou APIs externas.

---

### Objetivo

Aplicar na prática os conceitos de:

* Navegação entre telas
* Organização arquitetural
* Uso de Models
* Manipulação de dados em memória
* Construção de formulários com validação

---

### Arquitetura do Projeto

O projeto foi estruturado seguindo a separação de responsabilidades:

* Models: Representação dos dados (ex: usuário)
* Views: Interfaces do usuário (telas)
* ViewModels: Regras de negócio e lógica das telas
* Data: Armazenamento mockado em memória

Essa organização evita que a lógica fique diretamente nas telas, facilitando a manutenção do código.

---

### Estrutura de Pastas

```bash
lib/
 ├── main.dart
 ├── app/
 │    ├── models/
 │    ├── data/
 │    ├── viewmodels/
 │    └── views/
```

---

### Fluxo do Aplicativo

1. Ao iniciar, o usuário visualiza a Splash Screen
2. O app navega automaticamente para a tela de Login
3. Caso não tenha cadastro, o usuário acessa a tela de Cadastro
4. O cadastro é salvo em memória
5. O usuário retorna ao Login
6. O sistema valida os dados informados
7. Em caso de sucesso, o usuário é direcionado para a Home

---

### Telas do Aplicativo

#### Splash Screen

* Tela inicial do aplicativo
* Exibida por alguns segundos
* Redireciona automaticamente para o Login

#### Login

* Campo de e-mail/usuário
* Campo de senha
* Validação dos dados
* Botão para acessar cadastro

#### Cadastro

* Campos para criação de usuário
* Validação de formulário
* Armazenamento em lista mockada

#### Home

* Exibição de um ícone centralizado
* Texto de boas-vindas

---

### Armazenamento de Dados

Os dados dos usuários são armazenados em memória utilizando:

* List<UsuarioModel>

Não foi utilizado banco de dados ou API, conforme solicitado na atividade.

---

### Tecnologias Utilizadas

* Flutter
* Dart

---

### Como Executar o Projeto

1. Clonar o repositório:

```bash
git clone https://github.com/SEU_USUARIO/P1Marcelo.git
```

2. Acessar a pasta do projeto:

```bash
cd P1Marcelo
```

3. Instalar dependências:

```bash
flutter pub get
```

4. Executar:

```bash
flutter run
```

---

### Funcionalidades Implementadas

* Splash Screen funcional
* Navegação entre telas
* Cadastro de usuário em memória
* Login com validação
* Tela Home após autenticação

---

### Observações

Este projeto tem como objetivo fins educacionais, focando na prática dos conceitos de arquitetura, navegação e manipulação de dados em Flutter.

Todos os integrantes participaram do desenvolvimento do projeto.
