# LotteryRecord

RARA の VRChat ワールド（宝くじワールド）の、全世界の当せん記録です。
ワールドはこのリポジトリの GitHub Pages に置いた `winners.json` を読み込み、
殿堂ボードと全世界の残り本数を表示します。

このワールドのくじは架空のもので、実在の宝くじとは関係ありません。
ワールドの中のお金も架空のもので、換金などは一切できません。

## winners.json

```json
{
  "sale": 0,
  "updated": "2026-10-03T00:00:00+09:00",
  "remaining": {},
  "claims": [
    { "i": 0, "tier": "t1", "u": 1, "k": 1, "n": 100000, "name": "...", "time": "2026-10-03T00:00:00+09:00" }
  ]
}
```

- `sale`: 発売回（0 = 試作用の縮小版）
- `remaining`: 等級ごとの全世界の残り本数（省略時はワールド側で本数から計算）
- `claims`: 当せん済みの券。`i` は全世界で一意の券の通し番号、`u` ユニット、`k` 組、`n` 番号

---

Global record of top prizes for RARA's lottery world in VRChat. The world reads `winners.json`
from this repository's GitHub Pages. The lottery and the money in the world are fictional.
