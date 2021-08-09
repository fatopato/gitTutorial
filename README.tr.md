# Git'e Giriş

Git temelleri

## Git'i aktive et
Git'in takip edebilmesi için öncelikle çalışılacak klasörde git aktive edilir. Git başlatıldıktan sonra değişiklikler takip edilmeye başlanacaktır.

Git'i aktive etmek için şu komut çalıştırılır:
``` shell
git init 
```

Komut çalıştırıldıktan sonra '.git' adlı bir dosya otomatik oalrak oluşur (Gizli formatta oluşur görüntülenemeyebilir) 

## Dosyaları git'e ekleme
Takip edilecek dosyalar git'e eklenmelidir. Bunu aşağıdaki şekillerde yapabiliriz
Dosyalar tek tek şu şekilde eklenebilir:
``` shell
git add [filename]
```
Alternatif olarak klasördeki tüm dosyalar şu komut ile git'e eklenebilir:
``` shell
git add . 
```
Her bir dosya değişikliğinden sonra dosyalar yeniden eklenir.

## Değişiklikleri commit'lemek
Adding is not enough to save the changes to the local repository. After you add files to staging you need to commit changes to save.

In order to commit the changes:

``` shell
git commit -m "[commit message]" 
```

You can add commit message after -m parameter. For example:

``` shell
git commit -m "All files added to the workspace" 
```

## Push to Remote Repository (Optional)

If you have a remote repository, you can push your local changes.
First you need to specify the remote repo address:

``` shell
git remote add origin [repository address]
```

The remote repository address should be placed such as:
``` shell
git remote add origin https://github.com/fatopato/gitTutorial.git
```

**origin** is the remote repo name. You can give any name but origin is the common name for it.

After adding the remote repo now you can push the local code to the remote by:
``` shell
git push origin [branch_name]
```
You can specify the remote branch by changing the branch name but the common branch name for first commit is **master**
For example in order to the push local branch to remote master branch:

``` shell
git push origin master
```
