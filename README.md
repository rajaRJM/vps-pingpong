<h1 align="center"> 👋, PINGPONG</h1>
<h1 align="center"> // building the largest DePIN liquidity and service aggregator🏓#DePINFi
</h1>
<img src="https://pbs.twimg.com/profile_banners/1764537994072268800/1709813967/1500x500" />

# 🚀 Pingpong Mining di VPS

Berikut adalah petunjuk yang telah disusun dengan rapi untuk menjalankan Pingpong Mining di VPS:

## 🛠️ Instalasi Pingpong

1️⃣ **Instalasi Docker** 🐳
  ```shell
    sudo apt update && sudo apt install -y apt-transport-https ca-certificates curl software-properties-common && curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add - && sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" && sudo apt update && sudo apt install -y docker-ce && sudo systemctl start docker && sudo systemctl enable docker
  ```

2️⃣ **Mendapatkan Aplikasi Pingpong** 📥
  ```shell
    cd $HOME && wget https://pingpong-build.s3.ap-southeast-1.amazonaws.com/linux/latest/PINGPONG && chmod +x PINGPONG
  ```

3️⃣ **Menjalankan Screen** 🖥️
  ```shell
    screen -S pingpong
  ```

4️⃣ **Mencari ID Perangkat Anda** 🔍
  ```shell
    https://harvester.pingpong.build/devices
  ```

5️⃣ **Menjalankan Pingpong** 🏃
  ```shell
    ./PINGPONG --key your_device_id
  ```

## 📌 Langkah Tambahan (Jika Diperlukan)

- **Instalasi Libc6** 📚
    ```shell
    sudo echo "deb http://security.ubuntu.com/ubuntu jammy-security main" >> /etc/apt/sources.list && sudo apt -qy update && sudo apt -qy install libc6
    ```

- **Instalasi Screen** 🖥️
    ```shell
    sudo apt install screen -y
    ```

Jika Anda menemui kesalahan, jangan ragu untuk memberi tahu kami. Selamat mencoba! 👍
