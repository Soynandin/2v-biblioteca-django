# biblioteca-django

 Este projeto foi desenvolvido como parte das atividades da Residência de Software - Polo Jequié, com o tema Desenvolvimento de APIs com Django. O objetivo deste exercício é aplicar os conceitos de Class-Based Views (CBVs), além de explorar funcionalidades essenciais como paginação, filtros, busca e ordenação em uma API. Através deste exercício, os participantes da residência estão aprimorando suas habilidades em desenvolvimento de software e práticas de engenharia de software, com foco na criação de soluções escaláveis e bem estruturadas.

# API de Biblioteca com Django

Esta é uma API de Biblioteca construída com Django, utilizando **Class-Based Views (CBVs)**, com suporte para **paginação**, **filtros**, **busca** e **ordenação**.

## Funcionalidades

- **Paginação de Resultados**: Os endpoints fornecem suporte para a paginação dos dados retornados, facilitando a navegação em grandes volumes de registros.
- **Filtros, Busca e Ordenação**: É possível filtrar, buscar e ordenar os registros de livros, categorias e autores.
- **Views Baseadas em Classes (CBVs)**: A API foi implementada utilizando o padrão CBV para facilitar a organização e a reutilização do código.
- **URLs**: A API só funciona através do endereço `http://127.0.0.1:8000/api/`.

## Endpoints

### Livros
- **Lista de Livros**: `GET /livros/`  
  Retorna uma lista paginada de livros. Suporta filtros e ordenação.
  
- **Detalhes de Livro**: `GET /livros/<int:pk>/`  
  Retorna os detalhes de um livro específico com base no seu ID (`pk`).

### Categorias
- **Lista de Categorias**: `GET /categorias/`  
  Retorna uma lista paginada de categorias disponíveis.
  
- **Detalhes de Categoria**: `GET /categorias/<int:pk>/`  
  Retorna os detalhes de uma categoria específica com base no seu ID (`pk`).

### Autores
- **Lista de Autores**: `GET /autores/`  
  Retorna uma lista paginada de autores cadastrados.
  
- **Detalhes de Autor**: `GET /autores/<int:pk>/`  
  Retorna os detalhes de um autor específico com base no seu ID (`pk`).