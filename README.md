# 원신 파티 DPS 분석

캐릭터 4명을 골라 [gcsim](https://github.com/genshinsim/gcsim)을 브라우저 안에서 돌려 파티 DPS를 계산하는 사이트입니다.
무기·성유물·운명의 자리 순위, 성유물 주옵션·부옵션 자동 최적화, KQM DB 로테이션을 지원합니다.

사이트: https://kij00ng.github.io/genshin-dps/

## 파일
| 파일 | 내용 |
|---|---|
| `index.html` | 사이트 전체 (화면, 로테이션 조립, 최적화, 순위 계산) |
| `gcsim.wasm` | gcsim을 WebAssembly로 빌드한 것 (gzip 압축) |
| `wasm_exec.js` | Go WebAssembly 실행 도우미 (Go 배포본) |
| `kqm_presets.json` | KQM DB에 공유된 gcsim 설정에서 가져온 파티별 로테이션·장비 |

## 출처와 라이선스
- **gcsim**: Copyright (c) 2021 The gcsim contributors, [AGPL-3.0](LICENSE).
  이 사이트의 `gcsim.wasm`은 캐릭터를 추가·수정한 버전이며, 소스는 https://github.com/kij00ng/gcsim/tree/site-chars 에 있습니다.
- **이 사이트의 코드**도 같은 AGPL-3.0을 따릅니다.
- **KQM DB 로테이션**: [db.kqm.gg](https://db.kqm.gg)에 공유된 설정에서 가져왔습니다.
- **한국어 명칭**: genshin-db 데이터.
- **캐릭터 그림**: 게임 기본 초상화를 [enka.network](https://enka.network)에서 불러옵니다 (저장소에는 그림 파일이 없습니다).
- 원신(Genshin Impact)의 이름과 게임 데이터는 HoYoverse의 것이며, 이 사이트는 HoYoverse·KQM과 관계없는 개인 팬 사이트입니다.
