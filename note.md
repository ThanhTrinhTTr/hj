## TRỒNG CAM

An là một người rất thích cam, và hôm nay bạn ấy quyết định trồng nó trên một dải đất có độ dài $N$. “Trạm phát giống” là một điểm mà chứa rất nhiều hạt giống của cây cam, có tất cả $K$ điểm “Trạm phát giống” trên mảnh đất và mỗi điểm có vị trí là $Ki$ $(1 \le Ki \le N)$. Giỏ của An chỉ chứa đủ $w$ hạt giống, vì An không thể ước chừng số hạt còn lại trong giỏ nên chỉ khi hết hạt thì An mới có thể quay lại các điểm trước đó cũng như quay lại “Trạm phát giống” trước đó để lấy hạt. Thời gian di chuyển giữa hai điểm gần nhất là **1** đơn vị thời gian. 

Yêu cầu: Giả sử ban đầu An đứng ở vị trí đầu tiên trên dải đất kéo dài từ 1 đến $N$, tồn tại điểm “Trạm phát giống” ở vị trí thứ 1, thời gian gieo hạt không đáng kể cũng như An phải gieo hạt ở các điểm lần lượt theo thứ tự trừ trái sang phải, hãy xác định thời gian ngắn nhất để An có thể gieo hạt tại tất cả các điểm trên mảnh đất ngoại trừ “Trạm phát giống”. Nếu An không thể gieo hạt trên mảnh đất này thì không tồn tại cách gieo hạt trên mảnh đất và in ra -1.
## Input : 
#### Từ tệp văn bản TRONGCAM.INP gồm : 
-   Dòng đầu tiên gồm 3 số nguyên dương $N, K, w$  $(1 \le N, K \le 100, 1 \le w \le 2^{60} )$ : Độ dài mảnh đất, số lượng “Trạm phát giống” và lượng hạt giống tối đa mà giỏ của An có thể chứa được.
-   Dòng tiếp theo bao gồm $K$ số $Ki$ $(1 \le Ki \le N, 1 \le i \le K)$: Vị trí của các “Trạm phát giống” trên mảnh đất.

## Output
#### Ghi vào tệp TRONGCAM.OUT gồm một dòng duy nhất là thời gian ngắn nhất để có thể gieo hạt trên tất cả các điểm ngoại trừ “Trạm phát giống”. Nếu không tồn tại cách gieo hạt trên mảnh đất thì in ra -1.
## Sample Input 1 
```
4 2 1
1 4
```

## Sample Output 1
```
5
```
## Sample Input 2 
```
1 1 1
1

```

## Sample Output 
```
-1
```
## Giải thích :
-   Dưới đây là cách để An gieo hạt với thời gian ít nhất trong ví dụ đầu tiên:
       +   Từ vị trí 1 đến vị trí 2: Đi hết 1 đơn vị thời gian.
       +   Tại vị trí thứ 2 : Vì đây không phải “Trạm phát giống” nên An gieo hạt tại đây. Sau khi gieo hạt, số hạt trong túi đã hết nên An cần về “Trạm phát giống” trước đó (tại điểm 1) để lấy hạt : Mất 1 đơn vị thời gian để di chuyển từ vị trí 2 về vị trí 1 và quay trở lại vị trí 2.
       +   Từ vị trí 2 đến vị trí 3 : Đi hết 1 đơn vị thời gian.
       +   Tại vị trí thứ 3 : An gieo hạt giống. Dù số hạt trong túi đã hết nhưng điểm tiếp theo trên đường đi là “Trạm phát giống” nên An có thể lấy hạt ở điểm tiếp theo. Vì thế, An không cần quay lại điểm trước đó để lấy hạt.
       +   Từ vị trí 3 đến vị trí 4 : Đi hết 1 đơn vị thời gian.
       Vậy thời gian ngắn nhất có thể đạt được là 5 đơn vị thời gian.
   -  Ở ví dụ thứ 2, vì điểm thứ 1 là điểm duy nhất của mảnh đất mà điểm đó lại là “Trạm phát sóng” nên An không thể gieo hạt trên mảnh đất cũng như điều kiện để gieo hạt ở trên mảnh đất không thỏa mãn. Vì vậy kết quả in ra là -1.

## Subtask
  -  30% số test có $K$ = 1
  -  70% số test còn lại không ràng buộc gì thêm
