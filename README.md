# OpenAiMami IDB

This repository publishes the i64 database archive for the AiMaMi restoration.

## Archives

### 1.2.3

- Files (split per platform to stay under upload limits):
  - `1.2.3/AiMaMi-1.2.3-macos.zip` — `66052555` bytes — SHA-256 `05241898975004eac9fc3f7b8bffccb57fb85dd3b94523491b9d41ebe6d987e3`
  - `1.2.3/AiMaMi-1.2.3-windows.zip` — `70509195` bytes — SHA-256 `20be2a423e4d2985ea8e475b2d1f26584cfa6ecbfd0db55dc0fa2dcca43687e4`
- Contents: macOS 1.2.3 and Windows 1.2.3 i64 databases (both platforms on the same version)

| Entry | Size | SHA-256 |
| --- | ---: | --- |
| `macos/AiMaMi-1.2.3-macos.i64` | `66052349` bytes | `4181da5dbd266ac06dc456893a63f4afafc7e73e0ddae9f920d5409882dca455` |
| `windows/AiMaMi-1.2.3-windows.i64` | `70508981` bytes | `f7ed942fdd1383463580b927d4b2123f63ed54b4f3ec9ba270f5e6800c87415c` |

> Both databases organise the application functions into a `codexmate_lib/...` module folder tree. The macOS (symbol-rich) database carries the full application function set with names, comments and module folders; the Windows (stripped) database recovers command handler names, cross-platform string-signature names and per-module attribution for the app's own functions.

### 1.2.2 / 1.2.1

- File: `1.2.2/AiMaMi-1.2.2-i64-databases.zip`
- Size: `64072296` bytes
- SHA-256: `3b6b89c4cd326655ce3f57ea4a2895d512db9358e063f1b00f333b78d424d7dc`
- Contents: macOS i64 database (Windows 1.2.1 i64 pending SMB sync — not yet in this archive)

| Entry | Size | SHA-256 |
| --- | ---: | --- |
| `macos/AiMaMi-1.2.2-macos.i64` | `291155498` bytes | `2cc36fb77f3d2a245659eb28a8a7391a82b6e091a30a5d97aa74872392780b22` |

> Platform versions diverge: macOS=1.2.2, Windows=1.2.1. Windows 1.2.1 i64 will be added when synced.

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
