# Repository Structure Guide

## 각 모듈의 파일 구조

```
[Module]/
├── README.md           # 상세 설명 및 이론
├── [name].h            # 헤더 파일 (인터페이스)
├── [name].cpp          # 구현 파일
├── [name]_test.cpp     # 단위 테스트
├── CMakeLists.txt      # 빌드 설정
└── examples/
    ├── example1.cpp    # 기본 사용 예제
    ├── example2.cpp    # 고급 사용 예제
    └── benchmark.cpp   # 성능 벤치마크
```

## 코딩 스타일

### 네이밍 규칙
- **클래스**: PascalCase (예: `BinarySearchTree`)
- **함수**: camelCase (예: `insertNode`)
- **변수**: snake_case (예: `left_child`)
- **상수**: UPPER_CASE (예: `MAX_SIZE`)

### 파일 네이밍
- 헤더: `binary_search_tree.h`
- 구현: `binary_search_tree.cpp`
- 테스트: `binary_search_tree_test.cpp`

## 학습 순서 추천

### 1단계: 기초 자료구조 (1-2주)
- [ ] Array
- [ ] LinkedList
- [ ] Stack
- [ ] Queue

### 2단계: 트리 구조 (2-3주)
- [ ] Binary Tree
- [ ] Binary Search Tree
- [ ] AVL Tree
- [ ] Red-Black Tree

### 3단계: 기초 알고리즘 (2-3주)
- [ ] Sorting Algorithms
- [ ] Searching Algorithms
- [ ] Basic Graph (BFS, DFS)

### 4단계: 고급 알고리즘 (3-4주)
- [ ] Dynamic Programming
- [ ] Greedy Algorithms
- [ ] Graph Algorithms

### 5단계: CS 기초 통합 (지속적)
- [ ] Computer Architecture 연관성
- [ ] OS 개념 통합
- [ ] File System 이해
- [ ] Networking 적용

## 작성 팁

### README.md 작성시
1. **도입 배경** 섹션을 먼저 채우기
   - 왜 필요한지 이해하는 것이 중요
   
2. **구현** 섹션은 작은 단위로
   - 한 번에 모든 기능을 구현하지 말 것
   - 핵심 기능부터 점진적으로
   
3. **관련 CS 지식**은 구현 후에
   - 실제 구현해본 후 시스템 레벨 이해
   
4. **실사용 사례**는 마지막에
   - 여러 자료를 찾아보며 정리

### 코드 작성시
1. 먼저 테스트 케이스 작성 (TDD)
2. 간단한 구현부터 시작
3. 최적화는 나중에
4. 주석은 "왜"를 설명

### 복잡도 분석시
1. 수학적 증명 작성
2. 최선/평균/최악 케이스 모두 분석
3. 실제 측정 결과도 포함

## Git Workflow

### 브랜치 전략
- `main`: 완성된 모듈만
- `feature/[name]`: 새로운 모듈 작업
- `docs/[name]`: 문서 작업

### 커밋 메시지
```
[Category] Brief description

- Detailed change 1
- Detailed change 2

Related: #issue-number
```

예시:
```
[DataStructure] Implement Binary Search Tree

- Add BST basic operations (insert, delete, search)
- Add unit tests for all operations
- Write comprehensive README with complexity analysis

Related: #12
```

## 체크리스트

새 모듈을 완성했다고 할 수 있는 기준:

- [ ] README.md의 모든 섹션 작성
- [ ] 헤더 파일 작성 (인터페이스 정의)
- [ ] 구현 파일 작성 (모든 메서드)
- [ ] 테스트 코드 작성 (80% 이상 커버리지)
- [ ] 최소 2개 이상의 예제
- [ ] 복잡도 분석 (수학적 증명)
- [ ] 관련 CS 지식 섹션 작성
- [ ] 실전 문제 3개 이상 추가
- [ ] 코드 리뷰 완료
- [ ] 메인 README.md 체크박스 업데이트
