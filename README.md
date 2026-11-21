# Zall RW APK build

Repository khusus untuk pemulihan dan build **APK utama Zall RW**.

## Status awal
- Workflow build disiapkan untuk source hasil decompile Apktool.
- Source aplikasi utama belum dimasukkan ke repository ini.
- APK Admin `com.zallrw.admin` bukan source APK utama dan tidak digunakan sebagai pengganti.

## Menambahkan source
Letakkan arsip source Apktool yang benar di:
`source/Zall_RW_src_patched.zip`

Arsip harus berisi folder project dengan `AndroidManifest.xml`, `smali/`, `res/`, dan file Apktool terkait. Jangan memasukkan file rahasia atau private signing key ke repository.

## Build
Buka tab **Actions** → **Build Zall RW APK** → **Run workflow**.
Workflow akan memeriksa source, membangun APK unsigned, lalu mengunggah hasil build sebagai artifact.

## Batasan
Build artifact belum dianggap APK rilis siap pasang. APK perlu ditandatangani dengan signing key asli yang sah, diverifikasi, lalu diuji startup di emulator. Jangan mengganti package ID atau mengubah fitur utama saat mengintegrasikan redeem.
