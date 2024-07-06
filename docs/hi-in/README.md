# MySQL डेटाबेस बैकअप स्क्रिप्ट 🗄️

![Linux](https://img.shields.io/badge/Linux-white?style=flat-square&logo=linux&logoColor=black)
![MacOS](https://img.shields.io/badge/MacOS-white?style=flat-square&logo=apple&logoColor=black)
![Windows](https://img.shields.io/badge/Windows-white?style=flat-square&logo=windows&logoColor=black)
![Windows](https://img.shields.io/badge/Bash-white?style=flat-square&logo=gnu-bash&logoColor=black)

![GitHub मुद्दे](https://img.shields.io/github/issues/vinugawade/ms-bkp?style=flat-square)
![GitHub कोड का आकार (बाइटों में)](https://img.shields.io/github/languages/code-size/vinugawade/ms-bkp?style=flat-square)
![GitHub का आधिकारिक कमिट](https://img.shields.io/github/last-commit/vinugawade/ms-bkp?style=flat-square)

यदि आपको एक Linux सिस्टम पर MySQL डेटाबेस का बैकअप बनाना है, तो `ms-bkp` स्क्रिप्ट एक आसान उपाय प्रदान करता है। इससे आप डेटाबेस को निर्यात कर सकते हैं, विशिष्ट डेटाबेस को छोड़ सकते हैं, और बैकअप के लिए गंतव्य पथ सेट कर सकते हैं।

---

## स्थापना 🚀

1. **पूर्वदृष्टि क्लोन करें:**
    - नीचे दिए गए कमांड का उपयोग करके अपनी स्थानीय मशीन पर [ms-bkp](https://github.com/vinugawade/ms-bkp) रिपॉजिटरी क्लोन करें:

    ```bash
    git clone https://github.com/vinugawade/ms-bkp.git
    ```

2. **स्क्रिप्ट को एक वैश्विक स्थान पर मूव करें:**
    - नीचे दिए गए कमांड का उपयोग करके स्क्रिप्ट को अपने सिस्टम पर एक वैश्विक स्थान पर मूव करें:

    ```bash
    sudo mv /location/of/ms-bkp /usr/local/bin
    ```

3. **स्क्रिप्ट अनुमतियों को सेट करें:**
    - निम्नलिखित कमांडों में से किसी एक का चयन करके सभी को स्क्रिप्ट को निष्क्रिय करने की अनुमति दें:

    ```bash
    sudo chmod +x /location/of/ms-bkp
    ```

    या

    ```bash
    sudo chmod 0755 /location/of/ms-bkp
    ```

4. **$PATH में जोड़ें:**
    - `/usr/local/bin` को अपने `$PATH` में जोड़ें। यदि आप Bash शैली का उपयोग करते हैं, तो नीचे दिए गए कमांड को चलाएं:

    ```bash
    export PATH=$PATH:/usr/local/bin
    ```

    या

    ```bash
    export PATH=$PATH:/location/of/ms-bkp
    ```

    इससे एक चर में रखा जाएगा, संभावना एक फ़ाइल जैसे `~/.bash_profile`, `~/.bashrc`, या `~/.profile`। यदि आप नहीं जानते कि इसे कहां रखें, तो `~/.bashrc` एक अच्छा विकल्प है।

> **इसे लागू करने के लिए आपको शैल को पुनः प्रारंभ करने की आवश्यकता हो सकती है।**

---

## स्क्रिप्ट विकल्प 🎛️

`ms-bkp` स्क्रिप्ट निम्नलिखित विकल्पों का समर्थन करता है:

- `-u, --user`: MySQL उपयोगकर्ता नाम
- `-p, --password`: MySQL पासवर्ड
- `-o

, --only`: केवल निर्दिष्ट डेटाबेस को निर्यात करें
- `-s, --skip`: निर्दिष्ट डेटाबेस को निर्यात के दौरान छोड़ें (कॉमा से अलग)
- `-d, --dest`: बैकअप के लिए गंतव्य पथ (डिफ़ॉल्ट: ~/Downloads)

---

## उपयोग 🛠️

अब आप टर्मिनल में कहीं से भी स्क्रिप्ट का उपयोग कर सकते हैं। नीचे कुछ उदाहरण हैं।

```bash
ms-bkp -u your_mysql_user -p your_mysql_password -o your_database_name
```

```bash
ms-bkp -u your_mysql_user -p your_mysql_password -s db1,db2,db3 -d /path/to/backup
```

नीचे दिए गए GIF को देखें।

![Run ms-bkp script](images/feature.gif)

---

## पालक 👨🏻‍💻

<a href="https://vinux.in">
  <img
    src="https://api.daily.dev/devcards/c8457c6e687d407197d39cfaf513c57a.png?r=qqh"
    width="400"
    height=""
    alt="विनय गवडे का डेव कार्ड"
  />
</a>

💙✨ से बनाया गया है <a href="https://github.com/vinugawade">विनय गवडे</a>.

<a href="https://www.linkedin.com/in/vinu-gawade" target="_blank">
  <img
    src="https://github.com/vinugawade/vinugawade/blob/main/assets/images/media/LinkedIn.png?raw=true"
    alt="लिंक्डइन लोगो"
    width="150"
    height=""
  />
</a>
<a href="https://www.buymeacoffee.com/vinaygawade" target="_blank">
  <img
    src="https://github.com/vinugawade/vinugawade/blob/main/assets/images/media/Bmc.png?raw=true"
    alt="मुझे एक कॉफी खरीदें लोगो"
    width="150"
    height=""
  />
</a>
<a href="https://twitter.com/VinuGawade" target="_blank">
  <img
    src="https://github.com/vinugawade/vinugawade/blob/main/assets/images/media/Twitter.png?raw=true"
    alt="ट्विटर लोगो"
    width="150"
    height=""
  />
</a>

---

## लाइसेंस 🛂

![लाइसेंस](https://img.shields.io/github/license/vinugawade/ms-bkp?style=flat-square)

इस परियोजना का उपयोग [लाइसेंस](https://github.com/vinugawade/ms-bkp/blob/master/LICENSE) फ़ाइल के साथ जुड़ा हुआ है।
