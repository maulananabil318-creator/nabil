<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Etty Taylor - Pemesanan Pakaian Kustom</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <style>
        body { font-family: Arial, sans-serif; background-color: #f8f9fa; }
        .hero { background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); color: white; padding: 50px 0; text-align: center; }
        .product-list { margin: 20px 0; }
        .product-item { border: 1px solid #ddd; padding: 15px; margin: 10px; border-radius: 8px; background: white; }
        footer { background: #343a40; color: white; text-align: center; padding: 20px; }
    </style>
</head>
<body>
    <header class="hero">
        <div class="container">
            <h1>Etty Taylor</h1>
            <p>Pakaian Kustom Berkualitas Tinggi - Pesan Sekarang!</p>
            <p>Hubungi kami: <strong>081350393651</strong></p>
        </div>
    </header>

    <main class="container my-5">
        <section id="products">
            <h2>Jenis Pakaian yang Bisa Dipesan</h2>
            <p>Kami membuat berbagai jenis pakaian kecuali jaket dan jeans. Pilih dan pesan sesuai kebutuhan Anda.</p>
            <div class="row product-list">
                <div class="col-md-4 product-item">
                    <h4>Baju</h4>
                    <p>Baju kasual atau formal dengan bahan pilihan.</p>
                </div>
                <div class="col-md-4 product-item">
                    <h4>Kemeja</h4>
                    <p>Kemeja pria/wanita dengan desain eksklusif.</p>
                </div>
                <div class="col-md-4 product-item">
                    <h4>Gaun</h4>
                    <p>Gaun pesta atau sehari-hari yang elegan.</p>
                </div>
                <div class="col-md-4 product-item">
                    <h4>Celana Panjang (Non-Jeans)</h4>
                    <p>Celana formal atau santai dari bahan katun/wol.</p>
                </div>
                <div class="col-md-4 product-item">
                    <h4>Rok</h4>
                    <p>Rok mini, midi, atau maxi dengan variasi panjang.</p>
                </div>
                <div class="col-md-4 product-item">
                    <h4>Blouse</h4>
                    <p>Blouse wanita dengan detail bordir.</p>
                </div>
            </div>
        </section>

        <section id="order" class="my-5">
            <h2>Pesan Sekarang</h2>
            <form id="orderForm">
                <div class="mb-3">
                    <label for="name" class="form-label">Nama Anda</label>
                    <input type="text" class="form-control" id="name" required>
                </div>
                <div class="mb-3">
                    <label for="product" class="form-label">Jenis Pakaian</label>
                    <select class="form-control" id="product" required>
                        <option value="">Pilih...</option>
                        <option value="Baju">Baju</option>
                        <option value="Kemeja">Kemeja</option>
                        <option value="Gaun">Gaun</option>
                        <option value="Celana Panjang">Celana Panjang</option>
                        <option value="Rok">Rok</option>
                        <option value="Blouse">Blouse</option>
                    </select>
                </div>
                <div class="mb-3">
                    <label for="details" class="form-label">Detail Pesanan (ukuran, warna, bahan)</label>
                    <textarea class="form-control" id="details" rows="3" required></textarea>
                </div>
                <div class="mb-3">
                    <label for="phone" class="form-label">Nomor HP Anda</label>
                    <input type="tel" class="form-control" id="phone" required>
                </div>
                <button type="submit" class="btn btn-primary">Kirim Pesanan</button>
            </form>
            <p class="mt-3">Pesanan akan diproses dan konfirmasi via HP: <strong>081350393651</strong></p>
        </section>

        <section id="feedback" class="my-5">
            <h2>Kritik dan Saran</h2>
            <form id="feedbackForm">
                <div class="mb-3">
                    <label for="feedbackName" class="form-label">Nama Anda</label>
                    <input type="text" class="form-control" id="feedbackName" required>
                </div>
                <div class="mb-3">
                    <label for="feedbackMessage" class="form-label">Pesan Kritik/Saran</label>
                    <textarea class="form-control" id="feedbackMessage" rows="4" required></textarea>
                </div>
                <button type="submit" class="btn btn-secondary">Kirim</button>
            </form>
        </section>
    </main>

    <footer>
        <p>&copy; 2023 Etty Taylor. Semua hak dilindungi. Hubungi: 081350393651</p>
    </footer>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
    <script>
        // Script sederhana untuk menangani form (alert sebagai placeholder; ganti dengan backend jika perlu)
        document.getElementById('orderForm').addEventListener('submit', function(e) {
            e.preventDefault();
            alert('Pesanan Anda telah dikirim! Kami akan menghubungi via 081350393651.');
            // Di sini bisa tambahkan AJAX untuk kirim data ke server
        });

        document.getElementById('feedbackForm').addEventListener('submit', function(e) {
            e.preventDefault();
            alert('Terima kasih atas kritik dan saran Anda!');
            // Simpan lokal atau kirim ke email
        });
    </script>
</body>
</html>
