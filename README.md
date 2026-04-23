ZMK Lily58 untuk Super Mini / Promicro Wireless NRF52840.

[ZMK STUDIO](https://zmk.studio/)
Ada update baru ZMK Studio remapping tanpa perlu di flash 

[Full Dokumentasi ZMK](https://zmk.dev/docs)


Tools :
[ZMK Keymap Editor](https://nickcoutsos.github.io/keymap-editor/)
Video fork repository :
[Tutorial Mapping ZMK](https://youtu.be/cAi5pnkz48M)

<img width="3827" height="2705" alt="Image" src="https://github.com/user-attachments/assets/fa0b5a4a-d71e-4bee-a56c-bf8bce3d2299" />


Untuk Variant ini cukup plug Dongle ke USB Port di device anda.


Prosedur Reset Keyboard Split
Lakukan langkah-langkah berikut untuk mereset semua bagian keyboard split Anda:
- Masukkan setiap bagian keyboard split ke mode bootloader. Dengan cara tekan 2x tombol reset saat USB terhubung akan muncul drive baru, untuk flash nya cukup drag & drop di disk bootloader
- Flash salah satu bagian keyboard dengan firmware reset pengaturan setting_reset.uf2.
- Ulangi langkah 2 pada bagian lainnya dari keyboard split.
- Flash image firmware yang sebenarnya untuk setiap bagian keyboard split (misalnya my_board_left.uf2 untuk bagian kiri, my_board_right.uf2 untuk bagian kanan).
- Jika central dan peripheral tidak saling terhubung setelah menyelesaikan langkah-langkah ini, akan membantu untuk mereset central dan peripheral pada waktu yang hampir bersamaan. Biasanya dilakukan dengan menghubungkan pin reset ke ground pada setiap mikrokontroler keyboard Anda, menekan tombol reset, atau mematikan lalu menyalakan keduanya dengan sakelar daya.
- Setelah selesai, Anda harus menghapus/lupakan keyboard dari perangkat host mana pun yang sebelumnya terpasang, lalu lakukan pairing ulang, karena informasi pairing tersebut juga telah dihapus dari keyboard.
  
