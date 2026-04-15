[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=23574203&assignment_repo_type=AssignmentRepo)
# Day 10 Lab: Data Pipeline & Data Observability

**Student Email:** theanha2hvtls@gmail.com
**Name:** Nguyễn Thế Anh
---

## Mo ta

Bai lab day 10 yeu cau xay dung mot ETL pipeline don gian cho du lieu san pham.
Minh da lam cac buoc: extract du lieu tu file JSON, validate record loi, transform them cot discounted_price va processed_at, va load ra file CSV.
Ngoai ra, minh cung tao mot file garbage_data.csv de test agent voi data khong hop le va kiem tra cach agent xu ly loi.

---

## Cach chay (How to Run)

### Prerequisites
```bash
pip install pandas
```

### Chay ETL Pipeline
```bash
python solution.py
```

### Chay Agent Simulation (Stress Test)
```bash
python agent_simulation.py
```

---

## Cau truc thu muc

```
├── solution.py              # ETL Pipeline script
├── processed_data.csv       # Output cua pipeline
├── experiment_report.md     # Bao cao thi nghiem
└── README.md                # File nay
```

---

## Ket qua

- ETL pipeline chay duoc voi JSON input va luu file `processed_data.csv`.
- Data validation loai bo record co `price <= 0` hoac `category` rong.
- Transform da them `discounted_price` (giam 10%), chuan hoa `category` thanh Title Case, va them `processed_at`.
- File `garbage_data.csv` da duoc tao de test agent voi du lieu khong hop le.
- Agent simulation co the so sanh `processed_data.csv` (clean data) va `garbage_data.csv` (garbage data).
