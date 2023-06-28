# Unit Test with .Net 7 with xUnit and MOQ

# O que é Teste Unitário?

Um teste de unidade é o menor pedaço de código que pode ser logicamente isolado em um sistema, geralmente pensamos no menor pedaço de código logicamente isolado como nossas funções. 
Com este pequeno pedaço de código, podemos executar testes automatizados que garantem que nosso código esteja sempre gerando o resultado correto.

# Por que devo testar meu código?

Economiza tempo: em alguns casos, elimina a necessidade de testes manuais
Automação: a capacidade de testar novamente o código alterado em tempo real

# Código eficiente: 
certifique-se de que todos os cenários possíveis sejam cobertos e, para tornar o teste de unidade possível, precisamos estruturar nosso código de maneira que possamos realmente testá-lo. 
O que significa que precisamos seguir certos padrões como SOLID.

# Documentação: 
Ajude-nos a entender a lógica por trás de nossos métodos
Qualidade: Melhore a qualidade de nossa base de código, ajude-nos a evitar adicionar dívidas de tecnologia o máximo possível
Confiável: Quando os testes estão passando e sendo executados automaticamente, podemos ter lançamentos mais suaves e mais frequentes

# O que é Mocking? 
Quando um serviço depende de outro serviço e queremos testar esse serviço.
Em vez de fazer o processo de inicialização completo do segundo serviço, podemos MOCKAR ele (fingir que está totalmente funcional) e podemos executar nossos testes com base nisso.


# Comandos 
dotnet new console -n "SeuProjetoTest"

nuget packages
  dotnet add package Microsoft.NET.Test.Sdk 
  dotnet add package xunit 
  dotnet add package xunit.runner.visualstudio 
  dotnet add package coverlet.collector 

dotnet new xunit -n "SeuProjetoTest.Test"
dotnet add package Moq 
