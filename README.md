# Curso da Microsoft Learn: Criar uma API Web com os controladores do ASP.NET Core 
Primeiro projetinho API Web


SDK do .NET 6.0 precisa estar instalado.

Para criação de uma API Web com controladores ASP.NET Core:
- Crie uma pasta no local de sua preferência;
- Na IDE, abra a pasta e em seguida o terminal da IDE;
- Digite o comando 'dotnet new webapi -f net6.0'.

Para testar a api:
- Abra o terminal do projeto na IDE;
- No caminho do projeto que criou digite 'dotnet run';
- Instale REPL pelo terminal 'dotnet tool install -g Microsoft.dotnet-httprepl';
	(Ferramenta de linha de comando REPL HTTP do .NET irá fazer solicitações para a API)
- Para conexão com a API no REPL, digite 'httprepl https://localhost:{PORT}';
	(A 'PORT' está no arquivo 'launchSettings.json')
- No REPL digite 'connect https://localhost:{PORT}';
- Digite 'ls' para visualizar as APIs disponíveis;
- Digite 'cd {nome_api}' para mostrar uma saída da API;
- Caso dê algum erro de SSL, precisa gerar um certificado autoassinado para habilitar o uso de HTTPS:
	(Acesse https://learn.microsoft.com/en-us/dotnet/core/tools/dotnet-dev-certs)
- Para fazer solicitações CRUD:
	Para visualizar use 'get' ou 'get {id}' para retornar o dado específico;
	Para adicionar um dado novo 'post -c "{"name":"{nome}", "isGlutenFree":false}";
	Para atualizar 'put {id} -c "{"id": {id}, "name":"{nome}", "isGlutenFree":false}"';
	Para deletar 'delete {id}'.
- Sair do REPL digite 'exit';
- Sair do dotnet tecle Ctrl+C. 
