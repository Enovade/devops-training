# Pemasangan & Penggunaan Git

Latihan ini adalah untuk menunjukkan langkah pemasangan & penggunaan Git

## Langkah 1.0: Pemasangan *Git Client*
Latihan ini adalah untuk pemasangan ***Git client***

### Langkah 1.1: Pemasangan *Git Client*
* Muat turun Git client dari https://git-scm.com/downloads

* Setelah siap, buka aplikasi Git CMD, dan taip kod berikut untuk melihat versi aplikasi git:

```
git --version
```

## Langkah 2.0: Konfigurasi *Git client*
Latihan ini adalah untuk konfigurasi ***Git client***

### Langkah 2.1: Wujudkan GitHub *Personal access token*
* Di ***upper-right corner*** laman GitHub, klik ke profil foto dan pilih ***Settings***, seperti paparan berikut

<img width="188" alt="image" src="https://user-images.githubusercontent.com/99636296/162892035-d4e0fa1f-21e6-41a4-9948-2e414f506603.png">

* Di menu kiri, pilih ***Developer Settings***, seperti paparan berikut

<img width="279" alt="image" src="https://user-images.githubusercontent.com/99636296/162892266-d8ebd872-c71e-47c1-94ec-32c954f85704.png">

* Di menu kiri, pilih ***Personal access tokens*** dan klik ***Generate new token*** seperti paparan berikut

<img width="800" alt="image" src="https://user-images.githubusercontent.com/99636296/162892581-3c328a8c-e483-4bcd-a22a-eab38bd665f0.png">

* Masukkan **mygit** di ***Note***, pilih ***repo, admin:repo_hook & delete_repo*** dari senarai ***Select scopes*** dan klik ***Generate token*** seperti di paparan berikut

<img width="600" alt="image" src="https://user-images.githubusercontent.com/99636296/162894114-b348010a-4f8a-47e8-9e9f-a20b3fee70e2.png">

* Salin token seperti paparan berikut dan simpan token untuk kegunaan seterusnya

<img width="600" alt="image" src="https://user-images.githubusercontent.com/99636296/162901480-18652570-dee9-4630-af2e-ddd88679208e.png">


## Langkah 3.0: Penggunaan Git

### Langkah 3.1: Wujudkan *repository* baru
* Akses ke laman **github.com**, pilih menu ***Repositories*** dan klik ***New*** untuk wujudkan ***repository*** baru, seperti paparan berikut:

<img width="800" alt="image" src="https://user-images.githubusercontent.com/99636296/162782125-ed142ef0-5e99-4f1d-a663-1c8f3556a4b8.png">


*  Masukkan maklumat untuk ***Repository name***, ***Description***, pilih ***Private*** dan klik ***Create repository***, seperti paparan berikut:

<img width="800" alt="image" src="https://user-images.githubusercontent.com/99636296/162781563-4dda8502-74d0-4dd8-8705-cee1e81b5543.png">

* Berikut adalah contoh paparan ***repository*** yang baru diwujudkan

<img width="600" alt="image" src="https://user-images.githubusercontent.com/99636296/162782737-ebd51906-d696-40ac-bb09-af37ab2ffd99.png">


### Langkah 3.2: Penggunaan *Git client*
* Buka aplikasi ***Command Prompt*** untuk Windows atau ***Terminal*** untuk MacOS
* Wujudkan direktori baru - **mygit**

```
mkdir mygit
cd mygit
```
* Taip kod seperti berikut untuk wujudkan ***local repository*** dan muatnaik ke GitHub sebagai ***remote repository***

```
echo "# Aplikasi mygit" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/cikgu-enovade/mygit.git
git push -u origin main
```

Untuk **Username for 'https://github.com':** masukkan **GitHub username** contoh **cikgu-enovade**

Untuk **Password for 'https://cikgu-enovade@github.com':** masukkan token yang di wujudkan dari langkah [Langkah 2.1](#langkah-21-wujudkan-github-personal-access-token)

* Berikut adalah contoh paparan di aplikasi ***Command Prompt*** untuk Windows atau ***Terminal*** untuk MacOS jika berjaya

```
Username for 'https://github.com': cikgu-enovade
Password for 'https://cikgu-enovade@github.com': 
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 228 bytes | 114.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/cikgu-enovade/mygit.git
 * [new branch]      main -> main
Branch 'main' set up to track remote branch 'main' from 'origin'.
```

### Langkah 3.3: Semak GitHub *repository*
* Di laman GitHub, ***mygit project repository***, klik ***Refresh*** di browser untuk melihat maklumat baru seperti di paparan berikut

<img width="800" alt="image" src="https://user-images.githubusercontent.com/99636296/162907556-2a43bf5a-393d-41ff-a7ec-a9d1ac45836b.png">

### Langkah 3.4: Fungsi Git *pull*
* Di laman GitHub, akses ke ***mygit project repository***, klik ikon **pencil** untuk edit maklumat fail **README.md**, seperti di paparan berikut

<img width="800" alt="image" src="https://user-images.githubusercontent.com/99636296/162932796-c2b64357-5a69-4855-899d-67903eefae01.png">

* Tambah maklumat berikut **## Ujian git dengan GitHub** dan klik ***Commit changes***

![edit-2-readme](https://user-images.githubusercontent.com/99636296/162934540-6c382bb8-fdc6-474a-80ad-a174a618946b.png)

* Berikut adalah paparan jika berjaya

<img width="800" alt="image" src="https://user-images.githubusercontent.com/99636296/162934921-468299f5-e182-4cb5-bd80-7c35102a6612.png">

* Buka aplikasi ***Command Prompt*** untuk Windows atau ***Terminal*** untuk MacOS
* Pastikan berada di direktori **mygit**, taip kod berikut untuk muat turun maklumat terbaru dari ***repository*** GitHub

```
git pull
```
* Berikut adalah contoh paparan di aplikasi ***Command Prompt*** untuk Windows atau ***Terminal*** untuk MacOS jika berjaya

```
remote: Enumerating objects: 5, done.
remote: Counting objects: 100% (5/5), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), done.
From https://github.com/cikgu-enovade/mygit
   c2792e6..405c0b3  main       -> origin/main
Updating c2792e6..405c0b3
Fast-forward
 README.md | 1 +
 1 file changed, 1 insertion(+)
```
* Taip kod seperti berikut untuk melihat kandungan maklumat yang baru dimuat turun

```
cat README.md
```
atau untuk Windows  ***Command Prompt***

```
type README.md
```

* Berikut adalah contoh paparan jika berjaya

```
# Aplikasi mygit
## Ujian git dengan GitHub
```
