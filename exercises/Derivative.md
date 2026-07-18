# BÀI TẬP ĐẠO HÀM — LUYỆN TỪ CƠ BẢN ĐẾN SIÊU KHÓ
*(đồng bộ 100% với lý thuyết A1 – A3 đã xây dựng)*

**Cách dùng:** Với mỗi bài, hãy **tự làm trước**, cố gắng gọi tên đúng bước trong thuật toán (ví dụ: "đây là bước cô lập m", "đây là bước lập bảng xét dấu f'(x)") rồi mới đối chiếu lời giải. Lời giải luôn viết theo đúng khuôn/quy trình đã cho ở lý thuyết — không dùng mẹo tắt nào ngoài đó.

Ký hiệu độ khó: ⭐ cơ bản → ⭐⭐⭐⭐⭐ siêu khó / HSG.

---

## PHẦN 1 — A1: Đạo hàm cơ bản + quy tắc đại số

**Bài 1** (⭐) $y = 3x^4 - 2x^3 + 5x - 7$

**Bài 2** (⭐) $y = \sqrt{x} + \dfrac{1}{x}$

**Bài 3** (⭐⭐) $y = x^2\sin x$ *(quy tắc tích)*

**Bài 4** (⭐⭐) $y = \dfrac{2x-1}{x+3}$ *(quy tắc thương)*

**Bài 5** (⭐⭐) $y = e^x - \ln x + 3^x$

### Lời giải 1–5

**1.** Áp trực tiếp bảng gốc từng số hạng, dùng $(u\pm v)'=u'\pm v'$:
$$y' = 12x^3 - 6x^2 + 5$$

**2.** $\sqrt{x}=x^{1/2}$, $\dfrac1x = x^{-1}$:
$$y' = \frac{1}{2\sqrt{x}} - \frac{1}{x^2}$$

**3.** $(uv)'=u'v+uv'$ với $u=x^2, v=\sin x$:
$$y' = 2x\sin x + x^2\cos x$$

**4.** $\left(\dfrac{u}{v}\right)'=\dfrac{u'v-uv'}{v^2}$ với $u=2x-1,v=x+3$:
$$y' = \frac{2(x+3)-(2x-1)}{(x+3)^2} = \frac{7}{(x+3)^2}$$

**5.** Tra bảng gốc trực tiếp:
$$y' = e^x - \frac1x + 3^x\ln 3$$

---

## PHẦN 2 — A2: Đạo hàm hàm hợp (chain rule)

### 2.1. Một lớp hợp (⭐⭐)

**Bài 6** $y=(3x^2-5x+1)^7$
**Bài 7** $y=\sin(2x^2-1)$
**Bài 8** $y=e^{x^2+3x}$
**Bài 9** $y=\ln(x^2+1)$
**Bài 10** $y=\sqrt{4-x^2}$

### Lời giải 6–10 *(áp đúng "khuôn" 3 bước: bóc lớp ngoài → nhân $u'$ → dừng vì $u$ không còn hợp)*

**6.** Khuôn $(u^n)'=n u^{n-1}u'$, $u=3x^2-5x+1,\ u'=6x-5$:
$$y' = 7(3x^2-5x+1)^6(6x-5)$$

**7.** Khuôn $(\sin u)'=\cos u\cdot u'$, $u=2x^2-1,\ u'=4x$:
$$y' = 4x\cos(2x^2-1)$$

**8.** Khuôn $(e^u)'=e^u\cdot u'$, $u=x^2+3x,\ u'=2x+3$:
$$y' = (2x+3)e^{x^2+3x}$$

**9.** Khuôn $(\ln u)'=\dfrac{u'}{u}$, $u=x^2+1,\ u'=2x$:
$$y' = \frac{2x}{x^2+1}$$

**10.** Khuôn $(\sqrt{u})'=\dfrac{u'}{2\sqrt u}$, $u=4-x^2,\ u'=-2x$:
$$y' = \frac{-x}{\sqrt{4-x^2}}$$

---

### 2.2. Nhiều lớp lồng nhau — SIÊU KHÓ (⭐⭐⭐⭐ – ⭐⭐⭐⭐⭐)

> Quy trình: **lặp lại bước "bóc lớp ngoài + nhân $u'$"** cho tới khi lớp trong cùng chỉ còn là đa thức/biểu thức sơ cấp.

**Bài 11** (⭐⭐⭐⭐) $y=\sin^3\left(2x-\dfrac{\pi}{4}\right)$ *(3 lớp: mũ 3 → sin → tuyến tính)*

**Bài 12** (⭐⭐⭐⭐) $y=\sqrt{\ln(x^2+1)}$ *(3 lớp: căn → ln → đa thức)*

**Bài 13** (⭐⭐⭐⭐) $y=e^{\sin^2(3x)}$ *(4 lớp: $e^u$ → mũ 2 → sin → tuyến tính)*

**Bài 14** (⭐⭐⭐⭐) $y=\ln\big(\cos\sqrt{x}\big)$ *(3 lớp: ln → cos → căn)*

**Bài 15** (⭐⭐⭐⭐⭐) $y=\tan^2\big(\ln(x^2+1)\big)$ *(4 lớp: mũ 2 → tan → ln → đa thức)*

### Lời giải 11–15

**11.** Đặt $v=\sin\left(2x-\frac\pi4\right)$, $y=v^3$.
- Lớp ngoài (mũ 3): $y'=3v^2\cdot v'$
- Lớp trong ($v=\sin u$, $u=2x-\frac\pi4$): $v' = \cos\left(2x-\frac\pi4\right)\cdot 2$

$$y' = 6\sin^2\left(2x-\frac{\pi}{4}\right)\cos\left(2x-\frac{\pi}{4}\right)$$

**12.** Đặt $v=\ln(x^2+1)$, $y=\sqrt v$.
- Lớp ngoài (căn): $y' = \dfrac{v'}{2\sqrt v}$
- Lớp trong (ln): $v' = \dfrac{2x}{x^2+1}$

$$y' = \frac{x}{(x^2+1)\sqrt{\ln(x^2+1)}}$$

**13.** Đặt $u=\sin^2(3x)$ (bản thân $u$ đã là hợp!), $y=e^u$.
- Lớp 1 ($e^u$): $y'=e^u\cdot u'$
- Lớp 2 ($u=w^2$, $w=\sin 3x$): $u' = 2w\cdot w' = 2\sin(3x)\cdot 3\cos(3x)=6\sin3x\cos3x$

$$y' = 6\sin(3x)\cos(3x)\,e^{\sin^2(3x)} = 3\sin(6x)\,e^{\sin^2(3x)}$$
*(dùng thêm công thức nhân đôi $2\sin\theta\cos\theta=\sin2\theta$ để rút gọn — bước "hậu xử lý", không bắt buộc).*

**14.** Đặt $v=\cos\sqrt x$, $y=\ln v$.
- Lớp ngoài (ln): $y'=\dfrac{v'}{v}$
- Lớp trong (cos → căn, 2 lớp con): $v' = -\sin(\sqrt x)\cdot \dfrac{1}{2\sqrt x}$

$$y' = \frac{-\sin(\sqrt x)}{2\sqrt x\,\cos(\sqrt x)} = -\frac{\tan(\sqrt x)}{2\sqrt x}$$

**15.** Đặt $u=\ln(x^2+1)$, $v=\tan u$, $y=v^2$. Bóc từng lớp một, ngoài vào trong:
- Lớp 1 (mũ 2): $y'=2v\cdot v'$
- Lớp 2 (tan): $v' = \dfrac{1}{\cos^2 u}\cdot u'$
- Lớp 3 (ln): $u' = \dfrac{2x}{x^2+1}$

Ghép lại:
$$y' = 2\tan\big(\ln(x^2{+}1)\big)\cdot\frac{1}{\cos^2\big(\ln(x^2{+}1)\big)}\cdot\frac{2x}{x^2+1} = \frac{4x\tan\big(\ln(x^2{+}1)\big)}{(x^2+1)\cos^2\big(\ln(x^2{+}1)\big)}$$

---

## PHẦN 3 — A3: Ứng dụng đạo hàm (theo đúng cây quyết định)

### 3.1. Đơn điệu

**Bài 16** (⭐⭐) Xét đồng biến/nghịch biến của $y=x^3-3x^2-9x+5$.

**Bài 17** (⭐⭐⭐) Xét đồng biến/nghịch biến của $y = x+\dfrac{1}{x-1}$ (chú ý TXĐ).

### Lời giải 16–17 *(đúng 5 bước: TXĐ → f' → giải f'=0 → bảng dấu → kết luận)*

**16.**
- B1: TXĐ $=\mathbb R$.
- B2: $y'=3x^2-6x-9$.
- B3: $y'=0 \Leftrightarrow 3(x-3)(x+1)=0 \Leftrightarrow x=-1$ hoặc $x=3$.
- B4: Vì hệ số $x^2$ dương, $y'>0$ ở ngoài khoảng hai nghiệm, $y'<0$ ở giữa:

| $x$ | $-\infty$ | $-1$ | $3$ | $+\infty$ |
|---|---|---|---|---|
| $y'$ | $+$ | $0$ | $-\ \ 0\ \ +$ | |

- B5: **Đồng biến** trên $(-\infty;-1)$ và $(3;+\infty)$; **nghịch biến** trên $(-1;3)$.

**17.**
- B1: TXĐ $=\mathbb R\setminus\{1\}$.
- B2: $y' = 1-\dfrac{1}{(x-1)^2} = \dfrac{(x-1)^2-1}{(x-1)^2}=\dfrac{x(x-2)}{(x-1)^2}$.
- B3: $y'=0\Leftrightarrow x=0$ hoặc $x=2$ (mẫu luôn dương, không đổi dấu, chỉ **không xác định** tại $x=1$).
- B4: Dấu $y'$ trùng dấu tử $x(x-2)$, riêng bị "cắt" tại $x=1$:

| $x$ | $-\infty$ | $0$ | $1$ | $2$ | $+\infty$ |
|---|---|---|---|---|---|
| $y'$ | $+$ | $0\ \ -$ | ‖ | $-\ \ 0$ | $+$ |

- B5: **Đồng biến** trên $(-\infty;0)$ và $(2;+\infty)$; **nghịch biến** trên $(0;1)$ và $(1;2)$.

---

### 3.2. Cực trị

**Bài 18** (⭐⭐) $y=x^4-4x^2+3$.

**Bài 19** (⭐⭐⭐) $y=\sin x+\cos x$ trên toàn $\mathbb R$.

**Bài 20** (⭐⭐⭐⭐) $y=\dfrac{x^2+3}{x+1}$.

### Lời giải 18–20 *(tìm nghiệm f'=0, xét dấu đổi chiều HOẶC dùng f'')*

**18.**
- $y'=4x^3-8x=4x(x^2-2)=0 \Rightarrow x=0,\ x=\pm\sqrt2$.
- $y''=12x^2-8$. Tại $x=0$: $y''=-8<0\Rightarrow$ **cực đại**, $y_{CD}=y(0)=3$.
- Tại $x=\pm\sqrt2$: $y''=16>0\Rightarrow$ **cực tiểu**, $y_{CT}=y(\pm\sqrt2)=-1$.

**19.**
- $y'=\cos x-\sin x=0\Leftrightarrow \tan x=1\Leftrightarrow x=\dfrac\pi4+k\pi$.
- $y''=-\sin x-\cos x$.
- Tại $x=\dfrac\pi4+k2\pi$: $y''=-\sqrt2<0\Rightarrow$ **cực đại**, $y_{CD}=\sqrt2$.
- Tại $x=\dfrac{5\pi}4+k2\pi$: $y''=\sqrt2>0\Rightarrow$ **cực tiểu**, $y_{CT}=-\sqrt2$.
*(Đây là dạng "cực trị tuần hoàn" hay gặp trong HSG — luôn viết nghiệm dưới dạng $+k2\pi$ vì chu kỳ của $\sin,\cos$ là $2\pi$, không phải $\pi$.)*

**20.** TXĐ $\mathbb R\setminus\{-1\}$.
- $y' = \dfrac{2x(x+1)-(x^2+3)}{(x+1)^2}=\dfrac{x^2+2x-3}{(x+1)^2}=\dfrac{(x-1)(x+3)}{(x+1)^2}$.
- $y'=0\Leftrightarrow x=1$ hoặc $x=-3$.
- Xét dấu (mẫu luôn dương): dấu $y'$ trùng dấu $(x-1)(x+3)$.
- $y'$ đổi $(+)\to(-)$ tại $x=-3\Rightarrow$ **cực đại** $y_{CD}=y(-3)=-6$.
- $y'$ đổi $(-)\to(+)$ tại $x=1\Rightarrow$ **cực tiểu** $y_{CT}=y(1)=2$.

---

### 3.3. GTLN – GTNN trên đoạn $[a;b]$

**Bài 21** (⭐⭐) $y=x^3-3x+2$ trên $[-2;3]$.

**Bài 22** (⭐⭐⭐) $y=\sin x+\cos x$ trên $[0;\pi]$.

**Bài 23 — Vật lý** (⭐⭐⭐⭐) Một chất điểm chuyển động có quãng đường $s(t)=t^3-6t^2+9t$ (m), $t\in[0;5]$ (s).
a) Tìm thời điểm gia tốc bằng 0, tính vận tốc tại thời điểm đó.
b) Tìm vận tốc lớn nhất, nhỏ nhất trong khoảng thời gian khảo sát.

### Lời giải 21–23 *(đúng 3 bước "lối tắt": tìm nghiệm f'=0 trong đoạn → tính f tại MỌI điểm gồm 2 đầu mút + nghiệm → so sánh)*

**21.**
- B1: $y'=3x^2-3=0\Leftrightarrow x=\pm1$ (cả hai đều thuộc $[-2;3]$).
- B2: $y(-2)=0,\ y(-1)=4,\ y(1)=0,\ y(3)=20$.
- B3: So sánh $\{0,4,0,20\}$: $\max=20$ tại $x=3$; $\min=0$ tại $x=-2$ và $x=1$.

**22.**
- B1: $y'=\cos x-\sin x=0\Leftrightarrow x=\dfrac\pi4$ (thuộc $[0;\pi]$).
- B2: $y(0)=1,\ y\!\left(\dfrac\pi4\right)=\sqrt2,\ y(\pi)=-1$.
- B3: $\max=\sqrt2$ tại $x=\dfrac\pi4$; $\min=-1$ tại $x=\pi$.

**23.** Đây là bài **kết nối trực tiếp ý nghĩa vật lý của đạo hàm**: $v(t)=s'(t)$ (vận tốc), $a(t)=v'(t)=s''(t)$ (gia tốc).
- $v(t)=s'(t)=3t^2-12t+9$; $\ a(t)=v'(t)=6t-12$.

**a)** $a(t)=0\Leftrightarrow t=2$ (s). Khi đó $v(2)=3(4)-24+9=-3$ (m/s).
*Ý nghĩa vật lý: $v<0$ nghĩa là tại $t=2$s vật đang chuyển động theo chiều âm (đang "lùi lại").*

**b)** Coi $v(t)$ là **hàm cần tìm GTLN–GTNN trên đoạn $[0;5]$** — áp đúng thuật toán 3 bước của mục GTLN-GTNN, nhưng bây giờ hàm khảo sát là $v(t)$ chứ không phải $s(t)$:
- B1: $v'(t)=6t-12=0\Leftrightarrow t=2$ (thuộc $[0;5]$).
- B2: $v(0)=9,\ v(2)=-3,\ v(5)=24$.
- B3: $\max v = 24$ (m/s) tại $t=5$s; $\min v=-3$ (m/s) tại $t=2$s.

---

### 3.4. Tiếp tuyến tại một điểm

**Bài 24** (⭐⭐) Viết phương trình tiếp tuyến của $y=x^3-3x+1$ tại điểm có hoành độ $x_0=2$.

### Lời giải 24

- $f(2)=8-6+1=3$.
- $f'(x)=3x^2-3\Rightarrow f'(2)=12-3=9$.
- Áp công thức: $y=f'(x_0)(x-x_0)+f(x_0)$:
$$y = 9(x-2)+3 = 9x-15$$

---

### 3.5. Tiếp tuyến đi qua điểm ngoài đồ thị — SIÊU KHÓ

**Bài 25** (⭐⭐⭐⭐⭐) Cho $y=x^3-3x+2$. Viết phương trình tiếp tuyến của đồ thị, biết tiếp tuyến đi qua điểm $A(1;0)$.

### Lời giải 25 *(đúng quy trình: gọi tiếp điểm $x_0$ → viết PTTT tổng quát → thế điều kiện đi qua A → giải ra $x_0$)*

- Gọi tiếp điểm có hoành độ $x_0$. Ta có $f(x_0)=x_0^3-3x_0+2$, $f'(x_0)=3x_0^2-3$.
- PTTT tổng quát tại $x_0$: $y=f'(x_0)(x-x_0)+f(x_0)$.
- Tiếp tuyến đi qua $A(1;0)$ $\Rightarrow$ thế $x=1, y=0$ vào PTTT:
$$0 = (3x_0^2-3)(1-x_0)+x_0^3-3x_0+2$$
- Khai triển và rút gọn (đây là bước đại số "khó nuốt" nhất — làm cẩn thận từng số hạng):
$$0 = -2x_0^3+3x_0^2-1 \ \Longleftrightarrow\ 2x_0^3-3x_0^2+1=0$$
- Nhẩm nghiệm $x_0=1$ thỏa mãn $\Rightarrow$ phân tích nhân tử: $2x_0^3-3x_0^2+1=(x_0-1)^2(2x_0+1)$.
- Vậy $x_0=1$ (nghiệm kép) hoặc $x_0=-\dfrac12$.

**Với $x_0=1$:** $f(1)=0,\ f'(1)=0$. PTTT: $y=0$.

**Với $x_0=-\dfrac12$:** $f\!\left(-\dfrac12\right)=\dfrac{27}{8},\ f'\!\left(-\dfrac12\right)=-\dfrac94$.
$$y = -\frac94\left(x+\frac12\right)+\frac{27}{8} = -\frac94x+\frac94$$

**Kết luận:** Có **hai** tiếp tuyến qua $A(1;0)$: $y=0$ và $y=-\dfrac94x+\dfrac94$.
*(Bài học quan trọng: một điểm — kể cả điểm nằm trên đồ thị — vẫn có thể là giao của nhiều tiếp tuyến khác nhau. Luôn giải phương trình bậc 3 ẩn $x_0$ đầy đủ, không dừng lại ở nghiệm "hiển nhiên".)*

---

### 3.6. Cô lập tham số $m$ — mức HSG / VDC

**Bài 26** (⭐⭐⭐) Tìm $m$ để phương trình $x^3-3x-m=0$ có 3 nghiệm phân biệt.

**Bài 27** (⭐⭐⭐⭐) Tìm $m$ để bất phương trình $x^3-3x^2+m\ge 0$ đúng với mọi $x\in[0;3]$.

**Bài 28 — HSG** (⭐⭐⭐⭐⭐) Tìm $m$ để phương trình $\cos 2x-4\cos x=m$ có nghiệm.

### Lời giải 26–28 *(đúng 3 bước: cô lập m → khảo sát g(x) → đọc điều kiện từ bảng biến thiên)*

**26.**
- B1: Cô lập: $m=x^3-3x=g(x)$.
- B2: $g'(x)=3x^2-3=0\Leftrightarrow x=\pm1$. $g(-1)=2$ (cực đại), $g(1)=-2$ (cực tiểu); $g\to\mp\infty$ khi $x\to\mp\infty$.

| $x$ | $-\infty$ | $-1$ | $1$ | $+\infty$ |
|---|---|---|---|---|
| $g'$ | $+$ | $0\ -$ | $0\ +$ | |
| $g$ | $-\infty\nearrow$ | $2$ | $-2$ | $\nearrow+\infty$ |

- B3: Đường thẳng $y=m$ cắt đồ thị $g$ tại 3 điểm $\Leftrightarrow$ $m$ nằm **strictly giữa** giá trị cực tiểu và cực đại:
$$-2<m<2$$

**27.**
- B1: Cô lập: $m\ge -x^3+3x^2=g(x)$ với mọi $x\in[0;3]$ $\Leftrightarrow$ $m\ge \max_{[0;3]} g(x)$.
- B2: Khảo sát $g(x)=-x^3+3x^2$ trên $[0;3]$ bằng đúng thuật toán GTLN–GTNN (mục 3.3):
 $g'(x)=-3x^2+6x=0\Leftrightarrow x=0$ hoặc $x=2$; $g(0)=0,\ g(2)=4,\ g(3)=0$.
 $\Rightarrow \max_{[0;3]}g(x)=4$.
- B3: Kết luận: $m\ge 4$.

**28.** Đây là dạng **kết hợp đổi biến lượng giác + cô lập m** — kỹ thuật hay gặp nhất ở HSG khi phương trình có cả $\cos2x$ lẫn $\cos x$.
- Đặt $t=\cos x$, điều kiện $t\in[-1;1]$. Vì $\cos2x=2t^2-1$, phương trình trở thành:
$$2t^2-4t-1=m$$
- B1 (cô lập, biến bây giờ là $t$): $m=2t^2-4t-1=g(t),\ t\in[-1;1]$.
- B2: $g'(t)=4t-4=0\Leftrightarrow t=1$ — đúng đầu mút phải của miền. Vì hệ số $t^2$ dương (parabol quay bề lõm lên) và đỉnh rơi vào biên phải, nên $g$ **nghịch biến trên toàn bộ** $[-1;1]$:
 $g(-1)=5,\quad g(1)=-3$.
- B3: Miền giá trị của $g$ trên $[-1;1]$ là $[-3;5]$. Phương trình ban đầu có nghiệm $x$ $\Leftrightarrow$ tồn tại $t\in[-1;1]$ thỏa mãn $\Leftrightarrow$
$$-3\le m\le 5$$

---

## PHẦN 4 — Tổng hợp siêu khó (mức HSG/VDC, phối nhiều nhánh)

**Bài 29** (⭐⭐⭐⭐⭐) Tìm $m$ để hàm số $y=\dfrac13x^3-mx^2+(m+2)x-1$ đồng biến trên toàn $\mathbb R$.

**Bài 30** (⭐⭐⭐⭐⭐) Tìm GTLN, GTNN của $y=e^{x^2-4x}$ trên $[0;3]$.

### Lời giải 29 *(phối: A2 tính đạo hàm + kiến thức tam thức bậc hai không đổi dấu — mở rộng tự nhiên của nhánh "đơn điệu")*

- $y'=x^2-2mx+(m+2)$ — đây là tam thức bậc hai theo $x$, hệ số $a=1>0$.
- Để hàm **đồng biến trên $\mathbb R$**, cần $y'\ge 0$ với **mọi** $x$ (không chỉ trên một khoảng). Vì $a=1>0$ sẵn dương, điều kiện tương đương là:
$$\Delta' \le 0$$
- Tính: $\Delta' = m^2-(m+2)=m^2-m-2=(m-2)(m+1)$.
- Giải $(m-2)(m+1)\le 0 \Leftrightarrow -1\le m\le 2$.

**Kết luận:** $m\in[-1;2]$.
*(Ghi chú sư phạm: đây chính là phần mở rộng của nhánh "Đơn điệu" trong cây quyết định — khi câu hỏi là "đồng biến trên toàn $\mathbb R$" thay vì "tìm khoảng đồng biến", ta không lập bảng xét dấu nữa mà chuyển thẳng sang điều kiện $\Delta\le 0$ vì đó là cách duy nhất một parabol quay lên không bao giờ âm.)*

### Lời giải 30 *(phối: A2 chain rule để tính đạo hàm + A3 thuật toán GTLN-GTNN 3 bước)*

- B1 (tính đạo hàm bằng khuôn hàm hợp $(e^u)'=e^u\cdot u'$, với $u=x^2-4x,\ u'=2x-4$):
$$y' = (2x-4)e^{x^2-4x}$$
 $y'=0 \Leftrightarrow x=2$ (thuộc $[0;3]$), vì $e^{x^2-4x}>0$ luôn.
- B2: Tính $y$ tại 2 đầu mút và nghiệm:
 $y(0)=e^0=1$
 $y(2)=e^{-4}\approx 0{,}0183$
 $y(3)=e^{-3}\approx 0{,}0498$
- B3: So sánh $\{1;\ e^{-4};\ e^{-3}\}$:
$$\max_{[0;3]}y = 1 \text{ tại } x=0,\qquad \min_{[0;3]}y = e^{-4} \text{ tại } x=2$$

---

## BẢNG TRA CỨU NHANH — nhận diện dạng bài → thuật toán dùng

| Dấu hiệu trong đề | Dùng mục | Việc phải làm |
|---|---|---|
| "Tính đạo hàm của..." biểu thức đơn giản | A1 | Tra bảng + quy tắc tổng/tích/thương |
| Trong biểu thức có "hàm trong hàm" ($\sin(...), e^{(...)}$...) | A2 | Bóc lớp ngoài → nhân $u'$, lặp lại |
| "khoảng đồng biến / nghịch biến" | A3 – đơn điệu | TXĐ → $f'$ → bảng dấu |
| "đồng biến/nghịch biến trên $\mathbb R$" có tham số | A3 mở rộng | Đưa về điều kiện $\Delta\le 0$ (hoặc $\ge0$) của $f'$ |
| "cực đại, cực tiểu", "điểm cực trị" | A3 – cực trị | $f'=0$, xét đổi dấu hoặc dùng $f''$ |
| "GTLN, GTNN trên đoạn $[a;b]$" | A3 – GTLN-GTNN | $f'=0$ trong đoạn → tính $f$ tại mọi điểm → so sánh |
| "phương trình tiếp tuyến tại điểm..." | A3 – tiếp tuyến tại điểm | $y=f'(x_0)(x-x_0)+f(x_0)$ |
| "tiếp tuyến đi qua điểm A" / "có hệ số góc k" | A3 – tiếp tuyến qua điểm | Gọi $x_0$, viết PTTT tổng quát, thế điều kiện, giải PT ẩn $x_0$ |
| "tìm m để PT/BPT có nghiệm / có k nghiệm / đúng $\forall x$" | A3 – cô lập m | Cô lập $m=g(x)$, khảo sát $g$, đọc điều kiện từ bảng biến thiên |
| Vật lý: "quãng đường s(t)", "tìm vận tốc/gia tốc" | Ý nghĩa đạo hàm + A2/A3 | $v=s'(t)$, $a=v'(t)$, rồi áp GTLN-GTNN hoặc đơn điệu lên $v(t)$ hoặc $s(t)$ |

**Gợi ý luyện tiếp:** khi đã nhuần nhuyễn 30 bài này, hãy thử tự chế bài mới bằng cách **đổi hàm số** trong mỗi lời giải trên (giữ nguyên dạng $x^3+...$, $\sin(...)$, $e^{(...)}$...) — vì thuật toán không đổi, chỉ số liệu đổi, đó chính là cách "làm chủ lý thuyết" thật sự.
