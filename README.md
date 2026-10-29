# Phòng Thí Nghiệm Sắc Ký Sắc Tố Lá Cây (Virtual Plant Pigment Chromatography Lab)

Trang web mô phỏng thực hành thí nghiệm tách chiết hệ sắc tố quang hợp lá cây bằng phương pháp sắc ký giấy (Paper Chromatography), tích hợp bộ câu hỏi trắc nghiệm tương tác Sinh học 11, máy tính hệ số lưu giữ $R_f$ và biểu mẫu xuất báo cáo thu hoạch thực hành chuẩn học sinh/sinh viên.

Giao diện được thiết kế theo phong cách thực vật học thiên nhiên (Botanical Science) tinh tế và bảng ý tưởng Pinterest trực quan.

---

## 🌟 Các Tính Năng Nổi Bật

1. **Phòng Thí Nghiệm Ảo (Interactive Virtual Lab - 6 Bước Chuẩn):**
   - **Bước 1:** Chọn mẫu lá (*Rau bina, Khoai lang, Tía tô, Lá vàng mùa thu*) & Cắt nhỏ phiến lá bằng kéo.
   - **Bước 2:** Nghiền mẫu trong cối sứ với cát thạch anh $SiO_2$ (tạo ma sát phá màng tế bào) và dung môi Cồn 90°.
   - **Bước 3:** Lọc dịch chiết qua phễu lọc thu dung dịch sắc tố tinh khiết không cặn.
   - **Bước 4:** Kẻ vạch xuất phát chì cách mép 1.5 cm & Dùng ống mao quản chấm vết nhỏ (chấm đè 3 lần để vết đậm đặc).
   - **Bước 5:** Thiết lập bình sắc ký kín bão hòa dung môi (Ete dầu hỏa : Axeton 9:1), mực dung môi thấp hơn vạch mẫu.
   - **Bước 6:** Chạy sắc ký thời gian thực (Real-time Run) với hoạt ảnh phân tách 4 dải màu rõ rệt:
     - 🟧 **Caroten (β-Caroten):** Màu vàng cam ($R_f \approx 0.95$)
     - 🟨 **Xanthophyl:** Màu vàng chanh ($R_f \approx 0.75$)
     - 🟩 **Diệp lục a (Chlorophyll a):** Màu xanh lam/ngọc ($R_f \approx 0.65$)
     - 🟨🟩 **Diệp lục b (Chlorophyll b):** Màu xanh vàng/lục non ($R_f \approx 0.45$)
   - **Thước đo milimet ảo (Virtual Caliper):** Tự do kéo đo khoảng cách từ vạch xuất phát đến từng vết sắc tố và tính $R_f = \frac{d_{\text{chất}}}{d_{\text{dung môi}}}$.

2. **Bảng Khám Phá Kiến Thức (Pinterest-Style Botanical Board):**
   - Bộ sưu tập thẻ bài viết, hình ảnh thực tế phòng lab độ phân giải cao và bảng đối chiếu hóa sinh 4 sắc tố quang hợp.
   - Cơ chế quang hợp, quang phổ hấp thụ ánh sáng ($\lambda = 430\text{nm}, 662\text{nm}$), câu chuyện lá đổi màu mùa thu.

3. **Đấu Trường Trắc Nghiệm Tương Tác (Interactive Quiz):**
   - 12 câu hỏi trắc nghiệm Sinh học chất lượng cao bám sát đề thi THPT & Đại học.
   - Phản hồi Đúng/Sai tức thì kèm lời giải thích khoa học cặn kẽ cho từng đáp án.
   - Hệ thống tính điểm, độ chính xác và hiệu ứng chúc mừng (Confetti).

4. **Máy Tính Hệ Số $R_f$ & Phòng Luyện Tập:**
   - Kéo thanh trượt khoảng cách $d_{\text{dung môi}}$ và $d_{\text{chất}}$ để tự động tính $R_f$ và nhận diện sắc tố tương ứng.
   - Chế độ sinh đề bài toán thực nghiệm ngẫu nhiên để học sinh luyện tập tính nhanh.

5. **Sổ Báo Cáo Thu Hoạch Thực Hành (Lab Report & PDF Export):**
   - Biểu mẫu thu hoạch thực hành đầy đủ: Họ tên, Lớp, Trường, Ngày, Bảng số liệu $R_f$, Nhận xét hiện tượng và Kết luận.
   - Nút **"In / Lưu Báo Cáo (PDF)"** được định dạng chuẩn khổ giấy A4 sạch đẹp.

---

## 🚀 Hướng Dẫn Triển Khai Lên GitHub Pages (3 Cách Dễ Nhất)

### Cách 1: Tải Thư Mục `dist` Lên GitHub Pages (Nhanh nhất - Không cần cài đặt)
Thư mục `dist/` đã được build sẵn thành các file web tĩnh (`index.html`, `assets/`, `src/`):

1. Tạo một repository mới trên GitHub (ví dụ: `phong-thi-nghiem-sac-ki-la-cay`).
2. Tải toàn bộ nội dung bên trong thư mục **`dist/`** lên nhánh `main` (hoặc tạo nhánh `gh-pages`).
3. Vào repository trên GitHub > **Settings** > **Pages**.
4. Tại mục **Branch**, chọn `main` (hoặc `gh-pages`), thư mục `/ (root)` > Bấm **Save**.
5. Sau 1-2 phút, trang web của bạn sẽ hoạt động tại địa chỉ:
   `https://<tên-tài-khoản-github>.github.io/<tên-repo>/`

---

### Cách 2: Triển Khai Bằng GitHub Actions (Tự động build mã nguồn)
Nếu bạn đẩy toàn bộ mã nguồn của dự án lên GitHub:

1. Đẩy toàn bộ mã nguồn lên nhánh `main`.
2. Tạo file `.github/workflows/deploy.yml` với nội dung:
```yaml
name: Deploy to GitHub Pages

on:
  push:
    branches: [ main ]

jobs:
  build-and-deploy:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4

      - name: Setup Node.js
        uses: actions/setup-node@v4
        with:
          node-version: 20

      - name: Install Dependencies
        run: npm ci

      - name: Build Project
        run: npm run build

      - name: Deploy to GitHub Pages
        uses: peaceiris/actions-gh-pages@v4
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
          publish_dir: ./dist
```
3. GitHub sẽ tự động build và xuất bản trang web mỗi khi bạn cập nhật code!

---

### Cách 3: Chạy Trên Máy Cục Bộ (Local Development)

Yêu cầu: Đã cài đặt [Node.js](https://nodejs.org/) (phiên bản 18+ hoặc 20+).

```bash
# 1. Cài đặt các thư viện phụ thuộc
npm install

# 2. Khởi động máy chủ phát triển
npm run dev

# Mở trình duyệt tại: http://localhost:3000
```

Để đóng gói thành file tĩnh hoàn chỉnh:
```bash
npm run build
# Kết quả xuất ra thư mục dist/
```

---

## 📁 Cấu Trúc Mã Nguồn

```
├── index.html                  # File HTML chính với font thực vật học và thẻ meta SEO
├── package.json                # Danh sách thư viện (React 19, Vite, Tailwind CSS, Motion...)
├── vite.config.ts              # Cấu hình Vite với base relative ('./') chuẩn GitHub Pages
├── README.md                   # Hướng dẫn chi tiết dự án
├── dist/                       # THƯ MỤC WEB HOÀN CHỈNH ĐỂ XUẤT BẢN TRỰC TIẾP
│   ├── index.html              # Trang đơn đã đóng gói
│   ├── assets/                 # File JS và CSS đã nén tối ưu
│   └── src/assets/images/      # Hình ảnh độ nét cao của phòng thí nghiệm
└── src/
    ├── App.tsx                 # Điều hướng ứng dụng và quản lý phiên thí nghiệm
    ├── main.tsx                # Điểm khởi chạy React DOM
    ├── index.css               # Định kiểu Tailwind v4 và font chữ botanical
    ├── types/
    │   └── chromatography.ts   # Khai báo TypeScript cho sắc tố, mẫu lá và bài tập
    ├── data/
    │   └── chromatographyData.ts # Dữ liệu khoa học chuẩn (Rf, phổ hấp thụ, 12 câu hỏi)
    └── components/
        ├── Header.tsx          # Thanh điều hướng Top Bar chuẩn thiết kế
        ├── HeroBanner.tsx      # Banner giới thiệu phong cách thiên nhiên
        ├── VirtualLab.tsx      # Buồng thí nghiệm ảo 6 bước & đo Rf tương tác
        ├── KnowledgeBoard.tsx  # Bảng kiến thức Pinterest & bảng tra cứu sắc tố
        ├── QuizArena.tsx       # Đấu trường 12 câu trắc nghiệm tương tác
        ├── RfCalculator.tsx    # Máy tính Rf & bài tập tính nhanh
        ├── LabReportTab.tsx    # Biểu mẫu báo cáo thu hoạch xuất PDF
        └── Footer.tsx          # Chân trang & nguồn tài liệu tham khảo
```

---

## 🔬 Cơ Sở Khoa Học & Công Thức Tính

### 1. Hệ sắc tố quang hợp:
- **Diệp lục (Chlorophyll):**
  - Diệp lục a ($C_{55}H_{72}O_5N_4Mg$): Màu xanh lam ngọc, hấp thụ đỉnh $430\text{ nm}$ & $662\text{ nm}$.
  - Diệp lục b ($C_{55}H_{70}O_6N_4Mg$): Màu xanh vàng, hấp thụ đỉnh $453\text{ nm}$ & $642\text{ nm}$. Nhóm $-CHO$ phân cực tạo liên kết hydro mạnh với cellulose của giấy nên di chuyển chậm nhất.
- **Carotenoid:**
  - Caroten ($\beta$-Caroten, $C_{40}H_{56}$): Màu vàng cam, không phân cực, tan cực tốt trong pha động hữu cơ nên di chuyển nhanh nhất.
  - Xanthophyl ($C_{40}H_{56}O_2$): Màu vàng chanh, chứa oxy nên phân cực hơn carotens.

### 2. Công thức tính hệ số lưu giữ $R_f$:
$$R_f = \frac{d_{\text{chất}}}{d_{\text{dung môi}}}$$
*(Trong đó $0 \le R_f \le 1$, $d_{\text{chất}}$ là khoảng cách từ vạch xuất phát đến tâm vết sắc tố, $d_{\text{dung môi}}$ là khoảng cách đến vạch ngấn dung môi).*

---

*Chúc các bạn có những trải nghiệm thực hành sinh học trực quan và thú vị!*
