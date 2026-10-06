<p align="center">
  <img src="asset/bmwplay-icon.png" width="120" height="120" alt="BMWPlay icon" />
</p>

<h1 align="center">B M W P L A Y</h1>

<p align="center">
  CARPLAY RECEIVER · BMW X5 F15 · ANDROID
</p>

<p align="center">
  <a href="#english">English</a> &nbsp;·&nbsp; <a href="#繁體中文">繁體中文</a>
</p>

---

## English

BMWPlay turns an Android phone or tablet into a wired and wireless CarPlay receiver for the BMW X5 (F15). It has a clean black-and-white interface that follows the car's day/night mode.

### Features

| | |
|---|---|
| **Identity** | The iPhone sees the receiver as **BMW X5**. Manufacturer, model and OEM label default to BMW / X5 / BMW. |
| **BYD features** | HUD, instrument cluster, wheel keys, vehicle data and car-hotspot setup are disabled via `BydOutputSettings.BYD_FEATURES_ENABLED`. |
| **App** | Name `BMWPlay`, application ID `com.bmwplay.app`. |
| **Design** | Monochrome interface with square corners and hairline borders: white by day, black at night. It follows **Settings → CarPlay day/night mode**: *Always day* and *Always night* are fixed; *Follow Android system* and *Automatic (ambient light)* follow the car's day/night mode. The CarPlay connecting screen stays black. |

### Download

Download the APK from **[Releases](https://github.com/wuchunkei/BMWPlay/releases/latest)**.

Every push also builds an APK with GitHub Actions (**Actions → Build BMWPlay APK → Artifacts**).

Install it on the **Android receiver**, not on the iPhone.

### Important

This source build does **not** include an accessory identity, so on its own it cannot authenticate with an iPhone. See [docs/BUILD.md](docs/BUILD.md) for how identity assets are supplied to local release builds.

### Build from source

```sh
./gradlew :mobile:assembleDebug
```

Requires JDK 25 (as in CI) and the Android SDK. The output is `mobile/build/outputs/apk/debug/`.

### Documentation

- [Build from source](docs/BUILD.md)
- [Privacy and diagnostic reports](docs/PRIVACY.md)

---

## 繁體中文

BMWPlay 讓 Android 手機或平板變成 BMW X5（F15）用的有線／無線 CarPlay 接收器。介面是簡潔的黑白設計，會跟車子的日夜模式切換。

### 功能

| | |
|---|---|
| **車輛身份** | iPhone 會把接收器識別為 **BMW X5**，預設製造商／型號／OEM 標籤為 BMW / X5 / BMW。 |
| **BYD 功能** | 抬頭顯示、儀表板、方向盤按鍵、車輛數據和車載熱點設定，都經由 `BydOutputSettings.BYD_FEATURES_ENABLED` 關閉。 |
| **App** | 名稱 `BMWPlay`，套件 ID `com.bmwplay.app`。 |
| **設計** | 黑白單色介面，直角、細線框：白天白底黑字，夜間黑底白字。跟隨**設定 → CarPlay 日夜模式**：「固定日间」、「固定夜间」不會變；「跟隨 Android 系統」和「自動（環境光）」會跟車子的日夜模式切換。CarPlay 連線畫面維持黑色。 |

### 下載

到 **[Releases](https://github.com/wuchunkei/BMWPlay/releases/latest)** 下載 APK。

每次 push 也會由 GitHub Actions 自動編譯（**Actions → Build BMWPlay APK → Artifacts**）。

請安裝在 **Android 接收端**，不是 iPhone。

### 注意

這份原始碼**不含**配件身份檔，單靠它無法通過 iPhone 的認證。本機 release 版本如何提供身份檔，請看 [docs/BUILD.md](docs/BUILD.md)。

### 自行編譯

```sh
./gradlew :mobile:assembleDebug
```

需要 JDK 25（與 CI 相同）和 Android SDK，產出的 APK 在 `mobile/build/outputs/apk/debug/`。

---

## License and credits

BMWPlay is distributed under **GPL-3.0**. These credits are required by the upstream licenses:

- [DiPlay](https://github.com/shihabal3amri/DiPlay) by shihabal3amri, GPL-3.0
- [xcertplay](https://github.com/shilapi/xcertplay) by shilapi, GPL-3.0
- [DiAuto](https://github.com/shihabal3amri/DiAuto), AGPL-3.0, for the original home/settings layout

Full notices are in [docs/THIRD_PARTY_NOTICES.md](docs/THIRD_PARTY_NOTICES.md) and [docs/licenses](docs/licenses).

BMWPlay is not affiliated with or endorsed by BMW, Apple or BYD. CarPlay is a trademark of Apple Inc.; BMW and X5 are trademarks of BMW AG.
