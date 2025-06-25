# 📋 Vue Kanban Board

Este é um projeto simples de **quadro Kanban** construído com **Vue 3**, **BootstrapVue 3** e **vuedraggable**. O usuário pode adicionar tarefas e arrastá-las entre colunas de status: **Pendente**, **Em Progresso**, **Testar** e **Feito**.

## 🖼️ Demonstração

Interface simples e funcional para gerenciamento visual de tarefas. As tarefas podem ser movidas entre as colunas com drag-and-drop.

## 🚀 Tecnologias Utilizadas

- [Vue 3](https://vuejs.org/)
- [BootstrapVue 3](https://github.com/cdmoro/bootstrap-vue-3)
- [vuedraggable](https://github.com/SortableJS/vue.draggable.next)
- [Bootstrap 5](https://getbootstrap.com/)

## 📦 Instalação

```bash
# Clone o repositório
git clone https://github.com/seu-usuario/seu-repositorio.git

# Acesse a pasta do projeto
cd seu-repositorio

# Instale as dependências
npm install

```

##▶️ Executar o Projeto
```bash
npm run serve
```
O projeto será servido localmente em algo como http://localhost:8080

## 🧱 Estrutura do Projeto

- `App.vue`: Componente principal que organiza a estrutura da aplicação, gerencia o estado das tarefas e distribui os dados entre os componentes.
- `components/FormTask.vue`: Componente responsável pelo formulário de adicionar nova tarefa, com input e botão.
- `components/KanbanColumn.vue`: Componente reutilizável que representa uma coluna do Kanban, recebe um título, lista de tarefas e classe de estilo como props.
- `main.js`: Arquivo principal que inicializa a aplicação Vue 3 e configura o uso do BootstrapVue 3.

##✍️ Como Usar
1.Digite o nome de uma nova tarefa no campo de texto.

2.Pressione Enter ou clique em "adicionar".

3.A tarefa será adicionada à coluna Pendente.

4.Você pode arrastar e soltar tarefas entre as colunas para alterar o status.

## 📌 Observações
⚠️O estado das tarefas não é persistido (não há uso de banco de dados ou localStorage).

Este projeto foi desenvolvido com o intuito exclusivo de **aprendizado e treino prático** com Vue.js. 

