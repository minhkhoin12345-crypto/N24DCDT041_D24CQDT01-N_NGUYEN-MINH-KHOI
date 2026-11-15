# Thap Ha Noi

## 1. Gioi thieu

Chuong trinh thuc hien hai chuc nang:

1. Giai bai toan Thap Ha Noi bang de quy.
2. Kiem tra mot day chuyen dia co hop le theo luat Thap Ha Noi hay khong.

Quy uoc coc:
- 1 = A
- 2 = B
- 3 = C

## 2. Moi truong

- Ngon ngu: C++
- Tuong thich C++98
- Co the bien dich bang Dev-C++, TDM-GCC hoac GCC.

## 3. Bien dich

Neu su dung g++:

```bash
g++ main.cpp -o main.exe
```

Chay:

```bash
main.exe
```

## 4. Mode 1 - Giai Thap Ha Noi

Cu phap:

```text
1
n
```

Vi du n = 3:

```text
1
3
```

Ket qua mong doi:

```text
So buoc: 7
```

Cong thuc so buoc toi thieu:

```text
2^n - 1
```

Mot so truong hop:
- n = 0 -> 0 nuoc
- n = 1 -> 1 nuoc
- n = 2 -> 3 nuoc
- n = 3 -> 7 nuoc
- n = 5 -> 31 nuoc

Chuong trinh hien thi tung nuoc chuyen va trang thai cua ba coc sau moi nuoc.

## 5. Mode 2 - Kiem tra day chuyen dia

Cu phap:

```text
2
n m
from to
from to
...
```

Trong do:
- n: so dia
- m: so nuoc chuyen
- from: coc nguon
- to: coc dich

Vi du day hop le voi n = 2:

```text
2
2 3
1 2
1 3
2 3
```

Ket qua:

```text
Ket qua: ACCEPT
Ly do: Hop le: tat ca dia da o coc C dung thu tu
```

## 6. Cac luat duoc kiem tra

Validator kiem tra:
- Khong duoc lay dia tu coc rong.
- Chi duoc chuyen dia tren cung.
- Khong duoc dat dia lon len dia nho.
- Khong duoc chuyen mot coc sang chinh no.
- Sau khi ket thuc, tat ca dia phai nam tren coc C dung thu tu.
- Truong hop n = 0 phai co 0 nuoc chuyen.

## 7. Bo kiem thu - it nhat 12 ca

| ID | Noi dung | Expected |
|---|---|---|
| TC01 | Giai voi n = 0 | 0 nuoc |
| TC02 | Giai voi n = 1 | 1 nuoc |
| TC03 | Giai voi n = 2 | 3 nuoc |
| TC04 | Giai voi n = 3 | 7 nuoc |
| TC05 | Giai voi n = 5 | 31 nuoc |
| TC06 | Day chuyen hop le voi n = 2 | ACCEPT |
| TC07 | Dat dia lon len dia nho | REJECT |
| TC08 | Chuyen tu coc rong | REJECT |
| TC09 | Chua chuyen het dia sang C | REJECT |
| TC10 | n = 0 nhung co nuoc | REJECT |
| TC11 | Chuyen A -> A | REJECT |
| TC12 | Day chuyen khong hop le | REJECT |

## 8. Input mau

### TC01

```text
1
0
```

Expected: `So buoc: 0`

### TC02

```text
1
1
```

Expected: `So buoc: 1`

### TC03

```text
1
2
```

Expected: `So buoc: 3`

### TC04

```text
1
3
```

Expected: `So buoc: 7`

### TC05

```text
1
5
```

Expected: `So buoc: 31`

### TC06

```text
2
2 3
1 2
1 3
2 3
```

Expected: `ACCEPT`

### TC07

```text
2
2 3
1 2
1 2
2 3
```

Expected: `REJECT`

### TC08

```text
2
2 3
2 3
1 2
1 3
```

Expected: `REJECT`

### TC09

```text
2
2 1
1 2
```

Expected: `REJECT`

### TC10

```text
2
0 1
1 2
```

Expected: `REJECT`

### TC11

```text
2
2 3
1 1
1 3
2 3
```

Expected: `REJECT`

### TC12

```text
2
2 3
2 3
1 3
1 2
```

Expected: `REJECT`

## 9. Chay lai sau khi clone repository

Clone repository:

```bash
git clone <LINK_REPOSITORY>
```

Di chuyen vao thu muc:

```bash
cd <TEN_REPOSITORY>
```

Kiem tra SHA:

```bash
git rev-parse HEAD
```

Hoac:

```bash
git log --oneline -1
```

Bien dich:

```bash
g++ main.cpp -o main.exe
```

Chay:

```bash
main.exe
```

Thu lai mot ca, vi du:

```text
1
3
```

Kiem tra ket qua:

```text
So buoc: 7
```

## 10. Cau truc repository de xuat

```text
ThapHaNoi/
├── main.cpp
├── README.md
└── docs/
    └── anh_ket_qua/
        ├── A01.png
        ├── A02.png
        ├── A03.png
        ├── A04.png
        ├── A05.png
        ├── A06.png
        ├── A07.png
        ├── A08.png
        ├── A09.png
        ├── A10.png
        └── A11.png
```

## 11. Ket luan

Chuong trinh su dung de quy de giai bai toan Thap Ha Noi va co them validator de kiem tra tinh hop le cua day chuyen dia.

Bo kiem thu gom it nhat 12 ca doc lap, bao gom truong hop bien, truong hop hop le va cac truong hop vi pham luat chuyen dia.
