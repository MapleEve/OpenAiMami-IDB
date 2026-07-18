# OpenAiMami IDB

This repository publishes the i64 database archive for the AiMaMi restoration.

## Archives

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
