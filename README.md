# Simple_Sales_Automation
Sistem ini menggunakan n8n sebagai alat otomatisasi untuk mengambil data dari Google Sheets dan memasukkannya ke dalam database PostgreSQL di Neon.tech. Data tersebut kemudian dihubungkan ke Google Looker Studio untuk menghasilkan dashboard analitik.

# Teknologi yang Digunakan
1. n8n: Untuk otomatisasi alur kerja (workflow).
2. Google Sheets: Sebagai sumber data input.
3. Neon.tech: Database PostgreSQL berbasis cloud untuk penyimpanan data.
4. Google Looker Studio: Untuk visualisasi data dan pembuatan dashboard.

# Alur Kerja Sistem
1. Data transaksi diinput melalui Google Sheets.
2. Node Schedule Trigger di n8n menjalankan proses secara berkala.
3. Node Google Sheets mengambil baris data terbaru.
4. Node Postgres memasukkan data tersebut ke database Neon.
5. Dashboard di Looker Studio memperbarui grafik secara otomatis.

# Cara Penggunaan
1. Unduh file sales-automation-workflow.json yang ada di folder ini.
2. Import file tersebut ke dalam instance n8n kamu.
3. Konfigurasikan kredensial Google Sheets dan PostgreSQL kamu di n8n.
4. Jalankan workflow dan hubungkan database ke Looker Studio.
