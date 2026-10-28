# 2027 KBO 스토브리그

KBO 10개 구단의 2027 시즌 대비 이동(FA, 외국인 선수, 트레이드·영입, 드래프트, 방출·은퇴, 감독·코치)을 영입(+)과 유출(−)로 정리한 개인용 사이트입니다.

- 사이트: https://woojung37.github.io/2027-kbo/
- 데이터: `data/data.json` (매일 1회 갱신)
- 루머는 각 구단 페이지의 별도 섹션에 두고 +/− 합계에는 넣지 않습니다.

## 데이터 형식

`teams.<구단 id>` 아래에 다음 필드가 있습니다.

| 필드 | 설명 |
|---|---|
| `season2026` | 2026 시즌 성적 한 줄 |
| `items[]` | 확정·유력 이동. `cat`(fa, foreign, trade, draft, exit, coach), `dir`(in, out, stay), `name`, `pos`, `detail`, `status`(확정, 유력), `date`, `source`, `url` |
| `rumors[]` | 미확정 소문. `cat`, `dir`, `name`, `text`, `date`, `source`, `url` |
| `roster` | `foreign[]`, `fa[]`(FA 자격 예정), `notes[]` |
| `outlook` | `summary`, `strengths[]`, `weaknesses[]` |
