# homeludens-care

홈루덴스 고객용 **AS·케어 신청** 양식 — https://care.homeludens.co.kr
카카오톡 채널 커스텀 메뉴에 이 주소를 연결합니다.

- 고객이 "AS 요청"을 고르면 AS 진행관리(as.homeludens.co.kr)에, "이용 중 아쉬웠던 점"을 고르면 클레임 보고서(claim.homeludens.co.kr)에 새 건으로 들어갑니다.
- 원본: `homeludens_materials/intake/index.html` → `bash homeludens_materials/deploy_care.sh "메모"` 로 올림.
- DB 쪽 규칙: `homeludens_materials/claim-app/supabase/intake.sql` (접수 함수 submit_customer_request, 고객 업로드는 정해진 폴더에 새 파일만).
- `config.js` 의 키는 공개용(anon)입니다. 비밀값은 넣지 않습니다.
