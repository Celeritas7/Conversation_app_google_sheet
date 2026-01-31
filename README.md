# 🇲🇲 Burmese Learning App - Google Sheets Version

## ✨ Features
- 📚 **Learn Mode** - Practice conversations topic by topic
- 🎯 **Quiz Mode** - Test yourself with 3 difficulty levels
- 📊 **Review** - Track your progress
- 🔧 **Converter** - Test Burmese → Devanagari conversion
- ☁️ **Google Sheets** - Data loads fresh from your spreadsheet!

---

## 📁 Files
```
index.html    ← The entire app (single file, no build needed!)
README.md     ← This file
```

---

## 🚀 How to Use

### Option 1: Open Directly
Just double-click `index.html` to open in browser.
(Note: Some browsers block fetching from Google Sheets when opening locally)

### Option 2: Use Live Server (Recommended for local)
1. Open folder in VS Code
2. Install "Live Server" extension
3. Right-click `index.html` → "Open with Live Server"

### Option 3: Deploy to GitHub Pages
1. Create new repo on GitHub
2. Upload `index.html`
3. Settings → Pages → Deploy from branch → main
4. Your app will be at: `https://yourusername.github.io/repo-name/`

---

## 📊 Your Google Sheet Structure

Your Google Sheet ID: `1it_qxYycDn2P1aUyO38tAiiC77NbPefjN6Bw9xeR-Oc`

### Sheet 1: Burmese_Conversation (gid=0)
| Sr. No. | Tag | Burmese | English |
|---------|-----|---------|---------|
| 1 | Title | - | Topic Name |
| 2 | Description | - | Topic description |
| 3 | Bot | မင်္ဂလာပါ | Hello! |
| 4 | User | မင်္ဂလာပါ | Hello! |
| ... | ... | ... | ... |
| 10 | End | --------- | --------- |

### Sheet 2: Consonants (gid=1575080214)
| Burmese | Marathi1 | Marathi2 |
|---------|----------|----------|
| က | क | ग |
| ခ | ख | ग |
| ... | ... | ... |

### Sheet 3: Special_characters (gid=1881483613)
| Burmese_extra | Marathi |
|---------------|---------|
| ကျ | च |
| ချ | छ |
| ... | ... |

### Sheet 4: Vowels (gid=2032073827)
| Burmese_extra | Marathi_extra |
|---------------|---------------|
| ါ | ा |
| ီ | ी |
| ... | ... |

### Sheet 5: Special_words (gid=1662412889) ⚠️ SET THIS UP!
| Burmese | Devanagari |
|---------|------------|
| မင်္ဂလာပါ | मिंगलाबा |
| ကျေးဇူးတင်ပါတယ် | चेजूतिंबाते |

---

## ⚠️ Important: Set Up Special_words Sheet

Your Special_words sheet is empty! Add headers and data:

**Row 1 (Headers):**
```
Burmese | Devanagari
```

**Example data:**
```
မင်္ဂလာပါ | मिं2ग1ला2बा2
ကျေးဇူးတင်ပါတယ် | चे3जु2तिं2बा2दे1
```

---

## ✏️ How to Add New Topics

1. Open your Google Sheet
2. Go to `Burmese_Conversation` tab
3. Add rows following this pattern:

```
| Sr. No. | Tag         | Burmese              | English                    |
|---------|-------------|----------------------|----------------------------|
| 50      | Title       | -                    | At the Restaurant          |
| 51      | Description | -                    | Ordering food              |
| 52      | Bot         | မင်္ဂလာပါ။ ဘာမှာမလဲ။    | Hello. What would you like?|
| 53      | User        | မီနူးပြပါ။             | Please show me the menu.   |
| 54      | Bot         | ဒီမှာပါ။              | Here you go.               |
| 55      | End         | ---------            | ---------                  |
```

4. Refresh your app - new topic appears instantly!

---

## 🔧 Troubleshooting

### "Failed to load data"
- Make sure Google Sheet is public (Share → Anyone with link → Viewer)
- Check your internet connection

### Topics not showing
- Make sure each topic has `Title`, at least one `Bot`/`User`, and `End` tags
- Check for typos in Tag column

### Devanagari showing wrong
- Add the word to Special_words sheet with correct Devanagari
- Check Consonants/Vowels/Special_characters sheets

---

## 🎉 That's it!

Edit your Google Sheet → Refresh the app → See changes instantly!

No npm, no build, no deploy needed for content updates.
