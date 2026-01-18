# Design Patterns trong Java - Tài liệu Tổng quan

Tài liệu toàn diện về các Design Patterns trong Java, bao gồm lý thuyết, khái niệm, và hướng dẫn áp dụng.

## 📖 Mục lục

1. [Giới thiệu Design Patterns](#giới-thiệu-design-patterns)
2. [Phân loại Design Patterns](#phân-loại-design-patterns)
3. [Gang of Four (GoF) Overview](#gang-of-four-gof-overview)
4. [Creational Design Patterns](#creational-design-patterns)
5. [Structural Design Patterns](#structural-design-patterns)
6. [Behavioral Design Patterns](#behavioral-design-patterns)
7. [Advanced Design Patterns](#advanced-design-patterns)
8. [Concurrency Patterns](#concurrency-patterns)
9. [Enterprise Patterns](#enterprise-patterns)
10. [Functional Patterns](#functional-patterns)
11. [Design Pattern Interview Questions](#design-pattern-interview-questions)
12. [Ứng dụng của Design Patterns](#ứng-dụng-của-design-patterns)
13. [Tại sao nên học Design Patterns](#tại-sao-nên-học-design-patterns)

---

## Giới thiệu Design Patterns

### Khái niệm cơ bản

Design Patterns cung cấp các giải pháp có thể tái sử dụng cho các vấn đề thiết kế phần mềm phổ biến. Chúng giúp các nhà phát triển viết code sạch hơn, dễ bảo trì và có thể mở rộng.

### Đặc điểm chính

- **Reusable Solutions**: Giải pháp đã được kiểm chứng cho các vấn đề thường gặp
- **Best Practices**: Tập hợp các thực hành tốt nhất trong ngành
- **Common Vocabulary**: Ngôn ngữ chung để giao tiếp giữa các developers
- **Proven Solutions**: Đã được test và sử dụng rộng rãi trong thực tế

### Lợi ích

- Giúp giải quyết các vấn đề thiết kế phần mềm phổ biến
- Cải thiện khả năng tái sử dụng, đọc hiểu và bảo trì code
- Cho phép loose coupling giữa các components trong ứng dụng lớn
- Đơn giản hóa việc tạo đối tượng, giao tiếp và cấu trúc
- Tăng cường khả năng mở rộng và hỗ trợ tăng trưởng hệ thống sạch
- Cung cấp từ vựng chung cho developers để thảo luận về kiến trúc
- Được sử dụng nhiều trong frameworks, libraries và các dự án enterprise-level
- Giảm bugs bằng cách tuân theo các best practices đã được kiểm chứng

---

## Phân loại Design Patterns

Design Patterns được phân loại thành 3 nhóm chính theo mục đích sử dụng:

### 1. Creational Patterns (Nhóm tạo đối tượng)
Tập trung vào cách tạo đối tượng một cách linh hoạt và hiệu quả. Giúp kiểm soát cách và thời điểm các đối tượng được khởi tạo.

### 2. Structural Patterns (Nhóm cấu trúc)
Giải thích cách các class và object được kết hợp để tạo thành cấu trúc lớn hơn. Cải thiện tính linh hoạt của code bằng cách đơn giản hóa mối quan hệ giữa các components.

### 3. Behavioral Patterns (Nhóm hành vi)
Định nghĩa cách các đối tượng giao tiếp và phân phối trách nhiệm. Giúp quản lý workflows, tương tác và ra quyết định trong hệ thống.

---

## Gang of Four (GoF) Overview

### Lịch sử

Gang of Four (GoF) là bốn tác giả: Erich Gamma, Richard Helm, Ralph Johnson, và John Vlissides, những người đã viết cuốn sách kinh điển "Design Patterns: Elements of Reusable Object-Oriented Software" (1994).

### 23 Design Patterns cơ bản

GoF đã định nghĩa 23 design patterns cơ bản, được chia thành 3 nhóm:

**Creational (5 patterns)**:
- Singleton
- Factory Method
- Abstract Factory
- Builder
- Prototype

**Structural (7 patterns)**:
- Adapter
- Decorator
- Facade
- Composite
- Proxy
- Bridge
- Flyweight

**Behavioral (11 patterns)**:
- Observer
- Strategy
- Command
- Chain of Responsibility
- Template Method
- Iterator
- State
- Mediator
- Memento
- Visitor
- Interpreter

### Tầm quan trọng

- Nền tảng cho việc học và áp dụng design patterns
- Được sử dụng rộng rãi trong các framework và thư viện
- Cung cấp ngôn ngữ chung cho cộng đồng developers

---

## Creational Design Patterns

Các Creational Design Patterns xử lý việc tạo đối tượng một cách linh hoạt và hiệu quả. Chúng giúp bạn kiểm soát cách và thời điểm các đối tượng được khởi tạo.

### 1. Singleton Pattern
**Mục đích**: Đảm bảo một class chỉ có một instance duy nhất và cung cấp điểm truy cập toàn cục đến instance đó.

**Nội dung cần cover**:
- Khái niệm và lý thuyết
- Các cách implement (Eager, Lazy, Thread-safe, Enum)
- Khi nào nên dùng và không nên dùng
- Use cases thực tế (Logger, Configuration, Database Connection)
- So sánh với các pattern khác
- Ưu điểm và nhược điểm
- Các sai lầm phổ biến (anti-patterns)
- Performance considerations
- Alternatives (Dependency Injection)

### 2. Factory Method Pattern
**Mục đích**: Tạo đối tượng mà không cần chỉ định class cụ thể. Ủy thác việc khởi tạo cho các subclass.

**Nội dung cần cover**:
- Khái niệm và lý thuyết
- Cơ chế hoạt động (Product, Creator, Concrete Products/Creators)
- So sánh Simple Factory vs Factory Method
- Khi nào nên dùng
- Use cases (Document creation, UI components, Database connections)
- So sánh với Abstract Factory và Builder
- Ưu điểm và nhược điểm
- Các sai lầm phổ biến
- Best practices

### 3. Abstract Factory Pattern
**Mục đích**: Cung cấp interface để tạo families of related objects mà không chỉ định concrete classes.

**Nội dung cần cover**:
- Khái niệm và lý thuyết
- Cơ chế hoạt động (Abstract Factory, Concrete Factories, Products)
- So sánh với Factory Method
- Khi nào nên dùng
- Use cases (UI frameworks, Cross-platform applications)
- Ưu điểm và nhược điểm
- Complexity và maintenance considerations
- Best practices

### 4. Builder Pattern
**Mục đích**: Xây dựng các đối tượng phức tạp từng bước. Cho phép tạo các đối tượng khác nhau bằng cùng một construction code.

**Nội dung cần cover**:
- Khái niệm và lý thuyết
- Cơ chế hoạt động (Builder interface, Concrete Builders, Director, Product)
- Khi nào nên dùng
- Use cases (SQL Query Builder, HTTP Request Builder, Configuration Builder)
- So sánh với Factory và Constructor
- Ưu điểm và nhược điểm
- Fluent interface và method chaining
- Immutable objects với Builder
- Best practices

### 5. Prototype Pattern
**Mục đích**: Sao chép các đối tượng hiện có thay vì tạo mới từ đầu, đặc biệt hữu ích khi việc tạo đối tượng tốn kém.

**Nội dung cần cover**:
- Khái niệm và lý thuyết
- Cơ chế hoạt động (Prototype interface, Concrete Prototypes, Clone method)
- Shallow copy vs Deep copy
- Khi nào nên dùng
- Use cases (Object cloning, Configuration objects, Game development)
- So sánh với Factory và Builder
- Ưu điểm và nhược điểm
- Implementation trong Java (Cloneable interface)
- Best practices và pitfalls

### 6. Object Pool Pattern
**Mục đích**: Tái sử dụng các đối tượng đắt tiền thay vì tạo và hủy chúng liên tục.

**Nội dung cần cover**:
- Khái niệm và lý thuyết
- Cơ chế hoạt động (Pool, Reusable objects, Client)
- Khi nào nên dùng
- Use cases (Database connections, Thread pools, Memory pools)
- So sánh với Singleton và Factory
- Ưu điểm và nhược điểm
- Pool management strategies
- Performance considerations
- Best practices

### 7. Lazy Initialization Pattern
**Mục đích**: Trì hoãn việc tạo đối tượng, tính toán giá trị, hoặc thực hiện các thao tác tốn kém cho đến khi lần đầu tiên cần thiết.

**Nội dung cần cover**:
- Khái niệm và lý thuyết
- Cơ chế hoạt động
- Khi nào nên dùng
- Use cases (Lazy loading, On-demand initialization)
- So sánh với Eager initialization
- Ưu điểm và nhược điểm
- Thread-safety considerations
- Best practices

---

## Structural Design Patterns

Structural patterns giải thích cách các class và object được kết hợp để tạo thành cấu trúc lớn hơn. Chúng cải thiện tính linh hoạt của code bằng cách đơn giản hóa mối quan hệ giữa các components.

### 1. Adapter Pattern
**Mục đích**: Cho phép các interface không tương thích làm việc cùng nhau. Chuyển đổi interface của một class thành interface mà client mong đợi.

**Nội dung cần cover**:
- Khái niệm và lý thuyết
- Cơ chế hoạt động (Target, Adapter, Adaptee, Client)
- Class Adapter vs Object Adapter
- Khi nào nên dùng
- Use cases (Legacy code integration, Third-party libraries, API wrappers)
- So sánh với Bridge, Decorator, Facade
- Ưu điểm và nhược điểm
- Best practices

### 2. Decorator Pattern
**Mục đích**: Thêm hành vi mới cho đối tượng một cách động mà không thay đổi cấu trúc của chúng. Một alternative linh hoạt hơn so với subclassing.

**Nội dung cần cover**:
- Khái niệm và lý thuyết
- Cơ chế hoạt động (Component, Concrete Component, Decorator, Concrete Decorators)
- Khi nào nên dùng
- Use cases (Java I/O streams, UI components, Middleware)
- So sánh với Adapter, Composite, Strategy
- Ưu điểm và nhược điểm
- Multiple decorators và chaining
- Best practices

### 3. Facade Pattern
**Mục đích**: Cung cấp một interface đơn giản, thống nhất cho một tập hợp các interface phức tạp trong subsystem. Giảm độ phức tạp.

**Nội dung cần cover**:
- Khái niệm và lý thuyết
- Cơ chế hoạt động (Facade, Subsystems, Client)
- Khi nào nên dùng
- Use cases (API simplification, Framework interfaces, Service layers)
- So sánh với Adapter, Mediator, Abstract Factory
- Ưu điểm và nhược điểm
- Best practices

### 4. Composite Pattern
**Mục đích**: Tổ chức các đối tượng thành cấu trúc cây để đại diện cho part-whole hierarchies. Cho phép client xử lý các đối tượng đơn lẻ và compositions một cách thống nhất.

**Nội dung cần cover**:
- Khái niệm và lý thuyết
- Cơ chế hoạt động (Component, Leaf, Composite, Client)
- Khi nào nên dùng
- Use cases (File systems, UI components, Organization structures)
- So sánh với Decorator, Chain of Responsibility
- Ưu điểm và nhược điểm
- Tree traversal và operations
- Best practices

### 5. Proxy Pattern
**Mục đích**: Cung cấp placeholder hoặc đại diện cho đối tượng khác để kiểm soát truy cập đến nó.

**Nội dung cần cover**:
- Khái niệm và lý thuyết
- Cơ chế hoạt động (Subject, Real Subject, Proxy, Client)
- Các loại Proxy (Virtual, Remote, Protection, Smart Reference)
- Khi nào nên dùng
- Use cases (Lazy loading, Access control, Remote objects, Caching)
- So sánh với Decorator, Adapter, Facade
- Ưu điểm và nhược điểm
- Dynamic proxies trong Java
- Best practices

### 6. Bridge Pattern
**Mục đích**: Tách abstraction khỏi implementation để chúng có thể thay đổi độc lập. Sử dụng composition thay vì inheritance.

**Nội dung cần cover**:
- Khái niệm và lý thuyết
- Cơ chế hoạt động (Abstraction, Refined Abstraction, Implementor, Concrete Implementor)
- Khi nào nên dùng
- Use cases (Device drivers, UI frameworks, Database drivers)
- So sánh với Adapter, Strategy, State
- Ưu điểm và nhược điểm
- Decoupling abstraction và implementation
- Best practices

### 7. Flyweight Pattern
**Mục đích**: Giảm bộ nhớ bằng cách chia sẻ dữ liệu giữa nhiều đối tượng tương tự. Chỉ lưu trữ intrinsic state, extrinsic state được truyền vào.

**Nội dung cần cover**:
- Khái niệm và lý thuyết
- Cơ chế hoạt động (Flyweight, Concrete Flyweight, Flyweight Factory, Client)
- Intrinsic vs Extrinsic state
- Khi nào nên dùng
- Use cases (Text editors, Game development, Caching)
- So sánh với Singleton, Object Pool
- Ưu điểm và nhược điểm
- Memory optimization
- Best practices

---

## Behavioral Design Patterns

Behavioral patterns định nghĩa cách các đối tượng giao tiếp và phân phối trách nhiệm. Chúng giúp quản lý workflows, tương tác và ra quyết định trong hệ thống.

### 1. Observer Pattern
**Mục đích**: Định nghĩa dependency một-nhiều giữa các đối tượng. Khi một đối tượng thay đổi trạng thái, tất cả dependents được thông báo và cập nhật tự động.

**Nội dung cần cover**:
- Khái niệm và lý thuyết
- Cơ chế hoạt động (Subject, Observer, Concrete Subject, Concrete Observer)
- Push vs Pull model
- Khi nào nên dùng
- Use cases (Event handling, MVC architecture, Model updates)
- So sánh với Mediator, Chain of Responsibility
- Ưu điểm và nhược điểm
- Java Observable và Observer (deprecated)
- Modern implementations (Java 9+)
- Best practices

### 2. Strategy Pattern
**Mục đích**: Định nghĩa một họ các thuật toán, đóng gói từng thuật toán và làm cho chúng có thể thay thế lẫn nhau. Strategy cho phép algorithm thay đổi độc lập với clients sử dụng nó.

**Nội dung cần cover**:
- Khái niệm và lý thuyết
- Cơ chế hoạt động (Strategy, Concrete Strategies, Context)
- Khi nào nên dùng
- Use cases (Sorting algorithms, Payment methods, Compression algorithms)
- So sánh với State, Template Method, Command
- Ưu điểm và nhược điểm
- Strategy với Lambda expressions (Java 8+)
- Best practices

### 3. Command Pattern
**Mục đích**: Đóng gói một request như một đối tượng, cho phép parameterize clients với các request khác nhau, queue requests, và hỗ trợ undo operations.

**Nội dung cần cover**:
- Khái niệm và lý thuyết
- Cơ chế hoạt động (Command, Concrete Command, Invoker, Receiver, Client)
- Khi nào nên dùng
- Use cases (GUI buttons, Macro recording, Undo/Redo, Transaction logging)
- So sánh với Strategy, Chain of Responsibility
- Ưu điểm và nhược điểm
- Undo/Redo implementation
- Command queue và logging
- Best practices

### 4. Chain of Responsibility Pattern
**Mục đích**: Tránh coupling giữa sender của request và receiver bằng cách cho phép nhiều đối tượng có cơ hội xử lý request. Chain các receiving objects và truyền request dọc theo chain.

**Nội dung cần cover**:
- Khái niệm và lý thuyết
- Cơ chế hoạt động (Handler, Concrete Handlers, Client)
- Khi nào nên dùng
- Use cases (Exception handling, Event processing, Middleware, Authentication)
- So sánh với Decorator, Command, Composite
- Ưu điểm và nhược điểm
- Chain termination và default handlers
- Best practices

### 5. Template Method Pattern
**Mục đích**: Định nghĩa skeleton của thuật toán trong một method, deferring một số steps đến các subclass. Template Method cho phép subclass redefine một số steps của algorithm mà không thay đổi cấu trúc của algorithm.

**Nội dung cần cover**:
- Khái niệm và lý thuyết
- Cơ chế hoạt động (Abstract Class, Concrete Classes, Template Method, Hook Methods)
- Khi nào nên dùng
- Use cases (Framework design, Algorithm variations, Data processing pipelines)
- So sánh với Strategy, Factory Method
- Ưu điểm và nhược điểm
- Hook methods và control flow
- Best practices

### 6. Iterator Pattern
**Mục đích**: Cung cấp cách truy cập tuần tự các phần tử của một aggregate object mà không expose representation bên trong của nó.

**Nội dung cần cover**:
- Khái niệm và lý thuyết
- Cơ chế hoạt động (Iterator, Concrete Iterator, Aggregate, Concrete Aggregate)
- Khi nào nên dùng
- Use cases (Collections, Tree traversal, Database result sets)
- So sánh với Visitor, Composite
- Ưu điểm và nhược điểm
- Java Iterator interface
- Internal vs External iterators
- Best practices

### 7. State Pattern
**Mục đích**: Cho phép một đối tượng thay đổi hành vi khi internal state của nó thay đổi. Object sẽ xuất hiện như đã thay đổi class của nó.

**Nội dung cần cover**:
- Khái niệm và lý thuyết
- Cơ chế hoạt động (Context, State, Concrete States)
- Khi nào nên dùng
- Use cases (State machines, Game development, Workflow engines)
- So sánh với Strategy, Command
- Ưu điểm và nhược điểm
- State transitions và management
- Best practices

### 8. Mediator Pattern
**Mục đích**: Định nghĩa cách một tập hợp các đối tượng tương tác. Mediator thúc đẩy loose coupling bằng cách ngăn các đối tượng tham chiếu đến nhau một cách rõ ràng.

**Nội dung cần cover**:
- Khái niệm và lý thuyết
- Cơ chế hoạt động (Mediator, Concrete Mediator, Colleague, Concrete Colleagues)
- Khi nào nên dùng
- Use cases (GUI components, Chat applications, Air traffic control)
- So sánh với Observer, Facade, Command
- Ưu điểm và nhược điểm
- Centralized communication
- Best practices

### 9. Memento Pattern
**Mục đích**: Không vi phạm encapsulation, capture và externalize internal state của một đối tượng để đối tượng có thể được restore về state này sau đó.

**Nội dung cần cover**:
- Khái niệm và lý thuyết
- Cơ chế hoạt động (Originator, Memento, Caretaker)
- Khi nào nên dùng
- Use cases (Undo/Redo, Checkpointing, Snapshot functionality)
- So sánh với Command, State
- Ưu điểm và nhược điểm
- Memento storage và management
- Best practices

### 10. Visitor Pattern
**Mục đích**: Đại diện cho một operation được thực hiện trên các phần tử của một object structure. Visitor cho phép định nghĩa một operation mới mà không thay đổi các class của các phần tử mà nó hoạt động.

**Nội dung cần cover**:
- Khái niệm và lý thuyết
- Cơ chế hoạt động (Visitor, Concrete Visitors, Element, Concrete Elements, Object Structure)
- Khi nào nên dùng
- Use cases (Compiler design, AST traversal, Document processing)
- So sánh với Iterator, Composite, Strategy
- Ưu điểm và nhược điểm
- Double dispatch
- Best practices

### 11. Interpreter Pattern
**Mục đích**: Định nghĩa representation cho grammar của một ngôn ngữ và một interpreter sử dụng representation này để interpret sentences trong ngôn ngữ.

**Nội dung cần cover**:
- Khái niệm và lý thuyết
- Cơ chế hoạt động (Abstract Expression, Terminal Expression, Non-terminal Expression, Context)
- Khi nào nên dùng
- Use cases (Query languages, Regular expressions, Rule engines)
- So sánh với Composite, Visitor
- Ưu điểm và nhược điểm
- Grammar definition và parsing
- Best practices

---

## Advanced Design Patterns

Advanced topics bao gồm các nguyên tắc kiến trúc và khái niệm thiết kế hệ thống sâu hơn. Chúng giúp bạn xây dựng các hệ thống phần mềm cấp enterprise, có thể mở rộng và mạnh mẽ.

### 1. SOLID Principles
**Mục đích**: Năm nguyên tắc thiết kế hướng đối tượng giúp tạo ra code dễ bảo trì, mở rộng và test.

**Nội dung cần cover**:
- **S - Single Responsibility Principle**: Một class chỉ nên có một lý do để thay đổi
- **O - Open/Closed Principle**: Mở để mở rộng, đóng để sửa đổi
- **L - Liskov Substitution Principle**: Objects của superclass có thể được thay thế bằng objects của subclass
- **I - Interface Segregation Principle**: Clients không nên phụ thuộc vào interfaces mà họ không sử dụng
- **D - Dependency Inversion Principle**: Phụ thuộc vào abstractions, không phụ thuộc vào concretions
- Ví dụ vi phạm và cách sửa
- Mối quan hệ với Design Patterns
- Best practices

### 2. Dependency Injection Pattern
**Mục đích**: Một kỹ thuật của Inversion of Control (IoC) trong đó dependencies được cung cấp cho một đối tượng thay vì đối tượng tự tạo chúng.

**Nội dung cần cover**:
- Khái niệm và lý thuyết
- Inversion of Control (IoC) vs Dependency Injection
- Các loại DI (Constructor, Setter, Field, Interface)
- Khi nào nên dùng
- Use cases (Testing, Loose coupling, Framework integration)
- So sánh với Service Locator
- Ưu điểm và nhược điểm
- DI Containers (Spring, Guice)
- Best practices

### 3. Composition vs Inheritance
**Mục đích**: So sánh và hướng dẫn khi nào nên sử dụng composition thay vì inheritance.

**Nội dung cần cover**:
- Khái niệm Composition và Inheritance
- "Favor composition over inheritance"
- Khi nào dùng Inheritance
- Khi nào dùng Composition
- So sánh ưu nhược điểm
- Use cases cho mỗi approach
- Best practices
- Design Patterns sử dụng Composition

### 4. Event-Driven Architecture & Patterns
**Mục đích**: Kiến trúc dựa trên việc sản xuất, phát hiện, tiêu thụ và phản ứng với events.

**Nội dung cần cover**:
- Khái niệm Event-Driven Architecture (EDA)
- Components (Event Producers, Event Consumers, Event Channels, Event Processing)
- Khi nào nên dùng
- Use cases (Microservices, Real-time systems, IoT)
- So sánh với Request-Response
- Ưu điểm và nhược điểm
- Event patterns (Event Sourcing, CQRS, Pub/Sub)
- Best practices

### 5. CQRS Design Pattern
**Mục đích**: Command Query Responsibility Segregation - Tách biệt operations đọc và ghi vào các models khác nhau.

**Nội dung cần cover**:
- Khái niệm và lý thuyết
- Command vs Query separation
- Cơ chế hoạt động (Command Side, Query Side, Synchronization)
- Khi nào nên dùng
- Use cases (High-performance systems, Complex domains, Scalable applications)
- So sánh với Traditional CRUD
- Ưu điểm và nhược điểm
- Implementation strategies
- Best practices

### 6. Event Sourcing Patterns
**Mục đích**: Lưu trữ tất cả changes như một sequence of events thay vì chỉ lưu current state.

**Nội dung cần cover**:
- Khái niệm và lý thuyết
- Event Store và Event Stream
- Cơ chế hoạt động (Event Store, Event Handlers, Snapshots)
- Khi nào nên dùng
- Use cases (Audit trails, Time travel, Complex business logic)
- So sánh với Traditional persistence
- Ưu điểm và nhược điểm
- Snapshot và replay
- Best practices

### 7. CQRS vs Event Sourcing Patterns
**Mục đích**: So sánh và giải thích mối quan hệ giữa CQRS và Event Sourcing.

**Nội dung cần cover**:
- Sự khác biệt giữa CQRS và Event Sourcing
- Khi nào dùng CQRS alone
- Khi nào dùng Event Sourcing alone
- Khi nào kết hợp cả hai
- Use cases cho mỗi approach
- Trade-offs
- Best practices

### 8. Repository Pattern
**Mục đích**: Trừu tượng hóa việc truy cập dữ liệu, cung cấp interface đơn giản hơn cho data access layer.

**Nội dung cần cover**:
- Khái niệm và lý thuyết
- Cơ chế hoạt động (Repository interface, Concrete Repository, Domain entities)
- Khi nào nên dùng
- Use cases (Data access abstraction, Testing, Multiple data sources)
- So sánh với DAO, Active Record
- Ưu điểm và nhược điểm
- Generic Repository vs Specific Repository
- Best practices

### 9. MVC Design Pattern
**Mục đích**: Tách một ứng dụng thành Model, View, và Controller để có kiến trúc sạch. Cải thiện khả năng mở rộng, bảo trì và phát triển song song trong các hệ thống lớn.

**Nội dung cần cover**:
- Khái niệm và lý thuyết
- Components (Model, View, Controller)
- Flow và interactions
- Khi nào nên dùng
- Use cases (Web applications, Desktop applications, Mobile apps)
- So sánh với MVP, MVVM
- Ưu điểm và nhược điểm
- MVC variations
- Best practices

### 10. MVVM Design Pattern
**Mục đích**: Model-View-ViewModel - Tách logic presentation khỏi UI, đặc biệt hữu ích cho data binding.

**Nội dung cần cover**:
- Khái niệm và lý thuyết
- Components (Model, View, ViewModel)
- Data binding và commands
- Khi nào nên dùng
- Use cases (WPF, Android, Modern web frameworks)
- So sánh với MVC, MVP
- Ưu điểm và nhược điểm
- Best practices

### 11. Service Locator Pattern
**Mục đích**: Cung cấp một registry tập trung để tìm và cung cấp services.

**Nội dung cần cover**:
- Khái niệm và lý thuyết
- Cơ chế hoạt động (Service Locator, Service Registry, Client)
- Khi nào nên dùng
- Use cases (Legacy systems, Service discovery)
- So sánh với Dependency Injection
- Ưu điểm và nhược điểm
- Anti-pattern considerations
- Best practices

---

## Concurrency Patterns

Các pattern tập trung vào xử lý đa luồng và đồng bộ hóa trong môi trường concurrent.

### 1. Active Object Pattern
**Mục đích**: Tách method invocation khỏi execution để cho phép client và method execution chạy trong các threads khác nhau.

**Nội dung cần cover**:
- Khái niệm và lý thuyết
- Cơ chế hoạt động (Proxy, Method Request, Scheduler, Servant)
- Khi nào nên dùng
- Use cases (Asynchronous processing, Thread management)
- Ưu điểm và nhược điểm
- Best practices

### 2. Producer-Consumer Pattern
**Mục đích**: Xử lý bất đồng bộ giữa producer và consumer thông qua một shared buffer.

**Nội dung cần cover**:
- Khái niệm và lý thuyết
- Cơ chế hoạt động (Producer, Consumer, Buffer/Queue)
- Khi nào nên dùng
- Use cases (Task queues, Message processing, Data pipelines)
- So sánh với Observer
- Ưu điểm và nhược điểm
- Thread synchronization
- Best practices

### 3. Thread Pool Pattern
**Mục đích**: Quản lý một pool các worker threads để thực thi tasks, tránh overhead của việc tạo và hủy threads.

**Nội dung cần cover**:
- Khái niệm và lý thuyết
- Cơ chế hoạt động (Thread Pool, Worker Threads, Task Queue)
- Khi nào nên dùng
- Use cases (Web servers, Application servers, Parallel processing)
- So sánh với Object Pool
- Ưu điểm và nhược điểm
- Pool sizing và configuration
- Best practices

### 4. Read-Write Lock Pattern
**Mục đích**: Tối ưu hóa cho read-heavy workloads bằng cách cho phép multiple readers hoặc single writer.

**Nội dung cần cover**:
- Khái niệm và lý thuyết
- Cơ chế hoạt động (Read Lock, Write Lock, Lock Manager)
- Khi nào nên dùng
- Use cases (Caching, Database access, Configuration management)
- So sánh với Mutex, Semaphore
- Ưu điểm và nhược điểm
- Starvation và fairness
- Best practices

### 5. Double-Checked Locking Pattern
**Mục đích**: Lazy initialization thread-safe với reduced locking overhead.

**Nội dung cần cover**:
- Khái niệm và lý thuyết
- Cơ chế hoạt động (Double check, Synchronization)
- Khi nào nên dùng
- Use cases (Singleton initialization, Lazy loading)
- So sánh với Eager initialization
- Ưu điểm và nhược điểm
- Volatile keyword và memory model
- Pitfalls và best practices

---

## Enterprise Patterns

Các pattern tập trung vào các ứng dụng enterprise-level, microservices, và distributed systems.

### 1. Event Sourcing
**Mục đích**: Lưu trữ tất cả changes như một sequence of events thay vì chỉ lưu current state.

**Nội dung cần cover**:
- Khái niệm và lý thuyết (đã có trong Advanced)
- Enterprise-specific considerations
- Distributed event sourcing
- Event versioning và migration
- Best practices

### 2. CQRS
**Mục đích**: Command Query Responsibility Segregation cho enterprise applications.

**Nội dung cần cover**:
- Khái niệm và lý thuyết (đã có trong Advanced)
- Enterprise-specific considerations
- Distributed CQRS
- Consistency models
- Best practices

### 3. DTO (Data Transfer Object)
**Mục đích**: Object được sử dụng để đóng gói data và gửi nó từ một process hoặc network đến một process khác.

**Nội dung cần cover**:
- Khái niệm và lý thuyết
- Khi nào nên dùng
- Use cases (API responses, Service communication, Remote calls)
- So sánh với Value Objects, Entities
- Ưu điểm và nhược điểm
- Best practices

### 4. Value Object
**Mục đích**: Immutable objects với value semantics, được xác định hoàn toàn bởi giá trị của chúng.

**Nội dung cần cover**:
- Khái niệm và lý thuyết
- Value semantics vs Reference semantics
- Immutability
- Khi nào nên dùng
- Use cases (Money, Date, Address, Domain modeling)
- So sánh với Entities, DTOs
- Ưu điểm và nhược điểm
- Best practices

### 5. Service Mesh
**Mục đích**: Infrastructure layer cho microservices để xử lý service-to-service communication.

**Nội dung cần cover**:
- Khái niệm và lý thuyết
- Components (Sidecar, Control plane, Data plane)
- Khi nào nên dùng
- Use cases (Microservices, Service discovery, Load balancing)
- So sánh với API Gateway
- Ưu điểm và nhược điểm
- Best practices

---

## Functional Patterns

Các pattern tập trung vào functional programming paradigms và xử lý dữ liệu.

### 1. Map-Reduce Pattern
**Mục đích**: Xử lý song song và phân tán các tập dữ liệu lớn bằng cách chia nhỏ và kết hợp kết quả.

**Nội dung cần cover**:
- Khái niệm và lý thuyết
- Cơ chế hoạt động (Map phase, Reduce phase, Shuffle)
- Khi nào nên dùng
- Use cases (Big data processing, Distributed computing, Batch processing)
- So sánh với Pipeline
- Ưu điểm và nhược điểm
- Best practices

### 2. Pipeline Pattern
**Mục đích**: Xử lý dữ liệu qua một chuỗi các stages, output của stage này là input của stage tiếp theo.

**Nội dung cần cover**:
- Khái niệm và lý thuyết
- Cơ chế hoạt động (Pipeline, Stages, Data flow)
- Khi nào nên dùng
- Use cases (Data processing, ETL, Stream processing)
- So sánh với Chain of Responsibility, Map-Reduce
- Ưu điểm và nhược điểm
- Parallel pipelines
- Best practices

### 3. Memoization Pattern
**Mục đích**: Cache kết quả của function calls để tránh tính toán lại cho cùng input.

**Nội dung cần cover**:
- Khái niệm và lý thuyết
- Cơ chế hoạt động (Cache, Function wrapper)
- Khi nào nên dùng
- Use cases (Recursive functions, Expensive computations, Dynamic programming)
- So sánh với Caching
- Ưu điểm và nhược điểm
- Memory considerations
- Best practices

---

## Design Pattern Interview Questions

Phần này chuẩn bị cho các câu hỏi phỏng vấn phổ biến về design patterns. Nó củng cố sự rõ ràng về khái niệm và giúp bạn giải thích patterns một cách tự tin.

### Nội dung cần cover:

1. **Câu hỏi cơ bản về Design Patterns**
   - Design Pattern là gì?
   - Tại sao sử dụng Design Patterns?
   - Phân loại Design Patterns
   - Sự khác biệt giữa Design Pattern và Framework

2. **Câu hỏi về Creational Patterns**
   - Singleton: Các cách implement, Thread-safety
   - Factory vs Abstract Factory
   - Builder vs Constructor
   - Prototype: Shallow vs Deep copy
   - Khi nào dùng pattern nào?

3. **Câu hỏi về Structural Patterns**
   - Adapter vs Decorator vs Facade
   - Proxy vs Decorator
   - Composite: Khi nào dùng?
   - Bridge: Tách abstraction khỏi implementation

4. **Câu hỏi về Behavioral Patterns**
   - Observer vs Pub/Sub
   - Strategy vs State
   - Command: Undo/Redo implementation
   - Chain of Responsibility: Use cases
   - Template Method vs Strategy

5. **Câu hỏi về SOLID Principles**
   - Giải thích từng nguyên tắc
   - Ví dụ vi phạm và cách sửa
   - Mối quan hệ với Design Patterns

6. **Câu hỏi thực tế**
   - Design một hệ thống sử dụng patterns
   - Refactor code sử dụng patterns
   - So sánh các patterns cho use case cụ thể

7. **Câu hỏi nâng cao**
   - Anti-patterns
   - Performance considerations
   - Testing với Design Patterns

---

## Ứng dụng của Design Patterns

### Lợi ích chính

1. **Giải quyết vấn đề thiết kế phổ biến**
   - Cung cấp giải pháp đã được kiểm chứng cho các vấn đề thường gặp
   - Tránh phải "reinvent the wheel"

2. **Cải thiện code quality**
   - **Reusability**: Code có thể tái sử dụng
   - **Readability**: Code dễ đọc và hiểu
   - **Maintainability**: Dễ bảo trì và mở rộng

3. **Loose coupling**
   - Giảm sự phụ thuộc giữa các components
   - Dễ dàng thay đổi và test

4. **Đơn giản hóa**
   - **Object creation**: Đơn giản hóa việc tạo đối tượng
   - **Communication**: Đơn giản hóa giao tiếp giữa objects
   - **Structure**: Đơn giản hóa cấu trúc code

5. **Tăng cường khả năng mở rộng**
   - Hỗ trợ tăng trưởng hệ thống sạch
   - Dễ dàng thêm features mới

6. **Ngôn ngữ chung**
   - Cung cấp từ vựng chung cho developers
   - Dễ dàng thảo luận về kiến trúc

7. **Sử dụng trong thực tế**
   - Được sử dụng nhiều trong frameworks
   - Phổ biến trong libraries
   - Essential cho enterprise-level projects

8. **Giảm bugs**
   - Tuân theo best practices đã được kiểm chứng
   - Tránh các lỗi phổ biến

---

## Tại sao nên học Design Patterns

### Lý do chính

1. **Code chất lượng cao hơn**
   - Code dễ hiểu, cập nhật và mở rộng hơn
   - Tuân theo best practices

2. **Giải pháp đã được kiểm chứng**
   - Cung cấp solutions đã được test kỹ lưỡng
   - Tránh các pitfalls phổ biến

3. **Hiệu quả trong công việc**
   - Giúp giải quyết các thách thức tương tự nhanh chóng và hiệu quả
   - Áp dụng trong nhiều projects khác nhau

4. **Tái sử dụng components**
   - Tạo ra các components có thể tái sử dụng
   - Sử dụng trong nhiều applications khác nhau
   - Giảm redundancy và tiết kiệm thời gian phát triển

5. **Career advancement**
   - Essential skill cho senior developers
   - Được hỏi nhiều trong technical interviews
   - Cần thiết cho system design

6. **Understanding frameworks**
   - Hiểu cách frameworks hoạt động
   - Sử dụng frameworks hiệu quả hơn
   - Contribute vào open-source projects

7. **Problem-solving mindset**
   - Phát triển tư duy giải quyết vấn đề
   - Nhận diện patterns trong code hiện có
   - Refactor code tốt hơn

---

## 📚 Tài liệu tham khảo

- **Gang of Four (GoF)**: "Design Patterns: Elements of Reusable Object-Oriented Software" (1994)
- **Effective Java** by Joshua Bloch
- **Clean Code** by Robert C. Martin
- **Head First Design Patterns** by Eric Freeman & Elisabeth Robson
- **Refactoring Guru**: https://refactoring.guru/design-patterns
- **Java Design Patterns**: Best Practices và Community Resources

---

## 🎯 Hướng dẫn sử dụng tài liệu

Tài liệu này được tổ chức theo cấu trúc từ tổng quan đến chi tiết:

1. **Bắt đầu từ phần Giới thiệu** để hiểu khái niệm cơ bản
2. **Nghiên cứu từng nhóm Patterns** theo thứ tự: Creational → Structural → Behavioral
3. **Nâng cao** với Advanced Patterns và Enterprise Patterns
4. **Thực hành** với các ví dụ và use cases
5. **Chuẩn bị** cho interviews với phần Interview Questions

Mỗi pattern sẽ được phát triển chi tiết trong các tài liệu riêng biệt sau này, bao gồm:
- Khái niệm và lý thuyết chi tiết
- Cơ chế hoạt động
- Ví dụ code từ đơn giản đến phức tạp
- Use cases thực tế
- So sánh với các pattern khác
- Ưu điểm và nhược điểm
- Các sai lầm phổ biến
- Best practices

---

**Lưu ý**: Đây là tài liệu tổng quan. Các phần chi tiết về từng pattern sẽ được phát triển trong các tài liệu riêng biệt.
