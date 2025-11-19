# Sistema E-commerce MVC - Documentação do Projeto

## Visão Geral
Sistema de gerenciamento de e-commerce desenvolvido com padrão MVC (Model-View-Controller) utilizando PHP 8.2, MySQL, HTML5, CSS3 e JavaScript.

## Data de Criação
19 de Novembro de 2025

## Tecnologias
- **Backend:** PHP 8.2 com PDO
- **Frontend:** HTML5, CSS3 responsivo, JavaScript Vanilla
- **Banco de Dados:** MySQL 8.0 (Schema: site_mvc)
- **Arquitetura:** MVC puro (sem frameworks)
- **Servidor:** PHP Built-in Server (porta 5000)

## Estrutura do Projeto

### Model (Camada de Dados)
- `Model/CategoriaModel.php` - CRUD de categorias
- `Model/ProdutoModel.php` - CRUD de produtos com relacionamento
- `Model/ClienteModel.php` - CRUD de clientes

### Controller (Camada de Lógica)
- `Controller/CategoriaController.php` - Controle de categorias
- `Controller/ProdutoController.php` - Controle de produtos e catálogo
- `Controller/ClienteController.php` - Controle de clientes

### View (Camada de Apresentação)
- `View/layouts/` - Header e footer reutilizáveis
- `View/categorias/` - Interfaces para categorias (listar, criar, editar)
- `View/produtos/` - Interfaces para produtos (listar, criar, editar, catálogo)
- `View/clientes/` - Interfaces para clientes (listar, criar, editar)
- `View/home.php` - Página inicial

### Configuração
- `config/database.php` - Configuração PDO MySQL
- `index.php` - Front controller e roteamento

### Assets
- `assets/css/style.css` - CSS responsivo completo
- `assets/js/script.js` - Validações e interatividade

### Banco de Dados
- `database_setup.sql` - Script completo para MySQL Workbench

## Banco de Dados

### Schema
`site_mvc`

### Tabelas
1. **tbl_categoria** - Categorias de produtos
2. **tbl_produto** - Produtos com FK para categoria
3. **tbl_cliente** - Clientes cadastrados

### Configuração Atual
- Host: localhost
- Database: site_mvc
- User: root
- Password: (vazio)

## Funcionalidades Implementadas

### CRUD Completo
- ✅ Categorias (Create, Read, Update, Delete)
- ✅ Produtos (Create, Read, Update, Delete)
- ✅ Clientes (Create, Read, Update, Delete)

### Recursos Adicionais
- ✅ Catálogo público de produtos
- ✅ Relacionamento produto-categoria
- ✅ Controle de estoque
- ✅ Validação frontend (JavaScript)
- ✅ Validação backend (PHP)
- ✅ Mensagens de feedback (sessões)
- ✅ Design responsivo (mobile, tablet, desktop)
- ✅ Menu hambúrguer mobile

## Responsividade
- Desktop: > 768px
- Tablet: 481px - 768px
- Mobile: < 480px

## Segurança
- PDO com prepared statements
- Escapamento HTML
- Validação de dados
- Sessões PHP

## Arquivos Importantes
- `database_setup.sql` - **EXECUTAR NO MYSQL WORKBENCH**
- `README.md` - Documentação completa
- `index.php` - Ponto de entrada

## Workflow
- **Nome:** Start PHP Server
- **Comando:** `php -S 0.0.0.0:5000 -t .`
- **Porta:** 5000
- **Status:** Configurado e rodando

## Próximas Melhorias Sugeridas
- Sistema de carrinho de compras
- Sistema de busca e filtros
- Paginação de resultados
- Upload de imagens de produtos
- Sistema de pedidos
- Autenticação de administradores

## Notas de Desenvolvimento
- O padrão MVC foi implementado de forma pura, sem frameworks
- Todos os dados de exemplo estão incluídos no script SQL
- O sistema está pronto para uso após configurar o banco de dados
- Design moderno com paleta azul (#2563eb) e gradientes
