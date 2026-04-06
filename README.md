# Clinic Management

Du an mau quan ly phong kham gom:

- `client`: ReactJS + TypeScript + Redux + React Router + Axios + Bootstrap
- `server`: Python FastAPI + SQLAlchemy

## Chuc nang da scaffold

- Dang nhap bang username/password
- Dang nhap mo phong Google/Facebook de demo giao dien va luong API
- Quan ly benh nhan
- Quan ly bac si
- Dang ky lich kham
- Phan cong bac si theo chuyen khoa va trang thai ranh
- Cap nhat ket qua kham
- Tong hop ho so benh an theo benh nhan
- Tong hop lich su kham theo bac si
- Thong ke lich su kham theo khoang thoi gian

## Chay backend

```bash
cd server
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
uvicorn app.main:app --reload
```

Tai khoan mac dinh:

- Username: `admin`
- Password: `admin123`

## Ghi chu ky thuat

- Backend dang dung SQLite file va luu tai `C:\Users\lanph\OneDrive\Tài liệu\Playground\server\clinic.db`. Ban co the mo file nay bang DB Browser for SQLite sau khi chay server it nhat mot lan. Khi trien khai that, nhom co the doi `DATABASE_URL` trong `server/app/database.py` sang MySQL hoac SQL Server.
- OAuth Google/Facebook hien la mock flow de dap ung yeu cau demo login. Khi lam do an chinh thuc, nhom nen thay bang OAuth2 that voi client id/client secret.
