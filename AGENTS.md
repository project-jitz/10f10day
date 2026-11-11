# 10F / 10DAY — 작업 메모 (배운 점·고친 오류)

- v1.0.13: Set/Map은 JSON.stringify하면 `{}`가 됨 → 저장할 땐 배열로(`[...set]`), 불러올 땐 `new Set(arr)`로 되살릴 것. (G.visited 휴식세이브 후 `G.visited.add is not a function` 크래시)
