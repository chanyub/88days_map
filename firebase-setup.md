# 실시간 채팅 백엔드 설정 가이드

현재 채팅은 **로컬 스토리지**를 사용하므로 각 사용자별로만 메시지가 보입니다.
실제 공유 채팅을 원한다면 아래 옵션 중 하나를 선택하세요:

## 옵션 1: Firebase (추천, 무료)

### 1. Firebase 프로젝트 생성
1. [Firebase Console](https://console.firebase.google.com/)에 접속
2. "프로젝트 추가" 클릭
3. 프로젝트 이름: `88days-map`
4. Google Analytics 비활성화
5. 프로젝트 생성

### 2. Realtime Database 설정
1. "Realtime Database" → "데이터베이스 만들기"
2. 위치: asia-southeast1 (싱가포르)
3. 보안 규칙: "테스트 모드에서 시작"

### 3. 웹 앱 추가 및 설정
1. 웹 아이콘 (</>) 클릭 → 앱 등록
2. Firebase 구성 정보를 index.html에 추가:

```javascript
// index.html의 chatBackend 부분을 다음으로 교체:
window.chatBackend = {
  enabled: true,
  firebaseConfig: {
    apiKey: "your-api-key",
    authDomain: "your-project.firebaseapp.com", 
    databaseURL: "https://your-project-default-rtdb.asia-southeast1.firebasedatabase.app",
    projectId: "your-project-id",
    storageBucket: "your-project.appspot.com",
    messagingSenderId: "your-sender-id",
    appId: "your-app-id"
  }
};
```

## 옵션 2: Supabase (무료)
1. [Supabase](https://supabase.com/)에서 프로젝트 생성
2. 메시지 테이블 생성
3. API 키를 index.html에 추가

## 옵션 3: 간단한 방법 - GitHub Discussions 사용
현재 repository의 Discussions 탭을 활성화하여 방명록으로 사용

## 현재 상태
- ✅ 로컬 채팅 기능 완료
- ⏳ 백엔드 설정 대기
- 🔄 백엔드 연결시 자동으로 실시간 채팅 활성화

**참고:** 현재는 개인별 로컬 저장만 되며, 실시간 공유를 원하면 위 백엔드 설정이 필요합니다.