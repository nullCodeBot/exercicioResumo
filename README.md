Relatório de Aprendizagem em Programação Orientada a Objetos e Padrões de Desenvolvimento

1. Introdução

Neste relatório, apresento uma análise dos códigos desenvolvidos durante o estudo de Programação Orientada a Objetos e padrões de projeto em C#. Tive inúmeras oportunidades de aprender sobre pontos-chave, incluindo herança, polimorfismo, interfaces, padrão Disposable, boas práticas de design e refatoração de código.

2. Conhecimentos Adquiridos

2.1 Herança e Polimorfismo

Durante várias implementações, tive a oportunidade de usar herança e polimorfismo para criar sistemas flexíveis e reutilizáveis. Alguns registros interessantes incluem:

Sistema de Processamento de Documentos: Criei uma classe base Documento e classes derivadas DocumentoTexto, DocumentoHTML e DocumentoPDF, cada uma com sua implementação do método Imprimir() e ConteudoFormatado().

Sistema de Notificação: Criei uma classe base Notificacao e classes derivadas NotificacaoEmail, NotificacaoSMS e NotificacaoPush, com substituição do método Enviar().

E-commerce Simplificado: Uma classe abstrata Produto e classes concretas ProdutoFisico, ProdutoDigital e Servico, cada uma com sua própria implementação do método CalcularPrecoFinal().

Reflexão: O uso de herança e polimorfismo ajudou a eliminar a duplicação de código ao compartilhar características e comportamentos, tornando o sistema mais dinâmico e permitindo o tratamento de objetos de forma abstrata.

2.2 Interfaces e Single Responsibility Principle (SRP)

Além disso, comecei a aprender sobre interfaces, ajudando a desacoplar funcionalidades:

Uso de interfaces: Implementação de IEntregavel, ITributavel e IReembolsavel para produtos no sistema de e-commerce.

Repositórios: Uso de IRepositorio<T> para padronizar operações CRUD e herança de RepositorioBase<T> para reaproveitamento de funcionalidades comuns.

Reflexão: A implementação de interfaces permitiu a separação de responsabilidades e melhor organização do sistema, tornando-o mais escalável e modular.

2.3 Gerenciamento de Recursos com Disposable

Foi necessário garantir a liberação correta de recursos:

Classe GerenciadorConexao: Simula uma conexão com banco de dados e implementa IDisposable para liberação adequada de recursos.

Sistemas de Pagamento: Implementação do padrão Disposable em ProcessadorCartaoCredito, garantindo que a conexão seja encerrada corretamente após o uso.

Reflexão: O uso do padrão Disposable enfatizou a importância de liberar recursos com segurança, evitando vazamentos de memória. O bloco using permitiu que os objetos fossem descartados automaticamente após o uso.

2.4 Ocultação vs. Sobrescrita de Métodos

Sobrescrita (override): Permite modificar um método herdado, mantendo a compatibilidade com a classe base.

Ocultação (new): Substitui um método da classe base, mas sem manter a ligação com a versão original.

Reflexão: override é a melhor opção na maioria dos casos, pois garante que a chamada do método ocorra corretamente, mesmo quando o objeto é referenciado como um tipo base. O uso de new pode tornar o comportamento do código menos previsível.

2.5 Refatoração e Melhoramento de Código

O código foi refatorado para se tornar mais modular, organizado e reutilizável:

Implementação de interfaces para responsabilidade única.

Uso de métodos virtuais para eliminar redundância.

Utilização do padrão Disposable para garantir liberação de recursos.

Reflexão: A refatoração melhora a qualidade do código, tornando-o mais compreensível e fácil de manter no longo prazo.

3. Conclusão

Os exercícios demonstraram na prática conceitos fundamentais de POO e padrões de projeto, ajudando a construir um software mais organizado, flexível e manutenível.

Principais aprendizados:

-> Herança reduz a duplicidade de código e melhora a reutilização.

-> Interfaces promovem desacoplamento e expansibilidade.

-> Padrão Disposable evita problemas de gerenciamento de memória.

-> Polimorfismo permite tratar objetos de forma uniforme.

-> Refatoração melhora a estrutura do sistema e facilita manutenção futura.

Esses conceitos auxiliam no desenvolvimento de código profissional em C#, permitindo a expansão dos sistemas sem comprometer sua qualidade e organização.

**UM ADENDO, A PARTIR DO EXERCICIO 3.2, OS CÓDIGOS USADOS FORAM GERADOS POR AI**
