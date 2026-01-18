# Design Patterns trong Java - Tài liệu Tổng quan

Tài liệu toàn diện về các Design Patterns trong Java, bao gồm lý thuyết, khái niệm, và hướng dẫn áp dụng.

## Mục lục

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

Design Patterns là các giải pháp có thể tái sử dụng cho các vấn đề thiết kế phần mềm phổ biến. Chúng không phải là code cụ thể mà là các template hoặc mô tả cách giải quyết một vấn đề có thể áp dụng trong nhiều tình huống khác nhau.

Tại sao cần Design Patterns? Khi phát triển phần mềm, các developers thường gặp phải các vấn đề tương tự nhau. Thay vì phát minh lại giải pháp mỗi lần, Design Patterns cung cấp các giải pháp đã được kiểm chứng, giúp tiết kiệm thời gian và đảm bảo chất lượng code.

Design Patterns giúp các nhà phát triển viết code sạch hơn, dễ bảo trì và có thể mở rộng bằng cách:
- Cung cấp cấu trúc rõ ràng cho việc giải quyết vấn đề
- Tăng tính linh hoạt và khả năng tái sử dụng của code
- Giảm sự phụ thuộc giữa các thành phần
- Cải thiện khả năng giao tiếp giữa các developers

### Đặc điểm chính

**Reusable Solutions (Giải pháp tái sử dụng)**: Design Patterns cung cấp các giải pháp đã được kiểm chứng cho các vấn đề thường gặp. Thay vì phải suy nghĩ lại từ đầu, developers có thể áp dụng pattern phù hợp. Ví dụ, khi cần đảm bảo chỉ có một instance của một class, Singleton Pattern đã cung cấp giải pháp sẵn có.

**Best Practices (Thực hành tốt nhất)**: Các pattern được phát triển dựa trên kinh nghiệm của nhiều developers và đã được sử dụng thành công trong nhiều dự án. Chúng đại diện cho các cách tiếp cận tốt nhất đã được chứng minh trong thực tế.

**Common Vocabulary (Từ vựng chung)**: Design Patterns cung cấp ngôn ngữ chung để giao tiếp giữa các developers. Khi một developer nói "sử dụng Factory Pattern", các developer khác ngay lập tức hiểu ý định và cách triển khai. Điều này giúp giảm thời gian giải thích và tăng hiệu quả làm việc nhóm.

**Proven Solutions (Giải pháp đã được chứng minh)**: Các pattern đã được test và sử dụng rộng rãi trong thực tế. Chúng không phải là lý thuyết suông mà là các giải pháp đã được áp dụng thành công trong nhiều hệ thống thực tế, từ các ứng dụng nhỏ đến các hệ thống enterprise lớn.

### Lợi ích chi tiết

**Giải quyết vấn đề thiết kế phổ biến**: Trong quá trình phát triển phần mềm, developers thường gặp các vấn đề tương tự như: làm thế nào để tạo đối tượng một cách linh hoạt, làm thế nào để giảm sự phụ thuộc giữa các components, làm thế nào để quản lý trạng thái của đối tượng. Design Patterns cung cấp giải pháp cho những vấn đề này.

**Cải thiện khả năng tái sử dụng, đọc hiểu và bảo trì code**: Code sử dụng Design Patterns thường dễ đọc hơn vì nó tuân theo các cấu trúc quen thuộc. Khi một developer mới tham gia dự án, họ có thể nhanh chóng hiểu code nếu biết các pattern được sử dụng. Điều này cũng làm cho code dễ bảo trì hơn vì các thay đổi có thể được thực hiện theo cấu trúc pattern đã định.

**Loose coupling giữa các components**: Loose coupling có nghĩa là các components ít phụ thuộc vào nhau. Điều này quan trọng vì nó cho phép thay đổi một component mà không ảnh hưởng đến các component khác. Nhiều Design Patterns, như Dependency Injection và Observer, giúp đạt được loose coupling.

**Đơn giản hóa việc tạo đối tượng, giao tiếp và cấu trúc**: Creational Patterns đơn giản hóa việc tạo đối tượng bằng cách ẩn logic phức tạp. Structural Patterns giúp tổ chức code một cách rõ ràng. Behavioral Patterns đơn giản hóa cách các đối tượng giao tiếp với nhau.

**Tăng cường khả năng mở rộng**: Code được thiết kế tốt với Design Patterns dễ dàng mở rộng. Ví dụ, Strategy Pattern cho phép thêm thuật toán mới mà không cần sửa code hiện có. Điều này tuân theo nguyên tắc Open/Closed Principle.

**Từ vựng chung cho developers**: Khi developers sử dụng cùng một ngôn ngữ về Design Patterns, họ có thể giao tiếp hiệu quả hơn. Thay vì giải thích dài dòng về cách một hệ thống hoạt động, họ có thể nói "hệ thống sử dụng Observer Pattern" và mọi người đều hiểu.

**Sử dụng trong frameworks và libraries**: Hầu hết các framework và library phổ biến đều sử dụng Design Patterns. Hiểu Design Patterns giúp developers hiểu cách các framework hoạt động và sử dụng chúng hiệu quả hơn. Ví dụ, Spring Framework sử dụng Dependency Injection, Factory Pattern, và nhiều pattern khác.

**Giảm bugs**: Design Patterns đã được test kỹ lưỡng và sử dụng rộng rãi, nên chúng ít có lỗi hơn so với các giải pháp tự phát minh. Tuân theo các best practices đã được kiểm chứng giúp tránh các lỗi phổ biến.

---

## Phân loại Design Patterns

Design Patterns được phân loại thành 3 nhóm chính theo mục đích sử dụng. Việc phân loại này giúp developers dễ dàng tìm và hiểu các pattern phù hợp với vấn đề họ đang gặp phải.

### 1. Creational Patterns (Nhóm tạo đối tượng)

Creational Patterns tập trung vào cách tạo đối tượng một cách linh hoạt và hiệu quả. Chúng giúp kiểm soát cách và thời điểm các đối tượng được khởi tạo.

Tại sao cần Creational Patterns? Trong lập trình hướng đối tượng, việc tạo đối tượng bằng cách sử dụng toán tử `new` trực tiếp có thể dẫn đến các vấn đề:
- Code phụ thuộc vào class cụ thể, khó thay đổi
- Logic tạo đối tượng phức tạp bị rải rác trong code
- Khó test vì không thể mock hoặc thay thế đối tượng
- Không thể kiểm soát số lượng instance được tạo

Creational Patterns giải quyết các vấn đề này bằng cách:
- Ẩn logic tạo đối tượng phức tạp
- Cho phép tạo đối tượng mà không cần chỉ định class cụ thể
- Cung cấp cách kiểm soát việc tạo và lifecycle của đối tượng
- Tăng tính linh hoạt và khả năng tái sử dụng

Các pattern trong nhóm này bao gồm: Singleton, Factory Method, Abstract Factory, Builder, Prototype, Object Pool, và Lazy Initialization.

### 2. Structural Patterns (Nhóm cấu trúc)

Structural Patterns giải thích cách các class và object được kết hợp để tạo thành cấu trúc lớn hơn. Chúng cải thiện tính linh hoạt của code bằng cách đơn giản hóa mối quan hệ giữa các components.

Tại sao cần Structural Patterns? Khi xây dựng hệ thống phức tạp, các vấn đề thường gặp:
- Các interface không tương thích cần làm việc cùng nhau
- Cần thêm chức năng mới cho đối tượng mà không thay đổi cấu trúc
- Cần đơn giản hóa interface phức tạp
- Cần tổ chức đối tượng theo cấu trúc cây
- Cần kiểm soát truy cập đến đối tượng

Structural Patterns giải quyết các vấn đề này bằng cách:
- Kết nối các interface không tương thích (Adapter)
- Thêm chức năng động cho đối tượng (Decorator)
- Đơn giản hóa interface phức tạp (Facade)
- Tổ chức đối tượng theo cấu trúc cây (Composite)
- Kiểm soát truy cập (Proxy)
- Tách abstraction khỏi implementation (Bridge)
- Tối ưu bộ nhớ bằng cách chia sẻ dữ liệu (Flyweight)

Các pattern trong nhóm này giúp xây dựng hệ thống linh hoạt, dễ mở rộng và bảo trì.

### 3. Behavioral Patterns (Nhóm hành vi)

Behavioral Patterns định nghĩa cách các đối tượng giao tiếp và phân phối trách nhiệm. Chúng giúp quản lý workflows, tương tác và ra quyết định trong hệ thống.

Tại sao cần Behavioral Patterns? Trong hệ thống phức tạp, các vấn đề về giao tiếp và phân phối trách nhiệm thường xuất hiện:
- Làm thế nào để các đối tượng thông báo thay đổi cho nhau?
- Làm thế nào để chọn thuật toán phù hợp tại runtime?
- Làm thế nào để đóng gói request và hỗ trợ undo/redo?
- Làm thế nào để xử lý request qua một chuỗi handlers?
- Làm thế nào để định nghĩa skeleton của thuật toán?

Behavioral Patterns giải quyết các vấn đề này bằng cách:
- Định nghĩa cách các đối tượng giao tiếp (Observer, Mediator)
- Đóng gói thuật toán và cho phép thay đổi (Strategy, Command)
- Quản lý trạng thái và hành vi (State, Memento)
- Xử lý request qua chuỗi (Chain of Responsibility)
- Định nghĩa skeleton thuật toán (Template Method)
- Truy cập phần tử (Iterator, Visitor)

Các pattern trong nhóm này giúp quản lý các tương tác phức tạp giữa các đối tượng một cách có tổ chức và dễ bảo trì.

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

Cuốn sách của GoF có tầm quan trọng đặc biệt vì:

**Nền tảng cho việc học và áp dụng design patterns**: Đây là cuốn sách đầu tiên hệ thống hóa và đặt tên cho các design patterns. Nó cung cấp nền tảng vững chắc cho việc hiểu và áp dụng patterns trong thực tế. Tất cả các tài liệu và khóa học về design patterns đều tham khảo từ cuốn sách này.

**Được sử dụng rộng rãi trong các framework và thư viện**: Các pattern được mô tả trong cuốn sách đã được áp dụng rộng rãi trong các framework và thư viện phổ biến. Ví dụ, Spring Framework sử dụng nhiều pattern như Dependency Injection (dựa trên Factory và Strategy), Proxy, Template Method. Java Collections Framework sử dụng Iterator Pattern. Hiểu các pattern này giúp developers hiểu cách các framework hoạt động.

**Cung cấp ngôn ngữ chung cho cộng đồng developers**: Trước khi có cuốn sách này, mỗi developer có thể giải quyết cùng một vấn đề theo cách khác nhau và gọi tên khác nhau. Cuốn sách đã tạo ra một ngôn ngữ chung, giúp developers có thể giao tiếp hiệu quả về các giải pháp thiết kế. Khi một developer nói "sử dụng Observer Pattern", tất cả developers khác đều hiểu ý định và cách triển khai.

**Ảnh hưởng đến cách suy nghĩ về thiết kế phần mềm**: Cuốn sách không chỉ cung cấp các pattern cụ thể mà còn dạy cách suy nghĩ về thiết kế phần mềm. Nó giúp developers nhận ra các pattern trong code hiện có và áp dụng chúng một cách có ý thức.

---

## Creational Design Patterns

Các Creational Design Patterns xử lý việc tạo đối tượng một cách linh hoạt và hiệu quả. Chúng giúp bạn kiểm soát cách và thời điểm các đối tượng được khởi tạo.

### 1. Singleton Pattern

**Mục đích**: Đảm bảo một class chỉ có một instance duy nhất và cung cấp điểm truy cập toàn cục đến instance đó.

**Khái niệm và lý thuyết**:

Singleton Pattern đảm bảo rằng một class chỉ có một instance duy nhất trong toàn bộ ứng dụng và cung cấp một cách toàn cục để truy cập instance đó. Pattern này hữu ích khi bạn cần kiểm soát việc truy cập đến một tài nguyên được chia sẻ, như database connection, logger, hoặc configuration object.

Tại sao cần Singleton? Trong một số trường hợp, việc có nhiều instance của một class có thể gây ra vấn đề:
- Tốn kém tài nguyên: Một số đối tượng tốn kém để tạo (như database connection)
- Xung đột: Nhiều instance có thể gây xung đột (như file system access)
- State management: Cần một instance duy nhất để quản lý state toàn cục

**Cơ chế hoạt động**:

Singleton Pattern hoạt động bằng cách:
1. Private constructor: Ngăn việc tạo instance từ bên ngoài bằng toán tử `new`
2. Static instance: Lưu trữ instance duy nhất như một biến static
3. Static factory method: Cung cấp method public static để truy cập instance

**Các cách implement**:

1. **Eager Initialization**: Instance được tạo ngay khi class được load vào memory. Ưu điểm là đơn giản và thread-safe tự nhiên. Nhược điểm là instance được tạo ngay cả khi không sử dụng, tốn memory.

2. **Lazy Initialization**: Instance chỉ được tạo khi lần đầu tiên được yêu cầu. Ưu điểm là tiết kiệm memory. Nhược điểm là cần xử lý thread-safety nếu sử dụng trong môi trường đa luồng.

3. **Thread-safe với synchronized**: Sử dụng synchronized để đảm bảo thread-safety. Nhược điểm là chậm hơn vì mỗi lần truy cập đều phải lock.

4. **Double-Checked Locking**: Kiểm tra null hai lần, chỉ lock khi cần thiết. Hiệu quả hơn nhưng phức tạp hơn và cần sử dụng `volatile` keyword.

5. **Enum Singleton**: Sử dụng enum trong Java. Đây là cách được khuyến nghị nhất vì thread-safe tự nhiên, serialization-safe, và reflection-safe.

**Khi nào nên dùng**:

- Khi cần đảm bảo chỉ có một instance (database connection, logger, cache)
- Khi instance cần được truy cập toàn cục
- Khi việc tạo instance tốn kém và cần được kiểm soát
- Khi cần quản lý state toàn cục (configuration, registry)

**Khi nào không nên dùng**:

- Khi cần test: Singleton khó test vì global state
- Khi cần dependency injection: Singleton vi phạm Dependency Inversion Principle
- Khi cần nhiều instance với cấu hình khác nhau
- Trong môi trường distributed: Singleton không work trong distributed systems

**Use cases thực tế**:

- **Logger**: Một ứng dụng chỉ cần một logger instance để ghi log
- **Configuration**: Một instance để quản lý cấu hình toàn cục
- **Database Connection**: Một connection pool manager
- **Cache**: Một cache manager toàn cục
- **Thread Pool**: Một thread pool manager

**So sánh với các pattern khác**:

- **vs Factory**: Factory tạo nhiều instances, Singleton chỉ một instance
- **vs Object Pool**: Object Pool quản lý pool các objects, Singleton chỉ một instance
- **vs Dependency Injection**: DI tốt hơn cho testability và flexibility

**Ưu điểm**:
- Đảm bảo chỉ có một instance
- Tiết kiệm memory
- Truy cập toàn cục dễ dàng
- Lazy initialization có thể tiết kiệm tài nguyên

**Nhược điểm**:
- Khó test vì global state
- Vi phạm Single Responsibility Principle
- Thread-safety phức tạp
- Hidden dependencies
- Khó mở rộng và kế thừa

**Các sai lầm phổ biến**:

1. **Không thread-safe**: Trong môi trường đa luồng, có thể tạo nhiều instances
2. **Synchronized method chậm**: Synchronized method chậm hơn double-checked locking
3. **Reflection attack**: Có thể tạo instance mới bằng reflection nếu không có protection
4. **Serialization attack**: Có thể tạo instance mới khi deserialize nếu không implement readResolve()

**Performance considerations**:

- Eager initialization: Nhanh khi truy cập nhưng tốn memory ngay từ đầu
- Lazy initialization: Tiết kiệm memory nhưng có overhead khi check null
- Double-checked locking: Tối ưu nhất cho performance
- Enum: Không có overhead, được JVM tối ưu

**Alternatives**:

- **Dependency Injection**: Sử dụng DI container (Spring, Guice) để quản lý lifecycle. Tốt hơn cho testability và flexibility.
- **Factory Pattern**: Sử dụng Factory để tạo và quản lý instances
- **Service Locator**: Sử dụng Service Locator pattern (ít được khuyến nghị)

### 2. Factory Method Pattern

**Mục đích**: Tạo đối tượng mà không cần chỉ định class cụ thể. Ủy thác việc khởi tạo cho các subclass.

**Khái niệm và lý thuyết**:

Factory Method Pattern định nghĩa một interface để tạo đối tượng, nhưng để các subclass quyết định class nào sẽ được instantiate. Pattern này cho phép một class defer việc khởi tạo đến các subclass.

Tại sao cần Factory Method? Khi sử dụng `new` trực tiếp, code phụ thuộc vào class cụ thể. Điều này vi phạm Dependency Inversion Principle và làm cho code khó thay đổi. Factory Method giải quyết vấn đề này bằng cách:
- Tách logic tạo đối tượng khỏi business logic
- Cho phép thay đổi class được tạo mà không cần sửa code client
- Tuân theo Open/Closed Principle: mở để mở rộng, đóng để sửa đổi

**Cơ chế hoạt động**:

Factory Method Pattern bao gồm các thành phần:
- **Product**: Interface hoặc abstract class định nghĩa đối tượng được tạo
- **Concrete Products**: Các implementation cụ thể của Product
- **Creator**: Abstract class hoặc interface với factory method
- **Concrete Creators**: Các subclass implement factory method để tạo Concrete Products

Cách hoạt động: Client sử dụng Creator, Creator sử dụng factory method để tạo Product. Mỗi Concrete Creator quyết định Product nào được tạo.

**So sánh Simple Factory vs Factory Method**:

- **Simple Factory**: Một factory class tạo tất cả products. Đơn giản nhưng vi phạm Open/Closed Principle khi thêm product mới.
- **Factory Method**: Mỗi product có factory method riêng trong creator. Phức tạp hơn nhưng tuân theo Open/Closed Principle.

**Khi nào nên dùng**:

- Khi không biết trước class cụ thể nào sẽ được tạo
- Khi muốn tách logic tạo đối tượng khỏi business logic
- Khi muốn cho phép subclass quyết định object nào được tạo
- Khi logic tạo đối tượng phức tạp

**Use cases**:

- **Document creation**: Tạo Word, PDF, Excel documents dựa trên type
- **UI components**: Tạo buttons, dialogs dựa trên platform (Windows, Mac, Linux)
- **Database connections**: Tạo MySQL, PostgreSQL connections dựa trên configuration
- **Game development**: Tạo enemies, weapons dựa trên level

**So sánh với các pattern khác**:

- **vs Abstract Factory**: Factory Method tạo một loại object, Abstract Factory tạo families of related objects
- **vs Builder**: Factory Method tập trung vào creation, Builder tập trung vào construction từng bước
- **vs Simple Factory**: Factory Method sử dụng inheritance, Simple Factory sử dụng composition

**Ưu điểm**:
- Loose coupling: Client không phụ thuộc vào concrete classes
- Single Responsibility: Tách creation logic
- Open/Closed Principle: Dễ thêm product mới
- Centralized creation logic

**Nhược điểm**:
- Tăng complexity: Thêm abstraction layer
- Có thể over-engineering cho simple cases
- Cần maintain factory khi thêm product mới

**Các sai lầm phổ biến**:

1. **God Factory**: Một factory làm quá nhiều việc, vi phạm Single Responsibility Principle
2. **Không validate input**: Không kiểm tra type hợp lệ trước khi tạo
3. **Hard-coded strings**: Sử dụng magic strings thay vì enum hoặc constants
4. **Tạo instance mỗi lần**: Không cache hoặc reuse instances khi có thể

**Best practices**:

- Sử dụng enum thay vì strings cho type safety
- Validate input và throw meaningful exceptions
- Document các types được support
- Factory methods nên return interfaces, không phải concrete classes
- Kết hợp với Dependency Injection frameworks khi có thể

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

**Khái niệm và lý thuyết**:

Observer Pattern là một trong những pattern được sử dụng nhiều nhất. Nó định nghĩa một dependency một-nhiều giữa objects, trong đó khi một object (subject) thay đổi trạng thái, tất cả các objects phụ thuộc (observers) được thông báo và cập nhật tự động.

Tại sao cần Observer Pattern? Trong nhiều tình huống, bạn cần một số objects phản ứng với thay đổi của một object khác:
- UI components cần cập nhật khi data model thay đổi
- Event handling trong GUI applications
- Model-View separation trong MVC architecture
- Publish-Subscribe systems

Observer Pattern giải quyết vấn đề này bằng cách tách subject và observers, cho phép thêm hoặc xóa observers mà không ảnh hưởng đến subject.

**Cơ chế hoạt động**:

Observer Pattern bao gồm:
- **Subject**: Object có state và quản lý danh sách observers. Cung cấp methods để attach, detach, và notify observers.
- **Observer**: Interface định nghĩa method update() được gọi khi subject thay đổi
- **Concrete Subject**: Implementation cụ thể của Subject, lưu trữ state và notify observers khi state thay đổi
- **Concrete Observer**: Implementation cụ thể của Observer, phản ứng với thay đổi của subject

Flow: Subject thay đổi state → gọi notifyObservers() → tất cả observers nhận được thông báo → mỗi observer cập nhật theo cách riêng.

**Push vs Pull model**:

- **Push model**: Subject gửi tất cả thông tin cần thiết cho observer trong method update(). Observer nhận thông tin và xử lý. Ưu điểm: Observer không cần query subject. Nhược điểm: Subject phải biết observer cần gì.
- **Pull model**: Subject chỉ thông báo rằng có thay đổi, observer tự query subject để lấy thông tin cần thiết. Ưu điểm: Subject không cần biết observer cần gì. Nhược điểm: Observer phải có reference đến subject.

**Khi nào nên dùng**:

- Khi một object thay đổi và nhiều objects khác cần được thông báo
- Khi muốn tách coupling giữa subject và observers
- Khi số lượng observers không biết trước hoặc thay đổi động
- Trong event-driven architectures

**Use cases**:

- **Event handling**: GUI frameworks (Swing, JavaFX) sử dụng Observer cho event handling
- **MVC architecture**: Model (subject) thay đổi, Views (observers) được thông báo để cập nhật
- **Model updates**: Khi business model thay đổi, UI components tự động cập nhật
- **Stock market**: Stock prices thay đổi, multiple displays cập nhật
- **Publish-Subscribe systems**: Message queues, event buses

**So sánh với các pattern khác**:

- **vs Mediator**: Observer là one-to-many, Mediator là many-to-many. Observer subject không biết observers, Mediator biết tất cả colleagues.
- **vs Chain of Responsibility**: Observer notify tất cả, Chain of Responsibility chỉ một handler xử lý.
- **vs Pub/Sub**: Observer là synchronous, Pub/Sub thường là asynchronous với message broker.

**Ưu điểm**:
- Loose coupling: Subject không biết observers cụ thể
- Dynamic relationships: Có thể thêm/xóa observers tại runtime
- Broadcast communication: Một thay đổi có thể notify nhiều observers
- Open/Closed Principle: Dễ thêm observer mới

**Nhược điểm**:
- Unexpected updates: Observers có thể nhận update không mong muốn
- Order of notifications: Khó đảm bảo thứ tự notifications
- Memory leaks: Nếu không detach observers đúng cách
- Performance: Nếu có quá nhiều observers

**Java Observable và Observer (deprecated)**:

Java cung cấp `java.util.Observable` và `java.util.Observer` nhưng đã bị deprecated từ Java 9 vì:
- Không thread-safe
- Không thể extend từ class khác (vì Observable là class, không phải interface)
- Không linh hoạt

**Modern implementations (Java 9+)**:

- **PropertyChangeListener**: Sử dụng PropertyChangeSupport cho JavaBeans
- **Reactive Streams**: Sử dụng Flow API (Publisher, Subscriber)
- **Custom implementation**: Implement Observer Pattern từ đầu với interfaces
- **Event Bus**: Sử dụng libraries như Guava EventBus, Spring Events

**Best practices**:

- Sử dụng interfaces thay vì concrete classes
- Implement thread-safety nếu cần
- Cung cấp cách unsubscribe để tránh memory leaks
- Xem xét sử dụng modern alternatives (Reactive Streams, Event Bus)
- Document order of notifications nếu quan trọng

### 2. Strategy Pattern

**Mục đích**: Định nghĩa một họ các thuật toán, đóng gói từng thuật toán và làm cho chúng có thể thay thế lẫn nhau. Strategy cho phép algorithm thay đổi độc lập với clients sử dụng nó.

**Khái niệm và lý thuyết**:

Strategy Pattern cho phép bạn định nghĩa một family các thuật toán, đóng gói mỗi thuật toán, và làm cho chúng có thể thay thế lẫn nhau. Strategy cho phép algorithm thay đổi độc lập với clients sử dụng nó.

Tại sao cần Strategy Pattern? Khi bạn có nhiều cách để thực hiện một task và muốn chọn cách nào tại runtime:
- Nhiều thuật toán sắp xếp (QuickSort, MergeSort, BubbleSort)
- Nhiều phương thức thanh toán (Credit Card, PayPal, Bank Transfer)
- Nhiều cách nén dữ liệu (ZIP, RAR, 7Z)

Thay vì sử dụng if-else hoặc switch-case (vi phạm Open/Closed Principle), Strategy Pattern cho phép:
- Tách mỗi thuật toán vào class riêng
- Cho phép thay đổi thuật toán tại runtime
- Tuân theo Open/Closed Principle: mở để thêm strategy mới, đóng để sửa code hiện có

**Cơ chế hoạt động**:

Strategy Pattern bao gồm:
- **Strategy**: Interface định nghĩa method thực thi thuật toán
- **Concrete Strategies**: Các implementation cụ thể của Strategy, mỗi cái implement một thuật toán
- **Context**: Class sử dụng Strategy, giữ reference đến Strategy object và gọi method của nó

Flow: Client tạo Context với một Concrete Strategy → Context sử dụng Strategy để thực thi task → Có thể thay đổi Strategy tại runtime.

**Khi nào nên dùng**:

- Khi có nhiều cách để thực hiện một task và muốn chọn tại runtime
- Khi muốn tránh if-else hoặc switch-case phức tạp cho việc chọn thuật toán
- Khi muốn tách logic thuật toán khỏi class sử dụng nó
- Khi các thuật toán có thể được thay thế lẫn nhau

**Use cases**:

- **Sorting algorithms**: Chọn QuickSort, MergeSort, hoặc BubbleSort
- **Payment methods**: Chọn Credit Card, PayPal, hoặc Bank Transfer
- **Compression algorithms**: Chọn ZIP, RAR, hoặc 7Z
- **Validation strategies**: Chọn different validation rules
- **Discount calculation**: Chọn percentage, fixed amount, hoặc buy-one-get-one

**So sánh với các pattern khác**:

- **vs State**: Strategy thay đổi behavior dựa trên algorithm được chọn, State thay đổi behavior dựa trên internal state. Strategy là external, State là internal.
- **vs Template Method**: Strategy sử dụng composition, Template Method sử dụng inheritance. Strategy cho phép thay đổi toàn bộ algorithm, Template Method chỉ thay đổi một số steps.
- **vs Command**: Strategy tập trung vào algorithm, Command tập trung vào request encapsulation.

**Ưu điểm**:
- Tách logic thuật toán khỏi context
- Dễ thêm strategy mới (Open/Closed Principle)
- Loại bỏ conditional statements phức tạp
- Có thể thay đổi strategy tại runtime
- Mỗi strategy có thể test độc lập

**Nhược điểm**:
- Tăng số lượng classes
- Client phải biết các strategies khác nhau
- Overhead của việc tạo strategy objects
- Có thể over-engineering cho simple cases

**Strategy với Lambda expressions (Java 8+)**:

Với Java 8+, Strategy Pattern có thể được implement đơn giản hơn bằng lambda expressions và functional interfaces:

```java
// Thay vì tạo class cho mỗi strategy
context.setStrategy(x -> x * 2); // Double strategy
context.setStrategy(x -> x + 10); // Add strategy
```

Điều này giảm boilerplate code nhưng chỉ phù hợp cho strategies đơn giản. Với strategies phức tạp, vẫn nên sử dụng classes.

**Best practices**:

- Sử dụng Strategy khi có nhiều algorithms có thể thay thế
- Đảm bảo tất cả strategies implement cùng interface
- Xem xét sử dụng lambda cho simple strategies (Java 8+)
- Document behavior của mỗi strategy
- Có thể kết hợp với Factory để tạo strategies

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

SOLID là viết tắt của năm nguyên tắc được đặt tên bởi Robert C. Martin (Uncle Bob). Các nguyên tắc này giúp developers viết code sạch, dễ bảo trì và mở rộng.

**S - Single Responsibility Principle (Nguyên tắc Trách nhiệm Đơn nhất)**:

Một class chỉ nên có một lý do để thay đổi. Nói cách khác, một class chỉ nên có một trách nhiệm duy nhất.

Tại sao quan trọng? Khi một class có nhiều trách nhiệm:
- Khó hiểu và maintain
- Thay đổi một trách nhiệm có thể ảnh hưởng đến trách nhiệm khác
- Khó test vì phải test nhiều behaviors
- Vi phạm cohesion (gắn kết)

Ví dụ vi phạm: Class `User` vừa quản lý user data, vừa gửi email, vừa validate. Nếu thay đổi cách gửi email, phải sửa class User.

Cách sửa: Tách thành `User` (quản lý data), `EmailService` (gửi email), `UserValidator` (validate).

**O - Open/Closed Principle (Nguyên tắc Mở/Đóng)**:

Software entities (classes, modules, functions) nên mở để mở rộng nhưng đóng để sửa đổi.

Tại sao quan trọng? Khi cần thêm tính năng mới:
- Không nên sửa code hiện có (có thể gây bugs)
- Nên mở rộng thông qua inheritance hoặc composition
- Giảm risk khi thay đổi code đã test

Ví dụ vi phạm: Class `AreaCalculator` có method tính diện tích với if-else cho từng hình. Thêm hình mới phải sửa method này.

Cách sửa: Sử dụng Strategy Pattern hoặc polymorphism. Tạo interface `Shape` với method `calculateArea()`, mỗi hình implement interface này.

**L - Liskov Substitution Principle (Nguyên tắc Thay thế Liskov)**:

Objects của superclass có thể được thay thế bằng objects của subclass mà không làm thay đổi tính đúng đắn của chương trình.

Tại sao quan trọng? Đảm bảo rằng inheritance được sử dụng đúng cách:
- Subclass không nên làm yếu preconditions của superclass
- Subclass không nên làm mạnh postconditions của superclass
- Subclass phải có thể thay thế superclass trong mọi context

Ví dụ vi phạm: Class `Rectangle` có method `setWidth()` và `setHeight()`. Class `Square` extends `Rectangle` nhưng override để đảm bảo width = height. Điều này vi phạm LSP vì code expect Rectangle có thể set width và height độc lập.

Cách sửa: Không nên để Square extends Rectangle. Tạo interface `Shape` và cả hai implement nó.

**I - Interface Segregation Principle (Nguyên tắc Phân tách Interface)**:

Clients không nên phụ thuộc vào interfaces mà họ không sử dụng. Thay vì một interface lớn, nên có nhiều interfaces nhỏ, specific.

Tại sao quan trọng? Khi một interface quá lớn:
- Clients phải implement methods không cần thiết
- Thay đổi interface ảnh hưởng đến tất cả clients
- Vi phạm Single Responsibility Principle

Ví dụ vi phạm: Interface `Worker` có methods `work()`, `eat()`, `sleep()`. Class `Robot` implement Worker nhưng không cần eat() và sleep().

Cách sửa: Tách thành `Workable`, `Eatable`, `Sleepable`. Robot chỉ implement Workable.

**D - Dependency Inversion Principle (Nguyên tắc Đảo ngược Phụ thuộc)**:

High-level modules không nên phụ thuộc vào low-level modules. Cả hai nên phụ thuộc vào abstractions. Abstractions không nên phụ thuộc vào details. Details nên phụ thuộc vào abstractions.

Tại sao quan trọng? Giảm coupling và tăng flexibility:
- High-level modules không phụ thuộc vào implementation cụ thể
- Dễ dàng thay đổi implementation
- Dễ test bằng cách mock dependencies

Ví dụ vi phạm: Class `EmailService` phụ thuộc trực tiếp vào `SmtpClient`. Nếu muốn đổi sang API khác, phải sửa EmailService.

Cách sửa: Tạo interface `EmailProvider`, `SmtpClient` implement nó. `EmailService` phụ thuộc vào `EmailProvider` interface.

**Ví dụ vi phạm và cách sửa**:

Một class vi phạm nhiều nguyên tắc SOLID thường có các đặc điểm:
- Quá nhiều methods và responsibilities
- Hard dependencies vào concrete classes
- Khó test và maintain
- Khó mở rộng

Cách sửa: Áp dụng các Design Patterns phù hợp:
- Factory Pattern cho DIP
- Strategy Pattern cho OCP
- Adapter Pattern cho interface compatibility
- Decorator Pattern cho extending functionality

**Mối quan hệ với Design Patterns**:

Design Patterns giúp implement SOLID Principles:
- **Factory Pattern**: Implement DIP và OCP
- **Strategy Pattern**: Implement OCP
- **Observer Pattern**: Implement DIP
- **Adapter Pattern**: Implement ISP
- **Template Method**: Implement OCP và LSP

**Best practices**:

- Luôn nghĩ về SOLID khi thiết kế classes
- Refactor code vi phạm SOLID
- Sử dụng Design Patterns để implement SOLID
- Review code với SOLID principles
- Không over-apply: Đôi khi vi phạm nhỏ là acceptable

### 2. Dependency Injection Pattern

**Mục đích**: Một kỹ thuật của Inversion of Control (IoC) trong đó dependencies được cung cấp cho một đối tượng thay vì đối tượng tự tạo chúng.

**Khái niệm và lý thuyết**:

Dependency Injection (DI) là một kỹ thuật implement Inversion of Control (IoC), trong đó dependencies của một object được cung cấp từ bên ngoài thay vì object tự tạo chúng.

Tại sao cần Dependency Injection? Khi một class tự tạo dependencies:
- Tight coupling: Class phụ thuộc vào implementation cụ thể
- Khó test: Không thể mock dependencies
- Vi phạm Dependency Inversion Principle
- Khó thay đổi implementation

Ví dụ vi phạm: `UserService` tự tạo `EmailService` và `DatabaseService`. Khó test và thay đổi.

Cách sửa: Inject `EmailService` và `DatabaseService` vào constructor của `UserService`.

**Inversion of Control (IoC) vs Dependency Injection**:

- **IoC**: Nguyên tắc tổng quát - control flow được đảo ngược. Framework kiểm soát flow thay vì application code.
- **DI**: Một cách implement IoC - dependencies được inject vào object thay vì object tự tạo.

IoC có thể được implement bằng nhiều cách: DI, Service Locator, Template Method, Strategy Pattern. DI là cách phổ biến nhất.

**Các loại DI**:

1. **Constructor Injection**: Dependencies được inject qua constructor. Được khuyến nghị nhất vì:
   - Đảm bảo object được tạo với tất cả dependencies
   - Immutable (nếu sử dụng final)
   - Dễ test

2. **Setter Injection**: Dependencies được inject qua setter methods. Phù hợp khi:
   - Dependencies là optional
   - Cần thay đổi dependencies sau khi tạo object

3. **Field Injection**: Dependencies được inject trực tiếp vào fields (thường dùng annotations). Không được khuyến nghị vì:
   - Khó test (phải dùng reflection)
   - Ẩn dependencies
   - Không thể sử dụng final

4. **Interface Injection**: Object implement interface để nhận dependencies. Ít được sử dụng.

**Khi nào nên dùng**:

- Khi muốn giảm coupling giữa classes
- Khi cần test code (có thể mock dependencies)
- Khi muốn thay đổi implementation dễ dàng
- Trong framework-based applications (Spring, Guice)

**Use cases**:

- **Testing**: Mock dependencies để test unit
- **Loose coupling**: Giảm phụ thuộc giữa components
- **Framework integration**: Spring, Guice sử dụng DI
- **Configuration**: Thay đổi behavior thông qua configuration

**So sánh với Service Locator**:

- **Dependency Injection**: Dependencies được cung cấp cho object. Object không biết cách lấy dependencies.
- **Service Locator**: Object tự tìm dependencies từ Service Locator. Object biết về Service Locator.

DI được khuyến nghị hơn vì:
- Dependencies rõ ràng (visible trong constructor)
- Dễ test hơn
- Tuân theo Dependency Inversion Principle tốt hơn

**Ưu điểm**:
- Loose coupling
- Dễ test (có thể mock)
- Tuân theo SOLID principles
- Flexible và maintainable
- Dependencies rõ ràng

**Nhược điểm**:
- Tăng complexity ban đầu
- Cần DI container hoặc manual wiring
- Có thể over-engineering cho simple cases
- Learning curve cho developers mới

**DI Containers (Spring, Guice)**:

DI Containers quản lý lifecycle và dependencies:
- **Spring Framework**: Sử dụng annotations (@Autowired, @Component) hoặc XML configuration
- **Google Guice**: Sử dụng annotations và modules
- **Dagger**: Compile-time DI cho Android

Containers tự động:
- Tạo objects
- Resolve dependencies
- Manage lifecycle
- Provide scoping (singleton, prototype, etc.)

**Best practices**:

- Ưu tiên Constructor Injection
- Sử dụng interfaces cho dependencies
- Tránh Field Injection
- Sử dụng DI containers cho complex applications
- Document dependencies
- Không inject quá nhiều dependencies (có thể vi phạm SRP)

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

### Câu hỏi cơ bản về Design Patterns

**1. Design Pattern là gì?**

Design Pattern là các giải pháp có thể tái sử dụng cho các vấn đề thiết kế phần mềm phổ biến. Chúng không phải là code cụ thể mà là các template hoặc mô tả cách giải quyết một vấn đề có thể áp dụng trong nhiều tình huống khác nhau.

Design Patterns cung cấp:
- Giải pháp đã được kiểm chứng
- Best practices
- Ngôn ngữ chung cho developers
- Cấu trúc rõ ràng cho code

**2. Tại sao sử dụng Design Patterns?**

- Giải quyết vấn đề thiết kế phổ biến một cách hiệu quả
- Cải thiện code quality (readability, maintainability, reusability)
- Giảm coupling giữa components
- Tăng khả năng mở rộng
- Cung cấp từ vựng chung
- Được sử dụng trong frameworks và libraries
- Giảm bugs bằng cách tuân theo best practices

**3. Phân loại Design Patterns**

Design Patterns được phân loại thành 3 nhóm:
- **Creational**: Tập trung vào cách tạo đối tượng (Singleton, Factory, Builder, etc.)
- **Structural**: Tập trung vào cách kết hợp objects (Adapter, Decorator, Facade, etc.)
- **Behavioral**: Tập trung vào cách objects giao tiếp (Observer, Strategy, Command, etc.)

**4. Sự khác biệt giữa Design Pattern và Framework**

- **Design Pattern**: Là giải pháp cho một vấn đề cụ thể, có thể implement theo nhiều cách khác nhau
- **Framework**: Là một kiến trúc cụ thể với code implementation, cung cấp infrastructure cho ứng dụng

Framework thường sử dụng nhiều Design Patterns. Ví dụ: Spring Framework sử dụng Dependency Injection, Factory Pattern, Proxy Pattern.

### Câu hỏi về Creational Patterns

**1. Singleton: Các cách implement và Thread-safety**

Các cách implement Singleton:
- Eager Initialization: Đơn giản, thread-safe tự nhiên nhưng tốn memory
- Lazy Initialization: Tiết kiệm memory nhưng cần xử lý thread-safety
- Thread-safe với synchronized: An toàn nhưng chậm
- Double-Checked Locking: Hiệu quả, cần volatile keyword
- Enum Singleton: Được khuyến nghị nhất trong Java

Thread-safety quan trọng vì trong môi trường đa luồng, nhiều threads có thể tạo nhiều instances nếu không xử lý đúng.

**2. Factory vs Abstract Factory**

- **Factory Method**: Tạo một loại object. Mỗi concrete creator tạo một concrete product.
- **Abstract Factory**: Tạo families of related objects. Một factory tạo nhiều related products.

Ví dụ: Factory Method tạo Button (WindowsButton hoặc MacButton). Abstract Factory tạo cả Button và Dialog cùng theme (Windows hoặc Mac).

**3. Builder vs Constructor**

- **Constructor**: Đơn giản cho objects ít parameters. Khó đọc với nhiều parameters.
- **Builder**: Tốt cho objects với nhiều parameters, optional parameters. Dễ đọc, type-safe, có thể tạo immutable objects.

Builder Pattern phù hợp khi có nhiều hơn 4-5 parameters hoặc nhiều optional parameters.

**4. Prototype: Shallow vs Deep copy**

- **Shallow copy**: Chỉ copy references, không copy nested objects. Nhanh nhưng có thể gây side effects.
- **Deep copy**: Copy tất cả nested objects. An toàn nhưng chậm hơn và tốn memory hơn.

Chọn shallow copy khi nested objects là immutable hoặc không cần copy. Chọn deep copy khi cần độc lập hoàn toàn.

**5. Khi nào dùng pattern nào?**

- **Singleton**: Khi cần một instance duy nhất (Logger, Configuration)
- **Factory**: Khi logic tạo object phức tạp hoặc cần quyết định tại runtime
- **Builder**: Khi object có nhiều parameters hoặc optional parameters
- **Prototype**: Khi việc tạo object tốn kém và cần clone
- **Object Pool**: Khi objects đắt tiền và cần reuse

### Câu hỏi về Structural Patterns

**1. Adapter vs Decorator vs Facade**

- **Adapter**: Chuyển đổi interface để làm cho incompatible classes làm việc cùng nhau. Không thay đổi behavior.
- **Decorator**: Thêm behavior mới cho object. Có thể wrap nhiều decorators.
- **Facade**: Đơn giản hóa interface phức tạp. Cung cấp interface đơn giản cho subsystem.

**2. Proxy vs Decorator**

- **Proxy**: Kiểm soát truy cập đến object. Có thể lazy load, access control, caching.
- **Decorator**: Thêm behavior cho object. Tập trung vào functionality.

Proxy thay thế object, Decorator wrap object để thêm behavior.

**3. Composite: Khi nào dùng?**

Khi cần tổ chức objects theo cấu trúc cây và xử lý chúng thống nhất. Ví dụ: File system (File và Folder), UI components (Button và Panel chứa Buttons).

**4. Bridge: Tách abstraction khỏi implementation**

Bridge Pattern tách abstraction (interface) khỏi implementation (concrete class) để chúng có thể thay đổi độc lập. Sử dụng composition thay vì inheritance.

Ví dụ: Shape (abstraction) và DrawingAPI (implementation). Có thể thay đổi Shape hoặc DrawingAPI độc lập.

### Câu hỏi về Behavioral Patterns

**1. Observer vs Pub/Sub**

- **Observer**: Synchronous, direct communication. Subject biết observers.
- **Pub/Sub**: Asynchronous, thông qua message broker. Publisher và Subscriber không biết nhau.

Observer phù hợp cho tight coupling, Pub/Sub phù hợp cho loose coupling và distributed systems.

**2. Strategy vs State**

- **Strategy**: Thay đổi behavior dựa trên algorithm được chọn (external). Context chọn strategy.
- **State**: Thay đổi behavior dựa trên internal state. State object quản lý transitions.

Strategy là về "how" (cách làm), State là về "when" (khi nào).

**3. Command: Undo/Redo implementation**

Command Pattern lưu trữ commands trong history. Mỗi command có execute() và undo(). Undo stack lưu commands đã execute, Redo stack lưu commands đã undo.

**4. Chain of Responsibility: Use cases**

- Exception handling: Mỗi handler xử lý một loại exception
- Authentication/Authorization: Chain các validators
- Event processing: Process events qua middleware chain
- Logging: Chain các log handlers

**5. Template Method vs Strategy**

- **Template Method**: Sử dụng inheritance, định nghĩa skeleton algorithm, subclass implement steps.
- **Strategy**: Sử dụng composition, thay đổi toàn bộ algorithm.

Template Method cho phép thay đổi một số steps, Strategy cho phép thay đổi toàn bộ algorithm.

### Câu hỏi về SOLID Principles

**1. Giải thích từng nguyên tắc**

- **S - Single Responsibility**: Một class chỉ có một lý do để thay đổi
- **O - Open/Closed**: Mở để mở rộng, đóng để sửa đổi
- **L - Liskov Substitution**: Subclass có thể thay thế superclass
- **I - Interface Segregation**: Clients không phụ thuộc vào interfaces không sử dụng
- **D - Dependency Inversion**: Phụ thuộc vào abstractions, không phụ thuộc vào concretions

**2. Ví dụ vi phạm và cách sửa**

Ví dụ vi phạm SRP: Class `User` vừa quản lý data, vừa gửi email, vừa validate.
Cách sửa: Tách thành `User`, `EmailService`, `UserValidator`.

**3. Mối quan hệ với Design Patterns**

Design Patterns giúp implement SOLID:
- Factory Pattern implement DIP và OCP
- Strategy Pattern implement OCP
- Observer Pattern implement DIP
- Adapter Pattern implement ISP

### Câu hỏi thực tế

**1. Design một hệ thống sử dụng patterns**

Ví dụ: Design một hệ thống quản lý đơn hàng:
- Repository Pattern cho data access
- Factory Pattern cho tạo Order objects
- Observer Pattern cho notify khi order status thay đổi
- Strategy Pattern cho tính toán shipping cost
- Facade Pattern cho đơn giản hóa API

**2. Refactor code sử dụng patterns**

Các bước:
- Identify code smells (long methods, tight coupling, etc.)
- Chọn pattern phù hợp
- Refactor từng bước
- Test sau mỗi bước
- Đảm bảo không break existing functionality

**3. So sánh các patterns cho use case cụ thể**

Ví dụ: Cần thêm logging cho methods. Có thể dùng:
- Decorator Pattern: Wrap methods với logging
- AOP (Aspect-Oriented Programming): Intercept methods
- Proxy Pattern: Proxy object với logging

So sánh dựa trên: complexity, performance, maintainability, testability.

### Câu hỏi nâng cao

**1. Anti-patterns**

Các anti-patterns phổ biến:
- God Object: Một class làm quá nhiều việc
- Spaghetti Code: Code không có cấu trúc
- Golden Hammer: Sử dụng một pattern cho mọi vấn đề
- Premature Optimization: Tối ưu quá sớm
- Copy-Paste Programming: Copy code thay vì reuse

**2. Performance considerations**

- Singleton: Eager vs Lazy initialization
- Factory: Có thể cache created objects
- Observer: Có thể có performance issue với nhiều observers
- Proxy: Overhead của proxy layer
- Object Pool: Giảm object creation overhead

**3. Testing với Design Patterns**

- Dependency Injection giúp mock dependencies
- Factory Pattern giúp tạo test objects
- Strategy Pattern giúp test từng strategy độc lập
- Observer Pattern cần test notification flow
- Singleton khó test vì global state

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

## Tài liệu tham khảo

- **Gang of Four (GoF)**: "Design Patterns: Elements of Reusable Object-Oriented Software" (1994)
- **Effective Java** by Joshua Bloch
- **Clean Code** by Robert C. Martin
- **Head First Design Patterns** by Eric Freeman & Elisabeth Robson
- **Refactoring Guru**: https://refactoring.guru/design-patterns
- **Java Design Patterns**: Best Practices và Community Resources

---

## Hướng dẫn sử dụng tài liệu

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
