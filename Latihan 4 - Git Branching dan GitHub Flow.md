# *Git Branching & GitHub Flow*
Penggunaan ***Git Branching & GitHub Flow***

## Langkah 1.0: Wujudkan *git branch*

* Di laman GitHub, akses ke ***mygit project repository***, klik **main**, taip ***feature*** dan klik ***Create branch: feature from 'main'***, seperti paparan berikut

<img width="400" alt="image" src="https://user-images.githubusercontent.com/99636296/162960730-32d7598a-c223-4115-9cf5-390498b31d03.png">

* Berikut adalah contoh paparan jika berjaya

<img width="400" alt="image" src="https://user-images.githubusercontent.com/99636296/162961359-02bf6086-cf01-4343-b68a-d68451683664.png">


* Buka aplikasi ***Command Prompt*** untuk Windows atau ***Terminal*** untuk MacOS
* Pastikan berada di direktori **mygit**, taip kod berikut untuk lihat ***git branch*** sedia ada

```
git branch
```
* Berikut adalah contoh paparan

```
* main
```

* Taip kod berikut untuk muat turun maklumat terkini dari GitHub 

```
git pull
```

* Taip kod berikut untuk tukar ke ***feature branch***

```
git checkout feature
```

* Taip kod berikut untuk lihat senarai ***git branch***

```
git branch
```
* Berikut adalah contoh paparan jika berjaya

```
* feature
  main
```

## Langkah 2.0: Fungsi Git *add, commit & push*
* Di aplikasi ***Command Prompt*** untuk Windows atau ***Terminal*** untuk MacOS, taip kod seperti berikut

```
echo "# First Feature" >> uji-branch.md
git add uji-branch.md
git commit -m "tambah fail baru"
git push
```

* Berikut adalah contoh paparan jika berjaya
```
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 331 bytes | 331.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/cikgu-enovade/mygit.git
   dd44543..a5d987c  feature -> feature
```

## Langkah 3.0: Semak GitHub *branch repository*
* Di laman GitHub, ***mygit project repository***, pilih ***feature branch*** dan pastikan fail **uji-branch.md** wujud di senarai seperti paparan berikut

<img width="915" alt="image" src="https://user-images.githubusercontent.com/99636296/162964579-0ab9d605-d3d5-42f3-9561-8a82715e840c.png">

* Sila buat perbandingan di antara ***main branch*** dan ***feature branch***

## Langkah 4.0: Fungsi Git *merge*
* Di laman GitHub, ***mygit project repository***, dari menu klik ***pull request*** seperti paparan berikut

<img width="144" alt="image" src="https://user-images.githubusercontent.com/99636296/162965306-de45a9d4-a918-452b-bdbd-b629569ab883.png">

* Klik ***New pull request*** seperti paparan berikut

<img width="452" alt="image" src="https://user-images.githubusercontent.com/99636296/162975882-6da0c4ac-b462-4c14-b94f-e270b8b45089.png">


* Pilih ***feature branch*** dari senarai ***compare: branch*** seperti paparan berikut

<img width="780" alt="image" src="https://user-images.githubusercontent.com/99636296/162976355-e5038fa6-b770-47a8-8707-4f110dfe941c.png">

* Klik ***Create pull request*** seperti di paparan berikut 

<img width="261" alt="image" src="https://user-images.githubusercontent.com/99636296/162976575-fd52d3bb-3487-4ddd-9dea-e596bf11100c.png">

* Klik ***Create pull request*** sekali lagi seperti di paparan berikut

<img width="800" alt="image" src="https://user-images.githubusercontent.com/99636296/162976745-fe7a4bc9-5afe-429b-bfc7-d838e279efef.png">

* Klik ***Merge pull request***

<img width="800" alt="image" src="https://user-images.githubusercontent.com/99636296/162977136-05e5c9d4-1388-4062-b722-839a3197197c.png">

* Klik ***Confirm merge***

<img width="800" alt="image" src="https://user-images.githubusercontent.com/99636296/162977378-1e7a32f8-cebc-435e-91e3-158728b9d1e4.png">

* Akhir sekali klik ikon **<> Code** dari menu untuk lihat perubahan ***branch merging*** dari ***feature*** ke ***main branch***

<img width="800" alt="image" src="https://user-images.githubusercontent.com/99636296/162978115-f66ec02e-02d8-4c7e-9f33-b4cc1c5ccc02.png">
