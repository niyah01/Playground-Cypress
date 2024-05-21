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

- Membuat Branch Baru :
    1. git checkout -b "branchbaru"
    2. git branch
- Pindah Branch :
    1. git checkout <nama branch>
- Cek git version :
    1. git --version
- Setiap membuat repository baru maka harus :
    1. Run : 
        - npm init
            - setelah run npm init maka akan muncul file package.json
        - npm install cypress --save-dev
            - Maka akan muncul 2 file baru yaitu :
                - (node_modules)
                - package-lock.json
    2. Buat file baru dengan nama .gitignore
    3. Pindahkan node_modules ke file .gitignore, dengan menuliskan node_modules
    4. Click save,
    5. Cek apakah git ignore sudah tidak terbaca :
        - git status
    6. Setelah node modules tidak terbaca, maka :
        - git add .
        - git commit -m "Install cypress and Add file .gitignore"
        - git push

- Open cypress via visual studio code :
    1. npx cypress open
    2. Maka terbuka dan muncul pilihan :
        - E2E Testing
        - Component Testing
        Note :
            - karena kita QA maka pilih yang e2e testing.
        - kemudian klik continue
        - kemudian pilih browser contoh : chrome
        - kemudian klik start e2e testing chrome
        - kemudian akan membuka dashboardnya cypress
        - kemudian ada 2 pilihan :
            - Scaffold example specs
            - create new spec (kalau udah bisa mau bikin file baru)
        - maka pilih Scaffold example specs
        - maka akan membuka dialog 'Great! We added the following files to your project :...'
        - kemudian klik Okay, I got it!
        - coba cek di visual studio code nya, maka akan menambahkan beberapa files, diantaranya ada e2e yg di dalam nya ada :
            - 1-getting-started
            - 2-advanced-examples
        - maka 2 files itu boleh di ignore, boleh tidak di ignore. caranya dengan :
            - klik filenya
            - klik kanan
            - klik copy relative path pada file 1-getting-started
            - paste di dalam file .gitignore bersama node_modules tadi
            - klik copy relative path pada file 2-advanced-examples
            - paste di dalam file .gitignore
            - klik save
            - maka warnanya akan menjadi abu-abu
                Note :
                Alasannya kenapa di ignore? karena tidak perlu dipush di github changes kita. Karena 2 files itu buat bahan kita belajar ajah (sekedar di baca2 saja)
    3. git add .
    4. git commit -m "Update .gitignore file"
    5. git push