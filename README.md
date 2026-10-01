# chat_plan_document

`index.html`은 암호화된 기획 문서입니다. 브라우저로 열고 작성자 비밀번호를 입력하면 문서가 브라우저 안에서 복호화되어 열립니다.
저장소에는 암호문만 들어 있어 비밀번호 없이는 내용을 읽을 수 없습니다. (PBKDF2-SHA256 600,000회 · AES-256-GCM)

비밀번호는 저장소에 기록하지 않습니다. 작성자에게 문의하세요.

## 수정 모드

문서 왼쪽 패널의 **✏️ 수정 모드**에서 표 · 설명 · 제목을 직접 고칠 수 있고, 고친 내용은 `1 개정 이력`에 자동으로 기록됩니다.
수정 내용은 이 저장소의 `chat-plan-db` 이슈에 암호화되어 저장됩니다. 이 이슈를 직접 수정하거나 닫지 마세요.

처음 한 번 저장소 연결이 필요합니다: [토큰 만들기](https://github.com/settings/personal-access-tokens/new) → Repository access는 `chat_plan_document`만 → Repository permissions에서 **Issues: Read and write** → 문서의 연결 창에 붙여 넣기.
