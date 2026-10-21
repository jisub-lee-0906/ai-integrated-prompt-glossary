# AI 프롬프트 용어집 FAQ: 용어 선택부터 결과 검수까지

**Common questions about terminology, AI instructions and deliverables.**

[240개 실무 용어 사전](../glossary/README.md) · [English A–Z index](../glossary/ENGLISH_INDEX.md) · [실전 프롬프트 예시 12개](../examples/README.md) · [PDF 용어집](../book/AI_Integrated_Prompt_Glossary_KO.pdf)

## AI 프롬프트 용어집과 프롬프트 템플릿은 어떻게 다른가요?

템플릿은 요청문을 빠르게 시작하도록 돕고, 용어집은 요청 안에 어떤 작업 개념을 넣을지 판단하도록 돕습니다. 이 책은 용어의 뜻과 비슷한 개념의 차이를 설명한 뒤 실행 명령·설정·검수·수정 명령으로 연결합니다. 작업의 이름이 기억나지 않으면 [48개 작업 의도별 찾아보기](../glossary/TASK_FINDER.md)에서 출발하세요.

## 디자인 AI에 Isometric과 Orthographic View 중 무엇을 써야 하나요?

등각 투영은 세 축의 축척 조건을 만족하는 특정 직교 투영 방향입니다. 직교 투영은 거리에 따른 원근 축소가 없는 표현으로, 정면·측면 같은 도면 설명에도 쓰입니다. 3D 아이콘의 방향을 지정하려면 등각 조건을, 제품 정면 구조를 전달하려면 정면 직교 뷰를 구체적으로 요청하세요. [Isometric](../glossary/D7.md#d7-01) · [Orthographic View](../glossary/D7.md#d7-02)

## 커닝과 트래킹은 모두 글자 간격인데 무엇이 다른가요?

커닝은 AV 같은 특정 글자 쌍의 간격 보정이고, 트래킹은 선택한 문자열 전반의 자간 조절입니다. 로고의 한 쌍만 어색하면 커닝을, 라벨 전체의 밀도를 바꾸려면 트래킹을 지정하세요. 줄 사이 간격은 행간으로 따로 요청합니다. [Kerning](../glossary/D3.md#d3-02) · [Tracking](../glossary/D3.md#d3-03) · [Line Height](../glossary/D3.md#d3-04)

## “벡터 스타일”이라고 하면 편집 가능한 SVG가 나오나요?

벡터풍은 시각 양식이며 실제 파일이 벡터 경로로 구성된다는 보장은 아닙니다. 편집 가능한 SVG가 필요하면 path·viewBox·도형 구조와 납품 형식을 명시하고, PNG를 image 요소로 감싼 파일인지 검사하세요. [Vector Flat](../glossary/D5.md#d5-01) · [Bézier Path](../glossary/D5.md#d5-02)

## AI 이미지의 체크무늬 배경은 실제 투명 배경인가요?

체크무늬가 이미지 픽셀에 그려진 것이라면 투명 배경이 아닙니다. 실제 알파 채널이 포함된 파일을 요청하고 밝은 배경과 어두운 배경에 합성해 보세요. 가장자리의 반투명 값과 후광도 함께 확인합니다. [Alpha Channel](../glossary/D5.md#d5-07) · [Premultiplied / Straight Alpha](../glossary/V4.md#v4-04)

## 영상 생성에서 Dolly In과 Zoom In은 어떻게 다른가요?

달리 인은 카메라 위치가 피사체 쪽으로 움직이는 것이고, 줌 인은 렌즈 화각을 바꾸는 것입니다. 공간을 통과하며 접근하는 느낌을 원하면 카메라 이동과 배경 시차를 요청하세요. 제품 자체가 커지거나 형태가 바뀌지 않는지도 검사해야 합니다. [Dolly In / Out](../glossary/V1.md#v1-03) · [Zoom In / Out](../glossary/V1.md#v1-05)

## 프롬프트에 FPS와 코덱을 쓰면 실제 출력 파일도 바뀌나요?

문장에 숫자와 코덱을 적는 것만으로 파일 속성이 바뀌지는 않습니다. 지원하는 생성 설정, 편집 타임라인과 내보내기 설정에서 요구사항을 적용하고 최종 파일의 프레임 레이트·길이·코덱을 확인하세요. 프레임 레이트, 비트레이트, 비트 심도는 서로 다른 속성입니다. [Frame Rate](../glossary/V5.md#v5-02) · [Bitrate](../glossary/V5.md#v5-03) · [Codec](../glossary/V5.md#v5-04)

## AI 코딩 도구에 “중복 예약을 막아라”를 어떻게 구체화하나요?

같은 요청의 재시도, 데이터 변경 중간의 실패, 여러 요청의 동시 실행을 구별하세요. 멱등성 키의 범위·본문 일치·보존·결과 재사용 정책을 정하고, 데이터베이스 제약과 트랜잭션으로 예약 생성의 경쟁을 통제합니다. 외부 결제의 효과는 로컬 DB 트랜잭션과 별도 복구 경계로 다뤄야 합니다. [Idempotency](../glossary/S2.md#s2-06) · [Transaction](../glossary/S3.md#s3-05) · [Race Condition](../glossary/S7.md#s7-05)

## PDF는 무료이며, 영문 번역본도 있나요?

203쪽 한국어 PDF와 웹 용어집은 무료 열람과 개인 학습용 다운로드를 허용합니다. 영문 용어가 병기되어 있고 별도의 영문 소개·시작 예시가 있지만, 책 전체의 영문 번역본은 아닙니다. 재배포·수정본 배포·교재 수록 등의 이용은 [이용 조건](../LICENSE.md)을 확인하세요. [English overview](../README.en.md) · [English examples](QUICKSTART.en.md)

## AI의 도움을 받아 작성했나요? 오류는 어디로 제보하나요?

AI의 도움을 받아 원고와 예시를 구성하고 문서를 편집했습니다. 각 장에는 관련 기술 개념을 확인할 공식 참고자료를 연결했습니다. 오류는 항목 번호·쪽수·근거와 함께 제보해 주세요. [AI 활용 안내](../AI_USAGE.md) · [오류 제보](https://github.com/jisub-lee-0906/ai-integrated-prompt-glossary/issues/new?template=correction.yml)

© 2026 이지섭 · jisub0906@gmail.com · AI의 도움을 받아 작성.
