# Sentiment-Analysis
Phân tích tình cảm là một kỹ thuật xử lý ngôn ngữ tự nhiên (NLP) nhằm phân
tích văn bản và tính toán các kỹ thuật để tự động hóa việc trích xuất hoặc phân loại ý
kiến từ đánh giá ý kiến theo các mức dữ liệu: tích cực, tiêu cực hay trung lập. Phân
tích tình cảm được sử dụng rộng rãi trên nhiều lĩnh vực như Người tiêu dùng thông tin,
Tiếp thị, sách, ứng dụng, trang web và xã hội.
Phân tích tình cảm sử dụng khai thác dữ liệu và máy học(ML) để đưa ra những đánh
giá và dự đoán thành các loại:
+ Phân tích tình cảm chi tiết
+ Phân tích tình cảm chi tiết
+ Phân tích tình cảm dựa trên các khía cạnh
+ Phân tích ý định
- Phân tích tình cảm sử dụng hai phương pháp tiếp cận. Về phương pháp tiếp cận
dựa trên quy tắc, cách tiếp cận sử dụng thuật toán mô tả ý kiến chi tiết như phân tích
cú pháp, phân tích ngôn ngữ, Token hóa,....Thuật toán quét văn bản kỹ lưỡng để tìm
kiếm các từ khớp với quy tắc và danh sách từ được xác định trước, sau đó tính toán
phổ biến nhất. Tuy nhiên, kết quả của phương pháp này không đầy đủ và kém linh
hoat. Về phương pháp phân tích tình cảm tự động, phương pháp sử dụng các thuật
toán máy học có giám sát như hồi quy tuyến tính, hỗ trợ máy vecto, Naive Bayes,...làm
tắng mức độ chính xác và xử lý thông tin trên các tiêu chí một cách nhanh chóng
# Phân loại Navie Bayes 
Là 1 phương pháp phân loại có giám sát. Dù rất dễ hiểu và dễ cài đặt, nhưng kết
quả thu được lại rất tốt, vì thế đây là 1 phương pháp rất quan trọng trong NLP. Ứng
dụng đầu tiên trong NLP của máy phân loại này là phân loại văn bản. Gần đây, máy
phân loại này còn được ứng dụng thành công vào phần mềm lọc spam tự động.
Bài toán phân loại văn bản
Định nghĩa vector đặc trưng x biểu diễn số lần xuất hiện các từ trong văn bản, y là các
catalog (nhãn) mà văn bản thuộc về (ví dụ như thể thao, kinh tế, giải trí,. . . )
Cho 1 tập dữ liệu huấn luyện đã được gán nhãn D = (x(i), y(i)) với i ∈ (1, N). Ở
đây x(i)là vector đặc trưng thứ i trong tập huấn luyện,y(i) thuộc 1, 2, . . . , C là các nhãn
tương ứng với vector đó, x(i) = (x( 1i), x( 2i), . . . , x( di)) với x( di) là số lần xuất hiện của từ thứ
d trong từ điển (ta sẽ tiến hành gắn số thứ tự với từ, nên sẽ gọi là từ d).
Áp dụng công thứ Bayes, ta tính giá trị của p(y|x), nếu giá trị này lớn hơn 1 giá
trị t cho trước, ta kết luận nhãn của vector x là y
Công thức xác suất có điều kiện
P(A/B) = P(AB)
P(B) → P(A/B).P(B) = P(B/A).P(A) = P(AB)
Công thức xác suất đầy đủ
Giả sử B1, B2, . . . .Bn là 1 nhóm đầy đủ các biến cố. Xét biến cố A sao cho A xảy
ra chỉ khi một trong các biến cố B1, B2, . . . .Bn xảy ra. Khi đó :
P(A) =
nXi
=1
P(Bi).P(A/Bi)
Công thức xác suất Navie Bayes
Tử các công thức trên, ta có công thức xác suất Navie Bayes như sau:
P(Bk/A) = P(ABk
P(A) =
P(Bk).P(A/Bk
Pn i=1 P(Bi).P(A/Bi)
