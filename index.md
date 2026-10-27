---
layout: default
title: Beranda
---

<div class="hero">
  <h1>Selamat Datang di KOPMA</h1>
  <p>Koperasi Mahasiswa yang berdedikasi membangun kemandirian ekonomi, menumbuhkan jiwa wirausaha, dan melayani kebutuhan seluruh civitas akademika.</p>
  <div class="hero-actions">
    <a href="/gabung.html" class="btn btn-accent">Daftar Jadi Anggota</a>
    <a href="/layanan.html" class="btn-secondary">Lihat Layanan Kami</a>
  </div>
</div>

<h2 class="section-title">Layanan & Unit Usaha Kami</h2>

<div class="grid-cards">
  <div class="card">
    <div class="card-icon">🛒</div>
    <h3>Kopma Mart</h3>
    <p>Menyediakan kebutuhan harian mahasiswa, alat tulis kantor (ATK), snack, minuman, dan perlengkapan kuliah dengan harga terjangkau.</p>
  </div>
  
  <div class="card">
    <div class="card-icon">🖨️</div>
    <h3>Jasa Cetak & Fotokopi</h3>
    <p>Layanan cetak dokumen tugas akhir, fotokopi kilat, jilid skripsi, dan scan berkas dengan kualitas tajam dan cepat.</p>
  </div>
  
  <div class="card">
    <div class="card-icon">☕</div>
    <h3>Kopma Corner & Kafe</h3>
    <p>Tempat santai untuk berdiskusi, belajar kelompok, atau sekadar menikmati kopi dan camilan di lingkungan kampus.</p>
  </div>
  
  <div class="card">
    <div class="card-icon">👕</div>
    <h3>Merchandise & Konveksi</h3>
    <p>Pembuatan PDH, kaos kepanitiaan, jaket angkatan, lanyard, dan pernak-pernik kampus dengan harga khusus mahasiswa.</p>
  </div>
</div>

<h2 class="section-title">Berita & Informasi Terbaru</h2>

<div class="grid-cards">
  {% for post in site.posts limit:3 %}
    <div class="card">
      <div class="post-meta">{{ post.date | date: "%d %B %Y" }}</div>
      <h3 style="margin-top: 0.5rem;"><a href="{{ post.url | relative_url }}" style="text-decoration: none; color: inherit;">{{ post.title }}</a></h3>
      <p>{{ post.excerpt | strip_html | truncate: 120 }}</p>
      <a href="{{ post.url | relative_url }}" style="color: var(--primary); font-weight: 600; text-decoration: none; display: inline-block; margin-top: 0.8rem;">Baca Selengkapnya &rarr;</a>
    </div>
  {% else %}
    <p>Belum ada artikel terbaru.</p>
  {% endfor %}
</div>

<div class="content-box" style="text-align: center; background: #e8f5e9; border-color: #c8e6c9;">
  <h2 style="margin-top: 0; color: #155724;">Mari Bergabung Bersama Kami!</h2>
  <p style="color: #2e7d32; max-width: 650px; margin: 0 auto 1.2rem auto;">
    Dapatkan Sisa Hasil Usaha (SHU) tahunan, diskon belanja anggota di semua unit usaha, serta pelatihan kepemimpinan dan kewirausahaan.
  </p>
  <a href="/gabung.html" class="btn">Gabung Menjadi Anggota Sekarang</a>
</div>
