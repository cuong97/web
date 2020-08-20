<!-- TITLE:  Django: Quick Start -->
<!-- SUBTITLE: Step by step installation, commands, tutorials, and resources for new Django developers. -->

# Django: Quick Start

## Installation: Step by Step

Run the following commands in your Terminal:

1. Install `python3`: `brew install python3`
1. Install `virtualenv`: `pip3 install virtualenv`
1. Create a directory for your new project: `mkdir new-project && cd new-project`
1. Create a new `virtualenv` for the new project: `virtualenv env`
1. Activate the new `virtualenv`: `source env/bin/activate`
1. Install Django in the fresh `env`: `pip install django`
1. Generate scaffolding for your new Django project: `django-admin startproject proj`
1. Navigate to the new Django project directory: `cd proj`
1. Create a new Django app: `python manage.py startapp tasks`
1. Run the Django development server: `python manage.py runserver
1. Create môi trường: `mkvirtualenv test-1 --python=/usr/bin/python3`
1. Tắt môi trường ảo: `$ deactivate`
1. Goi moi truong ao: `$ workon test-1`
1. Trong môi trường, cài đặt gói Django bằng pip: `$ pip install django`
1. Xuất các package sử dụng ra file requirements.txt
  * `$ pip3 freeze > requirements.txt`
1. Và sử dụng để cài các gói đã xuất từ requirements.txt
  * `$ pip3 install -r requirements.txt`
1. cập nhật database từ mysql về models
  * `$ python manage.py inspectdb > blog/models.py`
-- load data to json
* `python manage.py loaddata app_name`
* `exec(open("./web/test_bcrypt.py").read())`
* `git reset --soft HEAD^`
* `CREATE DATABASE vna CHARACTER SET utf8 COLLATE utf8_general_ci;
* `CREATE USER 'vna'@'localhost' IDENTIFIED BY 'vna123';`
* `SET GLOBAL validate_password_length = 6;`
* `SET GLOBAL validate_password_number_count = 0;`
* `SET GLOBAL validate_password_policy=LOW;`
* `compilemessages and makemessages -l 'fr'`

## flask
-- connect mysql = mysql-connector-python
* `DATABSE_URI = 'mysql+mysqlconnector://{user}:{password}@{server}/{database}'.format(
    user=username, password=password, server=server, database=database_name)`
-- connect mysql = mysqlclient
* `DATABSE_URI = 'mysql://{user}:{password}@{server}/{database}'.format(
    user=username, password=password, server=server, database=database_name)`
## Git
* `git branch`
* `git checkout -b dev-cuong` : Tao Nhanh branch
* `git push --set-upstream origin dev-cuong` : push server
* `git chackout`
* `git merge`
* `git cherry-pick ...`
* `git stash` `->` `git stash pop`
* `git pull --rebase`
* add remote `git remote add origin https://github.com/user/repo.git`
* Gộp commit đã push `git rebase -i HEAD~(vị trí commit)`
* Gộp commit chưa push `git commit --amend`
* [docs] (https://docs.github.com/en/github/using-git/renaming-a-remote)
* [Git cơ bản](https://backlog.com/git-tutorial/vn/stepup/stepup7_5.html)
## Helpful Management Commands

* `python manage.py makemigrations`: Generates migrations for newly created Django apps.
* `python manage.py migrate`: Applies migrates generated by `makemigrations`

## Tutorials
The best tutorial for Django is located within the documentation. Follow all six steps and you'll know everything you need to know to hit the ground running!

* [Writing Your First Django App: Part 1 - Getting Started](https://docs.djangoproject.com/en/2.0/intro/tutorial01/)
* [Writing Your First Django App: Part 2 - Database Setup](https://docs.djangoproject.com/en/2.0/intro/tutorial02/)
* [Writing Your First Django App: Part 3 - Views/URLs](https://docs.djangoproject.com/en/2.0/intro/tutorial03/)
* [Writing Your First Django App: Part 4 - Forms](https://docs.djangoproject.com/en/2.0/intro/tutorial04/)
* [Writing Your First Django App: Part 5 - Testing](https://docs.djangoproject.com/en/2.0/intro/tutorial05/)
* [Writing Your First Django App: Part 6 - Templates](https://docs.djangoproject.com/en/2.0/intro/tutorial06/)

## Documentation
**Full documentation located here**: https://docs.djangoproject.com/en/2.0/

* [Models: Field Reference](https://docs.djangoproject.com/en/2.0/ref/models/fields/)
* [Views: Writing Views](https://docs.djangoproject.com/en/2.0/topics/http/views/)
* [Views: URL Dispatcher](https://docs.djangoproject.com/en/2.0/topics/http/urls/)
* [Views: Shortcuts](https://docs.djangoproject.com/en/2.0/topics/http/shortcuts/)
* [Templates: Overview](https://docs.djangoproject.com/en/2.0/topics/templates/)
* [Templates: Built-in Template Tags and Filters](https://docs.djangoproject.com/en/2.0/ref/templates/builtins/)

## Face Recognition
**full documentation located here**: https://github.com/ageitgey/face_recognition

## add key ssh github
* ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
* /home/cuong/.ssh/id_rsa_...
* cat /home/cuong/.ssh/id_rsa.pub
* run: ssh-add ~/.ssh/id_rsa

** sudo apt-get install libmysqlclient-dev python3-dev
PYTHONUNBUFFERED=1;DJANGO_SETTINGS_MODULE=web.local_settings

## Git Training

- Hướng dẫn về Git cơ bản cho người mới bắt đầu: Đọc ở [đây](http://backlogtool.com/git-guide/vn/intro/intro1_1.html) (Tiếng Việt), chú ý đọc cả phần **Nhập môn** và **Phát triển**.
- Sổ tay về Git: Đọc ở [đây](http://hnq90.github.io/git-guide/index.vi.html) hoặc [đây](https://learnxinyminutes.com/docs/vi-vn/git-vi/) (Tiếng Việt)
- Thực hành những thao tác căn bản với Git online: [Try Git](http://try.github.com/)  (Tiếng Anh)
- Những lệnh hay dùng: [Git Cheatsheet](http://www.git-tower.com/blog/git-cheat-sheet/)  (Tiếng Anh)
- Ebook hướng dẫn Git từ căn bản đến nâng cao: [Tiếng Anh](https://git-scm.com/book/en/v2) (updated 2014), [Tiếng Việt](https://git-scm.com/book/vi/v1) (updated 2009)
- Hướng dẫn sử dụng Git trên Netbean IDE: Đọc ở [đây](https://netbeans.org/kb/docs/ide/git.html)
- [Start a new git repository](http://kbroman.org/github_tutorial/pages/init.html)

## Git Client
Dưới đây là những phần mềm tương tác với Git qua giao diện đồ hoạ:
- [SourceTree](http://www.sourcetreeapp.com/) (Windows, Mac)
- [GitKraken](https://www.gitkraken.com/) (Windows, Mac, Linux)
- [GitExtension](https://github.com/gitextensions/gitextensions/releases) (Windows, Mac, Linux)
- [git-cola](http://git-cola.github.com/) (Windows, Linux)


## Cài đặt Git
- Windows: [Download](https://git-scm.com/book/vi/v1/B%E1%BA%AFt-%C4%90%E1%BA%A7u-C%C3%A0i-%C4%90%E1%BA%B7t-Git#Cài-Đặt-Trên-Windows)
- Linux: [Download](https://git-scm.com/book/vi/v1/B%E1%BA%AFt-%C4%90%E1%BA%A7u-C%C3%A0i-%C4%90%E1%BA%B7t-Git#Cài-Đặt-Trên-Linux)
- Mac: [Download](https://git-scm.com/book/vi/v1/B%E1%BA%AFt-%C4%90%E1%BA%A7u-C%C3%A0i-%C4%90%E1%BA%B7t-Git#Cài-Đặt-Trên-Mac)

## Cấu hình Git căn bản
Thiết lập thông tin cá nhân cho Git: (Sử dụng Git Bash hoặc Terminal để gõ các lệnh sau) **bắt buộc**
- `git config --global user.name "Ten cua ban"`
- `git config --global user.email <email rikkeisoft>`

- `git config --global core.safecrlf true`
- `git config --global color.ui true`
- `git config --global core.filemode false`

- `git config --global core.autocrlf input` (Cho Linux - Mac)
- `git config --global core.autocrlf true` (Cho Windows)

### Trường hợp code trên Windows nhưng chạy trên Linux
*Trong trường hợp code trên Windows nhưng code được đưa lên môi trường thực thi Linux bằng cách share folder hoặc upload trực tiếp, cần đảm bảo các file ở working copy có line endings kiểu Unix (LF) để chạy đúng trên môi trường Linux.*

Với các dự án này thì thực hiện config giống như trên môi trường Linux. Chú ý chỉ config cho riêng từng repository, không config global để tránh ảnh hưởng tới các repository có môi trường khác.
- `git config core.safecrlf true`
- `git config core.eol lf`
- `git config core.autocrlf input`
- Khi lưu file, cần chú ý file được lưu với line ending là LF (Có thể dùng plugin **Show and change line endings** của Netbeans để thay đổi line ending)

## Những điều chú ý khi dùng Git
- Viết nội dung commit có ý nghĩa và liên quan tới công việc đang làm.
 + Ví dụ: Issue #69, có yêu cầu: *"Viết chức năng đăng ký user cho hệ thống"* thì khi commit nên viết message là: **"Issue #69 Implement user registration feature"**

## Tip
- Bị lỗi liên quan đến line-ending:
```
git rm .gitattributes
git add -A
git reset --hard
```

## License
<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.

