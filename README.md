# 📊 CDF / EFK – Upcoming Publications (Scriptable Widget)

An **iOS Scriptable widget** that displays the **upcoming publications of the Swiss Federal Audit Office (CDF / EFK)** directly on your iPhone home screen.

The widget is **bilingual (FR / DE)**, updates automatically, and compensates for the delayed updates on the official website.

---
<img width="590" height="294" alt="Widget iOS" src="https://github.com/user-attachments/assets/b0f58479-e092-436e-b222-c3963e4cbaeb" />

---
## ✨ Features

- 📅 Displays **upcoming audit publications**
- 🌍 **Bilingual FR / DE**
  - automatic detection based on iPhone language  
  - or manual override via widget parameter (`fr` / `de`)
- ⏰ **Daily refresh at 00:30**
- 🔄 Automatically switches to the *next* upcoming publications even if the official CDF/EFK website has not yet been updated
- 🗂️ **Local cache** to reduce unnecessary network requests
- 🎨 Clean and minimal design, aligned with institutional colors
- 🔗 Tap on the widget to open the official CDF / EFK webpage
- 📅 Display of the message “Tonight, 11 p.m.” when posts are on the same day
- 🏷️ Audit number and entity acronym displayed together on a single line (e.g. `25221  ·  IPI`)
- 📆 Dates shown with full month name, without year (e.g. `1er avril`, `1. April`)

---

## 📱 Requirements

- iPhone running iOS
- **Scriptable** app (free)  
  👉 https://apps.apple.com/app/scriptable/id1405459188

---

## 🚀 Installation

1. Install **Scriptable** from the App Store
2. Open the **Scriptable** app
3. Create a **new script** (`+`)
4. Copy and paste the content of  
   `CDF_EFK_Widget_publications.js`
5. Name the script (e.g. `CDF – prochaines publications`)
6. Go back to the iOS home screen
7. Add a **Scriptable widget** (size **Medium**)
8. Configure the widget:
   - Long press on the widget
   - Select **Edit Widget**
   - Choose the script you created

### 🌍 Language override (optional)

In the Scriptable widget settings:

- `fr` → French
- `de` → German

By default, the widget uses the iPhone system language.

---

## 🧾 Displayed content

For each publication, the widget shows:

- **Publication date** (full month, no year – e.g. `1er avril` / `1. April`)
- **Audit number + entity acronym** on the same line (e.g. `25221  ·  OFEN`)
- **Audit title** (up to 2 lines)

Publications are separated by light dividers for readability. Over 50 federal entities are mapped to their official acronyms (FR & DE).

---

## ⏱️ Update logic

- 🟢 First run → immediate data load
- 🕛 Every day at **00:30**:
  - automatic refresh
  - removal of already published audits
- 💤 During the day:
  - data is served from the local cache for speed and efficiency

👉 This ensures the widget always shows the **correct upcoming publications**, even when the official CDF/EFK website is updated with a one-day delay.

---

## 🛠️ Troubleshooting

If the widget shows no data or incorrect content:

1. Open **Scriptable**
2. Select the script
3. Tap ▶️ **Run**
4. Check the console logs

Things to verify:
- internet connection
- access to `https://www.efk.admin.ch`
- Scriptable network permissions in iOS settings

---

## 🧩 Customization

The script is easy to extend:

- add or adjust **entity acronyms**
- limit the number of displayed publications
- tweak layout and typography
- extend to additional languages

---

## 📄 License

Internal / experimental use.  

---

## 🙌 Contributing

Improvements and suggestions are welcome  
(via pull requests or issues).
