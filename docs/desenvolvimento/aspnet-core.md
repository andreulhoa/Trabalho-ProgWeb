# Desenvolvimento com ASP.NET Core

ASP.NET Core é um framework de código aberto, multiplataforma, desenvolvido pela Microsoft, para a construção de aplicações web modernas, incluindo serviços RESTful, aplicações web e APIs. É conhecido por sua alta performance, flexibilidade e facilidade de uso.

## O que é ASP.NET Core?

ASP.NET Core é uma reescrita completa do ASP.NET tradicional, com foco em performance e modularidade. Ele foi projetado para ser executado no .NET Core, mas também é compatível com o .NET Framework. ASP.NET Core é ideal para criar aplicações web modernas que podem ser implantadas em várias plataformas, como Windows, macOS, e Linux.

## Principais Recursos do ASP.NET Core

- **Multiplataforma:** Execute suas aplicações em Windows, macOS e Linux.
- **Alta Performance:** ASP.NET Core é otimizado para alta performance, com benchmarks que o colocam entre os frameworks web mais rápidos disponíveis.
- **Arquitetura Modular:** Utilize apenas os pacotes e middlewares necessários para sua aplicação, mantendo-a leve e eficiente.
- **Injeção de Dependência:** ASP.NET Core tem suporte nativo para injeção de dependência, facilitando a criação de aplicações escaláveis e testáveis.
- **Suporte para MVC e Razor Pages:** Escolha entre MVC para aplicações baseadas em padrões ou Razor Pages para uma abordagem mais simples e eficiente.

## Criando uma Aplicação ASP.NET Core

Aqui está um exemplo básico de como criar uma nova aplicação ASP.NET Core usando a CLI do .NET:

```bash
dotnet new webapp -n MinhaAplicacao
cd MinhaAplicacao
dotnet run
