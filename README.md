# Playground-Cypress
Automation using Cypress

### Panduan

- Langkah-langkah untuk mengubungkan GitHub dengan Local drive :
    1. Buat repository baru di GitHub,
    2. Jangan lupa Add Readme file,
    3. Clone GitHub di Visual studio code,
    4. Run git clone <Link GitHub>
    5. Open folder,
    6. Cek status : git status
    7. Cek apakah sudah berhasil terhubung antara GitHub dengan Local drive : git remote -v
    8. Jika mempunyai 2 akun GitHub di laptop, maka lakukan
        - git config --list
        - cek user.name dan user.email
        - tekan q untuk keluar dari tampilan
        - jika ingin menggant Githubnya, maka lakukan
            - git config user.name <username GitHub)
            -git config user.email <user email>
        - Cek kembali : git config --list
            - enter2 sampai END dan cek apakah sudah benar username dan emailnya
            - tekan q untuk keluar dari tampilan
    9. Cek ada di branch mana : git branch,
    10. Edit README.md,
    11. Click save,
    12. Cek status : git status,
    13. Tambahkan ke staging area : git add README.md
    14. Atau untuk menambahkan semua file : git add .
    15. Kalau mau unstaging : git restore --staged <file>
    16. Kalau mau commit : git commit -m "messagenya apa",
    17. Publish ke GitHub : Git Push
