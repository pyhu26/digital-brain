---
aliases: 컴포넌트 설계 문서 포맷 
---

(문서 제목은 컴포넌트 Id 로)

## UI Design

이미지 첨부

> 경로 (mindomo 파일 경로) 
> 설명

## Functions

- 기능 1
- 기능 2
- ...

### 기능 1 
 (설명)...

### 기능 2 
 (설명)...

## Data design
```json
	//example
	props : {
		name : "",
		hasChilde : false,
		childs : [],
		parent : {}
	}
	
	global state : {
		theme : ""
	}
	
	local state : {
		activeColor : "blue",
	}
```

**History** (last modified : 2022-12-17 23:12)
- 0.1  초기 작성 (2022-12-01)
- 1.0  협의 완료 (2022-12-02)