# Entity Framework

Entity Framework (EF) é um ORM (Object-Relational Mapper) para .NET que permite aos desenvolvedores trabalhar com um banco de dados usando objetos .NET, eliminando a necessidade de grande parte do código SQL manual. O EF simplifica o acesso a dados em aplicativos .NET.

## Principais Recursos do Entity Framework

- **Modelo de Dados Baseado em Objetos:** O EF permite que você trabalhe com dados como objetos .NET, sem a necessidade de escrever SQL diretamente.
- **Suporte a Múltiplos Bancos de Dados:** Funciona com SQL Server, SQLite, PostgreSQL, MySQL, entre outros.
- **Migrations:** Migrations gerencia mudanças no esquema do banco de dados de maneira segura e automática.

## Usando Entity Framework

### Configurando o Contexto

O ponto central do EF é o `DbContext`, que é a ponte entre a aplicação .NET e o banco de dados:

```csharp
public class MeuContexto : DbContext
{
    public DbSet<Produto> Produtos { get; set; }

    protected override void OnConfiguring(DbContextOptionsBuilder optionsBuilder)
    {
        optionsBuilder.UseSqlServer(@"Server=meu_servidor;Database=minha_base_de_dados;Trusted_Connection=True;");
    }
}
