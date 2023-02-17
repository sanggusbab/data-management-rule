# 데이터 관리 규정(DataManageRule)

## 서문

    HandS는 관리 효율성과 사용자 권리 인식을 제고하기 위해 아래와 같은 방식으로 데이터 관리방식을 규정한다.
    데이터 관리 총칙의 대상은 HandS에서 발생하는 모든 데이터에 대한 처리 방침에 해당한다.
    HandS는 과도한 규정을 제정함으로서 작업의 창의성과 효율이 하락될 수 있음을 인지하고,
    모든 규정은 데이터 중앙 관리화를 통한 작업의 효율성과 창의성을 제고하기 위한 것임을 숙지한다.
    규정들은 최소한의 행동 행동양식에 제한을 두는 것을 원칙으로 하며,
    HandS는 책임감 있게 심도있는 고민을 통해 규정을 제정하도록 한다.
    데이터 관리 규정은 문화적으로 정착되기에 오래 걸리고,
    규정의 변화에 대해 데이터를 변화시키는데 투자되는 비용이 크므로,
    규정 제정의 전문성과 책임감 있는 참여의지가 필요하다.
    HandS는 학생들의 각자의 성장 및 이익을 위해 존재한다는 이념하에
    공정한 운영과 다양한 양질의 피드백을 받기 위해 그리고 회원들의 적극적인 참여 의지를 제고하기 위해,
    HandS는 공유 가능한 정보는 최대한의 범위로 공개하도록 한다.
    기본적으로 데이터를 수집한 후 정보들을 조합하여 개인정보를 유추할 가능성을 최소로 해야 한다.
    HandS는 개인 식별 가능 정보에 대한 보안 유지의 중요성을 인지하고,
    데이터의 내용을 기반으로 공개범위를 신중히 선정하거나,
    공개범위에 맞추어 데이터를 재가공하는 데 최선을 다한다.

- 언어의 정의

  - 폴더

    - 데이터를 담을 수 있는 주소 공간을 가진 객체

    - 모든 폴더는 {foldername}, {classgroupname}, {classname}을 갖는다.

  - 폴더명(folder code)

    - 폴더명은 {foldername}이라 표현한다.

    - {classname}은 {foldername}의 가장 오른쪽에 위치한 {class##}과 의미가 같다. "##"는 다른 문자로 대체될 수 있는 부분이다.

    - 일반적으로 상위폴더의 {foldername}은 {classgroupname}으로 표현된다. 세부 사항은 규정에서 다룬다.

    - 일반적으로 {foldername}은 "{classgroupname}\_{classname}"으로 표현된다. 세부 사항은 규정에서 다룬다.

  - 서버

    - 데이터를 포함하고 데이터에 접근할 수 있게 하는 장치 제반를 말한다.

  - 서버폴더

    - 서버폴더의 {classname}은 {default}로 표현한다.

    - {classgroupname}값으로 참조되는 서버폴더의 {foldername}은 {default}로 대체한다.

  - 파일
  
    - 폴더의 가장 끝단에 존재하는 데이터

    - 모든 파일은 {classgroupname}, {filename}, {ext}을 가진다.

  - 파일명(file code)

    - 파일명은 "full filename including extension"을 줄여 {fullfilenameIE}라 표현한다.

    - 부분파일명은 "filename including extension"을 줄여 {filenameIE}라 표현한다.

    - 파일의 내용을 적절히 표현하는 문자열을 {filename}이라 표현한다.

    - 파일의 확장자는 {ext}라 표현한다.

    - 일반적으로 상위폴더의 {foldername}은 {classgroupname}으로 표현된다. 세부 사항은 규정에서 다룬다.

    - 일반적으로 {filenameIE}는 {filename}.{ext}으로 표현된다. 세부 사항은 규정에서 다룬다.

    - 일반적으로 {fullfilenameIE}는 {classgroupname}\_{filename}.{ext}으로 표현된다. 세부 사항은 규정에서 다룬다.

  - 버전 (version code)

    - 버전명은 {verx-x}라 표현한다.

    - 대용

  - 비고 (reference code)

    - 비고는 {ref}라 표현한다.

    - 데이터의 메타데이터로서 색인이나 직관적인 이해에 도움을 준다.

  - 인덱스 (index code)

    - 인덱스는 {index}라 표현한다.

    - 폴더 내 정렬 시 깔끔한 UI를 제공받을 수 있게 한다.

  - 의존성 (dependency)

    - 의존성은 하나의 폴더 또는 파일을 기준으로 하위 데이터 간의 논리적 관계가 장기적으로 유지될 가능성을 말한다.

    - 예를 들어, 응용프로그램의 폴더와 라이브러리 사이의 의존성은 매우 강하다.

---

## 규정

"언어의 정의"에서 다룬 용어는 규정에서 다루는 용어와 의미가 같다.

- 제 01조. 협의

  - 01조 01항. 데이터 구조에 대한 모든 제반 사항은 "HandS 데이터 구조 협의체"(이하 "협의체")에 의해 결정된다.

  - 01조 02항. "협의체"는 회장과 서버관리자를 포함한 임원진 총 3인 이상으로 구성한다.

    - 01조 02항 01호. "협의체" 구성원은 회장이 선정한다.

  - 01조 03항. "협의체"에 발의 가능한 자는 HandS임원진으로 한정한다.

  - 01조 04항. "협의체"는 매년 1회 이상의 "데이터 구조에 대한 회의"(이하 "회의")를 주최하여 규정을 조정한다.

    - 01조 03항 01호. 규정의 조정으로는 "협의체"의 만장일치로 통과한 안건만 반영이 가능하다.

  - 01조 05항. 규정에 어긋나는 데이터는 강제로 수정될 수 있다.

  - 01조 06항. "협의체"는 데이터 사용자들의 규정 숙지 능력을 제고하기 위해 노력한다.

  - 01조 07항. "데이터 관리 규정"은 쉽게 공개될 수 있는 장소에 게시한다.

  - 01조 08항. "협의체"에서 데이터 읽기 또는 쓰기 권한이 있는 계정은 1년에 최소 1회 비밀번호를 갱신한다.

    - 01조 08항 01호. 계정 변경 내용 히스토리를 최소한의 인원만 열람가능한 데이터 서버에 저장한다.

    - 01조 08항 02호. 계정 변경 전에 미리 변경 후 열람 권한자들에게 수정 소식을 알릴 계획을 세운다.

  - 01조 09항. 서버관리자는 서버를 신설할 때, 로컬에서 최소 1개 이상의 디렉토리에 대해 접근 가능한 everyone 계정을 생성한다. 해당 계정의 아이디, 비밀번호, 접속방법을 쉽게 접근할 수 있는 장소에 게시한다.

  - 01조 10항. 개인정보와 관련된 내용은 최대한 공개되지 않도록 한다.

  - 01조 11항. HandS의 참여의 자율성과 책임의식 및 창의성 제고를 위해 공개 가능한 정보는 최대한의 범위로 공개를 한다.

  - 01조 12항. 모든 데이터 관리 장치는 물리적인 접근이 통제된 신뢰성이 높은 공간에 설치한다.

  - 01조 13항. 규정의 개정이 의결될 시, "협의체는" 해당 규정의 실질적 적용 계획과 규정이 정착될 수 있는 교육 및 개정안 배포 계획을 수립한다.

  - 01조 14항. 서버의 데이터 논리적 분류의 수를 최소한으로 설계하고, 의존성이 강한 데이터 집합의 논리적 분류의 수를 최대한 작게 설계함을 통해 분업 가능성과 부분개선 효과를 높인다.

    - 추가설명1: 논리적 분류의 수는 의존성이 강한 데이터 집합의 크기와 반비례하는 관계이다.
    - 추가설명2: 의존성 파일 집합의 크기는 의존성이 강한 데이터 집합의 수와 비례하는 관계이다.
    - 1,2에 대한 결론: 논리적 분류를 최소화하며 의존성이 강한 데이터 집합의 집합의 수를 줄일 수 없다. (한계)
    - 최종방안: 서버의 데이터와 의존성이 강한 데이터 집합 각각의 논리적 분류를 최소하하여 설계하는 방식 택한다.
    - 설명: 이는 data tree structure optimizing과, modular optimizing을 적용하는 것이다.
    - 해설: 어떠한 논리적 관계이든, 관계가 명확하고 관계의 수가 적은 설계를 추구한다는 것이다.
    - 해설2: data tree structure optimizing은 time complexity가 NlogN 에 근접할 수록 좋지만, 실질적으로는 modular optimizing이 있어야 가독성이 좋아져 작업 효율이 좋아진다.
    - cf) 01조 14항은 HandS의 데이터 중앙 관리에 있어 추구하는 근본 이념을 실천하는 매커니즘이다.

- 제 02조. 기본시항

  - 02조 01항. {default} = "HS"로 정한다.

  - 02조 02항. {ref} 사용 시 {classname} 우측에 "\_{ref}"를 추가한다.

  - 02조 03항. {ref} 사용 시 {filename} 우측에 "\_{ref}"를 추가한다.

  - 02조 04항. {ref} 없이 {verx-x}만 사용되는 {foldername}은 불가능하다.

    - 02조 04항 1호. {verx-x}와 {ref} 모두 사용 시 {classname} 우측에 "\_{verx-x}\_{ref}"를 추가한다.

  - 02조 05항. {ref} 없이 {verx-x}만 사용되는 {fullfilenameIE}은 불가능하다.

    - 02조 05항 1호. {verx-x}와 {ref} 모두 사용 시 {filename} 우측에 "\_{verx-x}\_{ref}"를 추가한다.

  - 02조 06항. {index} 사용 시 {classname} 좌측에 "{index}\_"를 추가한다.

  - 02조 07항. {index} 사용 시 {filename} 좌측에 "{index}\_"를 추가한다.

  - 02조 08항. {classgroupname}은 상위 폴더의 {foldername}에서 "{index}\_", "\_{verx-x}", "\_{ref}"가 제거된 문자열이다.

  - 02조 09항. {index}는 수의 나열로 된 문자열이다.

  - 02조 10항. 모든 {foldername}과 {fullfilenameIE}는 "{classgroupname}\_"을 왼쪽 끝에 포함한다.

  - 02조 11항. 서버 폴더의 {foldername}은 서버 운영체제에 맞게 서버관리자가 구성한다.

  - 02조 12항. {foldername}은 "{classgroupname}\_{index}\_{classname}\_{verx-x}\_{ref}"이다.

    - 02조 12항 01호. {foldername}에서 "\_{index}", "\_{verx-x}", "\_{ref}"는 생략할 수 있다.

  - 02조 13항. {filenameIE}는 "{filename}\_{verx-x}\_{ref}.{ext}"이다.

    - 02조 13항 01호. "\_{verx-x}", "\_{ref}"가 사용되지 않은 경우에만 {filenameIE}에서 "\_{verx-x}", "\_{ref}"는 각각 사용되지 않은 요소에 상응하여 생략된다.

  - 02조 14항. {fullfilenameIE}는 "{classgroupname}\_{index}\_{filenameIE}"이다.

    - 02조 14항 01호. "\_{index}"가 사용되지 않은 경우에만 {fullfilenameIE}에서 "\_{index}"는 생략된다.

  - 02조 15항. {classgroupname}은 "{default}\_{class01}\_{class02}\_{class03}..."이다.

- 제 03조. 추가사항

  - 03조 01항. 의존성이 강한 데이터은 해당 집합의 최상위 폴더 또는 파일을 제외한 모든 데이터의 {default} 값은 최상위 폴더 또는 파일의 {classname} 또는 {filename}으로 갱신하여 사용한다.

    - 03조 01항 01호. 기타 데이터 공간과의 의존성이 강한 데이터는 {default} 문자열의 좌측끝에 해당 데이터 공간의 {classgroupname}을 참조하여 "{classgroupname}\_"을 포함한다.

    - 03조 01항 02호. 서버와의 의존성이 강한 데이터는 {default} 문자열의 좌측끝에 "HS\_"을 포함한다.

  - 03조 02항. {flodername}과 {fullfilenameIE}는 영문, 숫자, "_"로 구성된 문장만을 사용한다.

  - 03조 03항. 모든 폴더는 각 폴더에서 이루어지는 기능을 담은 README.txt 파일을 포함한다.

- 제 04조. 추천

  - 04조 01항. {verx-x}로서 {RVS}{YYYY}{MM}{DD} 글자수를 맞추어 날짜 형식을 쓰는걸 추천한다.

    - 04조 01항 01호. {verx-x}의 특수목적 사용 설명

      - {RVS} : RevisionCode : 유사파일 간의 개정순번 매길 때 사용한다. (3글자)

      - {YYYY} : YearCode : 년도를 나타낼 때 사용한다. (4글자)

      - {MM} : MonthCode : 월을 나타낼 때 사용한다. (2글자)

      - {DD} : DayCode : 일을 나타낼 때 사용한다. (2글자)

  - 04조 02항. 분업 가능성을 염두에 두고 데이터 구조를 확립함을 추천한다.

  - 04조 03항. 폴더에서 정렬 기능을 유용히 사용하려면 사용 빈도 또는 사용 목적에 따라 {index}를 붙이는 것을 추천한다.

    - 04조 03항 01호. 한 폴더 내에서 사용 목적에 따른 {index}를 먼저 설정하고 이후 인접한 {index} 사이에서 사용 빈도에 따른 {index}를 부분적으로 적절히 조율하여 정함을 추천한다.

  - 04조 04항. {index}는 가장 큰 자리 수와 가장 작은 자리 수가 "4"인 3자리 수 "4#4" 꼴을 사용하는 것을 추천한다.

    - 04조 04항 01호. 이는 offset 기법으로 추후에 추가될 데이터의 성질에 따라 인접한 {index} 사이의 숫자로 삽입해야할 수 있다. {index}로서 "4#4"를 사용한다면 인접한 두 {index} 사이에 최대 9개의 {index}를 더 넣을 수 있다.

    - 04조 04항 02호. {index}로서 "3#2"과같이 양끝이 "0"이 아니면 위의 01호와 동일한 효과를 가질 수 있다. 기능상 조금의 차이는 있다. 본인의 설계에 맞추어 설정한다.

    - 04조 04항 03호. 위의 01호에서 언급한 방식을 적용하면 가독성이 떨어진다. {index}를 중간에 삽입할 때, 사용하는 {index}의 수가 적다면 데이터들의 {index}를 일일이 수정하는 것도 나쁘지 않다.

  - 04조 05항. .zip과같은 압축파일형태의 데이터 저장은 권장하지 않는다. (색인 및 데이터 접근성이 저하되고, 데이터 재사용률이 떨어진다.)

  - 04조 06항. 중괄호 "{}"로 감싸진 부분은 구분코드(Division Code)라고 부른다.

  - 04조 07항. 파일명과 폴더명에 공백문자열을 쓰지 않고, 가독성을 위해 단어의 조합의 경우 단어 또는 의미를 가질 수 있는 문자열 단위의 제일 왼쪽 글자만 대문자로 표기함을 추천한다.

  - 04조 08항. 예를 들어 VisualStudio 프로젝트 폴더와 같이 의존성이 매우 강한 데이터 집합의 최상위 데이터는 {default}를 공백 ""으로 설정할 수 있다.

    - 04조 08항 01호. 04조 08항은 {foldername}과 {fullfilenameIE}의 형식의 제한 규정을 거의 전부 해제시킬 수 있는 조항으로, 다른 규정 들에 대한 숙지가 된 상태에서 활용하도록 한다.

  - 04조 09항. 기본적으로 {foldername}에서 사용하는 {ref}는 짧은 코드의 {classname}을 보조설명하는 역할의 코드이지만, {filename}의 경우는 짧은 문자열형식이 아닌 {foldername}에서 사용하는 {ref}에서의 관례를 차용할 것을 추천한다.

    - 04조 09항 01호. {fullfilenameIE}에서 {filename}을 짧은 코드 형식으로 쓰고, {ref}를 사용하게 되면 불필요하게 {fullfilenameIE}가 길어지게 된므로 의존성이 높은 데이터 집합의 최상이 데이터 파일이 아니라면 04조 09항을 따르는 것을 추천한다.

  - 04조 10항. 폴더명 또는 파일명을 자연스럽게 하기 위해 동일한 {class##}, {filename} 상에서 {ref}만으로 구분짓는 것을 시도 할 수 있다. 하지만 사용했다고 믿는 {ref}는 사실 {verx-x}에 해당한다.

  - 04조 11항. 05조 03항 03호에 의거 README.txt의 {classgroupname}은 생략함을 추천한다.

- 제 05조. 예외 가능 사항

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

  - 05조 07항. {class##}는 되도록 짧은 코드로 사용함을 추천한다. (2~4글자 정도의 약어를 추천)

  - 05조 08항. 01조 09항에서 언급한 everyone 계정의 개설은 서버의 성질에 따른 "협의체"에 의결에 따라 허용되지 않을 수 있다.

  - 05조 09항. 01조 12항에서 필요한 공간이 비용적 또는 행정적인 등의 문제로 마련이 되기 힘든 경우에 임시적인 조치로 물리적인 접근이 가능한 공간에 두는 것이 허용될 수 있다.

    - 05조 09항 01호. 물리적인 접근이 가능한 공간에 둘 경우 만일의 사태를 대비하여 클라우드 서비스와 연동하여 백업 서버를 마련한다.

    - 05조 09항 02호. 위의 각 호와는 별도로 사건 및 사고를 예방하고, 적절한 추후 조치를 결정하기 위해 영상 기록 장치의 촬영 또는 기타 출입 관리 기기 등과 같은 설치물이 있는 장소에 둔다.

  - 05조 10항. {RVS}, {verx-x} 이 둘과 {index}는 기본 이념이 명백히 다르지만 둘 모두 폴더 또는 파일을 구분짓는 용도로는 혼용하여 사용함이 허용될수 있다.

### 전반적인 예시

        예시 : 폴더 기본
            - {classgroupname} = {class01}_{class02}_{class03}
            - {foldername} = {class01}_{class02}_{class03}_{class##}
            - {foldername} = {classgroupname}_{classname}

        예시 : 서버폴더
            - 주소 공간 = C://users/home/hands/desktop/handsdrive/
            - {classname} = AA
            - 서버폴더 하위폴더의 {foldername} = AA_{class}

        예시 :  {classgroupname}_{index}_{class##}_{verx-x}_{ref}
            - 서버 주소 공간 = C://users/AAAsdrive/
            - 서버 classname = AAA
            - 현재 주소 공간 : C://users/AAAdrive/AAA_001FI_Finance/AAA_001FI_HR_20191021_HumanResource
            - {classgroupname} = AAA_001FI
            - {index} = None
            - {class##} = HR
            - verx-x = 20191021
            - {ref} = HumanResource

        예시 : {classgroupname}_{index}_{filename}_{verx-x}_{ref}.{ext}
            - 서버 주소 공간 = C://users/ABCsdrive/
            - 서버 classname = BBB
            - 파일 데이터 공간 : C://users/ABCdrive//BBB_FI_Finance/BBB_FI_001_FE_v1-0_FinanceEngine.exe
            - {fullfilenameIE} = HS_FI_01FEv1-0-0_FinanceEnginfirst.exe
            - {classgroupname} = BBB_FI
            - {index} = 001
            - {filename} = FE
            - {verx-x} = v1-0-0
            - {ref} = FinanceEnginfirst
            - {ext} = exe

        예시 : {ref}
            - 기존폴더명: HS_AA_BB
            - 변경폴더명: HS_AA_BB_Babo

        예시 : {folder}
            - 상위폴더명: HS_AA_BB_Babo
                - 하위폴더명: HS_AA_BB_CC_Cocaine

        예시 : {file}
            - 상위폴더명: HS_AA_BB_Babo
                - 하위파일명: HS_AA_BB_MapleStoryEngine.exe

        예시 : {verx-x}
            - 상위폴더명: HS_AA_BB_Babo
                - 하위파일명: HS_AA_BB_MapleStoryEngine_ver03-01.exe

        예시 : {verx-x} + {ref}
            - 상위폴더명: HS_AA_BB_Babo
                - 하위파일명: HS_AA_BB_MSE_ver03-01_MapleStoryEngine.exe

        예시 : derivated file
            - 상위폴더명: HS_AA_BB_Babo
                - 하위파일명(파생원인파일): HS_AA_BB_MSE_ver03-01_MapleStoryEngine.exe
                - 파생결과파일01: MSE_movement.c
                - 파생결과파일02: MSE_main.c
                - 파생결과파일02: MSE_README.md

        예시 : derivatied file in folder
            - 상위폴더명: HS_AA_BB_Babo
                - 하위파일명(파생원인파일): HS_AA_BB_MSE_ver03-01_MapleStoryEngine.exe
                - 하위폴더명(파생파일모음폴더): HS_AA_BB_MSE
                    - 파생결과파일01: MSE_movement.c
                    - 파생결과파일02: MSE_main.c
                    - 파생결과파일02: MSE_README.md
                    - 
        예시 : {RVS}{YYYY}{MMMM}{DD}
            - HS_AA_BB_MSE_00120230101_MapleStoryEngine.exe
            - HS_AA_BB_MSE_00220230101_MapleStoryEngine.exe
            - HS_AA_BB_MSE_00320230103_MapleStoryEngine.exe
            - HS_AA_BB_MSE_00420230107_MapleStoryEngine.exe
            - HS_AA_BB_MSE_00520230112_MapleStoryEngine.exe
            - HS_AA_BB_MSE_00620230125_MapleStoryEngine.exe
            - HS_AA_BB_MSE_00720230201_MapleStoryEngine.exe
            - HS_AA_BB_MSE_00820230421_MapleStoryEngine.exe

        예시 : english character recommanded
            - HS_DS_Design (추천)
            - HS_DS_디자인부서 (비추천)

        예시 : {index}
            - 상위폴더명: HS_01_AA (index : 01)
                - 하위폴더명: HS_AA_01BB
            - 상위폴더명: HS_02AA (index : None)
                - 하위폴더명: HS_02AA_01CC

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
  - HS_AP_ApplyPublic : {default}/ : 전회원지원신청폴더
    - a
      - a-d
    - b
      - b-c
    - README.txt : HS_AP_Apply /
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
  - HS_EC_ExternalCooperation : {default}/ : 대외협력부서
    - a
      - a-d
    - b
      - b-c
    - README.txt : HS_EC_ExternalCooperation/
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
    - HS_MS_HR_HumanResource : HS_MS_ManageSupport/
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
  - HS_PA_PublicForAll : {default}/ : 공용폴더(핸즈전체공개_공유)
    - a
      - a-d
    - b
      - b-c
    - README.txt :HS_PA_PublicForAll/
  - HS_PE_PublicExecutives : {default}/ : 공용폴더(임원진공개_공유)
    - a
      - a-d
    - b
      - b-c
    - README.txt : HS_PE_PublicExecutives/
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
