# Assemblies

Assemblies são os blocos de construção fundamentais de uma aplicação .NET. Eles contêm o código compilado (IL - Intermediate Language), bem como metadados e recursos, como imagens ou textos, necessários para a execução do programa.

## O que é um Assembly?

Um assembly pode ser um arquivo `.dll` (biblioteca de link dinâmico) ou um arquivo `.exe` (executável). Ele inclui todos os metadados necessários para que o .NET identifique e carregue corretamente os tipos contidos nele.

## Tipos de Assemblies

Existem dois tipos principais de assemblies:

- **Assemblies Privados:** Utilizados exclusivamente por uma aplicação. Eles são implantados junto com a aplicação e não podem ser compartilhados com outras aplicações.
- **Assemblies Compartilhados:** Instalados no GAC (Global Assembly Cache) e podem ser compartilhados por várias aplicações.

## Estrutura de um Assembly

Cada assembly contém:

- **Manifesto:** Contém metadados sobre o assembly, incluindo informações sobre versões, cultura e referências a outros assemblies.
- **Metadados de Tipo:** Contêm definições de todos os tipos (classes, interfaces, etc.) incluídos no assembly.
- **Código IL:** O código intermediário que será compilado em tempo de execução pelo CLR.
- **Recursos:** Dados como imagens, arquivos de texto, e outros recursos necessários para a aplicação.

## Vantagens do Uso de Assemblies

- **Modularidade:** Assemblies permitem dividir o código em módulos, facilitando a manutenção e a reutilização.
- **Versionamento:** O manifesto do assembly permite versionamento, garantindo que as aplicações utilizem a versão correta das bibliotecas.
- **Distribuição Simplificada:** Assemblies podem ser facilmente distribuídos e instalados, especialmente os assemblies compartilhados através do GAC.

## Criando e Usando Assemblies

Aqui está um exemplo básico de como criar e usar assemblies no .NET:

### Criando um Assembly

```bash
csc /target:library /out:MeuAssembly.dll MeuCodigo.cs
