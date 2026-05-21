Chay code

1. Tao moi truong ao:

   ```powershell
   python -m venv .venv
   ```

2. Kich hoat moi truong ao:

   ```powershell
   .\.venv\Scripts\Activate.ps1
   ```

   Neu PowerShell bao loi execution policy, chay:

   ```powershell
   Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
   .\.venv\Scripts\Activate.ps1
   ```

3. Nang cap pip va cai thu vien:

   ```powershell
   python -m pip install --upgrade pip
   pip install -r requirements.txt
   ```

4. Bo cac model ca nhan vao file/folder `weights`.

5. Chay app:

   ```powershell
   streamlit run app.py
   ```

Luu y:

- Nen chay app bang lenh nay neu PowerShell khong nhan lenh `streamlit`:

  ```powershell
  python -m streamlit run app.py
  ```

- De thoat moi truong ao:

  ```powershell
  deactivate
  ```

Test app

1. Chon task: Detection / Tracking / Draw Zone.
2. Lua chon confidence.
3. Lua chon model.
4. Chon dau vao: Image / Video / Webcam.
5. Tai video/image.
6. Tai toa do count zone hoac ve zone o page "Draw Zone" neu can thiet.
