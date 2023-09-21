Global setup:
```bash
  git config --global user.name "group4comunity"
  git config --global user.email "group4community@gmail.com"
```
Step Push On Repo:
```bash
  git init
  git add .
  git commit -m"first commit"
  git remote add origin https://github.com/user_name/new_repo.git
  git push -u origin main/master/dev/staging
```
Step Push Again:
```bash
   git add .
   git commit -m"second commit"
   git push origin main/master/dev/staging
```
Step Collaboration in origin:
```bash
   git clone https://src-git/...
 ```
After change :
```bash
   git add .
   git status // see changes
   git commit -m"Bug Fixing"
   git checkout b "feat/searching" // ini untuk mempersingkat git branch feat/search dan git checkout feat/searching
   git push origin "feat/searching"
 ```
Step Collaboration in upstream:
```bash
  git remote add upstream https://github.com/src_repo_kantor/repo_kantor.git
  git remote -v //opsional/ untuk lihat list remote
  git checkout -b "feat/feat-name"
  git add .
  git commit -m"what created change"
  git push origin "feat/feat-name"
```
Step lanjutan jika ada yang salah setelah di upstream.
Kondisi untuk udah ada di branch yang ada salah tadi:
```bash
  git add .
  git commit -m"resolve conflict"
  git push origin "feat/feat-name"
  baru pull request lewat githubnya.
```
Kondisi branch sudah dihapus branchnya tadi:
```bash
  git add .
  git commit -m"resolve conflict"
  git checkout -b "feat/feat-name"
  git push origin "feat/feat-name"
  artinya sudah dipush ke origin tinggal langsung pull request lewat github.
```
Menghapus branch di repo/remote-repo collab :
```bash
  git remote add upstream https://github.com/src_repo_kantor/crepo_kantor.git
  git push --delete nama_branch
```
Check update di remote repository:
```bash
  git remote dulu
  git fetch
```
Ambil update-an nya :
```bash
  git pull 
```
Membuat working branch baru di upstream dan origin secara bersamaan:
```bash
  git push --set-upstream origin nama-branch
```
Berpindah ke branch sebelumnya :
```bash
  git checkout -    // kalo berpindah ke branch yang dituju bisa pakai git checkout -nama_branch
```
Mengubah nama branch local :
```bash
  git branch -m nama-branch-lama nama-branch-baru
  ```
Menggabungkan perubahan dari branch lain ke branch yang sedang aktif :
```bash
  git merge nama-branch-lain
```
Melihat Setting Git :
```bash
  git config --list
```
Documentation and helper :
```bash
  git help config
  ```

