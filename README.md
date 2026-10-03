# Sistema de Gerenciamento de Tributos — Web

Interface web de um sistema para administração, consulta e emissão de tributos municipais, com foco no **Imposto Predial e Territorial Urbano (IPTU)**. O sistema permite controlar contribuintes, gerenciar imóveis e gerar guias de pagamento de forma digital.

Este repositório é exclusivamente o **Frontend** (camada de apresentação). Toda a lógica de negócio e o banco de dados ficam em uma API Backend independente, consumida via requisições RESTful.

## Funcionalidades

- Portal inicial com informações do projeto e avisos do sistema
- Tela de login e área administrativa
- Gestão de contribuintes e imóveis
- Geração de guias de pagamento do IPTU
- Páginas de apoio ao desenvolvimento: paleta de cores e campo de testes

> Algumas funcionalidades dependem da integração com o Backend e podem estar em desenvolvimento.

## Tecnologias

| Camada | Tecnologias |
| --- | --- |
| Frontend (este repositório) | HTML5, CSS3 e JavaScript (Vanilla) |
| Backend (repositório externo) | API RESTful em Java (Spring Boot) com PostgreSQL |

## Arquitetura

Sistema distribuído em duas partes que se comunicam por HTTP/JSON:

```
[ Navegador ]  →  Frontend (HTML/CSS/JS)  →  API REST (Spring Boot)  →  PostgreSQL
```

## Estrutura do Projeto

```
prg04projetoweb/
├── .vscode/                      # Configurações do editor
├── infrastructure/
│   ├── assets/
│   │   ├── audio/
│   │   │   └── background-music.mp3
│   │   ├── css/
│   │   │   └── style.css         # Estilos globais
│   │   ├── favicon/              # Ícones do site
│   │   ├── images/               # Imagens responsivas (400, 700 e 1000 px)
│   │   └── js/                   # Scripts: manipulação do DOM e requisições à API
│   └── pages/
│       ├── index.html            # Página inicial
│       ├── login.html            # Acesso ao sistema
│       ├── admin.html            # Área administrativa
│       ├── paleta.html           # Paleta de cores do sistema
│       ├── sandbox.html          # Campo de testes
│       └── atividade-3.html      # Atividade da disciplina
└── README.md
```

| Pasta / Arquivo | Descrição |
| --- | --- |
| `infrastructure/assets/` | Recursos estáticos: áudio, CSS, favicons, imagens e scripts JS |
| `infrastructure/pages/` | Todas as telas do sistema, incluindo a página inicial (`index.html`) |
| `infrastructure/pages/index.html` | Ponto de entrada: apresentação do projeto e avisos |

## Como Executar

1. Clone o repositório:
   ```bash
   git clone <url-do-repositorio>
   cd prg04projetoweb
   ```
2. Abra a pasta no VS Code e instale a extensão **Live Server**.
3. Clique com o botão direito em `infrastructure/pages/index.html` e escolha **Open with Live Server**.
4. Para as funcionalidades que dependem de dados, mantenha o Backend em execução e configure o endereço da API nos scripts em `assets/js/`.

## Autor

Desenvolvido por **Eduardo Nascimento Santos**.