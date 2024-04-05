## TRỒNG CAM

An là một người rất thích cam, và hôm nay bạn ấy quyết định trồng nó trên một dải đất có độ dài **N**. “Trạm phát giống” là một điểm mà chứa rất nhiều hạt giống của cây cam, có tất cả **K** điểm “Trạm phát giống” trên mảnh đất và mỗi điểm có vị trí là \mathbit{k}_\mathbit{i} $(1 $ \le $ \mathbit{k}_\mathbit{i}  \le N)$. Giỏ của An chỉ chứa đủ \mathbit{w} hạt giống, vì An không thể ước chừng số hạt còn lại trong giỏ nên chỉ khi hết hạt thì An mới có thể quay lại các điểm trước đó cũng như quay lại “Trạm phát giống” trước đó để lấy hạt. Thời gian di chuyển giữa hai điểm gần nhất là 1 đơn vị thời gian. 

Yêu cầu: Giả sử ban đầu An đứng ở vị trí đầu tiên trên dải đất kéo dài từ 1 đến N, tồn tại điểm “Trạm phát giống” ở vị trí thứ 1, thời gian gieo hạt không đáng kể cũng như An phải gieo hạt ở các điểm lần lượt theo thứ tự trừ trái sang phải, hãy xác định thời gian ngắn nhất để An có thể gieo hạt tại tất cả các điểm trên mảnh đất ngoại trừ “Trạm phát giống”. Nếu An không thể gieo hạt trên mảnh đất này thì không tồn tại cách gieo hạt trên mảnh đất và in ra -1.
## Input

Gồm ~1~ dòng chứa ~2~ số nguyên ~A~ và ~B~ ~(1 \le A, B \le 1000)~, cách bởi ~1~ dấu cách.

## Output

Ghi ra tổng ~A + B~.

## Sample Input 
```
3 4
```

## Sample Output 
```
7
```

## Subtask
- 30% số test có ~A \le 100~
- ~30\%~ số test tiếp theo có ~A \le 500~
- ~40\%~ số test còn lại không có điều kiện gì thêm

## Note

Gợi ý: Sử dụng toán tử "+".
