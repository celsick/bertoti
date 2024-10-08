# Atividade 1: Comentário do livro de engenharia de software no Google | 8.8.2024

## Primeiro trecho
We see three critical differences between programming and software engineering: time, scale, and the trade-offs at play.
On a software engineering project, engineers need to be more concerned with the passage of time and the eventual need for change.
In a software engineering organization, we need to be more concerned about scale and efficiency, both for the software we produce as well as for the organization that is producing it.
Finally, as software engineers, we are asked to make more complex decisions with higher-stakes outcomes, often based on imprecise estimates of time and growth.

### Comentário
O trecho destaca três principais diferenças entre programação e engenharia de software: em projetos de engenharia de software, os engenheiros precisam estar mais preocupados com a passagem do tempo e a mudança,
diferentemente das organizações de engenharia de software, que focam mais na escala e eficiência. Em contrapartida, também é destacado que, como engenheiros de software, são solicitadas decisões mais complexas,
mesmo baseadas em estimativas de tempo imprecisas, que deveriam ser consideradas mais cruciais. 

## Segundo trecho
Within Google, we sometimes say, “Software engineering is programming integrated over time.”
Programming is certainly a significant part of software engineering: after all, programming is how you generate new software in the first place.
If you accept this distinction, it also becomes clear that we might need to delineate between programming tasks (development) and software engineering tasks (development, modification, maintenance).
The addition of time adds an important new dimension to programming. 
Cubes aren’t squares, distance isn’t velocity.
Software engineering isn’t programming.

### Comentário
O parágrafo destaca que engenharia de software é programação integrada ao longo tempo. São duas coisas distintas, porém a programação é com certeza uma parte significante da engenharia de software, pois é apartir dela que um novo software é desenvolvido. Além disso, aceitar essa distinção é crucial, justamente para destacar-se a diferença entre tarefas de programação e tarefas de engenharia de software, onde a primeira é apenas o desenvolvimento,
enquanto a outra engloba modificação e manutenção que podem ocorrer com o tempo. Concluindo, assim como o autor destaca: "A Adição de tempo cria uma nova
dimensão à programação". <br> Assim como cubos não são quadrados — embora os quadrados estejam presentes em cubos, engenharia de software não é 
programação, embora toda a programação seja crucial dentro dela.

# Atividade 2: Três exemplos de trade-offs citando requisitos não funcionais | 15.8.2024

## 1. Java X Python
Java é conhecido por sua robustez, desempenho e escalabilidade. Com uma forte tipagem e um sistema de tipos estáticos, Java oferece segurança de tipo e facilita a manutenção e a refatoração de grandes bases de código. Seu gerenciamento de memória com coleta de lixo e o modelo de concorrência são bem desenvolvidos, o que é ideal para aplicações empresariais complexas e sistemas de alta performance. Além disso, o Java tem um ecossistema vasto e maduro com uma grande quantidade de bibliotecas e frameworks, o que facilita o desenvolvimento de soluções complexas e escaláveis. No entanto, sua sintaxe mais verbosa pode levar a um desenvolvimento mais lento e menos flexível em comparação com linguagens mais dinâmicas.

Python, por outro lado, é valorizado por sua simplicidade e legibilidade, tornando o desenvolvimento mais rápido e menos propenso a erros. Com uma sintaxe concisa e uma vasta coleção de bibliotecas e frameworks, Python é ideal para prototipagem rápida, desenvolvimento web, e análise de dados. A linguagem é altamente dinâmica, o que facilita alterações e testes rápidos durante o desenvolvimento. No entanto, Python pode ter desempenho inferior em comparação com Java devido à sua natureza interpretada e menos eficiente em operações de baixo nível. Sua tipagem dinâmica também pode introduzir erros que são detectados somente em tempo de execução. A escolha entre Java e Python deve ser baseada nos requisitos específicos do projeto, como necessidade de desempenho, rapidez de desenvolvimento e flexibilidade.

## 2. Windows x Linux
Windows oferece uma interface gráfica amigável e um suporte robusto para uma ampla gama de softwares e aplicativos comerciais. Com um ecossistema bem integrado para usuários finais e suporte para uma variedade de hardware, o Windows é amplamente utilizado em ambientes corporativos e domésticos. Suas ferramentas de administração e suporte técnico são extensivas, e a compatibilidade com muitas aplicações de terceiros torna-o uma escolha popular para muitos usuários. No entanto, a natureza proprietária do Windows pode levar a custos de licença, e a segurança pode ser uma preocupação maior devido à sua popularidade como alvo para malware e ataques.

Linux, por outro lado, é um sistema operacional de código aberto conhecido por sua flexibilidade e segurança. Ele é altamente configurável, o que permite personalização extensiva para atender a necessidades específicas, e geralmente oferece melhor desempenho em hardware mais antigo. A natureza de código aberto e a ausência de custos de licença fazem do Linux uma escolha atraente para servidores e sistemas de missão crítica. No entanto, a curva de aprendizado pode ser mais acentuada para usuários que não estão familiarizados com o ambiente de linha de comando e o suporte para alguns aplicativos comerciais pode ser limitado. A escolha entre Windows e Linux depende das necessidades do usuário ou do ambiente de trabalho, considerando fatores como custo, flexibilidade, segurança e compatibilidade de software.

## 3. MongoDB x MySQL
**MongoDB** oferece flexibilidade e escalabilidade horizontal, sendo ideal para aplicações que lidam com dados semi-estruturados e que precisam de um esquema adaptável. Sua estrutura de documentos BSON permite um design de dados mais fluido, e suas capacidades de escalabilidade e replicação são vantajosas para aplicativos com grandes volumes de dados e alta demanda. No entanto, a falta de um esquema fixo pode levar a inconsistências, e sua consistência eventual pode ser um problema para sistemas que exigem alta precisão imediata.

**MySQL**, por sua vez, é robusto para aplicativos que necessitam de consistência e integridade dos dados, com suporte sólido a transações ACID. É ideal para sistemas com um esquema bem definido e que exigem alta precisão dos dados, como sistemas financeiros. Contudo, sua escalabilidade vertical é limitada e a administração de um banco de dados relacional pode ser mais complexa. Em resumo, a escolha entre MongoDB e MySQL deve depender das necessidades específicas do projeto, e em muitos casos, usar ambos pode ser uma estratégia eficaz para aproveitar os pontos fortes de cada um.

# Atividade 3: Escolher uma arquitetura de um sistema real que ele discute e comentar seus trade-offs | 15.8.2024
https://x.com/alexxubyte

[ESCOLHER UMA ARQUITETURA DE UM SISTEMA REAL QUE ELE DISCUTE (e.g. netflix), COLOCAR A IMAGEM QUE ELE POSTOU E DISCUTIR OS TRADE-OFFS APRESENTADOS (REQUISITOS NÃO FUNCIONAIS)]

![architectureofnetflix](https://github.com/user-attachments/assets/5a8833d2-e534-4664-818b-a938941d346d)

### 1. **Descentralização vs. Consistência**  
**Descentralização**: A Netflix adota uma estrutura descentralizada com microservices, permitindo que equipes diferentes desenvolvam e escalem suas partes do sistema de maneira independente.  
**Consistência**: A descentralização pode criar desafios de consistência de dados, que a Netflix aborda com sistemas de armazenamento e cache para garantir informações atualizadas, mas nem sempre em tempo real.

### 2. **Escalabilidade vs. Complexidade**  
**Escalabilidade**: A arquitetura da Netflix é feita para escalar horizontalmente, o que significa adicionar mais instâncias de serviços conforme a demanda aumenta, sem depender de um único servidor potente.  
**Complexidade**: Essa escalabilidade e o uso de microservices aumentam a complexidade na gestão do sistema, com desafios de comunicação entre serviços, coordenação de atualizações e monitoramento.

### 3. **Resiliência vs. Custo**  
**Resiliência**: A Netflix investe em resiliência, usando técnicas como failover e redundância de dados, além de práticas como o Chaos Engineering para testar o sistema em condições adversas.  
**Custo**: Essas medidas aumentam os custos operacionais, já que a infraestrutura, os testes e as operações necessárias para manter essa alta disponibilidade são caros.

### 4. **Desempenho vs. Flexibilidade**  
**Desempenho**: A Netflix implementa técnicas como caching, balanceamento de carga e otimização de rede para garantir alta performance no streaming.  
**Flexibilidade**: No entanto, essas otimizações podem limitar a flexibilidade no design e evolução dos serviços, restringindo adaptações para novas demandas.

### 5. **Automatização vs. Controle Manual**  
**Automatização**: A Netflix automatiza muitas operações, incluindo implantações e gestão de falhas, o que aumenta a eficiência e minimiza erros humanos.  
**Controle Manual**: Apesar dos benefícios, há situações em que o controle manual é necessário para lidar com problemas complexos ou mudanças específicas, criando um desafio no equilíbrio entre automação e intervenção humana.

# Atividade 4: Fazer classes UML ao lado do código Java mostrando a relação entre eles, como feito no quadro | 23.8.2024

![Mídia](https://github.com/user-attachments/assets/c45b3961-526e-449e-b499-2395eb32e0cc)

## Código em Java | Classes UML

<div class=cl>
package Atividade04;

import java.util.List;
import java.util.LinkedList;

public class LivroAutor {

    public class Biblioteca {
        //* Atributos
        private String nome;
        private String endereco;
        private int telefone;
        private List<Livro> livros; //* Relacionamento com a classe livros

        //* Construtor de classe
        public String getNome() {
            return nome;
        }
        public void setNome(String nome) {
            this.nome = nome;
        }

        public String getEndereco() {
            return endereco;
        }
        public void setEndereco(String endereco) {
            this.endereco = endereco;
        }

        public int getTelefone() {
            return telefone;
        }
        public void setTelefone(int telefone) {
            this.telefone = telefone;
        }

        public List<Livro> getLivros() {
            return livros;
        }
        public void setLivros(List<Livro> livros) {
            this.livros = livros;
        }
    }

    public class Livro {
        //* Atributos
        private String titulo;
        private int anoPublicacao;
    }
}
</div>
