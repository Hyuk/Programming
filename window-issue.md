# 윈도우 이슈 팁

## 윈도우 구동시 시작 프로그램 제어
* 작업표시줄 > 마우스 우클릭 > 작업관리자 > 시작프로그램 탭
* 은행 관련 프로그램 모두 활성 끄기

## 프로그램 충돌 방지
* "Windows Key + R" > msconfig > 서비스 탭

## file explorer freezing issue.
* Open CMD windows(Admin), then type below code
 ```bash
Dism /online /cleanup-image /restorehealth

sfc /scannow

# 재부팅
 ```

 ```bash
bcdedit /set disabledynamictick yes

# 재부팅
 ```

 * 폴더 옵션 > 일반 > 개인 정보 보호 > 지우기