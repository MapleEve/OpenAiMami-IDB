# OpenAiMami IDB

This repository publishes the i64 database archive for the AiMaMi restoration.

## 这是什么 / What this is

AiMaMi 是一个闭源的 Rust + Tauri 2 桌面应用。本仓单独发布它的 **IDA 参考数据库（.i64）**，供 [OpenAiMami](https://github.com/MapleEve/OpenAiMaMi) 主仓库的脱敏文本证据链回指核对。主仓库不直接保存大体积 `.i64` 文件，IDB 作为独立 Git LFS 资产存在，保持与主仓库源码历史分离。

每个版本的数据库都已把应用自身函数按 `codexmate_lib/...` 模块路径归入 IDA function folder 目录树：
- **macOS（带符号）**：全量应用函数命名 + 注释 + 模块目录树。
- **Windows（strip 后）**：恢复命令 handler 名 + 跨平台字符串签名名 + 按模块归属（panic-Location 锚定 + 严格调用图传播）。

## 如何使用 / How to use

```bash
# 克隆（跳过 LFS 大文件下载，按需取）
GIT_LFS_SKIP_SMUDGE=1 git clone https://github.com/MapleEve/OpenAiMami-IDB.git
cd OpenAiMami-IDB

# 按需拉取某版本的 archive
git lfs pull --include="1.2.3/*"

# 解压
unzip 1.2.3/AiMaMi-1.2.3-macos.zip    # -> macos/AiMaMi-1.2.3-macos.i64
unzip 1.2.3/AiMaMi-1.2.3-windows.zip  # -> windows/AiMaMi-1.2.3-windows.i64
```

用 IDA Pro 9.3+ 打开 `.i64`，在 Functions 窗口按 `codexmate_lib/...` 目录树浏览。

## Archives

### 1.2.3

- Files (split per platform to stay under upload limits):
  - `1.2.3/AiMaMi-1.2.3-macos.zip` — `87445656` bytes — SHA-256 `f227bc5565a4977916cefa9cf5e5ac92745541229fba5cb0f2c128832d137b1d`
  - `1.2.3/AiMaMi-1.2.3-windows.zip` — `101505379` bytes — SHA-256 `3d46c1fc5f778b8110f6e8c1b05ef2a949aa5b559564d7f26c42a89692332a68`
- Contents: macOS 1.2.3 and Windows 1.2.3 i64 databases (both platforms on the same version, current baseline)

| Entry | Size | SHA-256 |
| --- | ---: | --- |
| `macos/AiMaMi-1.2.3-macos.i64` | `87445450` bytes | `2948a65eb86f525702bd018f4486ddbe5113cc1859ce8ad3d9b9cb4fb2d4e758` |
| `windows/AiMaMi-1.2.3-windows.i64` | `101505165` bytes | `29d948bf85dd48ed54b33c10642efd9cc6c33e3e88b88fed1e2f2831edbd9eff` |

> 1.2.3 是当前 baseline。macOS 库承载全量 1638 个应用函数的命名+注释+目录树；Windows（strip）库恢复 115 个命令 handler 真名 + 242 个跨平台字符串签名名 + 938 个函数的按模块归属。对应脱敏证据见 OpenAiMami 主仓 `evidence/full-chain/` 下 1.2.3。

### 1.2.2 / 1.2.1

- File: `1.2.2/AiMaMi-1.2.2-i64-databases.zip`
- Size: `117553032` bytes
- SHA-256: `f65d1e2cea971c37b059bf558e7e5aa51ad5957d9a4e9145bf7da9470f8cecda`
- Contents: macOS 1.2.2 and Windows 1.2.1 i64 databases

| Entry | Size | SHA-256 |
| --- | ---: | --- |
| `macos/AiMaMi-1.2.2-macos.i64` | `48981731` bytes | `637d2e0c3a66717d6313c5aa7b2f00de3b2ed794823677a0f779b85811ebf7d1` |
| `windows/AiMaMi-1.2.1-windows.i64` | `68570619` bytes | `98b4aa7bed9800d93638817e7fc06833491cdcf4af9350f2a5b7f13697430681` |

> Platform versions diverge: macOS=1.2.2, Windows=1.2.1. Both databases organise the application functions into a `codexmate_lib/...` module folder tree; the Windows (stripped) database additionally recovers command handler names and per-module attribution for the app's own functions.

### 1.1.8

- File: `1.1.8/AiMaMi-1.1.8-i64-databases.zip`
- Size: `117621545` bytes
- SHA-256: `439dd41b5217020e30088cc45cb0add337997985501201f580cb54013276cbe6`
- Contents: macOS and Windows i64 databases

| Entry | Size | SHA-256 |
| --- | ---: | --- |
| `macos/AiMaMi-1.1.8-macos.i64` | `56890831` bytes | `3bc94bdbd30d1a1206d9733806000d278967f76f242fcac75b5d45349df7b904` |
| `windows/AiMaMi-1.1.8-windows.i64` | `62276896` bytes | `01878495032aca39a123c9d0008c73bce10032255f5939baf5328b16b49c317b` |

> macOS entry is the x86_64 slice analysis database for 1.1.8.

### 1.1.1

- File: `1.1.1/AiMaMi-1.1.1-i64-databases.zip`
- Size: `132908153` bytes
- SHA-256: `31347fa9146f7c68b271158cdd7d4ab8413f9510439e09df157a87f2ead91b68`
- Contents: macOS and Windows i64 databases

| Entry | Size | SHA-256 |
| --- | ---: | --- |
| `macos/AiMaMi-1.1.1-macos.i64` | `196278010` bytes | `b8ad5b96491b8512742ad58cbbaa252175fdac3955833404810fe3d8c041b0f6` |
| `windows/AiMaMi-1.1.1-windows.i64` | `375327078` bytes | `ebf7bc745ebf3332d5596a29c0ca5654b8f959cab16de67f46caa46761cd3e5d` |

### 1.0.9

- File: `1.0.9/AiMaMi-1.0.9-i64-databases.zip`
- Size: `858599362` bytes
- SHA-256: `7fce9b1e319b5eca8ab6216974b069b57baea3d9f177699f0383d5ea46d39825`
- Contents: macOS and Windows i64 databases

The main OpenAiMami repository can reference this archive instead of storing it in source history.
Keep this repository independent so the IDB Git LFS payload remains separate from the main repository.
