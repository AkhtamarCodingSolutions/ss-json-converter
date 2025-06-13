# 🔐 SS Outline Converter – Конвертация `ss://` Outline ссылок в JSON для Shadowsocks

A simple, modern web tool that converts `ss://` Outline VPN keys to Shadowsocks JSON config format.  
Простой и современный веб-инструмент для преобразования `ss://` ссылок из Outline VPN в JSON-конфигурацию Shadowsocks.

🔗 Live / Онлайн: [https://akhtamarcodingsolutions.github.io/ss-json-converter](https://akhtamarcodingsolutions.github.io/ss-json-converter)

---

## 📺 Special Use Case: Android TV / Особый случай: Android TV

🛑 The Outline app does **not work** on Android TV.  
🛑 Приложение Outline **не работает** на Android TV.

This converter provides a simple workaround:  
Этот конвертер — простое обходное решение:

✅ You can convert your `ss://` Outline link and import it into a Shadowsocks client that works on Android TV.  
✅ Вы можете преобразовать ссылку Outline и импортировать её в Shadowsocks клиент, совместимый с Android TV.

Examples of working clients / Примеры работающих клиентов:
- Shadowsocks TV (from GitHub or F-Droid)
- Other open-source Shadowsocks apps for TV

---

## 🌟 Why? / Зачем это нужно?

Many users receive Outline VPN access via `ss://` links but cannot use it on Android TV.  
Многие получают доступ к Outline VPN по `ss://` ссылкам, но не могут использовать его на Android TV.

This tool makes it easy to convert those links into the JSON format required by Shadowsocks apps.  
Этот инструмент упрощает преобразование таких ссылок в JSON формат, нужный Shadowsocks.

---

## ✨ Features / Возможности

- ✅ **Fast & Private** / Быстро и конфиденциально: работает прямо в браузере  
- 🎨 **Modern, minimal UI** / Современный минималистичный интерфейс  
- 🧠 **Supports both Outline formats** / Поддержка двух форматов ссылок Outline:
  - `ss://base64(method:pass@host:port)`  
  - `ss://base64(method:pass)@host:port)`  
- 📋 **One-click Copy** / Копирование JSON в один клик  
- 💾 **Export to JSON** / Скачивание JSON-файла  
- 📱 Mobile and Android TV friendly / Поддержка мобильных устройств и Android TV  

---

## 🚀 How to Use / Как использовать

1. Paste your `ss://` link / Вставьте вашу `ss://` ссылку в поле ввода.  
2. Click **Convert** / Нажмите **Convert**.  
3. Click **Copy JSON** or **Download JSON** / Нажмите **Copy JSON** или **Download JSON** для копирования или скачивания.

Example / Пример:

```
ss://YWVzLTI1Ni1nY206TXlTM2NyM3RQYXNzdzByZCE=@relay.examplevpn.com:443/?outline=1#Sample%20VPN%20for%20Android%20TV

```

Output / Результат:

```json
{
    "server": "relay.examplevpn.com",
    "server_port": 443,
    "local_port": 1080,
    "password": "MyS3cr3tPassw0rd!",
    "method": "aes-256-gcm",
    "remarks": "Outline Server"
}
```

---

## 🛠 Local Development / Локальная разработка

```bash
git clone https://github.com/yourusername/ss-outline-converter.git
cd ss-outline-converter
open index.html  # or use any static server / или используйте статический сервер
```

To deploy to GitHub Pages / Для публикации через GitHub Pages:

```bash
# Push to main branch / Запушьте в ветку main
# Go to Repo → Settings → Pages → Enable Pages from main / Настройте GitHub Pages через настройки репозитория
```

---

## 🤔 FAQ / Частые вопросы

**Q: Is this safe? / Это безопасно?**  
A: Yes. All conversion happens in your browser. / Да, всё происходит прямо в браузере, ничего не отправляется в интернет.

**Q: Can I use this on Android TV? / Работает ли на Android TV?**  
A: Yes! Just use the exported JSON with a Shadowsocks TV-compatible client. / Да! Просто используйте JSON с клиентом, поддерживающим Android TV.

**Q: Why not just use Outline app? / Зачем, если есть Outline?**  
A: Outline does not work on Android TV. This is a workaround. / Outline не работает на Android TV. Это обходное решение.

---

## 📄 License / Лицензия

MIT – Free to use and modify. / MIT — свободное использование и модификация.

---

## 🙌 Credits / Благодарности

Inspired by: / Вдохновлено:
- [Shadowsocks](https://github.com/shadowsocks)
- [eesheesh/ss-decode](https://gist.github.com/eesheesh/e2da0e61a85e50ebf23651eb1921517f)
