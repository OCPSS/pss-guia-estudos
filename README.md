# 📚 Guia de Estudos — Projetos de Sistemas de Software

Guia de estudos para a disciplina de **Projetos de Sistemas de Software (PSS)** da **UFES**, com foco no desenvolvimento de sistemas em **Java** orientados a objetos, aplicando princípios de engenharia de software e padrões de projeto.

> 💡 **Dica:** faça os exercícios e atividades **no caderno**. Nas provas você vai escrever código à mão, então pratique assim desde o início.

---

## Sumário

1. [Como usar este guia](#como-usar-este-guia)
2. [Requisitos básicos](#requisitos-básicos)
3. [Conteúdo da disciplina](#conteúdo-da-disciplina)
4. [Requisitos adicionais](#requisitos-adicionais)
5. [Dicas importantes](#dicas-importantes)
6. [Ferramentas](#ferramentas)
7. [Referências](#referências)

---

## Como usar este guia

O conteúdo está organizado em três níveis:

| Nível | O que é | Quando estudar |
|---|---|---|
| **Requisitos básicos** | Base de Java, OO, Swing e UML | Antes ou logo no início da disciplina |
| **Conteúdo da disciplina** | Acoplamento, coesão, SOLID e padrões de projeto | Ao longo do semestre |
| **Requisitos adicionais** | Git, banco de dados, logging e variáveis de ambiente | Antes dos trabalhos práticos |

### 🧭 Ordem de estudo sugerida

1. Fundamentos de Java e Orientação a Objetos
2. Collections e Exceptions
3. UML (diagrama de classes primeiro)
4. Maven e Git
5. Acoplamento, coesão e princípios SOLID
6. Padrões de projeto (criacionais → estruturais → comportamentais)
7. Java Swing
8. Persistência com DAO/Repository, logging e variáveis de ambiente

Use as caixas de seleção (`- [ ]`) para acompanhar seu progresso em uma cópia do guia.

---

## Requisitos básicos

### ☕ Java (JDK 17 ou 21)

Domine a linguagem: sintaxe, APIs principais e boas práticas.

#### Fundamentos

- [ ] Variáveis
- [ ] Tipos primitivos e não primitivos
- [ ] Métodos (funções)
- [ ] Arrays e `ArrayList`
- [ ] Packages e imports

#### Orientação a Objetos

- [ ] Classes, objetos e métodos
- [ ] Construtores
- [ ] Encapsulamento
- [ ] Herança e superclasses
- [ ] Classes abstratas
- [ ] Interfaces
- [ ] Polimorfismo
- [ ] Abstração
- [ ] Enums
- [ ] Modificador `final`

#### Collections e estruturas de dados

- [ ] `List`, `ArrayList` e `LinkedList`
- [ ] `Stack`
- [ ] `Queue`
- [ ] `Map` e `HashMap`
- [ ] `HashSet` e `LinkedHashSet`

#### Funcionalidades avançadas

- [ ] Records
- [ ] Streams
- [ ] Exceptions (`try`, `catch`, `throw`, `throws`)
- [ ] Reflection API

#### Threads e concorrência *(opcional — aprenda pelo menos o básico)*

- [ ] `Thread` e concorrência
- [ ] Sincronização

### 🖼️ Interface gráfica com Java Swing

- [ ] `JFrame`, `JDialog` e `JPanel`
- [ ] Componentes e eventos
- [ ] Layouts e listeners

### 📐 UML

- [ ] Diagrama de classes
- [ ] Diagrama de sequência
- [ ] Diagrama de estados

---

## Conteúdo da disciplina

### 🔗 Acoplamento e coesão

- [ ] **Baixo acoplamento:** classes dependem pouco umas das outras
- [ ] **Alta coesão:** cada classe tem um propósito bem definido

O resultado é um código mais modular e fácil de manter.

### 📦 Gerenciador de dependências (Maven)

- [ ] Uso do Maven
- [ ] Instalação e configuração
- [ ] Configuração do `pom.xml`
- [ ] Ciclo de vida do projeto: build, execução e testes

### 🔠 Princípios SOLID

| Sigla | Princípio | Ideia central |
|---|---|---|
| **S** | Single Responsibility | Uma classe deve ter um único motivo para mudar |
| **O** | Open/Closed | Aberta para extensão, fechada para modificação |
| **L** | Liskov Substitution | Subclasses devem poder substituir suas superclasses sem quebrar o programa |
| **I** | Interface Segregation | Prefira várias interfaces específicas a uma interface genérica |
| **D** | Dependency Inversion | Dependa de abstrações, não de implementações concretas |

### 🔁 Outros princípios

| Princípio | Ideia central |
|---|---|
| **DRY** (Don't Repeat Yourself) | Evite duplicar lógica; cada conhecimento deve ter uma única representação |
| **Lei de Demeter** | Um objeto deve conversar apenas com seus "vizinhos" diretos, evitando cadeias como `a.getB().getC().fazer()` |

### 🧠 Padrões de projeto (GoF)

#### 🏗️ Criacionais

| Padrão | Ideia central |
|---|---|
| Singleton | Garante uma única instância de uma classe |
| Factory Method | Delega às subclasses a decisão de qual objeto criar |
| Abstract Factory | Cria famílias de objetos relacionados sem especificar classes concretas |
| Builder | Constrói objetos complexos passo a passo |

#### 🧱 Estruturais

| Padrão | Ideia central |
|---|---|
| Adapter | Faz interfaces incompatíveis trabalharem juntas |
| Proxy | Fornece um substituto que controla o acesso a outro objeto |
| Façade | Oferece uma interface simples para um subsistema complexo |
| Composite | Trata objetos individuais e composições de forma uniforme (estrutura em árvore) |
| Decorator | Adiciona comportamento a um objeto dinamicamente, sem herança |

#### 🧩 Comportamentais

| Padrão | Ideia central |
|---|---|
| Strategy | Encapsula algoritmos intercambiáveis |
| Chain of Responsibility | Passa uma requisição por uma cadeia de tratadores |
| Observer | Notifica automaticamente os interessados quando um objeto muda |
| Command | Encapsula uma ação como objeto (permite desfazer, enfileirar, registrar) |
| Memento | Salva e restaura o estado de um objeto sem violar o encapsulamento |
| State | Altera o comportamento do objeto conforme seu estado interno |
| Template Method | Define o esqueleto de um algoritmo, deixando passos para as subclasses |

#### 📦 Outros padrões úteis

| Padrão | Ideia central |
|---|---|
| DAO | Isola o acesso ao banco de dados do resto do sistema |
| Repository | Abstrai a persistência como uma coleção de objetos de domínio |
| Prototype | Cria novos objetos clonando um existente |
| Flyweight | Compartilha objetos para economizar memória |

---

## Requisitos adicionais

### 🌱 Git e GitHub

- [ ] Versionamento básico
- [ ] Branches, commits e pull requests
- [ ] Repositórios privados
- [ ] Adicionar o professor como colaborador

### 🗃️ Banco de dados e persistência

- [ ] SQLite
- [ ] H2
- [ ] MySQL (via JDBC)
- [ ] Operações CRUD
- [ ] Aplicação dos padrões DAO e Repository

### 📊 Logging

- [ ] Escrita e leitura de logs
- [ ] Formatos: JSON, XML, CSV ou banco de dados

### 🔐 Variáveis de ambiente

- [ ] Uso de arquivos `.env` com bibliotecas como [dotenv-java](https://github.com/cdimascio/dotenv-java)

---

## Dicas importantes

### 📆 Rotina de estudos

- Revise o conteúdo **na mesma semana** em que foi apresentado.
- Faça os exercícios **no caderno**.
- Foque em entender o problema e qual é a melhor solução, não só em decorar código.

### 📝 Provas

- Getters e setters podem ser indicados com um comentário (`// getters` / `// setters`), desde que todos sejam usados.
- Implemente corretamente os métodos que a questão pede.
- Priorize as questões de **maior valor e menor dificuldade**.

### 👥 Trabalhos

- Crie repositórios **privados** no GitHub e adicione o professor como colaborador.
- Planeje desde o início:
  - a estrutura do banco de dados;
  - a arquitetura do sistema;
  - a divisão de tarefas da equipe.

> ⚠️ **Atenção:** o projeto pode ultrapassar **100 classes**. Não deixe para a última hora.

---

## Ferramentas

Ferramentas disponíveis no laboratório:

| Categoria | Ferramentas |
|---|---|
| JDK | Java 17 ou 21 |
| IDE | NetBeans, VS Code, Eclipse ou IntelliJ |
| Modelagem UML | Astah Community |
| Versionamento | GitHub ou GitLab |

---

## Referências

### 📖 Livros

- **Clean Code** — Robert C. Martin
- **Effective Java** — Joshua Bloch
- **Design Patterns: Elements of Reusable Object-Oriented Software** — Gamma, Helm, Johnson e Vlissides (GoF)
- **UML Essencial** — Martin Fowler
- **Engenharia de Software** — Ian Sommerville

### 🌐 Sites e documentação

- [Refactoring.Guru — Padrões de projeto](https://refactoring.guru/pt-br/design-patterns)
- [Documentação oficial do Java](https://docs.oracle.com/en/java/javase/21/)
- [Maven — Guia de introdução](https://maven.apache.org/guides/getting-started/)
- [Pro Git (livro gratuito, em português)](https://git-scm.com/book/pt-br/v2)
