# Java-Interview-questions-for-Freshers
Chứa các câu hỏi lý thuyết java cho phỏng vấn

## Cơ bản và cú pháp Java (Geeksforgeek) https://www.geeksforgeeks.org/java-interview-questions/#java-interview-questions-for-freshers
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

## Top 30 các câu hỏi phỏng vấn java thường gặp và cách trả lời (Vtiacademy) https://vtiacademy.edu.vn/top-30-cac-cau-hoi-phong-van-java-thuong-gap-va-cach-tra-loi.html
### Các câu hỏi về java core
1. Java là gì? Đặc điểm chính của Java là gì?
    - Java là ngôn ngữ lập trình, là ngôn ngữ hướng đối tượng hoàn toàn, độc lập nền tảng.
    - Java có hỗ trợ các tính năng đặc biệt như, quản lý bộ nhớ động GC, xử lý ngoại lệ Exception.
    - Do là ngôn ngữ hướng đối tượng nên nó chứa đầy đủ các tính chất của lập trình hướng đối tượng với các tính chất như tính kế thừa, tính đóng gói, tính da hình, tính trừu tượng.
    - Java không hỗ trợ đa kế thừa.
2. Sự khác biệt giữa abstract class và interface trong java là gì?
    - Abstract Class: là một class có thể chứa cả abstract method và method được triển khai cụ thể, đồng thời nó cũng có thể chứa các biến instance, constructor. Một class con chỉ có thể kế thừa 1 class. Các phương thức và thuộc tính của abstract class có thể có bất kỳ mức truy cập nào (default, public, private, protected).
    - Interface: chỉ chứa các abstract method (trước java 8) và các default method từ java 8, phạm vi truy cập mặc định của phương thức là public abstract và các biến mặc định là public static final
3. Khác biệt giữa == và .equals() trong Java?
    - "==" sẽ so sánh địa chỉ ô nhớ của 2 đối tượng so sánh.
    - "equals() sẽ so sánh giá trị của 2 đối tượng
4. Java Memory Management hoạt động như thế nào?
    - Java sử dụng Garbage Collection để quản lý bộ nhớ. khi đối tượng không còn được sử dụng thì GC sẽ tự động giải phóng bộ nhớ của đối tượng đó.
5. Tại sao Java được gọi là ngôn ngữ đa luồng (multithreaded)?
    - Java hỗ trợ việc xử lý đa luồng thông qua package java.lang.Thread, nó cho phép chương trình thực thi đồng thời nhiều tác vụ song song, tận dụng hiệu suất của hệ thống.
    - Để triển khai luồng ta có thể extends Thread class hoặc implement Runnable. hoặc từ java 17 có thể triển khai virtual thread
6. Phạm vi (scope) của biến trong Java là gì?
    - Biến là cục bộ (local) khi được khai báo trong một method và sẽ bị huỷ sau khi method hoàn thành.
    - Biến toàn cục (Global) khi được khai báo ở mức class
7. Tại sao phương thức main() luôn là static trong Java?
    - Phương thức main luôn có keyword static là vì static là method hoặc biến được khai báo thuộc về class chứ không phải bất kì object nào được tạo ra cho nên có thể sử dụng mà không cần khởi tạo object. Do main() là điểm khởi đầu của chương trình nên khi JVM chạy sẽ không cần tạo object của class chứa nó.
8. Java có hỗ trợ đa kế thừa không?
    - Java không hỗ trợ đa kế thừa cho class. Một class chỉ có thể kế thừa duy nhất 1 class khác nhưng có thể triển khai nhiều Interface.
### Các câu hỏi phỏng vấn Java OOP
1. OOP là gì và tại sao nó quan trọng trong Java?
    - Là phương pháp lập trình tập trung vào việc tạo ra các đối tượng có thể tương tác với nhau. Chứa dữ liệu dưới dạng các trường và mã(method).
2. Các tính chất cơ bản của OOP là gì?
    - Tính kế thừa
    - Tính đóng gói
    - Tính trừu tượng
    - Tính đa hình
3. Kế thừa trong Java là gì?
    - Đây là khả năng của một class mới (class con) có thể sử dụng các thuộc tính và phương thức của một class hiện có (class cha). Class con kế thừa từ class cha thông qua cơ chế kế thừa, cho phép tái sử dụng mã nguồn và xây dựng mối quan hệ giữa class cha và class con.
4. Lớp là gì?
    - Class là một bản mô tả của một đối tượng. nó định nghĩa các thuộc tính (dữ liệu) và phương thức (hành vi) của đối tượng đó
5. Đối tượng trong java là gì?
    - Object là thể hiện của class, nó bao gồm các thuộc tính và phương thức
6. Có thể sử dụng thuộc tính trong Interface không?
    - Có thể sử dụng thuộc tính trong interface nhưng phải được khai báo với từ khoá final.
7. Interface có thể là final không?
    - Interface không thể là final bởi vì nó cần có các implement class thì mới sử dụng được.
8. Làm thế nào để ngăn chặn việc kế thừa trong java?
    - Để ngăn chặn việc kế thừa trong java ta sẽ thêm keyword final

## Top 20 câu hỏi phỏng vấn Java OOP phổ biến nhất Link: (https://www.facebook.com/groups/devoiminhdidauthe/permalink/23937668312543548/)


















