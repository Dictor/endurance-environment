## 에어심 환경 구축
1.  언리언 엔진 다운로드 (https://www.unrealengine.com/ko/download) 에픽 회원가입 필요, 크리에이터용
2. 엔진 설치 (4.26)
3. VS2019 커뮤니티 설치 프로그램 다운로드하여 실행한 후 오른쪽 체크 모두 해제하고 "C++을 이용한 데스크톱 개발" 체크하고 설치
4. git clone https://github.com/Microsoft/AirSim.git
5. x64 Native Tools Command Prompt for VS2019 실행
6. cd <깃 클론한 경로> 
7. build.cmd 실행

## 현재 맵 들여오기
1. Airsim/Unreal/Environments/ 하위에 현재 저장소 clone
2. GenerateProjectFiles.bat 실행
3. AirSim\Unreal\Environments\Blocks에서 update_from_git.bat 실행하고 Blocks.project 열기 (bat 미실행시 Airsim 플러그인 미발견 오류 발생함)
4. Blocks.uproject 파일을 연다
5.'파일'을 클릭한다 → 프로젝트 패키지 → window(64bit)
6. 패키지 파일로 임의 경로 

* Could not find NetFxSDK install dir; 오류시 https://www.microsoft.com/en-us/download/details.aspx?id=53321 에서 Dev Pack 설치 (4.6.2아니면 오류나는 듯)
