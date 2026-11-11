# 10F / 10DAY — 작업 메모 (배운 점·고친 오류)

- v1.0.13: Set/Map은 JSON.stringify하면 `{}`가 됨 → 저장할 땐 배열로(`[...set]`), 불러올 땐 `new Set(arr)`로 되살릴 것. (G.visited 휴식세이브 후 `G.visited.add is not a function` 크래시)
- v1.0.14: 쓰러진 뒤 0.9초(die→ending 대기) 동안 E·키 입력이 먹혀 계단으로 내려가 저장될 수 있었음 → interact·keydown에서 P.dead면 무시.
- v1.0.14: 로딩(boot) 끝나기 전 lobbyAct가 불리면 텍스처(TX) 없이 buildFloor가 돌아 크래시 → G.booted 전엔 로비 입력 무시.
- 테스트: `?dev` 로 열면 window.__g(step·interact 등) 노출 → 헤드리스 봇으로 10~1층·엔딩·터치 자동 점검 가능.
