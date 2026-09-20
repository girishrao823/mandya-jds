# ಜೆ.ಡಿ.ಎಸ್ ಮಂಡ್ಯ ಜಿಲ್ಲಾ ಘಟಕ — ವೆಬ್‌ಸೈಟ್

ಸ್ಥಿರ (static) HTML/CSS/JS ವೆಬ್‌ಸೈಟ್. ಯಾವುದೇ ಬ್ಯಾಕೆಂಡ್ ಅಥವಾ ಡೇಟಾಬೇಸ್ ಇಲ್ಲ.

## ಫೈಲ್ ರಚನೆ
```
index.html   - ಮುಖ್ಯ ಪುಟ
style.css    - ವಿನ್ಯಾಸ
script.js    - ನ್ಯಾವಿಗೇಷನ್ ಮೆನು ಸ್ಕ್ರಿಪ್ಟ್
images/      - ಫೋಟೋಗಳು
```

## ಸ್ಥಳೀಯವಾಗಿ ಪರೀಕ್ಷಿಸಲು
`index.html` ಫೈಲ್ ಅನ್ನು ಬ್ರೌಸರ್‌ನಲ್ಲಿ ನೇರವಾಗಿ ತೆರೆಯಿರಿ, ಅಥವಾ:
```
python -m http.server 8080
```
ನಂತರ http://localhost:8080 ಗೆ ಭೇಟಿ ನೀಡಿ.

## GitHub Pages ಮೂಲಕ ಉಚಿತ ಪ್ರಕಟಣೆ (ಶಿಫಾರಸು)
1. GitHub.com ನಲ್ಲಿ ಹೊಸ **ಸಾರ್ವಜನಿಕ** repository ರಚಿಸಿ (ಉದಾ: `mandya-jds`).
2. ಈ ಫೋಲ್ಡರ್‌ನಲ್ಲಿ ಟರ್ಮಿನಲ್ ತೆರೆದು:
   ```
   git init
   git add .
   git commit -m "Initial website"
   git branch -M main
   git remote add origin https://github.com/<your-username>/mandya-jds.git
   git push -u origin main
   ```
3. Repository → **Settings → Pages** ಗೆ ಹೋಗಿ, Source ಅನ್ನು `main` branch, `/root` ಆಗಿ ಆಯ್ಕೆಮಾಡಿ, Save ಒತ್ತಿ.
4. ಕೆಲವು ನಿಮಿಷಗಳಲ್ಲಿ ಸೈಟ್ `https://<your-username>.github.io/mandya-jds/` ನಲ್ಲಿ HTTPS ಮೂಲಕ (ಸುರಕ್ಷಿತವಾಗಿ) ಲಭ್ಯವಾಗುತ್ತದೆ.
5. ಸ್ವಂತ ಡೊಮೇನ್ ಇದ್ದರೆ, Settings → Pages → Custom domain ನಲ್ಲಿ ಸೇರಿಸಬಹುದು ಮತ್ತು "Enforce HTTPS" ಆನ್ ಮಾಡಿ.

## ಪ್ರಕಟಿಸುವ ಮೊದಲು ಪರಿಶೀಲಿಸಿ
- [ ] ಜಿಲ್ಲಾಧ್ಯಕ್ಷರ ಸಂಪರ್ಕ ಸಂಖ್ಯೆ/ಇಮೇಲ್ ಸೇರಿಸಿ (`index.html` ನಲ್ಲಿ `[ಸಂಪರ್ಕ ಸಂಖ್ಯೆ]` ಹುಡುಕಿ)
- [ ] ಜಿಲ್ಲಾ ಕಚೇರಿ ಪೂರ್ಣ ವಿಳಾಸ ಸೇರಿಸಿ
- [ ] ಸಾಮಾಜಿಕ ಮಾಧ್ಯಮ ಕೊಂಡಿಗಳನ್ನು (Facebook/Twitter/YouTube) ಫೂಟರ್‌ನಲ್ಲಿ ಅಪ್‌ಡೇಟ್ ಮಾಡಿ
- [ ] ಫೋಟೋಗಳ ಹಕ್ಕುಸ್ವಾಮ್ಯ/ಒಪ್ಪಿಗೆ ಖಚಿತಪಡಿಸಿಕೊಳ್ಳಿ

## ಭದ್ರತಾ ಟಿಪ್ಪಣಿಗಳು
- ಇದು ಸ್ಥಿರ ಸೈಟ್ ಆಗಿರುವುದರಿಂದ SQL/DB ದಾಳಿಗಳ ಅಪಾಯ ಇಲ್ಲ.
- ಯಾವುದೇ ಫಾರ್ಮ್ (ಸದಸ್ಯತ್ವ ನೋಂದಣಿ) ಮುಂದೆ ಸೇರಿಸಿದರೆ, ಅದನ್ನು ಸುರಕ್ಷಿತ ಮೂರನೇ ವ್ಯಕ್ತಿ ಸೇವೆ (Google Forms, Formspree, ಇತ್ಯಾದಿ) ಮೂಲಕ ಮಾತ್ರ ಸಂಪರ್ಕಿಸಿ; ಸೂಕ್ಷ್ಮ ಡೇಟಾವನ್ನು ನೇರವಾಗಿ ಕ್ಲೈಂಟ್ ಸೈಡ್ ಜಾವಾಸ್ಕ್ರಿಪ್ಟ್‌ನಲ್ಲಿ ನಿರ್ವಹಿಸಬೇಡಿ.
- GitHub Pages ಸ್ವಯಂಚಾಲಿತವಾಗಿ HTTPS ಒದಗಿಸುತ್ತದೆ.
