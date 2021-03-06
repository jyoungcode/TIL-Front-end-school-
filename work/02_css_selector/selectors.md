---

### 진행 내용

- CSS 선택자
- CSS 선택자 우선 순위
- CSS 상속

---

### CSS 선택자

수업 중 정리 예정...|

유형 | 선택자 | 설명|
--- | --- | ---|
**전역 선택자** | * |
-  |  |모든 요소 타입의 수식명을 나타낸다. 혼란을 피하기 위해 `*`을 생략하지 않는걸 권장합니다.
- | | 예를 들어 div:first-child과 div:first-child를 생각해보면 이해가 빠릅니다. 여기서 div `*:first-child`가 더 가독성이 좋을 것입니다.|
**일반 선택자** | E | 요소 선택자 |
- | | 문서 안에 선택된 element |
 | E(P) E(C) | 자손 선택자 | 부모요소의 자식을 선택 할 때 사용 |
**속성 선택자** | [attr^="value"] | 시작하는 속성 값이 일치하는 경우 선택|
        | [attr$="value"] | 끝나는 속성 값이 일치하는 경우 선택|
        | [attr*="value"] | 속성 값을 포함하는 경우 선택|
        | [attr|="value"] | 하이픈(-)으로 구분되는 단어가 일치할 때 선택 (국내에서 잘 사용하지 않는다.)|
        | [attr~="value"] | 공백으로 구분되는 단어가 일치할 때 선택|
        | [attr="value"] | 속성의 값이 일치 하는 경우|
**가상 클래스** | :link | <a> 요소의 기본 상태 (그냥 일반선택자로 사용)|
         | :visited | <a> 요소의 방문한 상태|
         | :hover | 요소에 마우스 커서가 올라간 상태|
         | :active | 요소를 마우스 커서로 누른 상태|
         | :focus | 요소에 키보드 포커스가 적용된 상태|
         | :nth-child(an + b) | 부모 요소의 자식 요소 중, 수학 표현식에 따른 계산 결과를 처리 후 선택|
         | :first-child | 부모 요소의 첫번째 자식 요소일 경우 선택|
         | :last-child | 부모 요소의 마지막 자식 요소일 경우 선택|
         | :only-child | 부모 요소의 유일한 자식 요소일 경우 선택|
         | :not(selector) | () 안의 선택자를 제외한 나머지 대상 요소 선택|
         | :nth-last-child(an + b) | 부모 요소의 자식 요소 중, 수학 표현식에 따른 계산 결과를 처리 후 선택 (뒤로부터 색인)|
         | :nth-of-type(an + b) | 동일한 유형 중, 수학 표현식에 따른 계산 결과를 처리 후 선택|
         | :nth-last-of-type(an + b) | 동일한 유형 중, 수학 표현식에 따른 계산 결과를 처리 후 선택 (뒤로부터 색인)|
**가상 요소** | :root | 루트 요소 선택|
        | :empty | 요소 내 내용이 빈 경우 선택|
        | :target | 문서의 URI의 조각 식별자(/#id)를 가진 요소 선택|
        | :enabled | 폼 요소 컨트롤 중 활성화|
        | :disabled | 사용 불가능한 상태|
        | :checked | 체크 되어있는 유저 인터페이스 요소 E (즉 라디오 버튼 혹은 체크박스)|
        | :invalid | input 요소의 종류에 따라 검증에 실패하면 녹색으로 잘못되면 빨간색으로 나타난다.|
        | :read-only | form 요소의 속성으로 읽기만 가능하게 한다. ie에서 지원하지 않는다.|
        | :read-write | read-only 속성이 아닐때 쓰기가 가능한 속성|
        | :optional | required 속성이 지정 되지 않은 input 요소|
        | :out-of-range | input의 지정된 문자 길이 값이 넘어가면 발생한다.|
         | :lang(language) | 요소에 lang 속성이 language인 것을 선택(속성 선택자가 더 직관적일 수 있다)|
