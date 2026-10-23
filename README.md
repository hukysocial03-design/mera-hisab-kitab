# Mera Hisab Kitab — Free APK Builder (Mobile Friendly)

This package builds a personal Android APK with free GitHub Actions. APK is not included; GitHub must build it first.

## Phone-only setup (step by step)
1. Download this ZIP to your Android phone. In Files / Downloads, tap it and choose Extract. If your phone cannot extract ZIP files, use a trusted ZIP file manager.
2. Open github.com in Chrome. Open your public repository `mera-hisab-kitab`.
3. In the repo page, tap **Add file → Upload files**. If you cannot see it, open Chrome menu ⋮ and enable **Desktop site**.
4. Upload the extracted project's CONTENTS (not the outer folder): `package.json`, `capacitor.config.json`, `www` folder, `assets` folder, and `.github` folder. GitHub's web uploader may not preserve hidden `.github` folders on some mobile browsers. If it fails, use the browser's Desktop site; make sure `.github/workflows/build-apk.yml` exists in the repository after upload.
5. Tap **Commit changes**. Ensure the default branch is `main`.
6. Open **Actions** → **Build Mera Hisab Kitab APK** → **Run workflow** → **Run workflow**. If Actions are disabled, enable them in the repository's Actions settings.
7. Wait for a green successful run. Open the run, scroll to **Artifacts**, tap `Mera-Hisab-Kitab-APK` to download its ZIP.
8. Extract that artifact ZIP and tap `app-debug.apk`. Allow “Install unknown apps” for the browser/files app if Android asks. Only install the APK you built from your own repository.

## App features
- Income, expenses, categories, debts, bills/fees and budget
- Dark mode
- PDF report with a custom file name; choose **Save as PDF** in Android print dialog
- Visible Backup and Restore controls
- CSV export and charts

## Important
- This workflow has not been run here; no APK is included yet.
- Use JSON Backup regularly. Clearing app data can erase local records. Restore replaces current records, so backup first.
- Public repository means source code is visible. Do not upload your financial backup or private records to GitHub.
