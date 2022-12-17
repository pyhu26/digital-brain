## How to process DevTask 

> **DevTask?**    
> 개발 항목을 의미하며 일반적으로 WBS 상 Task 하나를 의미한다.      
> DevTask 로 할당 받은 항목은 아래의 순서로 개발한다.

[![](https://mermaid.ink/img/pako:eNpFj8FqwkAQhl9lmLO-QA6FmmivJfWW9TAkkxg0u7LZKCLectNLDxYKpQhtD4Ue2lv7TFnfwWUp5DZ8388_MztMVcYYYL5Um3RO2sA0ElLI2yTiNUypXsDldO4OfzNwEIbDGxgl91oZZbYrBvv6aNufmZAjr8IkdHUQ87rkjaOhp1ESU06pUbqUBXTfn5enD7Dtuz2fXCbymbHbV5eFhO7r17YvffHY60kSc19hn9vu7ejkxMu7_tZ_gwOsWFdUZu61nZAAAs2cKxYYuDEjvRAo5N7lqDHqYStTDIxueIDNKiPDUUmFpgqDnJY176-4rXHu?type=png)](https://mermaid.live/edit#pako:eNpFj8FqwkAQhl9lmLO-QA6FmmivJfWW9TAkkxg0u7LZKCLectNLDxYKpQhtD4Ue2lv7TFnfwWUp5DZ8388_MztMVcYYYL5Um3RO2sA0ElLI2yTiNUypXsDldO4OfzNwEIbDGxgl91oZZbYrBvv6aNufmZAjr8IkdHUQ87rkjaOhp1ESU06pUbqUBXTfn5enD7Dtuz2fXCbymbHbV5eFhO7r17YvffHY60kSc19hn9vu7ejkxMu7_tZ_gwOsWFdUZu61nZAAAs2cKxYYuDEjvRAo5N7lqDHqYStTDIxueIDNKiPDUUmFpgqDnJY176-4rXHu)

### DevTask 할당
개발 항목의 담당자로 지정이 된 상태

### Prototype 작성
개발 항목의 요구사항을 우선 구현한 상태
 - 컴포넌트로 분리하여 개발하지 않음
 - Data는 [[Mock Server]] 및 하드코딩 상태로 진행

### Code Review
 - Refactoring 방향 결정
 - Code 수정

### Design 문서 작성
Design 문서는 md 파일로 작성하며 아래의 구조를 갖춘다.

- UI Design
	- Mindomo를 사용하여 스케치 or Prototype 스크린 샷
- Define functions
	- 기능을 정의하되 DevTask의 요구사항이 모두 반영되어야 한다.
- Data Design
	- 컴포넌트에서 사용할 Data 구조를 정의한다.
	
[[Format.Design-Component]] 템플릿을 사용한다. ([[Templater 사용법]])

### Refactoring 완료
컴포넌트로 분리하여 개발완료된 상태

### DevTask 완료
DevTask 해당하는 GitIssue가 완료된 상태