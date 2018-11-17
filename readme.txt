### Step-By-Step GitHub Project ###
git init
git add README.md
git commit -m "first commit"
git remote add origin git@github.com:demwf/SmartLend.git
git push -u origin master

---=== ������ ������ ��� ���������� ��� ������� ������/������ ===---

1. ��������� ssh-agent (� ������� git BASH)
eval "$(ssh-agent -s)"

2. �������� ��������������� ���� � ssh-agent
ssh-add ~/.ssh/id_rsa

3. ���������� ���������� � ������
git remote add origin git@github.com:demwf/SmartLend.git

4. �������� ������ ������� ��� ���������� �����������. ��� �����/������
git remote set-url origin git@github.com:demwf/SmartLend.git

5. ���������� username � email ��� ������� ��������
git config --global user.name "demwf"
git config --global user.email "demwf@yandex.ru"

6. ��������� ���������� ���������� ����������� � ���������:
git remote -v

7. �������
��������
git add .
git commit -m "First"

����� ���������
git push -u origin master
