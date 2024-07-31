# Java-Interview-questions-for-Freshers
Chứa các câu hỏi lý thuyết java cho phỏng vấn

## Cơ bản và cú pháp Java
1. Java là một ngôn ngữ độc lập nền tảng như thế nào?
    - Độc lập nền tảng tức là java không phụ thuộc vào bất kì nền tảng nào (windows, linux hay macos..., các phần cứng).
    - Không như những ngôn ngữ khác, java có trình biên dịch JavaC, nó có nhiệm vụ biên dịch code ra mã bytecode (.class file) - Mã Bytecode này là trung gian giữa mã nguồn và các mã máy cụ thể khác nhau(Tức là từ mã bytecode có thể biên dịch ra nhiều mã máy khác nhau).
    - Với từng môi trường, hệ điều hành hay phần cứng khác nhau thì JVM(được xây dựng tương thích với đa nền tảng) sẽ thông dịch mã Bytecode thành mã máy và thực thi nó.
    - Just-In-Time Compilation (JIT): là phương pháp kết hợp biên dịch và thông dịch để tối ưu hoá hiệu suất. JIT thực thi trong runtime, Khi JVM phát hiện mã Bytecode được thực thi nhiều lần(method được dùng chung), JIT sẽ biên dịch đoạn mã đó thành mã máy ngay lập tức và lưu trữ để tránh thông dịch lại các đoạn mã giống nhau, giúp tối ưu hoá hiệu suất của JVM.
2. JVM menory storages Java?
    - Class(method) Area: Lưu trữ dữ liệu của class-level, bao gồm các field, các biến static, method data.... Mỗi JVM chỉ có 1 Class Area và các tài nguyên trong vùng này đều chia sẻ.
    - Heap Area: Các đối tương được tạo ra sẽ được lưu trữ ở vùng này, Heap sẽ chịu trách nhiệm phân bổ bộ nhớ cho các đối tượng này trong runtime.
    - Stack Area: Lưu trữ dữ liệu, 1 phần kết quả trả về cho phương thức và thực hiện liên kết động. Mỗi luồng được tạo ra sẽ có một Stack runtime được tạo ra để phục vụ luồng đó, khi luồng kết thúc thì chúng cũng bị huỷ.
    - PC Register: Lưu trữ địa chỉ của lệnh thực thi hiện tại của luồng, Mỗi luồng sẽ có một thanh ghi khác nhau.
    - Native Method Stacks: lưu trữ tất cả các phương thức gốc được sử dụng.
3. Sự khác nhau giữa JVM, JRE, JDK
    - JVM là viết tắt của máy ảo Java, nó là một phần của JRE. JVM là một loại trình thông dịch chịu trách nhiệm chuyển đổi mã bytecode thành mã máy. Bản thân JVM phụ thuộc vào nền tảng, môi trường mà nó hoạt động.
    - JRE là viết tắt của Java Runtime Environment, nó là gói cài đặt cung cấp môi trường để chạy chương trình hoặc ứng dụng Java trên bất kì máy nào.
    - JDK là viết tắt của Java Development kit (Bộ công cụ phát triển java), nó cung cấp môi trường để phát triển và thực thi java
4. Đặc điểm nổi bật của Java
    - Đơn giản (Simple ): Java khá đơn giản và dễ tiếp cận.
    - Độc lập nền tảng (Platform Independent): Có thể thực thi không phụ thuộc vào nền tảng, chỉ cần có mã bytecode và nền tảng đó chứa JVM
    - Thông dịch (Interperted):Là ngôn ngữ kết hợp cả thông dịch và biên dịch.
    - Các tính năng mạnh mẽ (Robust): Trình thu gom rác GC, Exception handling, Type checking ...
    - Hướng đối tượng (Object - Oriented): Java là ngôn ngữ hướng đối tượng hoàn toàn, tất cả các chương trình để phải khai báo trong class, Object, nó có 4 tính chất đặc biệt của hướng đối tượng như: Tính kế thừa - inheritance, tính đóng gói - encapsulation, tính đa hình - polymorphism, tính trừu tượng - abstraction.
    - Bảo mật (Secured): Java an toàn nhờ trình thông dịch JVM.
    - Hiệu năng cao (High Performance): nhanh hơn các ngôn ngữ lập trình thông dịch truyền thống khác.
    - Linh hoạt (Dynamic): Java hỗ trợ việc nạp các class và interface động, tức là ta có thể nạp chúng vào bộ nhớ khi cần mà không phải biên dịch lại toàn bộ chương trình. Giúp Java linh hoạt và dễ mở rộng.
    - Phân tán (Distributed): Java có các thư viện hỗ trợ phát triển các ứng dụng phân tán, tức là các ứng dụng có thể chạy trên nhiều máy tính kết nối với nhau qua mạng.
    - Đa luồng (Multithreaded): Java hỗ trợ đa luồng, cho phép chương trình thực hiện nhiều tác vụ đồng thời trong các luồng riêng biệt.
5. f
6. f
7. t
8. e
9. t
10. e
11. t
12. 
