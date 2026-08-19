# Knights College Cursor

Animated cursor packs for Knights College characters. Windows installers are
included; macOS users can convert the same packages with MaCursor.

Created and packaged by **@Neilzou1**.

## Latest Update

**v1.4.0 adds Argo, Grantly, and Oscar as ready-to-install Windows packs.**
Each new ZIP contains 13 animated cursor states, transparent previews, and
current-user install, apply, restore, and uninstall helpers.

## Pointer Preview

| Argo | Grantly | Oscar |
| --- | --- | --- |
| ![Argo pointer preview](packs/argo/preview/pointer.gif) | ![Grantly pointer preview](packs/grantly/preview/pointer.gif) | ![Oscar pointer preview](packs/oscar/preview/pointer.gif) |

| Diderich | Theo | Paul | Celio | Li Jun |
| --- | --- | --- | --- | --- |
| ![Diderich pointer preview](packs/diderich/preview/pointer.gif) | ![Theo pointer preview](preview/pointer.gif) | ![Paul pointer preview](packs/paul/preview/pointer.gif) | ![Celio pointer preview](packs/celio/preview/pointer.gif) | ![Li Jun pointer preview](packs/lijun/preview/pointer.gif) |

## Download

Download from the GitHub Releases page, then extract the ZIP before installing.

- Latest release:
  [Knights College Cursor v1.4.0](https://github.com/Theozou-159/KnightsCollegeCursor/releases/tag/v1.4.0)
- New in v1.4.0:
  - `ArgoCursor-v1.0.0-Windows-Default-by-Neilzou1.zip`
  - `GrantlyCursor-v0.1.0-Windows-by-Neilzou1.zip`
  - `OscarCursor-v0.1.1-Windows-Default-by-Neilzou1.zip`
- Previous Diderich, Theo, and Li Jun downloads:
  [Knights College Cursor v1.3.0](https://github.com/Theozou-159/KnightsCollegeCursor/releases/tag/v1.3.0)
  includes:
  - `DiderichCursor-v1.1.6-Windows-Default-FunctionalHotspotFix-by-Neilzou1.zip`
  - `TheoCursor-v2.0.0-Windows-Default-by-Neilzou1.zip`
  - `LiJunCursor-v1.0.1-Windows-Default-by-Neilzou1.zip`
- Existing Paul and Celio downloads:
  [Knights College Cursor v1.2.0](https://github.com/Theozou-159/KnightsCollegeCursor/releases/tag/v1.2.0)
  includes:
  - `PaulCursor-v1.0.0-Windows-All-Sizes-by-Neilzou1.zip`
  - `CelioCursor-v0.1.0-Windows-All-Sizes-by-Neilzou1.zip`
- Existing Diderich downloads:
  [Knights College Cursor v1.1.1](https://github.com/Theozou-159/KnightsCollegeCursor/releases/tag/v1.1.1)
  includes:
  - `DiderichCursor-v1.0.0-Windows-1080p-by-Neilzou1.zip`
  - `DiderichCursor-v1.0.0-Windows-2K-by-Neilzou1.zip`
  - `DiderichCursor-v1.0.0-Windows-4K-by-Neilzou1.zip`
  - `DiderichCursor-v1.0.0-Windows-Large105-by-Neilzou1.zip`
  - `DiderichCursor-v1.0.0-Windows-XL110-by-Neilzou1.zip`
- Existing Theo download:
  - `TheoCursor-v1.0.0-Windows-by-Neilzou1.zip`

## Size Guide

Paul and Celio all-size ZIPs contain these folders:

- `Default`: the standard pack.
- `1080p`: smaller, for FHD screens.
- `2K`: medium-small, for QHD screens.
- `4K`: approved baseline scale, labeled for high-DPI screens.
- `Large105`: slightly larger than the baseline.
- `XL110`: largest test size with fit protection.

Each size uses its own Windows cursor scheme and install folder, so several
sizes can be installed and tested side by side.

The Argo, Grantly, and Oscar downloads are ready-to-install Default-size Windows
cursor packages. Diderich's older all-size download stays available from v1.2.0
for users who need the legacy size variants.

## Install

1. Download the character ZIP from Releases.
2. Extract the ZIP.
3. For Paul or Celio, open the size folder you want.
4. Double-click the install `.bat` file:
   - Diderich: `Install-Diderich-Cursors.bat`
   - Theo v2: `Install-TheoCursor-v2-Cursors.bat`
   - Paul: `Install-Paul-Cursors.bat`
   - Celio: `Install-Celio-Cursors.bat`
   - Li Jun: `Install-LiJun-Cursors.bat`
   - Argo: `Install-Argo-Cursors.bat`
   - Grantly: `Install-Grantly-Cursors.bat`
   - Oscar: `Install-Oscar-Cursors.bat`
5. If Windows Defender SmartScreen appears, choose **More info** -> **Run
   anyway** only if you trust this package.

The installers register their schemes without changing your current cursor by
default. To switch later, open **Mouse Properties** -> **Pointers**, choose the
character scheme, then click **Apply**. The optional `Apply-*-Cursors.bat`
scripts install and switch immediately.

The installers copy cursor files to the current user's local app data folder,
for example:

```text
%LOCALAPPDATA%\DiderichCursor\Cursors
%LOCALAPPDATA%\TheoCursor\Cursors
%LOCALAPPDATA%\PaulCursor\Cursors
%LOCALAPPDATA%\PaulCursor2K\Cursors
%LOCALAPPDATA%\CelioCursor\Cursors
%LOCALAPPDATA%\CelioCursor2K\Cursors
%LOCALAPPDATA%\LiJunCursor\Cursors
%LOCALAPPDATA%\ArgoCursor\Cursors
%LOCALAPPDATA%\GrantlyCursor\Cursors
%LOCALAPPDATA%\OscarCursor\Cursors
```

All installers back up the Windows cursor scheme list before registering a new
scheme:

```text
%LOCALAPPDATA%\KnightsCollegeCursor\CursorSchemeBackups
```

If a test install ever leaves the Windows scheme list in a bad state, run
`Restore-Cursor-Scheme-Backup.bat` from the character package to restore the
latest saved scheme list.

## macOS With MaCursor

The downloads use Windows `.cur` and `.ani` files. On macOS 15 Sequoia or
later, [MaCursor](https://github.com/writronic/MaCursor) can convert them into
a native macOS cursor theme:

1. Install the latest MaCursor `.dmg` from its Releases page.
2. Download and fully extract the Argo, Grantly, or Oscar ZIP from this
   project's Releases page.
3. In MaCursor, choose **File -> Convert Theme...** (`Shift-Command-O`) and
   select the extracted character folder containing the `.inf` file and
   `cursors` folder.
4. Review **Mapped** and **Warnings & ignored**. Choose **Add & Edit...** if
   you want to check the cursor mapping, animation, or hotspots first.
5. Click **Add to Library**, select the imported theme, and click **Apply**.
6. Optional: open **MaCursor -> Settings -> General** and install the
   **Helper Tool** so the theme is reapplied after login or a user switch.

Use MaCursor's **Restore** button to return to the default macOS cursors.
MaCursor is a third-party application and is not bundled with this project.

## Included Cursor States

Each character pack includes:

- Normal Select
- Help Select
- Working in Background
- Busy
- Precision Select
- Text Select
- Unavailable
- Vertical Resize
- Horizontal Resize
- Diagonal Resize NW-SE
- Diagonal Resize NE-SW
- Move
- Link Select

## More Previews

Diderich:

- [Latest transparent Pointer preview](packs/diderich/preview/pointer.gif)
- [Final contact sheet](packs/diderich/preview/diderich-cursor-final-contact-sheet.png)
- [32px review sheet](packs/diderich/preview/diderich-cursor-final-32px-review.png)
- [Hotspot review sheet](packs/diderich/preview/diderich-cursor-final-hotspot-review.png)
- [Dark background check](packs/diderich/preview/diderich-cursor-final-dark-mode-check.png)

Theo:

- [Latest transparent Pointer preview](preview/pointer.gif)
- [Final contact sheet](preview/theo-cursor-final-contact-sheet.png)
- [32px review sheet](preview/theo-cursor-final-32px-review.png)
- [Hotspot review sheet](preview/theo-cursor-final-hotspot-review.png)
- [Dark-mode eye check](preview/theo-cursor-final-dark-mode-eye-check.png)

Li Jun:

- [Transparent Pointer preview](packs/lijun/preview/pointer.gif)

Argo, Grantly, and Oscar:

- [Argo Pointer preview](packs/argo/preview/pointer.gif)
- [Grantly Pointer preview](packs/grantly/preview/pointer.gif)
- [Oscar Pointer preview](packs/oscar/preview/pointer.gif)

## Manual Install

If the one-click script does not work:

1. Right-click the `.inf` file.
2. Choose **Install**.
3. Open **Mouse Properties** -> **Pointers**.
4. Choose the matching cursor scheme.

You can also manually choose individual files from the `cursors` folder.

## License And Asset Notice

Installer and uninstall scripts are licensed under the MIT License. See
[`SCRIPT_LICENSE.md`](SCRIPT_LICENSE.md).

Character artwork, cursor images, animations, and preview assets are not covered
by the MIT License. They are fan-made derivative assets based on third-party
game characters. All rights to the original characters and source artwork belong
to their respective owners. See [`ASSET_NOTICE.md`](ASSET_NOTICE.md).

This project is unofficial, non-commercial, and not affiliated with the original
rights holder. Please do not sell, commercially redistribute, or reuse the
artwork/assets as your own.

---

## 中文说明

Knights College Cursor 是一套角色动态鼠标指针包，目前包含迪德里奇、西奥、保罗、
西里奥、李军、亚戈、格兰特利和奥斯卡八套角色主题。压缩包内含 Windows 安装器；
macOS 用户可以通过 MaCursor 转换同一套 `.cur` 和 `.ani` 文件。

制作与打包：**@Neilzou1**。

### 最新更新

**v1.4.0 新增亚戈、格兰特利和奥斯卡三套可直接安装的 Windows 鼠标包。**
每个新 ZIP 都包含 13 个动态鼠标状态、透明预览，以及安装、立即应用、恢复和卸载
辅助脚本。

### 指针预览

| 亚戈 | 格兰特利 | 奥斯卡 |
| --- | --- | --- |
| ![Argo pointer preview](packs/argo/preview/pointer.gif) | ![Grantly pointer preview](packs/grantly/preview/pointer.gif) | ![Oscar pointer preview](packs/oscar/preview/pointer.gif) |

| 迪德里奇 | 西奥 | 保罗 | 西里奥 | 李军 |
| --- | --- | --- | --- | --- |
| ![Diderich pointer preview](packs/diderich/preview/pointer.gif) | ![Theo pointer preview](preview/pointer.gif) | ![Paul pointer preview](packs/paul/preview/pointer.gif) | ![Celio pointer preview](packs/celio/preview/pointer.gif) | ![Li Jun pointer preview](packs/lijun/preview/pointer.gif) |

### 下载

请从 GitHub Releases 下载角色 ZIP，下载后先解压再安装。

- 最新 Release：
  [Knights College Cursor v1.4.0](https://github.com/Theozou-159/KnightsCollegeCursor/releases/tag/v1.4.0)
- v1.4.0 新增：
  - `ArgoCursor-v1.0.0-Windows-Default-by-Neilzou1.zip`
  - `GrantlyCursor-v0.1.0-Windows-by-Neilzou1.zip`
  - `OscarCursor-v0.1.1-Windows-Default-by-Neilzou1.zip`
- 之前的迪德里奇、西奥和李军下载：
  [Knights College Cursor v1.3.0](https://github.com/Theozou-159/KnightsCollegeCursor/releases/tag/v1.3.0)
  里包含：
  - `DiderichCursor-v1.1.6-Windows-Default-FunctionalHotspotFix-by-Neilzou1.zip`
  - `TheoCursor-v2.0.0-Windows-Default-by-Neilzou1.zip`
  - `LiJunCursor-v1.0.1-Windows-Default-by-Neilzou1.zip`
- 已有保罗和西里奥下载：
  [Knights College Cursor v1.2.0](https://github.com/Theozou-159/KnightsCollegeCursor/releases/tag/v1.2.0)
  里包含：
  - `PaulCursor-v1.0.0-Windows-All-Sizes-by-Neilzou1.zip`
  - `CelioCursor-v0.1.0-Windows-All-Sizes-by-Neilzou1.zip`
- 已有迪德里奇下载：
  [Knights College Cursor v1.1.1](https://github.com/Theozou-159/KnightsCollegeCursor/releases/tag/v1.1.1)
  里包含：
  - `DiderichCursor-v1.0.0-Windows-1080p-by-Neilzou1.zip`
  - `DiderichCursor-v1.0.0-Windows-2K-by-Neilzou1.zip`
  - `DiderichCursor-v1.0.0-Windows-4K-by-Neilzou1.zip`
  - `DiderichCursor-v1.0.0-Windows-Large105-by-Neilzou1.zip`
  - `DiderichCursor-v1.0.0-Windows-XL110-by-Neilzou1.zip`
- 已有西奥下载：
  - `TheoCursor-v1.0.0-Windows-by-Neilzou1.zip`

### 尺寸说明

保罗和西里奥的 All Sizes ZIP 里包含这些文件夹：

- `Default`：标准尺寸。
- `1080p`：偏小，适合 FHD 屏幕。
- `2K`：中小尺寸，适合 QHD 屏幕。
- `4K`：基准尺寸，适合高 DPI 屏幕。
- `Large105`：比基准尺寸稍大。
- `XL110`：最大的测试尺寸，带防裁切处理。

每个尺寸都有独立 Windows 鼠标方案名和安装目录，可以同时安装，方便并排试。

亚戈、格兰特利和奥斯卡都是可以直接安装的 Windows 默认尺寸鼠标包。需要旧版
迪德里奇多尺寸包的用户，仍可从 v1.2.0 下载旧版 All Sizes ZIP。

### 安装

1. 从 Releases 下载角色 ZIP。
2. 解压 ZIP。
3. 如果是保罗或西里奥，先打开你想用的尺寸文件夹。
4. 双击安装 `.bat`：
   - 迪德里奇：`Install-Diderich-Cursors.bat`
   - 西奥 v2：`Install-TheoCursor-v2-Cursors.bat`
   - 保罗：`Install-Paul-Cursors.bat`
   - 西里奥：`Install-Celio-Cursors.bat`
   - 李军：`Install-LiJun-Cursors.bat`
   - 亚戈：`Install-Argo-Cursors.bat`
   - 格兰特利：`Install-Grantly-Cursors.bat`
   - 奥斯卡：`Install-Oscar-Cursors.bat`
5. 如果 Windows Defender SmartScreen 弹出提示，请只在你信任这个包的情况下选择
   **More info** -> **Run anyway**。

安装脚本默认只注册鼠标方案，不会立刻改掉你当前正在用的鼠标。想切换时，请打开
**Mouse Properties** -> **Pointers**，在 **Scheme** 里选择对应角色方案，再点
**Apply**。如果想立刻切换，也可以运行 `Apply-*-Cursors.bat`。

安装脚本会在注册新方案前先备份 Windows 的鼠标方案列表：

```text
%LOCALAPPDATA%\KnightsCollegeCursor\CursorSchemeBackups
```

如果测试安装后 Windows 的方案列表异常，可以运行对应角色包里的
`Restore-Cursor-Scheme-Backup.bat`，恢复最近一次保存的方案列表。

### 在 macOS 上使用 MaCursor

macOS 15 Sequoia 或更新版本可以使用第三方应用
[MaCursor](https://github.com/writronic/MaCursor) 转换这些 Windows 鼠标文件：

1. 从 MaCursor 的 Releases 页面下载最新版 `.dmg` 并安装。
2. 从本项目 Releases 页面下载亚戈、格兰特利或奥斯卡 ZIP，并完整解压。
3. 在 MaCursor 中选择 **File -> Convert Theme...**（`Shift-Command-O`），
   选择解压后的角色文件夹；该文件夹中应有 `.inf` 文件和 `cursors` 文件夹。
4. 检查 **Mapped** 和 **Warnings & ignored**。如需先核对映射、动画或热点，选择
   **Add & Edit...**。
5. 点击 **Add to Library**，选中导入的主题，再点击 **Apply**。
6. 可选：打开 **MaCursor -> Settings -> General**，安装 **Helper Tool**，让主题在
   登录或切换用户后自动重新应用。

如需恢复系统鼠标，点击 MaCursor 工具栏中的 **Restore**。MaCursor 是第三方应用，
不包含在本项目下载包内。

### 包含的鼠标状态

每套角色包都包含：

- 普通选择
- 帮助选择
- 后台运行
- 忙碌
- 精确选择
- 文本选择
- 不可用
- 垂直缩放
- 水平缩放
- 对角线缩放 NW-SE
- 对角线缩放 NE-SW
- 移动
- 链接选择

### 手动安装

如果一键安装脚本无法运行：

1. 右键点击 `.inf` 文件。
2. 选择 **Install**。
3. 打开 **Mouse Properties** -> **Pointers**。
4. 选择对应的鼠标方案。

也可以从 `cursors` 文件夹里手动为每个鼠标状态选择对应文件。

### 最新透明 Pointer 预览

- [迪德里奇](packs/diderich/preview/pointer.gif)
- [西奥](preview/pointer.gif)
- [李军](packs/lijun/preview/pointer.gif)
- [亚戈](packs/argo/preview/pointer.gif)
- [格兰特利](packs/grantly/preview/pointer.gif)
- [奥斯卡](packs/oscar/preview/pointer.gif)

### 许可与素材说明

安装和卸载脚本使用 MIT License，见 [`SCRIPT_LICENSE.md`](SCRIPT_LICENSE.md)。

角色图像、鼠标图像、动画和预览素材不适用 MIT License。这些素材是基于第三方
游戏角色制作的非官方 fan-made derivative assets。原角色和原始素材的权利归对应
权利方所有，见 [`ASSET_NOTICE.md`](ASSET_NOTICE.md)。

本项目为非官方、非商业、个人使用向项目，与原权利方无关联。请不要出售、商业再
分发，或把其中的图像/素材当作自己的素材复用。
