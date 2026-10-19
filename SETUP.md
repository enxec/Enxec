# Enxec README 전체본

## 적용

`README.md`는 마지막에 제공한 원문의 파도 배너, 소개 문구, 조회수, Streak를 유지하고 AI·기술 카드와 깨진 activity graph 영역을 교체한 전체본입니다. 표기는 Enxec / PALDYN으로 맞췄습니다.

이전에 선택한 작업실 배너를 사용하려면 `README-workspace.md`의 내용을 저장소 루트 `README.md`로 사용하세요. 해당 배너는 `assets/enxec-workspace.png`에 포함되어 있으며, 이미지에는 Enxec만 표시됩니다.

`assets/`와 `.github/`도 저장소 루트에 함께 올리세요. 기존 폴더는 삭제하지 말고 합칩니다. 라이선스 파일과 THIRD-PARTY-NOTICES.md도 함께 보관하세요. `README.md` 코드만 붙여넣고 이미지 파일을 생략하면 로컬 이미지가 표시되지 않습니다.

## Snake 갱신

포함된 `.github/workflows/readme-snake.yml`을 enxec/enxec의 기본 브랜치에 올린 후, Actions → Update contribution snake → Run workflow를 실행하세요. `.github`는 숨김 폴더입니다.

워크플로는 두 Snake SVG만 갱신하도록 구성했으며, README와 기술 배지는 수정하지 않습니다. GitHub의 기본 토큰을 사용합니다. 저장소/조직 정책이나 브랜치 보호가 직접 푸시를 막는 경우 별도 권한 검토가 필요합니다. 해당 정책은 임의로 해제하지 마세요.

설치 직후 사용할 초기 Snake SVG는 이전 패키지에 포함된 2026-10-19 스냅샷입니다. 이번 전체본 작업에서 기여 데이터를 새로 조회한 것은 아닙니다. 첫 실행 성공 후 생성된 결과로 교체됩니다.

예약은 기존 워크플로의 하루 한 번 설정을 유지했습니다. 실제 실행 시점이나 성공을 보장하는 것은 아니므로 Actions 기록에서 확인하세요. 사용자 저장소에 업로드하거나 워크플로를 실행한 상태는 아닙니다.

## 표시와 외부 서비스

AI·기술 카드와 Snake는 패키지 안의 SVG를 읽습니다. 작업실 배너도 로컬 PNG입니다. 원문의 파도 배너·조회수·Streak는 기존 외부 서비스 주소를 그대로 사용하므로, 그 서비스에 문제가 생기면 해당 이미지는 표시되지 않을 수 있습니다. 이번 작업에서 외부 이미지 서비스의 응답은 확인하지 않았습니다.

로컬 파일 존재, SVG XML, README의 이미지 경로, 워크플로 YAML을 검사했습니다. GitHub 페이지에서의 실제 렌더링은 확인하지 않았습니다.

참고:
- https://github.com/Platane/snk
- https://raw.githubusercontent.com/Platane/snk/v3/svg-only/action.yml
- https://raw.githubusercontent.com/actions/checkout/v7/action.yml
