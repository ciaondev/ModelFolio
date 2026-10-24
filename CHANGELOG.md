# 바뀐 점 · Changelog

버전 번호는 `modelfolio/version.py` 한곳에서 정하고 설치 파일·About·공유 파일(.mfolio)·업데이트 확인이 같이 씁니다.
릴리스 알림에는 아래에서 그 버전 칸이 그대로 나옵니다(앱 화면 언어에 맞춰 한국어 또는 English).

The version number lives in one place (`modelfolio/version.py`) and is shared by the installer, About, share files (.mfolio)
and the update check. The update notice shows the matching section below, in the app's display language.

## 0.4.0 — 2026-10-24

### 한국어
첫 공개 릴리스입니다.
- **자동 칠하기:** 파츠 이름(한/영)·모양으로 역할을 정해 테마(실차·피규어·기계·장난감)별 배색으로 색·재질 칠하기. 배색마다 지금 작품 미리보기 그림, 🎲 다른 조합, 좌우 대칭·같은 원래 색 파츠는 같은 색, 미리보기 후 적용·되돌리기.
- **부위 칠하기 붓:** 한 덩어리 메시도 부위별로. 표면 클릭 → 꺾임·오목한 홈·색 경계까지 비슷한 면 자동 고르기(범위 조절, 한 겹 넓히기·좁히기), 붓으로 문질러 칠하기·지우기, 고른 곳 경계를 붓으로 다듬기, 되돌리기. 고품질 렌더·3MF(삼각형마다 색)·GLB(꼭짓점 색)·공유 파일에 반영.
- **glTF·FBX 자동 그룹:** 노드 계층(문짝·바퀴 등)으로 분해 그룹 초안, glTF 기본색 텍스처를 바르게 찾기, 가짜 그림자 판은 처음부터 숨김.
- **키 스위치:** 파츠를 눌리는 키로(청·갈·적축 소리, 키보드 키·도레미 연결, 만지기·발표에서 클릭). 키보드 플레이트 MX 구멍에 스위치 모델 꽂기, 키캡 끼우기·빼기, 키캡 그룹째 누르기, 어긋난 키캡 자동 바로잡기.
- **작품 공유 파일(.mfolio):** 작품 하나를 파일 하나로 내보내기·가져오기. 편집용(원본 포함)·보기용, 렌더·AI 기록 넣기(선택), PC 경로·사진 촬영 정보(EXIF) 지움, 가져올 때 크기·형식·내용 검사, 형식 버전·최소 앱 버전·단계별 변환.
- **모델로 내보내기:** 3MF(파츠 이름·색, Bambu Studio 부품 이름까지)·GLB·STL(파츠마다, zip). 조립 상태 또는 지금 화면 그대로. 앨범 카드 우클릭·작품 정보 탭에서. Fusion은 삽입 → 메시 삽입으로 열립니다.
- **보기용 공유 파일 보호:** 모델·사진을 AES-GCM으로 봉인해 ModelFolio에서만 열리고(압축을 풀어도 쓸 수 없음), 라이브러리에도 봉인된 채로 둡니다. 선택: 화면용 메시 거칠게(50%·25%, 원래 메시는 파일에 넣지 않음), 비밀번호(가져올 때 물음). 보기용으로 받은 작품은 모델 내보내기·다시 내보내기·고치기가 막힙니다(공유 파일 형식 1.1).
- **라이브러리 보호:** 라이브러리 형식을 바꾸기 전에 자동 백업, 더 새 앱이 만든 라이브러리는 읽기 전용으로 열기.
- **English 화면:** 설정 → 일반 → 언어.
- **간섭 검사·틈 만들기:** 겹침·틈 부족·맞닿음 찾기, 받는 쪽 구멍 넓히기·핀 줄이기, 깨진(열린) 메시도 계산.
- **부품 갈아 끼우기·합치기:** 고친 부품 파일로 그 파츠만 바꾸기, 따로 저장한 부품 파일을 한 작품으로 합치기.
- **분해 경로 편집:** 그룹·경유점·단계·자동 시간, 경로 여러 개와 버전 기록, 분해 유형 18가지, 경첩·슬라이드 동작.
- **고품질 렌더·AI 배경:** 큰 모델을 멀리서 찍을 때 뒤가 잘리던 것 고침, 반광 바닥, 반사 바닥 정리, AI 배경 후보 여러 장·기록·시드, 각도 맞춤, 물 장면.
- **앨범:** 디자인 시안 A 스튜디오·B 매거진·C 전시관·D 추천(모든 시안에서 카드 우클릭 메뉴, 창 너비에 맞춰 줄바꿈), 새 시작 화면.
- **예제 작품·문제 보고:** 처음 실행하면 곰 키링 예제를 넣을지 묻기, About의 [문제 보고]·[로그 폴더](로그 파일에서 사용자 폴더·이름은 지움).
- **이용허락서 1.2:** 개인·1인 사업자·학교·비영리 무료, 근로자를 둔 사업장과 공공기관의 업무용 사용은 문의, 앱 자체의 판매·유료 서비스 제공 금지(유료 의뢰 작업 납품은 가능), 결과물 제한 없음, Ciaon의 코드·그림·문서로 AI 학습 금지. 오픈소스 고지에 AI 모델 이름·라이선스와 OCCT 교체·소스 안내를 보완.
- **라이브러리 기본 위치:** 새로 만들 때 문서 폴더가 OneDrive 안이면 사용자 폴더 아래(`C:\Users\<이름>\ModelFolio Library`)로(동기화 충돌 방지). 이미 있는 라이브러리는 그대로.
- **새 버전 알림:** 하루 한 번 확인 → [지금 설치](SHA-256 확인 후 설치)·[나중에]·[이 버전 건너뛰기], 설정 → 일반 → 업데이트에서 끄기, 인터넷이 없으면 조용히 넘어감.

### English
First public release.
- **Auto color:** assigns roles from part names (Korean/English) and shapes and paints colors and materials with theme palettes (real car, figure, machine, toy). Preview thumbnails of your work for each palette, 🎲 shuffle, matching colors for mirrored parts and parts that shared an original color, preview before applying, undo.
- **Region paint brush:** paint regions of even a single-piece mesh. Click a surface to auto-select similar faces up to creases, concave grooves and color changes (adjustable range, grow/shrink by a ring), brush to paint or erase, refine the selection edge with the brush, undo. Included in high-quality renders, 3MF (per-triangle color), GLB (vertex colors) and share files.
- **glTF/FBX auto groups:** explode group drafts from the node hierarchy (doors, wheels and so on), correct glTF base-color textures, fake shadow planes hidden from the start.
- **Key switches:** turn parts into keys you can press (blue/brown/red switch sounds, keyboard keys and do-re-mi notes, click in hands-on and presentation). Plug MX switch models into a keyboard plate, fit and remove keycaps, press grouped keycaps together, and automatic repair of misaligned keycaps.
- **Share files (.mfolio):** export and import one work as one file. Editable (with originals) or View-only, optional render/AI history, PC paths and photo capture info (EXIF) removed, size/format/content checks on import, format version, minimum app version and step-by-step upgrades.
- **Model export:** 3MF (part names and colors, including Bambu Studio part names), GLB, STL (one per part, zipped). Assembled or exactly as shown. From the album card's right-click menu or the work's Info tab. Fusion opens it via Insert → Insert Mesh.
- **View-only share protection:** the model and photos are sealed with AES-GCM so they open only in ModelFolio (unzipping the file gives nothing usable), and stay sealed in the library. Optional: coarser display mesh (50% or 25%; the original mesh is not included), password (asked on import). Works received as view-only can't be exported as models, re-exported or modified (share format 1.1).
- **Library safety:** automatic backup before the library format changes; libraries made by a newer app open read-only.
- **English UI:** Settings → General → Language.
- **Interference check and clearance fixes:** find overlaps, too-tight gaps and contacts; widen the receiving hole or shrink the pin; works on broken (open) meshes too.
- **Replace and merge parts:** swap a single part with a fixed part file, or merge separately saved part files into one work.
- **Explode path editor:** groups, waypoints, steps and auto timing, multiple paths with version history, 18 explode styles, hinges and sliders.
- **Rendering and AI backgrounds:** fixed the far side being cut off when rendering a large model from a distance, semi-gloss floor, cleaner reflective floor, multiple AI candidates with history and seeds, angle matching, water scenes.
- **Album:** design styles A Studio, B Magazine, C Exhibition, D Featured (card right-click menu in every style, rows wrap to the window width), new start screen.
- **Sample work and problem reports:** offers a Bear Keyring sample on first launch; Report a problem and Log folder in About (user folder and name are removed from the log).
- **License 1.2:** free for individuals, sole proprietors, schools and non-profits; business use at workplaces with employees or public institutions needs permission; selling the app itself or offering it as a paid service is not allowed (delivering paid commissioned work is fine); no restrictions on output; no AI training on Ciaon's code, graphics and documents. The open-source notices now list the AI models and their licenses, and how to replace OCCT and get its source.
- **Default library location:** a new library goes under your user folder (`C:\Users\<name>\ModelFolio Library`) when Documents is inside OneDrive, to avoid sync conflicts. Existing libraries stay where they are.
- **Update notice:** checks once a day → Install now (installs after verifying SHA-256), Later or Skip this version; turn it off in Settings → General → Updates; quietly skipped when offline.

## 0.3.0 — 2026-10-18

### 한국어
내부 시험판(공개하지 않음). 아이콘·시작 화면·About, 이용허락서, 설치 파일, 새 버전 확인의 뼈대.

### English
Internal preview (not published). Icon, start screen, About, license, installer and the first update check.
