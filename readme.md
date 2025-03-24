# Autenticação com SAML2 em C#
 
Este projeto é uma aplicação ASP.NET Core que implementa um provedor de serviço (SP) que pode se autenticar por meio do protocolo SAML2 utilizando a biblioteca Sustainsys.Saml2 em um provedor de identidade (IDP) de teste da própria biblioteca.
 
## Tecnologias Utilizadas 
- ASP.NET Core
- Sustainsys.Saml2 
 
## Estrutura do Projeto

```bash
.
├── Pages                          # Contém as páginas Razor, que são usadas para gerar conteúdo HTML dinâmico.
│   ├── Index.cshtml               
│   └── Index.cshtml.cs            
├── Properties                     # Contém configurações adicionais, como informações sobre o ambiente de execução.
│   └── launchSettings.json        
├── Program.cs                     # Configura a autenticação SAML2 na aplicação ASP.NET Core
├── appsettings.json               # Configurações gerais da aplicação, como parâmetros de inicialização e configuração de serviços.             
├── metadata-sp.xml                # Arquivo de metadados do Service Provider (SP)
├── saml-csharp.csproj             # Dependências. 
├── readme.md     
```

## Instalação
1. Clone o repositório:

   ```sh
   git clone https://github.com/luizakuze/saml-csharp 
   ```
2. Adicione a seguinte linha ao arquivo  `/etc/hosts`:

   ```sh
   127.0.0.1 sp-csharp-local
   ```
2. Instale as dependências:

   ```sh
   dotnet restore saml-csharp.csproj
   ```
3. Execute a aplicação:

   ```sh
   dotnet run saml-csharp.csproj
   ``` 
 