# My CV - LaTeX

## Hướng dẫn build

### 1. Cài đặt các package cần thiết
Bạn cần cài đặt các package sau (trên Ubuntu/Debian):

```bash
sudo apt update
sudo apt install texlive-xetex texlive-latex-extra texlive-fonts-recommended latexmk fonts-font-awesome
```

Nếu muốn đầy đủ nhất, có thể cài:
```bash
sudo apt install texlive-full
```

### 2. Build file PDF

```bash
cd resume
latexmk -xelatex main.tex
```

Sau khi chạy xong, file `main.pdf` sẽ xuất hiện trong thư mục `resume/`.

## Ghi chú
- Nếu bạn muốn build thủ công, có thể dùng lệnh:
  ```bash
  xelatex main.tex
  ```
  (chạy 2-3 lần để cập nhật cross-reference)
- Nếu muốn build bằng Docker, hãy yêu cầu để được cung cấp file cấu hình. 