# Hẹn hò 3D 1-1 — APK

Hai người thật gặp nhau bằng avatar 3D chibi trên quả cầu công viên
(nơi gặp gỡ) rồi hẹn hò riêng trong quán cà phê (nơi hẹn hò), đồng bộ
qua Firebase Realtime DB. Bản web đóng gói APK bằng Capacitor 6.

- Package: `com.henho.online`
- Version: 1.0.0 (versionCode 1)
- Build: GitHub Actions (`.github/workflows/build-apk.yml`) chạy
  `./gradlew assembleDebug`, APK ở artifact `hen-ho-3d-apk`.
- App cần mạng để kết nối máy chủ Firebase (chat, hiện diện, lời mời).

Icon launcher: `assets-b64/icon.png.b64` (base64, vì đường đẩy GitHub
chỉ nhận text) — CI giải mã bằng `scripts/decode-assets.sh` rồi
`scripts/make-launcher-icon.py` tạo adaptive icon.
