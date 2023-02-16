# 데이터 관리 규정(DataManageRule)

## 서문

    HandS는 관리 효율성과 사용자 권리 인식울 제고하기 위해 아래와 같은 방식으로 데이터 관리방식을 규정한다.
    데이터 관리 총칙의 대상은 HandS에서 발생하는 모든 데이터에 대한 처리 방침에 해당한다.
    HandS는 과도한 규정을 제정함으로서 작업의 창의성과 효율이 하락될 수 있음을 인지하고,
    모든 규정은 데이터 중앙 관리화를 통한 작업의 효율성과 창의성을 제고하기 위한 것임을 숙지한다.
    규정들은 최소한의 행동 행동양식에 제한을 두는 것을 원칙으로 하며,
    HandS는 책임감 있게 심도있는 고민을 통해 규정을 제정하도록 한다.
    데이터 관리 규정은 문화적으로 정착되기에 오래 걸리고,
    규정의 변화에 대해 데이터를 변화시키는데 투자되는 비용이 크므로,
    규정 제정의 전문성과 책임감 있는 참여의지가 필요하다.

- 언어의 정의
  - 폴더
    - 파일을 담고 있는 파일 주소 공간
    - 모든 폴더는 classname을 갖는다.
  - 서버폴더
    - 서버폴더의 classname은 주소공간을 대표하는 단어로 표현한다.

            예시
                - 주소 공간 : C://users/home/hands/desktop/handsdrive/
                - classname : HS
  - 폴더명
    - classname과 언더바 "\_"로 구성된다.
    - classname은 {class##} 형태로 대표된다.
    - 폴더명은 {classgroupname}으로 표현을 대체할 수 있다.

            예시
                - {classgroupname} = {class01}\_{class02}\_{class03}\_{class04}
  - 파일
    - 폴더의 가장 끝단에 존재하는 데이터

  - 파일명
    - 폴더명의 일부와 "\_"로 구성된다.
    - 모든 파일은 filename을 포함한다.
    - filename은 {file.xxx}라 표현한다.
    - {file.xxx}는 {filename}.{ext}으로 대체할 수 있다.
  - 버전
    - 파일에 버전을 의미한다.
    - 버전명은 {verx-x}라 표현한다.
  - 비고
    - 참조하라고 붙인 단어나 문자 또는 문장을 의미한다.
    - 비고 형식의 classname은 {ref} 형태로 대표한다.
  - 인덱스
    - filename 또는 classname의 앞에 붙일 수 있는 수의 나열을 의미한다.
    - 인덱스는 {index}로 표현한다.
    - 폴더 내 정렬 시 깔끔한 UI를 제공받을 수 있게 한다.
- 전체에 대한 예시

        총예시 (폴더)
            - 주소 공간 : C://users/home/hands/desktop/handsdrive/HS_01FI_Finance
            - {classgroupname} = HS_FI_Finance
            - {index} = 01
            - {class##} = FI
            - {ref} = Finance
            - classname = 01FI_Finance
        총예시 (파일)
            - 주소 공간 : C://users/home/hands/desktop/handsdrive/HS_FI_Finance/HS_FI_01FEv1-0-0_FinanceEnginfirst.exe
            - {classgroupname} = HS_FI
            - {index} = 01
            - {filename} = FE
            - {verx-x} = V1-0-0
            - {ref} = FinanceEnginfirst
            - {ext} = exe
            - 파일명 = HS_FI_01FEv1-0-0_FinanceEnginfirst.exe

---

## 규정

- 제 01조. 협의
  - 01조 01항. 데이터 구조에 대한 모든 제반 사항은 "HandS 데이터 구조 협의체"(이하 "협의체")에 의해 결정된다.
  - 01조 02항. "협의체"는 회장과 서버관리자를 포함한 임원진 총 3인 이상으로 구성한다.
    - 01조 02항 01호. "협의체" 구성원은 회장이 선정한다.
  - 01조 03항. "협의체"에 발의 가능한 자는 HandS임원진으로 한정한다.
  - 01조 04항. "협의체"는 매년 1회 이상의 "데이터 구조에 대한 회의"(이하 "회의")를 주최하여 규정을 조정한다.
    - 01조 03항 01호. 규정의 조정으로는 "협의체"의 만장일치로 통과한 안건만 반영이 가능하다.
  - 01조 05항. 규정에 어긋나는 데이터는 강제로 수정될 수 있다.
  - 01조 06항. "협의체"는 데이터 사용자들의 규정 숙지 능력을 제고하기 위해 노력한다.
  - 01조 07항. "데이터 관리 규정"은 쉽게 공개될 수 있는 장소에 보관 및 저장한다.
- 제 02조. 기본시항
  - 02조 01항. {default} = "HS"이다.
  - 02조 02항. 폴더명 가장 우측에 "\_{ref}"를 추가할 수 있다.

        예시
            - 기존폴더명: HS_AA_BB
            - 변경폴더명: HS_AA_BB_Babo
  - 02조 03항. {file.xxx}을 "file\_{ref}.xxx"로 대체할 수 있다.
  - 02조 04항. {class##}를 "{index}\_{class##}"로 대체할 수 있다.
  - 02조 04항. {file.xxx}를 "{index}\_{file.xxx}"로 대체할 수 있다.
- 제 03조. 세부사항
  - 03조 01항. {classgroupname}은 상위폴더의 {ref}를 제외한 {classgroupname}을 포함한다.

        예시
            - 상위폴더명: HS_AA_BB_Babo
                - 하위폴더명: HS_AA_BB_CC_Cocaine
  - 03조 02항. 파일명은 {classgroupname}_{file.xxx}으로 구성된다.

        예시
            - 상위폴더명: HS_AA_BB_Babo
                - 하위파일명: HS_AA_BB_MapleStoryEngine.exe
    - 03조 02항 01호. 파일에 버전구분이 필요할 시 {file.xxx}는 "file\_{verx-x}.xxx"로 대체할 수 있다.

            예시
                - 상위폴더명: HS_AA_BB_Babo
                    - 하위파일명: HS_AA_BB_MapleStoryEngine_ver03-01.exe
    - 03조 02항 02호. {verx-x}와 {ref} 모두 사용될 시 {file.xxx}는 "file\_{verx-x}\_{ref}.xxx"로 대체할 수 있다.

            예시
                - 상위폴더명: HS_AA_BB_Babo
                    - 하위파일명: HS_AA_BB_MSE_ver03-01_MapleStoryEngine.exe
    - 03조 02항 03호. 파생결과로 생성되는 파일은 {classgroupname}은 파생 원인 파일의 {filename}로 대체할 수 있다.

            예시
                - 상위폴더명: HS_AA_BB_Babo
                    - 하위파일명(파생원인파일): HS_AA_BB_MSE_ver03-01_MapleStoryEngine.exe
                    - 파생결과파일01: MSE_movement.c
                    - 파생결과파일02: MSE_main.c
                    - 파생결과파일02: MSE_README.md
    - 03조 02항 04호. 03호에서 파생 결과로 생성된 파일은 상위폴더의 {classgroupname}과 파생 원인 파일의 {filename}을 포함하는 {classgroupname}의 폴더의 하위에서 관리할 수 있다.

            예시
                - 상위폴더명: HS_AA_BB_Babo
                    - 하위파일명(파생원인파일): HS_AA_BB_MSE_ver03-01_MapleStoryEngine.exe
                    - 하위폴더명(파생파일모음폴더): HS_AA_BB_MSE
                        - 파생결과파일01: MSE_movement.c
                        - 파생결과파일02: MSE_main.c
                        - 파생결과파일02: MSE_README.md
  - 03조 03항. 폴더명과 파일명은 영문, 숫자, "_"로 구성된 문장만을 사용한다.
  - 03조 04항. 모든 폴더는 각 폴더의 목적을 담은 README.txt 파일을 포함한다.
- 제 04조. 추천
  - 04조 01항. {verx-x}로서 {RVS}{YYYY}{MM}{DD}글자수를 맞추어 날짜 형식을 쓰는걸 추천한다.

        예시
            - HS_AA_BB_MSE_00120230101_MapleStoryEngine.exe
            - HS_AA_BB_MSE_00220230101_MapleStoryEngine.exe
            - HS_AA_BB_MSE_00320230103_MapleStoryEngine.exe
            - HS_AA_BB_MSE_00420230107_MapleStoryEngine.exe
            - HS_AA_BB_MSE_00520230112_MapleStoryEngine.exe
            - HS_AA_BB_MSE_00620230125_MapleStoryEngine.exe
            - HS_AA_BB_MSE_00720230201_MapleStoryEngine.exe
            - HS_AA_BB_MSE_00820230421_MapleStoryEngine.exe
  - 04조 02항. 습관적으로 {ref}로서 영문을 쓰는 습관을 추천한다.

        예시
            - HS_DS_Design (추천)
            - HS_DS_디자인부서 (비추천)
  - 04조 03항. 파일의 모듈러 방식의 관리를 추천하며 이를 가장 잘 반영한 모델은 03조 02항 04호의 예시에 해당한다.
  - 04조 04항. 폴더에서 정렬 기능을 유용히 사용하려면 classname 왼쪽 끝을 {index}로 시작하는 것을 추천한다.

        예시
            - 상위폴더명: HS_01AA
                - 하위폴더명: BS_01AA_01BB
            - 상위폴더명: HS_02AA
                - 하위폴더명: BS_02AA_01BB
        cf) 이 방법은 하위폴더의 classgroupname에도 영향을 끼칠 수 있으므로 신중히 순서를 고려해야한다.
  - 04조 05항. .zip과같은 압축파일형태의 데이터 저장은 권장하지 않는다. (접근성 저하로 인한 데이터 재사용률이 떨어진다.)
- 제 05조. 예외
  - 05조 01항. 응용프로그램 등에 의해 자동 생성되는 의존성 폴더, 파일에 한하여 예외가 허용될 수 있다.
  - 05조 02항. 폴더명과 파일명에 한글로 전달해야할 목적성이 뚜렷하다면 {filename}과 {ref}에 한글이 허용될 수 있다.
  - 05조 03항. 아래 각 호에 따라 README.txt 파일 생성하지 않는 것이 허용될 수 있다.
    - 05조 03항 01호. 임시적으로 사용할 목적으로 생성한 폴더의 경우
    - 05조 03항 02호. 응용프로그램의 의존성 문제로 인하여 README.txt가 중복되는 경우
    - 05조 03항 03호. README.txt의 내용이 빈번히 수정될 것으로 예상될 경우
    - 05조 03항 04호. 폴더의 목적이 별도의 README.txt를 보지 않아도 자명히 이해될 경우
    - 05조 03항 05호. README.txt의 경우 {classgroupname}의 생략이 허용될 수 있다.
  - 05조 04항. 03조 02항 04호에서 하위파일(파생원인파일)이 없더라도 해당 조항 내용이 허용될 수 있다.
  - 05조 05항. 02조 04항 그리고 02조 05항에서 언급한대로 왼쪽 끝을 {index} 시작하는 classname 그리고 filename의 폴더의 하위폴더에서는 상위 폴더의 classname에서의 "{index}\_" 생략이 허용될 수 있다.
  - 05조 06항. {index}의 창의적인 삽입 기법이 있다면 협의체의 회의를 거쳐 규정을 조정한다.

## 데이터

용어의 정의

- 데이터 : 폴더와 파일울 대표하는 단어이며, 주소와 이름을 갖는다.
- {dataname} : 데이터의 이름
- {directoryroot} : 데이터의 주소 공간
- {default} : 서버폴더의 주소 공간
- {relativeaddress} : 데이터의 상대 주소공간 ( {directoryroot} = {default}/{relativeaddress} )

tab으로 데이터의 위계관계를 구분한다. (같은 디렉토리의 데이터는 동일한 "열\_column"에 나열된다.)

서버에 최초 존재하는 데이터는 다음과 같이 표현하고,

- {dataname} : {directoryroot} : 폴더설명

위 데이터를 제외하고는 다음과 같이 표현하다.

- {dataname} : {relativeaddress}

## 데이터 구조

- HS : {default}/../ : default폴더 내용
  - HS_DS_Design : {default}/ : 디자인부서
    - a
      - a-d
    - b
      - b-c
    - README.txt : HS_DS_Design /
  - HS_ED_Education : {default}/ : 교육부서
    - a
      - a-d
    - b
      - b-c
    - README.txt : HS_ED_Education/
  - HS_ETC_Extra : {default}/ : 기타폴더(잡)
    - a
      - a-d
    - b
      - b-c
    - README.txt : HS_ETC_Extra/
  - HS_FI_Finance : {default}/ : 회계총무
    - a
      - a-d
    - b
      - b-c
    - README.txt : HS_FI_Finance/
  - HS_HM_HeadManage : {default}/ : 중앙관리
    - a
      - a-d
    - b
      - b-c
    - README.txt : HS_HM_HeadManage/
  - HS_MS_ManageSupport : {default}/ : 관리부서
    - a
      - a-d
    - b
      - b-c
    - README.txt : HS_MS_ManageSupport/
  - HS_PJ_Project : {default}/ : 프로젝트부서
    - a
      - a-d
    - b
      - b-c
    - README.txt : HS_PJ_Project/
  - HS_PB_Public : {default}/ : 공공폴더(공개_공유)
    - a
      - a-d
    - b
      - b-c
    - README.txt : HS_PB_Public/
  - HS_SP_Supporters : {default}/ : 서포터즈부서
    - a
      - a-d
    - b
      - b-c
    - README.txt : HS_SP_Supporters/
  - HS_TC_Technical : {default}/ : 기술부서
    - a
      - a-d
    - b
      - b-c
    - README.txt : HS_TC_Technical/
  - HS_MKT_Marketing : {default}/ : 홍보부서
    - a
      - a-d
    - b
      - b-c
    - README.txt : HS_MKT_Marketing/
  - README.txt : {default}/ : README.txt 파일

---

## About NAS

### NAS 용어

- {유료도메인} : 없음
- {name} : colie
- {filestation별칭} : filestation
- {notestation별칭} : notestation
- {innerIPV4} : 192.168.219.100
- {publicIPV4} : 112.148.121.43
- {smbConnection} : //colie | smb://colie | //{innerIPV4}
- {QuickConnect} : http://QuickConnect.to/colie

### 기본 내용

- 도메인 : {유료 도메인} -> {name}.synology.me 가능!
- “app | Playstore”에서 : DSFile 어플로 접속가능

### 포트 (라우터 포트포워딩 필요)

- ftps://{name}.synology.me:21 -> ftp ssl인증 프로토콜 서비스 (원격 파일서비스)
- http://{name}.synology.me:5000 -> 시놀로지 나스 메인 홈
- https://{name}.synology.me:5001 -> 시놀로지 나스 메인 홈 {ssl}
- http://{name}.synology.me/{filestation별칭}:7000 -> 시놀로지 나스 메인 홈
- https://{name}.synology.me/{filestation별칭}:7001 -> 시놀로지 나스 메인 홈 {ssl}
- http://{name}.synology.me/{notetation별칭}:9350 -> 시놀로지 나스 메인 홈
- https://{name}.synology.me/{notestation별칭}:9351 -> 시놀로지 나스 메인 홈 {ssl}
- vpn server: 1723 -> TCP
- vpn server: 1701 -> UDP
- 기타 포트 : admin만 forwarding 변경 가능

### 추가 내용

- 공유폴더
  - 공유폴더 정보
    - 일반
    - 이름
    - 설명
    - 디스크 파티션(볼륨)
    - 권한별 MetaDataRead Option
    - 휴지통활성화
  - 암호화
    - 암호화 키
  - 고급
    - 데이터 무결성 체크섬 활성화
    - 데이터 압축 활성화
    - 공유폴더 할당량 활성화
  - 권한
    - 로컬사용자
      - admin
      - hong12gil
    - 액세스 없음
    - 읽기/쓰기
    - 읽기 전용
    - 사용자 지정 (사용자 또는 그룹)
      - admin
      - hong12gil
        - 관리
          - 기타 하위 권한 목록
        - 읽기
          - 기타 하위 권한 목록
        - 쓰기
          - 기타 하위 권한 목록
      - 기타사용자{System Process}
  - 고급권한
    - 기타 내용
- 사용자
  - 사용자 정보
    - 이름
    - 설명
    - 이미일
    - 패스워드
    - 알림 메일 보내기
      - 알림 메일에 사용자 패스워드 표시
    - 패스워드 변경 허용 옵션
      - 패스워드 유효성 : 사용자 패스워드 변경 불가
  - 그룹
    - admin
    - http
    - user
  - 공유 폴더 권한
    - 액세스 없음
    - 읽기/쓰기
    - 일기 전용
  - 사용자 할당량 할당
    - 폴더 – 유효할당량 – 그룹할당량 – 사용자 할당량
  - 응용 프로그램 권한 할당
    - FTP
    - FileStation
    - NoteStation
    - Universal Search
  - 사용자 속도 제한 설정
    - 서비스 – 결과 – 속도 제한 – 업로드 제한 KB/s – 다운로드 제한 (KB/s)
