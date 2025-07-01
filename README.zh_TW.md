# fcitx5-boshiamy

## 簡介

`fcitx5-boshiamy` 是一個為 Fcitx5 輸入法框架提供嘸蝦米輸入法支援的獨立模組。本專案從原始的 [fcitx5-table-extra](https://github.com/fcitx/fcitx5-table-extra) 倉庫中提取嘸蝦米碼表，使其能夠獨立使用。

## 需求

- 執行時依賴：`fcitx5-im`、`fcitx5-chinese-addons`、`libime`
- 建置依賴：`cmake`、`extra-cmake-modules`、`boost`

## 建置與安裝

```bash
mkdir build
cd build
cmake .. -DCMAKE_INSTALL_PREFIX=<fcitx 的安裝路徑>
cmake --build .
cmake --install .  # 可能需要使用 root 權限
```
## 專案概覽
本專案為從原始[fcitx5-table-extra](https://github.com/fcitx/fcitx5-table-extra)倉庫中獨立提取出的嘸蝦米碼表，方便單獨使用。

## 聲明
本專案**非原始** fcitx5-table-extra 專案或 Fcitx 團隊官方維護，僅為個人提取與修改方便使用之版本。

原始碼與資料均遵循 fcitx5-table-extra 所屬的版權與授權規範。

本套件程式碼依 GPLv3（或更新版本）授權釋出。
