# 🚀 HackerOne Notifier

![logo-h1](https://github.com/user-attachments/assets/06ffd2e2-f298-48fc-a731-7e0d9e75712b)

## Inspiration

_*For me, hacking is about persistence, creativity, and pushing boundaries in the most elegant way possible.*_

> The code is art, like music and other creative fields. I created H1-Notifier out of passion and love for coding. Writing code is not just a habit, it's discipline, focus, and a way of life. Throughout this project, I constantly listened to these tracks:
> 
> - [Agua y Ensalada](https://www.youtube.com/watch?v=OeqjLSCVKvU) - Luis7Lunes: "El rap es la cura y también viene en pasta, la balanza se inclina pa'l que poco descansa, mejor duerma lo suficiente."
> - [Uno](https://www.youtube.com/watch?v=xEx7t7PqR2A) - Ali Aka Mind: "Así que vamos mano no bajes el ritmo please, me lo digo yo a mí mismo cuando todo pinta gris. Yo no hago rap pa' ser el mejor MC del país, yo solo hago lo que puedo pa' ver mi negra feliz."

Contributing to the infosec community — researchers, hackers, and builders — inspires me to give my best in every line of code I write.

> Always the same creative hacker, but more evolved. - [Juan Felipe Oz](https://x.com/PwnedRar_)

## ⭐ Support the Project

If you find this project useful, please give it a star ⭐ to help others discover it!

### Overview

HackerOne Notifier is an automated bot that monitors new programs launched on HackerOne and sends email notifications whenever a new program is detected. The process is fully automated using GitHub Actions and runs every **3 hours**.

## 📌 Features
- Uses Selenium to scrape HackerOne’s program directory.
- Sends email notifications when new programs are detected.
- Runs on **GitHub Actions** every 3 hours automatically.
- Supports manual execution via GitHub Actions' workflow dispatch.
- Deploys seamlessly with GitHub Actions without requiring manual setup.

## ⚙️ Setup & Configuration

#### 1️⃣ Fork the Repository
```sh
git clone https://github.com/JFOZ1010/H1Notifier.git
cd H1Notifier
```

#### 2️⃣ Add Secrets in GitHub
You must configure the following GitHub Secrets in your repository:
1. Navigate to Settings > Secrets and variables > Actions.
2. Click "New repository secret" and add the above secrets.
![settings-SECRETS](https://github.com/user-attachments/assets/0f2d45dc-65f4-4a60-a6aa-427a4eafe446)


3️⃣ (Optional) Using Gmail as Sender

If you are using a personal Gmail account, you need to enable Less Secure Apps or generate an App Password (recommended).

<img width="691" alt="imagen" src="https://github.com/user-attachments/assets/985ad1d5-a8a6-4dec-8236-3697cf576a26" />


## 🚀 Running the Script

🔹 Automatic Execution (GitHub Actions)

The script runs every 3 hours automatically.

You can also trigger it manually in the Actions tab by selecting "Run workflow".

🔹 Manual Execution (Local Testing)

If you want to test the script locally, install the dependencies:

```bash
python3 -m venv venv
source venv/bin/activate;
pip install -r requirements.txt
```
> Do not forget to create your `.env` file with the EMAIL_USER, EMAIL_PASS, EMAIL_RECEIVER credentials.
> ![env-credentials](https://github.com/user-attachments/assets/7680abe7-3802-4273-9cef-410196939107)


Then run the script:
```bash
python notifier.py
```

⚡ GitHub Actions Workflow

1. Go to Actions in your repository.
2. Select the workflow and click "Run workflow".
![githubActions](https://github.com/user-attachments/assets/f252837e-79ff-438f-ada8-8aa6543feb19)

# 🙌 Acknowledgments

Created with ❤️ by JFOZ1010. If you find this project helpful, consider giving it a ⭐ and sharing it with others!

### 🔥 Contributing

Feel free to open issues or pull requests if you find improvements or bugs!
