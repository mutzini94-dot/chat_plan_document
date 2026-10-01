# chat_plan_document

`index.html`은 암호화된 기획 문서입니다. 브라우저로 열고 작성자 비밀번호를 입력하면 문서가 브라우저 안에서 복호화되어 열립니다.
저장소에는 암호문만 들어 있어 비밀번호 없이는 내용을 읽을 수 없습니다. (PBKDF2-SHA256 600,000회 · AES-256-GCM)

비밀번호는 저장소에 기록하지 않습니다. 작성자에게 문의하세요.

## 댓글

문서 안의 댓글은 이 저장소의 `chat-plan-db` 이슈에 저장됩니다. 이슈의 본문과 댓글은 모두 문서 비밀번호로 암호화되어 있어 공개 저장소에서도 내용이 보이지 않습니다. 이 이슈를 직접 수정하거나 닫지 마세요.

처음 한 번, 저장소 소유자가 문서를 열어 왼쪽 패널의 **저장소 연결하기**에서 토큰을 연결해야 합니다.

1. GitHub → Settings → Developer settings → Fine-grained tokens → Generate new token
2. Repository access: Only select repositories → `chat_plan_document`
3. Repository permissions → **Issues: Read and write** (다른 권한은 주지 않습니다)
4. 문서의 연결 창에 토큰 붙여 넣기

댓글을 보고 쓰려면 문서가 `https://` 주소로 열려야 합니다. Settings → Pages에서 `main` 브랜치를 배포하면 됩니다.
