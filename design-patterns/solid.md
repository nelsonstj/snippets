# SOLID
S - [SRP] Single Responsability Principle (Princípio da Responsabilidade Única) - coesão.
O - [OCP] Open/Closed Principle (Princípio do Aberto/Fechado) - herança, interface e composição.
L - [LSP] Liskov Substitution Principle (Princípio da Substituição de Liskov) - extensível sem modificações
I - Interface Segregation Principle (Princípio da Segregação de Interfaces) - coesão em interfaces (módulos enxutos)
D - Dependency Inversion Principle (Princípio da Inversão de Dependências) - depender de abstrações e não de classes concretas

1. SRP — Single Responsibility Principle:
Princípio da Responsabilidade Única — Uma classe deve ter um, e somente um motivo para mudar.
Esse princípio declara que uma classe deve ser especializada em um único assunto e possuir apenas uma responsabilidade dentro do software, ou seja, a classe deve ter uma única tarefa ou ação para executar.
A violação do SRP pode gerar alguns problemas, sendo eles:
- Falta de coesão: uma classe não deve assumir responsabilidades que não são suas;
- Alto acoplamento: mais responsabilidades geram um maior nível de dependências, deixando o sistema engessado e frágil para alterações;
- Dificuldades na implementação de testes automatizados: é difícil de “mockar” esse tipo de classe;
- Dificuldades para reaproveitar o código;

2. OCP — Open-Closed Principle:
Princípio Aberto-Fechado — Objetos ou entidades devem estar abertos para extensão, mas fechados para modificação, ou seja, quando novos comportamentos e recursos precisam ser adicionados no software, devemos estender e não alterar o código fonte original.

3. LSP — Liskov Substitution Principle:
Princípio da substituição de Liskov — Uma classe derivada deve ser substituível por sua classe base.
Exemplos de violação do LSP:
- Sobrescrever/implementar um método que não faz nada;
- Lançar uma exceção inesperada;
- Retornar valores de tipos diferentes da classe base;

4. ISP — Interface Segregation Principle:
Princípio da Segregação da Interface — Uma classe não deve ser forçada a implementar interfaces e métodos que não irão utilizar.
Esse princípio basicamente diz que é melhor criar interfaces mais específicas ao invés de termos uma única interface genérica.

5. DIP — Dependency Inversion Principle:
Princípio da Inversão de Dependência — Dependa de abstrações e não de implementações.
Programar pra interfaces e não para uma implementação ou para classes concretas.

# service locator
- responsável por injetar as dependencias. Conhece as interfaces e as classes concretas.
- IoC Containers
- Startup.ConfigureServices