# Baseイメージ
FROM python:3

RUN apt-get update

# ROOTにパスワードをセット
RUN echo 'root:jeewv084543tjrjfj49f7' |chpasswd

# ユーザを作成
RUN useradd m1z0r3
RUN echo 'm1z0r3:mu51c_15_mag1c' |chpasswd
RUN usermod -aG sudo m1z0r3

# sudoをインストール
RUN apt-get install -y sudo

# Flaskのインストール
RUN pip install --trusted-host pypi.org --trusted-host pypi.python.org --trusted-host files.pythonhosted.org flask

RUN echo 'm1z0r3{fl4sk_15_mag1c}' > /flag.txt
RUN chown root:root /flag.txt
RUN chmod 600 /flag.txt
RUN echo 'h1nt5 are first f1ag...' > /flog.txt
RUN chown www-data:www-data /flog.txt

CMD ["sudo", "-u", "www-data", "python", "/usr/local/src/work/app.py"]