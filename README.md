smishing-detection-prototype/
│
├── data/                  # เก็บ Dataset 
│   ├── raw/               # ข้อมูลดิบที่เพิ่งโหลดหรือสแครปมา
│   └── processed/         # ข้อมูลที่ Clean แล้ว พร้อมเทรน
│
├── notebooks/             # เก็บไฟล์ Jupyter Notebook (.ipynb)
│   ├── 01_data_generation.ipynb   # โค้ดปั๊มข้อมูลด้วย LLM
│   └── 02_model_training.ipynb    # โค้ดเทรน Bi-LSTM
│
├── models/                # เก็บไฟล์โมเดลที่เทรนเสร็จแล้ว (เช่น .h5, .pkl)
│
├── src/                   # Source Code หลักของระบบ
│   ├── agentic/           # โค้ดฝั่ง Agentic AI (ต่อ API LLM)
│   ├── hybrid/            # โค้ดฝั่ง Hybrid (Bi-LSTM + Levenshtein)
│   └── dashboard/         # โค้ดหน้าเว็บ Streamlit / FastAPI
│
├── .env                   # ไฟล์เก็บ API Key (ห้ามอัปขึ้น GitHub เด็ดขาด!)
├── .gitignore             # ไฟล์บอก Git ว่าไม่ต้องจำไฟล์ไหนบ้าง
├── requirements.txt       # ไฟล์รวมรายชื่อ Library ที่ใช้ (pip freeze)
└── README.md              # หน้าปกอธิบายโปรเจกต์
