# Sistema de Gerenciamento de Tributos - Web

## Sobre o Projeto
Esta é a interface web de um sistema desenvolvido para a administração, consulta e emissão de tributos municipais, com foco principal na gestão do Imposto Predial e Territorial Urbano (IPTU). O software permite o controle de contribuintes, o gerenciamento de imóveis e a geração de guias de pagamento de forma digital.

A aplicação adota uma arquitetura de sistemas distribuídos, onde este repositório atua exclusivamente como o **Frontend** (camada de apresentação). Toda a lógica de negócios e banco de dados é consumida via requisições RESTful a uma API **Backend** independente.

## Tecnologias Utilizadas
* **Frontend:** HTML5, CSS3 e JavaScript (Vanilla)
* **Backend (Repositório Externo):** API RESTful estruturada em Java (Spring Boot) e PostgreSQL

## Estrutura do Projeto
* `assets/`: Recursos estáticos (CSS, imagens e scripts JS para manipulação do DOM e requisições).
* `pages/`: Telas secundárias do sistema (gestão, cadastros, relatórios).
* `index.html`: Portal inicial de login/acesso.
