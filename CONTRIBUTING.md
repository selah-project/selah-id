# Berkontribusi pada Edisi Indonesia Selah

Terima kasih telah membantu edisi ini menjadi lebih akurat, lebih
jernih, dan lebih wajar. Anda tidak harus ahli: jelaskan apa yang
Anda amati, berikan dasar yang Anda punya, dan bedakan keyakinan
dari usulan.

## Melaporkan masalah atau meminta perbaikan

- Bukalah **issue** bila bacaan itu perlu didiskusikan, ada
  beberapa pilihan, atau Anda tidak yakin bagaimana rekaman
  penyelarasan harus diubah.
- Bukalah **pull request** bila kekeliruan dan penggantinya
  sudah jelas.
- Untuk bug aplikasi, atau soal keamanan/akun/privasi, gunakan
  [dukungan Selah](https://selahproject.com/support).

## Yang perlu disertakan

Kitab, pasal, ayat, token Ibrani terkait; teks saat ini; teks
usulan; alasan perubahan; dan dasar leksikal, gramatikal,
kontekstual, atau terbitan yang menopangnya. Sebutkan juga apakah
Anda penutur asli bahasa Indonesia dan apakah Anda membaca bahasa
Ibrani secara langsung.

## Cara mengubah rekaman

Berkas berada di `<kitab>/<pasal>/<ayat>.json`.

- Ubahlah `translation` dan `gloss` token terkait bersama-sama
  bila keduanya terdampak.
- Pertahankan `book`, `chapter`, `verse`, `ref`, nilai `surface`
  Ibrani, serta urutan dan jumlah token — kecuali Anda melaporkan
  cacat penyelarasan.
- Jangan mengubah bidang asal (model, tier, tanggal) agar
  perbaikan tampak seperti pembuatan baru.
- Pertahankan konvensi kurung siku, nama-nama Ilahi, dan `⟨את⟩`.
- Hindari perubahan format belaka yang tak berhubungan.

Periksalah JSON yang Anda ubah:

```bash
python3 -m json.tool genesis/1/1.json >/dev/null
```

Bahasa Ibrani lebih dahulu. Bila dua bacaan sama-sama dapat
dibela, jelaskan perbedaannya — jangan menyodorkan selera sebagai
kepastian. Jangan menyalin terjemahan modern yang berhak cipta.

## Pekerjaan berbantuan AI

Nyatakan penggunaan model bahasa atau terjemahan mesin yang
substansial — beserta tinjauan manusia yang Anda lakukan. Jangan
kirim penulisan-ulang massal tanpa tinjauan. Kontributor
bertanggung jawab atas setiap kata yang diusulkannya.

## Lisensi, atribusi, dan tinjauan

Dengan berkontribusi Anda menyatakan berhak melakukannya dan
setuju bahwa bahan yang dimasukkan dibagikan di bawah
[CC BY-SA 4.0](LICENSE.md). Riwayat Git memelihara catatan publik
dan atribusi. Tim pemelihara menimbang usulan terhadap bahasa
Ibrani, konvensi, sumber, dan penyelarasan — dapat menerima,
memoles bersama, menunggu dasar lebih banyak, atau menolak dengan
alasan. Kritiklah bacaan, bukan orangnya.
