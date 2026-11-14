# NotchRP — rilis & feed pembaruan

Repo ini **hanya menyimpan aset rilis**. Kode sumber NotchRP tidak ada di sini.

NotchRP adalah overlay *Dynamic Island* untuk GTA San Andreas (SA-MP 0.3.DL):
playtime, ledger uang, statistik job, terjemahan chat, dan lirik musik, tanpa
pernah merebut fokus dari game.

## Unduh

| Cara | Berkas | Ukuran |
|---|---|---|
| Launcher (dianjurkan) | [`NotchRP-launcher.zip`](../../releases/latest/download/NotchRP-launcher.zip) | ±0,1 MB |
| Installer offline | [`NotchRP-Setup.exe`](../../releases/latest/download/NotchRP-Setup.exe) | ±86 MB |

`NotchRP-launcher.zip` diekstrak ke folder GTA San Andreas (folder yang sama
dengan `gta_sa.exe`), lalu jalankan `NotchRP Launcher.exe`. Aplikasi lengkapnya
diunduh sekali dan setelah itu memperbarui dirinya sendiri.

## Feed pembaruan

Aplikasi dan launcher membaca rilis terbaru dari URL tetap:

```
https://github.com/aryaawcksn/NotchRP/releases/latest/download/
```

Karena itu setiap rilis wajib membawa aset dengan nama **persis** seperti ini:

```
latest.yml                          manifest electron-updater
launcher.json                       manifest launcher (unduh pertama)
NotchRP-<versi>-setup.exe           installer
NotchRP-<versi>-setup.exe.blockmap  delta update
NotchRP-<versi>-launcher.zip        launcher + NotchChat.asi untuk folder GTA
NotchRP-Setup.exe                   alias stabil untuk link unduh
NotchRP-launcher.zip                alias stabil untuk link unduh
```

Jangan menandai rilis sebagai *prerelease*: `latest/download/` akan
melewatinya dan updater akan melihat rilis stabil sebelumnya.

## Kebutuhan

Windows 10/11 64-bit, GTA San Andreas v1.0 US dengan SA-MP 0.3.DL, dan koneksi
internet untuk update otomatis.

---

Bukan produk resmi Rockstar Games. GTA San Andreas adalah merek dagang
Rockstar Games; repo ini tidak berisi aset game apa pun.
