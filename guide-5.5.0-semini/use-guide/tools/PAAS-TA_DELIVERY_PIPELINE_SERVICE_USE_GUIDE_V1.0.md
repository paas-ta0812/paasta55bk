
# [PaaS-TA 배포 파이프라인 서비스 사용자 가이드]

## 목차
1. [문서 개요](#1)
	* [1.1. 목적](#1-1)
	* [1.2. 범위](#1-2)
2. [배포 파이프라인 서비스 신청](#2)
	* [2.1. PaaS-TA 사용자 포탈 접속](#2-1)
	* [2.2. 배포 파이프라인 서비스 신청](#2-2)
	* [2.3. 배포 파이프라인 접속](#2-3)
3. [배포 파이프라인 사용자 매뉴얼](#3)
	* [3.1. 배포 파이프라인 사용자 메뉴 구성](#3-1)
	* [3.2. 배포 파이프라인 사용자 메뉴 설명](#3-2)
	* [3.2.1. 사용자 관리](#3-2-1)
	* [3.2.1.1. 사용자 대시보드](#3-2-1-1)
	* [3.2.1.1.1. 사용자 목록 검색 조회](#3-2-1-1-1)
	* [3.2.1.1.2. 사용자 상세 조회/수정](#3-2-1-1-2)
	* [3.2.2. 파이프라인](#3-2-2)
	* [3.2.2.1. 나의 파이프라인](#3-2-2-1)
	* [3.2.2.2. 파이프라인 신규 생성](#3-2-2-2)
	* [3.2.2.2.1. 파이프라인 신규 생성(1)](#3-2-2-2-1)
	* [3.2.2.2.2. 파이프라인 신규 생성(2)](#3-2-2-2-2)
	* [3.2.2.2.3. 파이프라인 신규 생성(3)](#3-2-2-2-3)
	* [3.2.2.3.   파이프라인 대시보드](#3-2-2-3)
	* [3.2.2.3.1. 파이프라인 목록 검색 조회](#3-2-2-3-1)
	* [3.2.2.3.2. 파이프라인 상세 정보 조회](#3-2-2-3-2)
	* [3.2.2.3.3. 파이프라인 수정](#3-2-2-3-3)
	* [3.2.2.3.4. 파이프라인 삭제](#3-2-2-3-4)
	* [3.2.2.4.   파이프라인 상세](#3-2-2-4)
	* [3.2.2.4.1. 참여자 관리](#3-2-2-4-1)
	* [3.2.2.4.1.1. 참여자 추가](#3-2-2-4-1-1)
	* [3.2.2.4.1.2.    참여자 목록 검색 조회](#3-2-2-4-1-2)
	* [3.2.2.4.1.3.    참여자 상세 정보 조회/수정](#3-2-2-4-1-3)
	* [3.2.2.4.1.4.    참여자 삭제](#3-2-2-4-1-4)
	* [3.2.2.4.2. 빌드 Job](#3-2-2-4-2)
	* [3.2.2.4.2.1.    빌드 Job 생성](#3-2-2-4-2-1)
	* [3.2.2.4.2.2.    빌드 Job 구성 조회/수정](#3-2-2-4-2-2)
	* [3.2.2.4.2.3.    빌드 Job 실행](#3-2-2-4-2-3)
	* [3.2.2.4.2.4.    빌드 Job 정지](#3-2-2-4-2-4)
	* [3.2.2.4.2.5.    빌드 Job 로그/히스토리](#3-2-2-4-2-5)
	* [3.2.2.4.2.6.    빌드 Job 로그 다운로드](#3-2-2-4-2-6)
	* [3.2.2.4.2.7.    빌드 Job 추가](#3-2-2-4-2-7)
	* [3.2.2.4.2.8.    빌드 Job 복제](#3-2-2-4-2-8)
	* [3.2.2.4.2.9.    빌드 Job 삭제](#3-2-2-4-2-9)
	* [3.2.2.4.3. 테스트 Job](#3-2-2-4-3)
	* [3.2.2.4.3.1.    테스트 Job 생성](#3-2-2-4-3-1)
	* [3.2.2.4.3.2.    테스트 Job 구성 조회/수정](#3-2-2-4-3-2)
	* [3.2.2.4.3.3.    테스트 Job 실행](#3-2-2-4-3-3)
	* [3.2.2.4.3.4.    테스트 Job 정지](#3-2-2-4-3-4)
	* [3.2.2.4.3.5.    테스트 Job 로그/히스토리](#3-2-2-4-3-5)
	* [3.2.2.4.3.6.    테스트 Job 추가](#3-2-2-4-3-6)
	* [3.2.2.4.3.7.    테스트 Job 품질 이슈 결과](#3-2-2-4-3-7)
	* [3.2.2.4.3.8.    테스트 Job 복제](#3-2-2-4-3-8)
	* [3.2.2.4.3.9.    테스트 Job 삭제](#3-2-2-4-3-9)
	* [3.2.2.4.4. 배포 Job](#3-2-2-4-4)
	* [3.2.2.4.4.1.    배포 Job 생성](#3-2-2-4-4-1)
	* [3.2.2.4.4.2.    배포 Job 구성 조회/수정](#3-2-2-4-4-2)
	* [3.2.2.4.4.3.    배포 Job 실행](#3-2-2-4-4-3)
	* [3.2.2.4.4.4.    배포 Job 정지](#3-2-2-4-4-4)
	* [3.2.2.4.4.5.    배포 Job 로그/히스토리](#3-2-2-4-4-5)
	* [3.2.2.4.4.6.    배포 Job 현재 작업으로 롤백](#3-2-2-4-4-6)
	* [3.2.2.4.4.7.    배포 Job 추가](#3-2-2-4-4-7)
	* [3.2.2.4.4.8.    배포 Job 복제](#3-2-2-4-4-8)
	* [3.2.2.4.4.9.    배포 Job 삭제](#3-2-2-4-4-9)
	* [3.2.2.4.5. Job 작업 정렬](#3-2-2-4-5)
	* [3.2.2.4.6. 새 작업 그룹 추가](#3-2-2-4-6)
	* [3.2.3.     파이프라인 관리](#3-2-3)
	* [3.2.3.1.   Cloud Foundry 정보 관리](#3-2-3-1)
	* [3.2.3.1.1. Cloud Foundry 계정 등록](#3-2-3-1-1)
	* [3.2.3.1.2. Cloud Foundry 계정 수정](#3-2-3-1-2)
	* [3.2.4.     품질 관리](#3-2-4)
	* [3.2.4.1.   품질 이슈](#3-2-4-1)
	* [3.2.4.2.   코딩 규칙](#3-2-4-2)
	* [3.2.4.3.   품질 프로파일](#3-2-4-3)
	* [3.2.4.3.1. 품질 프로파일 생성](#3-2-4-3-1)
	* [3.2.4.3.2. 품질 프로파일 복제](#3-2-4-3-2)
	* [3.2.4.3.3. 품질 프로파일 수정](#3-2-4-3-3)
	* [3.2.4.3.4. 품질 프로파일 프로젝트 연결](#3-2-4-3-4)
	* [3.2.4.3.5. 품질 프로파일 삭제](#3-2-4-3-5)
	* [3.2.4.4.   품질 게이트](#3-2-4-4)
	* [3.2.4.4.1. 품질 게이트 생성](#3-2-4-4-1)
	* [3.2.4.4.2. 품질 게이트 복제](#3-2-4-4-2)
	* [3.2.4.4.3. 품질 게이트 수정](#3-2-4-4-3)
	* [3.2.4.4.4. 품질 게이트 조건 추가](#3-2-4-4-4)
	* [3.2.4.4.5. 품질 게이트 프로젝트 연결](#3-2-4-4-5)
	* [3.2.4.4.6. 품질 게이트 삭제](#3-2-4-4-6)

# <div id='1'/> 1. 문서 개요

## <div id='1-1'/> 1.1 목적
본 문서는 배포 파이프라인 서비스를 사용할 사용자의 사용 방법에 대해 기술하였다.

## <div id='1-2'/> 1.2 범위
본 문서는 Windows 환경을 기준으로 배포 파이프라인 서비스를 사용할 사용자의 사용 방법에 대해 작성되었다.

# <div id='2'/> 2. 배포 파이프라인 서비스 신청

## <div id='2-1'/> 2.1 PaaS-TA 사용자 포탈 접속
1. PaaS-Ta 사용자 포탈에 접속하여 “로그인”을 클릭한다.
![002](../images/pipeline/image002.png)

2. 사용자 계정과 비밀번호를 입력한 후 “LOGIN” 버튼을 클릭하여 사용자 포탈에 로그인한다.
![003](../images/pipeline/image003.jpg)

3. 로그인 한 후 카탈로그 페이지로 이동한다.
![004](../images/pipeline/image004.jpg)


## <div id='2-2'/> 2.2 배포 파이프라인 서비스 신청
1. 배포 파이프라인 서비스를 선택한다.
![005](../images/pipeline/image005.png)

2. 신청하고자 하는 공간을 선택한다. 이미 배포 파이프라인을 사용중인 ORG에서는 아래 첨부 사진과 같이 에러가 출력된다.
![006](../images/pipeline/image006.jpg)

3. 서비스 이름을 입력한다. 이미 신청한 배포 파이프라인의 이름이 있을 경우 아래 첨부 사진과 같이 에러가 출력된다.
![007](../images/pipeline/image007.jpg)

4. 신청을 진행한 후 스페이스 페이지의 서비스 탭에서 파이프라인 서비스 생성을 확인한다.
![008](../images/pipeline/image008.png)

## <div id='2-3'/> 2.3 배포 파이프라인 접속
1. PaaS-TA 포탈의 스페이스 페이지에서 신청된 배포 파이프라인의 “대시보드” 버튼을 클릭하여 접속을 진행한다.
![009](../images/pipeline/image009.png)

2. 배포 파이프라인 접속을 확인한다.
![010](../images/pipeline/image010.jpg)

3. 이 때 ***배포 파이프라인 서비스를 처음 생성한 사용자가 관리자가 된다.*** 우측 상단의 사용자 관리 메뉴를 클릭하여 사용자 대시보드로 이동한다.

***※ 처음 접속하는 사용자는 관리자의 승인이 없을 경우 접속할 수 없습니다.***


# <div id='3'/> 3. 배포 파이프라인 사용자 매뉴얼
본 장에서는 배포 파이프라인의 메뉴 구성 및 화면 설명에 대해서 기술하였다.

## <div id='3-1'/> 3.1 배포 파이프라인 사용자 메뉴 구성
배포 파이프라인 서비스는 파이프라인을 조회 및 관리하는 부분과 Cloud Foundry 계정 정보를 관리하는 부분, 소스 코드의 품질을 관리하는 부분, 부여된 권한에 따라 사용자를 관리할 수 있는 사용자 관리 부분으로 구성되어 있다.

***※ 기본적으로 사용자는 사용자 관리, 파이프라인 관리, 품질 관리 메뉴가 보이지 않는다.***
<table>
  <tr>
    <td>메뉴</td>
    <td>분류</td>
		<td>설명</td>
  </tr>
  <tr>
    <td>사용자 관리</td>
    <td>사용자 대시보드</td>
	  <td>파이프라인을 사용하는 사용자들의 정보 조회 및 관리</td>
  </tr>
  <tr>
		<td>파이프라인</td>
		<td>파이프라인 대시보드</td>
		<td>파이프라인 등록, 목록 및 상세 조회, 삭제, 참여자 권한 등의 기능을 관리</td>
  </tr>
	<tr>
		<td>파이프라인 관리</td>
		<td>Cloud Foundry 정보 관리</td>
		<td>Cloud Foundry 계정 정보를 관리</td>
  </tr>
	<tr>
		<th rowspan="4">품질 관리</th>
		<td>품질 이슈</td>
		<td>수행된 소스 코드의 오류 해결 여부 및 오류의 수준, 활성화 상태를 관리</td>
  </tr>
	<tr>
		<td>코딩 규칙</td>
		<td>표준화된 소스 코드의 코딩 양식을 관리</td>
	</tr>
	<tr>
		<td>품질 프로파일</td>
		<td>소스 코드의 품질을 분석하기 위한 기준이 되는 코딩 규칙을 관리</td>
	</tr>
	<tr>
		<td>품질 게이트</td>
		<td>소스 코드의 품질 분석 결과 정해진 품질 기준 값을 초과하거나 미달하지 않았는지에 대한 기준을 관리</td>
	</tr>
</table>


## <div id='3-2'/> 3.2 배포 파이프라인 사용자 메뉴 설명
본 장에서는 배포 파이프라인의 4개 메뉴에 대한 설명을 기술한다.

### <div id='3-2-1'/> 3.2.1. 사용자 관리
사용자 관리 메뉴는 관리자에게만 보이는 메뉴로써 본 장에서는 배포 파이프라인 서비스를 사용하는 사용자들의 권한 관리 및 정보 조회와 관리에 대한 설명을 기술한다.

#### <div id='3-2-1-1'/> 3.2.1.1. 사용자 대시보드

##### <div id='3-2-1-1-1'/> 3.2.1.1.1. 사용자 목록 검색 조회
1. 상단의 우측 메뉴에 “사용자 관리” 버튼을 클릭한다.
![011](../images/pipeline/image011.png)

2. 사용자 대시보드로 이동한다.
![012](../images/pipeline/image012.png)

3. 사용자 대시보드 목록에서 검색할 수 있는 조건에는 사용자 아이디를 검색어로 하는 검색과 검색 타입이 관리자/사용자인 검색 2개가 있다. 검색어를 입력 후 “ENTER”를 하거나 “돋보기” 버튼을 클릭한다.
![013](../images/pipeline/image013.png)
![014](../images/pipeline/image014.png)

##### <div id='3-2-1-1-2'/> 3.2.1.1.2. 사용자 상세 조회/수정
1. 사용자 대시보드에서 아이디를 선택하여 사용자 상세 조회/수정 페이지로 이동한다.
![015](../images/pipeline/image015.png)

2. 사용자의 정보를 상세 조회한다.
![016](../images/pipeline/image016.jpg)

3. 정보를 수정하고자 할 때 입력 값을 새롭게 입력한다. 권한은 관리자/사용자로 선택할 수 있다.
![017](../images/pipeline/image017.jpg)

4. 입력 값을 수정 후 “수정” 버튼을 클릭한다.
![018](../images/pipeline/image018.png)

5. 수정된 정보를 확인한다.
![019](../images/pipeline/image019.jpg)


### <div id='3-2-2'/> 3.2.2. 파이프라인
본 장에서는 파이프라인을 관리하는 2개 방법에 대한 설명을 기술한다.

***※ 기본적으로 사용자는 파이프라인을 보기만 할 수 있고, 생성, 조회, 수정, 삭제할 수 없다. 하지만 파이프라인 참여자 권한이 부여되었을 경우에는 조건에 따라 파이프라인 생성, 조회, 수정, 삭제가 가능해진다.***

#### <div id='3-2-2-1'/> 3.2.2.1. 나의 파이프라인
1.	어떤 페이지에 있든 상관없이 Drop down 메뉴의 나의 파이프라인 버튼을 클릭하면 대시보드로 이동한다.
![020](../images/pipeline/image020.png)
![021](../images/pipeline/image021.jpg)
2.	나의 파이프라인에서 목록의 파이프라인 명을 클릭하면 해당 파이프라인의 상세 페이지로 이동한다.
![022](../images/pipeline/image022.png)
![023](../images/pipeline/image023.png)

#### <div id='3-2-2-2'/> 3.2.2.2. 파이프라인 신규 생성
##### <div id='3-2-2-2-1'/> 3.2.2.2.1. 파이프라인 신규 생성(1)
1. 상단 메뉴의 “파이프라인 목록” 을 클릭하면 파이프라인 명 입력만으로 즉시 파이프라인을 신규 생성할 수 있다.
![024](../images/pipeline/image024.png)
2. 등록 버튼을 누른 후 대시보드에 추가된 파이프라인을 확인할 수 있다.
![025](../images/pipeline/image025.png)
3. Drop down 메뉴에도 등록된 파이프라인을 확인할 수 있다.
![026](../images/pipeline/image026.png)
##### <div id='3-2-2-2-2'/> 3.2.2.2.2. 파이프라인 신규 생성(2)
1.	오른쪽 상단의 “신규 생성” 버튼을 클릭한다.
***※ 사용자는 “신규 생성” 버튼이 활성화되지 않는다.***
![027](../images/pipeline/image027.png)
2.	파이프라인 신규 생성 페이지로 이동한다.
![028](../images/pipeline/image028.png)
3.	파이프라인 명은 필수로 입력받기 때문에 파이프라인 명을 반드시 입력한 후 “생성” 버튼을 클릭한다.
![029](../images/pipeline/image029.png)
4.	생성된 후 파이프라인 대시보드에서 새로 추가된 파이프라인 명을 확인한다.
![030](../images/pipeline/image030.png)

##### <div id='3-2-2-2-3'/> 3.2.2.2.3. 파이프라인 신규 생성(3)
***※ 사용자는 파이프라인에 대한 참여자 권한이 주어지지 않으면 파이프라인 상세 페이지로 이동할 수 없다.***
1. 오른쪽 상단의 “신규 생성” 버튼을 클릭한다.
![031](../images/pipeline/image031.png)
2. 파이프라인 신규 생성 페이지로 이동한다.
![032](../images/pipeline/image032.jpg)
3. 이후 생성 과정은 3.2.2.2.2. 파이프라인 신규 생성(2) 참고.

#### <div id='3-2-2-3'/> 3.2.2.3. 파이프라인 대시보드
##### <div id='3-2-2-3-1'/> 3.2.2.3.1. 파이프라인 목록 검색 조회
1. 목록에서 검색할 수 있는 조건은 파이프라인 명과 날짜/업데이트/이름순 필터 2개이다.
![033](../images/pipeline/image033.png)
2.	검색어를 입력 후 “ENTER”를 하거나 “돋보기” 버튼을 클릭한다.
![034](../images/pipeline/image034.png)
3.	목록 조회/검색 목록 조회일 때 모두 검색 타입 필터를 선택하면 즉시 반영된다.
![035](../images/pipeline/image035.png)

##### <div id='3-2-2-3-2'/> 3.2.2.3.2. 파이프라인 상세 정보 조회
1.	파이프라인 대시보드에서 파이프라인 명을 눌러 파이프라인 상세 페이지로 이동한다.
![036](../images/pipeline/image036.jpg)
2.	파이프라인 상세페이지에서 오른쪽 상단에 “정보보기/수정” 버튼을 클릭한다.
![037](../images/pipeline/image037.png)
3.	파이프라인 정보보기/수정 페이지로 이동하여 해당 파이프라인의 정보를 상세 조회한다.
![038](../images/pipeline/image038.png)


##### <div id='3-2-2-3-3'/> 3.2.2.3.3. 파이프라인 수정
1.	파이프라인 정보보기/수정 페이지에서 입력 값을 수정 후 “수정” 버튼을 클릭한다.
![039](../images/pipeline/image039.jpg)

2.	수정하고 나면 파이프라인 상세 페이지로 이동한다. 다시 “정보보기/수정” 버튼을 클릭하여 변경된 값을 확인한다.
![040](../images/pipeline/image040.jpg)

##### <div id='3-2-2-3-4'/> 3.2.2.3.4. 파이프라인 삭제
1.	파이프라인 정보보기/수정 페이지에서 “파이프라인 삭제” 버튼을 클릭한다.
![041](../images/pipeline/image041.png)
2.	삭제 후에 파이프라인 대시보드로 이동하여 파이프라인이 삭제되었는지 확인한다.
![042](../images/pipeline/image042.jpg)


#### <div id='3-2-2-4'/> 3.2.2.4. 파이프라인 상세
본 장에서는 파이프라인에 참여하는 참여자 추가, 수정, 삭제 및 권한 부여 등 전반적인 참여자 관리와 하나의 파이프라인에 대한 Job들을 생성 및 실행, 삭제, 로그/히스토리 조회, 참여자 등을 관리하는 방법에 대해 기술한다.
##### <div id='3-2-2-4-1'/> 3.2.2.4.1. 참여자 관리
###### <div id='3-2-2-4-1-1'/> 3.2.2.4.1.1. 참여자 추가
***※	관리자는 파이프라인 생성자이므로 기본적으로 생성 권한을 가진 참여자이다.***
1.	파이프라인 상세페이지에서 참여자 탭을 선택한다.
![043](../images/pipeline/image043.png)
2.	우측 상단에 “참여자 추가” 버튼을 클릭한다.
![044](../images/pipeline/image044.png)
3.	참여자 추가 페이지로 이동하여 현재 배포 파이프라인에 초대된 사용자를 검색하고, 선택한다. 권한은 보기, 생성, 실행 권한 중 한 개를 선택하여 “추가” 버튼을 클릭한다.
![045](../images/pipeline/image045.png)
4.	참여자 탭에서 추가된 참여자를 확인한다.
![046](../images/pipeline/image046.png)

###### <div id='3-2-2-4-1-2'/> 3.2.2.4.1.2. 참여자 목록 검색 조회
1.	참여자 목록에서 검색할 수 있는 조건은 참여자 아이디 검색 1개이다.
![047](../images/pipeline/image047.png)
2.	검색어를 입력 후 “ENTER”를 하거나 “돋보기” 버튼을 클릭한 후 검색 조회를 한다.
![048](../images/pipeline/image048.jpg)

###### <div id='3-2-2-4-1-3'/> 3.2.2.4.1.3.	참여자 상세 정보 조회/수정
1.	참여자 목록에서 정보 조회할 참여자 아이디를 선택한다.
![049](../images/pipeline/image049.png)
2.	참여자 상세 정보 조회/수정 페이지로 이동하여 참여자의 상세 정보를 조회한다.
![050](../images/pipeline/image050.jpg)
3.	수정하고자 하는 권한을 선택하여 “수정” 버튼을 클릭한다.
![051](../images/pipeline/image051.png)
4.	참여자 목록에서 수정된 참여자의 권한을 확인한다.
![052](../images/pipeline/image052.png)


###### <div id='3-2-2-4-1-4'/> 3.2.2.4.1.4.	참여자 삭제
1.	참여자 목록에서 삭제할 참여자 아이디를 선택한다.
![053](../images/pipeline/image053.png)
2.	참여자 상세 정보 조회/수정 페이지로 이동한다.
![053-2](../images/pipeline/image053(2).png)
3.	“참여자 삭제” 버튼을 클릭한다.
![054](../images/pipeline/image054.png)
4.	참여자 목록에서 참여자가 삭제되었음을 확인한다.
![055](../images/pipeline/image055.jpg)


##### <div id='3-2-2-4-2'/> 3.2.2.4.2. 빌드 Job
###### <div id='3-2-2-4-2-1'/> 3.2.2.4.2.1. 빌드 Job 생성
1.	파이프라인 상세 페이지에서 ‘이곳을 클릭하여 새 작업 추가’ 버튼을 클릭한다.
![056](../images/pipeline/image056.png)
2.	구성 상세페이지로 이동한다.
![057](../images/pipeline/image057.jpg)
3. 작업 유형을 선택한 후 원하는 저장소를 입력 유형으로 선택한다. 그 후에 선택한 저장소의 아이디와 비밀번호를 입력 후 해당하는 저장소의 경로를 입력하여 “조회” 버튼을 클릭한다. 조회한 Branch를 선택 후 작업 트리거는 각자의 상황에 맞게 선택한다.<br>
![058](../images/pipeline/image058.jpg)

4.	생성된 빌드 Job 을 파이프라인 상세 페이지에서 확인한다.
![059](../images/pipeline/image059.png)

***※ 빌드 Job 생성은 관리자와 파이프라인 참여자 중 생성 권한을 가진 참여자만 생성이 가능하다.***

###### <div id='3-2-2-4-2-2'/> 3.2.2.4.2.2. 빌드 Job 구성 조회/수정
1. 생성된 빌드 Job 의 “구성” 아이콘을 클릭한다.<br>
![060](../images/pipeline/image060.png)
2. 구성 상세페이지로 이동하여 생성 시 저장해 놓았던 구성 정보들을 조회한다.
![061](../images/pipeline/image061.jpg)
3. 수정 시에는 각 입력 폼에 수정할 정보들을 다시 입력한 후 “저장” 버튼을 클릭한다.
![062](../images/pipeline/image062.png)
4. 구성 상세페이지로 이동하여 수정된 정보들을 확인한다.
![063](../images/pipeline/image063.jpg)

***※ 빌드 Job 구성 조회는 파이프라인 참여자이면 모두 조회가 가능하다. 하지만 수정은 관리자와 파이프라인 참여자 중 생성 권한을 가진 참여자만 수정이 가능하다.***

###### <div id='3-2-2-4-2-3'/> 3.2.2.4.2.3. 빌드 Job 실행
1. 파이프라인 상세페이지에서 “실행” 아이콘을 클릭한다.<br>
![064](../images/pipeline/image064.png)
2. 실행이 될 때 파란색으로 바뀌며 깜빡이는 것을 확인할 수 있다. (실행 중에 “로그/히스토리” 아이콘을 클릭하여 실시간으로 로그를 조회할 수 있다.)
![065](../images/pipeline/image065.jpg)
3. 실행이 완료되면 초록색으로 바뀌며 작업 부분에 Build(실행완료) 로 표시된다.
![066](../images/pipeline/image066.jpg)

***※	빌드 Job 실행은 관리자와 파이프라인 참여자 중 생성 권한과 실행 권한을 가진 참여자만 가능하다.***


###### <div id='3-2-2-4-2-4'/> 3.2.2.4.2.4. 빌드 Job 정지
1.	실행 중인 빌드 Job을 정지 및 취소하고 싶을 때 “정지” 아이콘을 클릭한다.
![067](../images/pipeline/image067.png)
2.	정지된 빌드 Job은 주황색으로 바뀌는 것을 확인할 수 있다.
![068](../images/pipeline/image068.jpg)

***※	빌드 Job 정지는 관리자와 파이프라인 참여자 중 생성 권한과 실행 권한을 가진 참여자만 가능하다.***


###### <div id='3-2-2-4-2-5'/> 3.2.2.4.2.5.	빌드 Job 로그/히스토리
1.	빌드 Job 실행이 진행 중일 때 “로그/히스토리” 아이콘을 클릭하여 실시간으로 로그를 조회할 수 있다.
![069](../images/pipeline/image069.png)
2.	로그 조회 페이지로 이동한다. 실시간으로 로그가 보이고 있는 것을 확인한다.
![070](../images/pipeline/image070.jpg)
3.	빌드 Job 실행이 완료된 것을 확인하고, 히스토리를 확인한다.
![071](../images/pipeline/image071.jpg)
4.	로그/히스토리 페이지에서 상단의 “취소” 버튼 또는 “실행” 버튼을 클릭하여 Job을 취소하고, 실행할 수 있다.
![072](../images/pipeline/image072.png)
![073](../images/pipeline/image073.png)
5.	로그/히스토리 페이지에서 “구성” 버튼을 클릭하면 빌드 Job 구성 조회 페이지로 이동한다.
![074](../images/pipeline/image074.png)
6.	로그/히스토리 페이지에서 “목록” 버튼을 클릭하면 파이프라인 상세페이지로 이동한다.
![075](../images/pipeline/image075.png)

***※	빌드 Job 로그/히스토리는 관리자와 모든 파이프라인 참여자가 조회 가능하나 실행 및 정지 버튼은 생성 권한과 실행 권한을 가진 참여자만 가능하다.***

###### <div id='3-2-2-4-2-6'/> 3.2.2.4.2.6.	빌드 Job 로그 다운로드
1.	빌드 Job 실행이 성공하면 로그/히스토리 페이지에서 “다운로드” 버튼이 활성화된다. 활성화된 “다운로드” 버튼을 클릭한다.<br>
![076](../images/pipeline/image076.png)
2.	Build 된 파일(ex. war, jar, zip 등)이 다운로드 된다.
![077](../images/pipeline/image077.png)

***※	빌드 Job 로그 다운로드는 관리자와 모든 파이프라인 참여자가 가능하다.***

###### <div id='3-2-2-4-2-7'/> 3.2.2.4.2.7.	빌드 Job 추가
1.	파이프라인 상세페이지에서 빌드 Job의 “추가” 버튼을 클릭한다.
![078](../images/pipeline/image078.png)
2.	구성 상세페이지로 이동한다.
![079](../images/pipeline/image079.jpg)
3.	빌드 Job 생성과 같이 입력 폼에 알맞은 값들을 입력한 후 ”저장” 버튼을 클릭한다.(작업 유형은 빌드 이외에도 테스트, 배포 유형 선택이 가능하다.)
![080](../images/pipeline/image080.jpg)
4.	추가된 빌드 Job 을 확인한다.<br>
![081](../images/pipeline/image081.png)
5.	작업 트리거에서 이 작업(Job)을 새 작업 그룹으로 구성을 체크하면 새로운 그룹으로 Job이 추가된다. (이후에 새 작업 그룹 추가 항목에서 설명하겠습니다.)

***※	빌드 Job 추가는 관리자와 생성 권한을 가진 파이프라인 참여자만 가능하다.***

###### <div id='3-2-2-4-2-8'/> 3.2.2.4.2.8.	빌드 Job 복제
1.	파이프라인 상세페이지에서 빌드 Job의 “복제” 버튼을 클릭한다.
![082](../images/pipeline/image082.png)
2. 빌드 Job 이 복제된 것을 확인한다.
![083](../images/pipeline/image083.jpg)

***※	빌드 Job 복제는 관리자와 생성 권한을 가진 파이프라인 참여자만 가능하다.***

###### <div id='3-2-2-4-2-9'/> 3.2.2.4.2.9.	빌드 Job 삭제
1.	파이프라인 상세페이지에서 빌드 Job의 “삭제” 버튼을 클릭한다.
![084](../images/pipeline/image084.png)
2.	빌드 Job 이 삭제된 것을 확인한다.
![084-2](../images/pipeline/image084(2).png)

***※	빌드 Job 삭제는 관리자와 생성 권한을 가진 파이프라인 참여자만 가능하다.***


##### <div id='3-2-2-4-3'/> 3.2.2.4.3. 테스트 Job
###### <div id='3-2-2-4-3-1'/> 3.2.2.4.3.1. 테스트 Job 생성
1.	Job의 “추가” 버튼을 클릭한다.
![084-3](../images/pipeline/image084(3).png)
2.	구성 페이지로 이동하여 작업 유형을 테스트(Test)로 선택한 후 입력 유형에서 원하는 품질 프로파일과 품질 게이트, 작업 그룹을 선택한다. 그 후에 작업 트리거는 각자의 상황에 맞게 선택한다.
![085](../images/pipeline/image085.jpg)
3.	“저장” 버튼을 클릭하고, 파이프라인 상세페이지에서 테스트 Job 생성된 것을 확인한다.
![086](../images/pipeline/image086.png)

***※	테스트 Job 생성은 관리자와 파이프라인 참여자 중 생성 권한을 가진 참여자만 생성이 가능하다.***

###### <div id='3-2-2-4-3-2'/> 3.2.2.4.3.2. 테스트 Job 구성 조회/수정
1.	생성된 테스트 Job 의 “구성” 아이콘을 클릭한다.
![087](../images/pipeline/image087.png)
2.	구성 상세페이지로 이동하여 생성 시 저장해 놓았던 구성 정보들을 조회한다.
![087-2](../images/pipeline/image087(2).png)
3.	수정 시에는 각 입력 폼에 수정할 정보들을 다시 입력한 후 “저장” 버튼을 클릭한다.
![088](../images/pipeline/image088.png)
4.	구성 상세페이지로 이동하여 수정된 정보들을 확인한다.
![089](../images/pipeline/image089.jpg)

***※	테스트 Job 구성 조회는 파이프라인 참여자이면 모두 조회가 가능하다. 하지만 수정은 관리자와 파이프라인 참여자 중 생성 권한을 가진 참여자만 수정이 가능하다.***

###### <div id='3-2-2-4-3-3'/> 3.2.2.4.3.3.	테스트 Job 실행
1.	파이프라인 상세페이지에서 테스트 Job의 “실행” 아이콘을 클릭한다.
![090](../images/pipeline/image090.png)
2.	실행이 될 때 파란색으로 바뀌며 깜빡이는 것을 확인할 수 있다. (실행 중에 “로그/히스토리” 아이콘을 클릭하여 실시간으로 로그를 조회할 수 있다.)
![091](../images/pipeline/image091.jpg)
3. 실행이 완료되면 초록색으로 바뀌며 작업 부분에 Test(실행완료) 로 표시된다.

***※	테스트 Job 실행은 관리자와 파이프라인 참여자 중 생성 권한과 실행 권한을 가진 참여자만 가능하다.***

###### <div id='3-2-2-4-3-4'/> 3.2.2.4.3.4.	테스트 Job 정지
1.	실행 중인 테스트 Job을 정지 및 취소하고 싶을 때 “정지” 아이콘을 클릭한다.
![092](../images/pipeline/image092.png)
2.	정지된 빌드 Job은 주황색으로 바뀌는 것을 확인할 수 있다
![093](../images/pipeline/image093.jpg)

***※	테스트 Job 정지는 관리자와 파이프라인 참여자 중 생성 권한과 실행 권한을 가진 참여자만 가능하다.***

###### <div id='3-2-2-4-3-5'/> 3.2.2.4.3.5.	테스트 Job 로그/히스토리
1.	빌드 Job 실행이 진행 중일 때 “로그/히스토리” 아이콘을 클릭하여 실시간으로 로그를 조회할 수 있다.
![094](../images/pipeline/image094.png)
2.	로그 조회 페이지로 이동한다. 실시간으로 로그가 보이고 있는 것을 확인한다.
![095](../images/pipeline/image095.jpg)
3.	테스트 Job 실행이 완료된 것을 확인하고, 히스토리를 확인한다.
![096](../images/pipeline/image096.jpg)
4.	“실행”, “취소”, “구성”, “목록” 버튼은 3.2.2.4.2.5. 빌드 Job 로그/히스토리 항목을 참고한다.

***※	테스트 Job 로그/히스토리는 관리자와 모든 파이프라인 참여자가 조회 가능하나 실행 및 정지 버튼은 생성 권한과 실행 권한을 가진 참여자만 가능하다.***


###### <div id='3-2-2-4-3-6'/> 3.2.2.4.3.6.	테스트 Job 품질 이슈 결과
1.	테스트 Job의 로그/히스토리 “품질 이슈 결과” 버튼을 누르면 수행된 소스 코드의 오류 해결 여부 및 오류의 수준, 활성화 상태를 관리하는 품질 관리 대시보드로 이동한다.
![097](../images/pipeline/image097.jpg)
2.	품질 관리 대시보드에 대해서는 이후 3.2.4 품질 관리 부분을 참고한다.

***※	테스트 Job 품질 이슈 결과는 관리자와 모든 파이프라인 참여자가 조회 가능하다.***

###### <div id='3-2-2-4-3-7'/> 3.2.2.4.3.7.	테스트 Job 추가
1.	파이프라인 상세페이지에서 테스트 Job의 “추가” 버튼을 클릭한다.
![098](../images/pipeline/image098.png)
2.	그 이후의 과정은 3.2.2.4.2.7. 빌드 Job 추가 항목을 참고한다.

***※	테스트 Job 추가는 관리자와 생성 권한을 가진 파이프라인 참여자만 가능하다.***

###### <div id='3-2-2-4-3-8'/> 3.2.2.4.3.8.	테스트 Job 복제
1.	파이프라인 상세페이지에서 테스트 Job의 “복제” 버튼을 클릭한다.
![099](../images/pipeline/image099.png)
2.	테스트 Job 이 복제된 것을 확인한다.
![100](../images/pipeline/image100.jpg)

***※	테스트 Job 복제는 관리자와 생성 권한을 가진 파이프라인 참여자만 가능하다.***

###### <div id='3-2-2-4-3-8'/> 3.2.2.4.3.9.	테스트 Job 삭제
1.	파이프라인 상세페이지에서 테스트 Job의 “삭제” 버튼을 클릭한다.
![101](../images/pipeline/image101.png)
2.	테스트 Job 이 삭제된 것을 확인한다.
![102](../images/pipeline/image102.jpg)

***※	테스트 Job 삭제는 관리자와 생성 권한을 가진 파이프라인 참여자만 가능하다.***


##### <div id='3-2-2-4-4'/> 3.2.2.4.4.	배포 Job
###### <div id='3.2.2.4.4.1'/> 3.2.2.4.4.1.	배포 Job 생성
1. Job의 “추가” 버튼을 클릭한다.<br>
![103](../images/pipeline/image103.png)
2.	구성 페이지로 이동하여 작업 유형을 배포(Deploy)로 선택한 후 유형에서 원하는 배포 유형을 선택, 파이프라인 관리에서 저장해 놓은 Cloud Foundry 정보를 선택한다. (Cloud Foundry 정보를 가져오기 위해서는 선행 과정이 필요하다. 과정은 3.2.3.1. Cloud Foundry 정보 관리 항목을 참고한다). 그다음 MANIFEST 사용 여부를 체크 후 입력 유형과 작업 트리거를 차례로 입력한다.
![104](../images/pipeline/image104.jpg)
3.	“저장” 버튼을 클릭하고, 파이프라인 상세페이지에서 배포 Job이 생성된 것을 확인한다.
![105](../images/pipeline/image105.png)

***※	배포 Job 생성은 관리자와 파이프라인 참여자 중 생성 권한을 가진 참여자만 생성이 가능하다.***

###### <div id='3-2-2-4-4-2'/> 3.2.2.4.4.2.	배포 Job 구성 조회/수정
1.	생성된 배포 Job 의 “구성” 아이콘을 클릭한다.
![106](../images/pipeline/image106.png)
2.	구성 상세페이지로 이동하여 생성 시 저장해 놓았던 구성 정보들을 조회한다.
![104](../images/pipeline/image104.png)
3.	수정 시에는 각 입력 폼에 수정할 정보들을 다시 입력한 후 “저장” 버튼을 클릭한다.
![107](../images/pipeline/image107.png)
4.	구성 상세페이지로 이동하여 수정된 정보들을 확인한다.

***※	 배포 Job 구성 조회는 파이프라인 참여자이면 모두 조회가 가능하다. 하지만 수정은 관리자와 파이프라인 참여자 중 생성 권한을 가진 참여자만 수정이 가능하다.***

###### <div id='3-2-2-4-4-3'/> 3.2.2.4.4.3.	배포 Job 실행
1.	파이프라인 상세페이지에서 배포 Job의 “실행” 아이콘을 클릭한다.
![108](../images/pipeline/image108.png)
2.	실행이 될 때 파란색으로 바뀌며 깜빡이는 것을 확인할 수 있다. (실행 중에 “로그/히스토리” 아이콘을 클릭하여 실시간으로 로그를 조회할 수 있다.)
![109](../images/pipeline/image109.jpg)
3. 실행이 완료되면 초록색으로 바뀌며 작업 부분에 Deploy(실행완료) 로 표시된다.
![110](../images/pipeline/image110.jpg)

***※	배포 Job 실행은 관리자와 파이프라인 참여자 중 생성 권한과 실행 권한을 가진 참여자만 가능하다.***

###### <div id='3-2-2-4-4-4'/> 3.2.2.4.4.4.	배포 Job 정지
1.	실행 중인 배포 Job을 정지 및 취소하고 싶을 때 “정지” 아이콘을 클릭한다.
![111](../images/pipeline/image111.png)
2.	정지된 배포 Job이 주황색으로 바뀌는 것을 확인할 수 있다.
![112](../images/pipeline/image112.jpg)

***※	배포 Job 정지는 관리자와 파이프라인 참여자 중 생성권한과 실행 권한을 가진 참여자만 가능하다.***

###### <div id='3-2-2-4-4-5'/> 3.2.2.4.4.5.	배포 Job 로그/히스토리
1.	배포 Job 실행이 진행 중일 때 “로그/히스토리” 아이콘을 클릭하여 실시간으로 로그를 조회할 수 있다.
![113](../images/pipeline/image113.png)
2.	로그 조회 페이지로 이동한다. 실시간으로 로그가 보이고 있는 것을 확인한다.
![114](../images/pipeline/image114.jpg)
3.	배포 Job 실행이 완료된 것을 확인하고, 히스토리를 확인한다.
![115](../images/pipeline/image115.jpg)
4.	PaaS-TA 포탈로 Cloud Foundry 계정을 만들어 배포한 결과 PaaS-TA 포탈 대시보드에서 공간의 애플리케이션 부분에 ‘testtest’라는 애플리케이션이 배포되었음을 확인할 수 있다.
![116](../images/pipeline/image116.png)

***※	배포 Job 로그/히스토리는 관리자와 모든 파이프라인 참여자가 조회 가능하나 실행 및 정지 버튼은 생성권한과 실행 권한을 가진 참여자만 가능하다.***

###### <div id='3-2-2-4-4-6'/> 3.2.2.4.4.6.	배포 Job 현재 작업으로 롤백
1.	배포 Job 의 로그/히스토리 페이지에서 “현재 작업으로 롤백” 버튼을 클릭한다.
![117](../images/pipeline/image117.png)
2.	현재 작업으로 롤백하는 창이 뜨고 Cloud Foundry 정보와 조직/공간 입력 값을 수정할 수 있다.
예를 들어 애플리케이션 명을 ‘test-hrjin’이라 수정하고 “롤백” 버튼을 클릭한다.
![118](../images/pipeline/image118.png)
3.	롤백을 진행한다.
![119](../images/pipeline/image119.jpg)
4.	롤백 진행 후 PaaS-TA 포탈에서 확인한 결과 ‘test-hrjin’ 이란 이름의 애플리케이션이 배포 완료되었다.
![120](../images/pipeline/image120.png)

***※	배포 Job 현재 작업으로 롤백은 관리자와 생성권한과 실행 권한을 가진 참여자만 가능하다.***

###### <div id='3-2-2-4-4-7'/> 3.2.2.4.4.7.	배포 Job 추가
1.	파이프라인 상세페이지에서 테스트 Job의 “추가” 버튼을 클릭한다.
![121](../images/pipeline/image121.png)
2.	그 이후의 과정은 3.2.2.4.2.7. 빌드 Job 추가, 3.2.2.4.3.7. 테스트 Job 추가 항목을 참고한다.

***※	배포 Job 추가는 관리자와 생성권한을 가진 파이프라인 참여자만 가능하다.***

###### <div id='3-2-2-4-4-8'/> 3.2.2.4.4.8.	배포 Job 복제
1.	파이프라인 상세페이지에서 배포 Job의 “복제” 버튼을 클릭한다.
![122](../images/pipeline/image122.png)
2.	배포 Job 이 복제된 것을 확인한다.
![123](../images/pipeline/image123.jpg)

***※	배포 Job 복제는 관리자와 생성권한을 가진 파이프라인 참여자만 가능하다.***

###### <div id='3-2-2-4-4-9'/> 3.2.2.4.4.9.	배포 Job 삭제
1.	파이프라인 상세페이지에서 배포 Job의 “삭제” 버튼을 클릭한다.
![124](../images/pipeline/image124.png)
2.	배포 Job 이 삭제된 것을 확인한다.
![125](../images/pipeline/image125.jpg)

***※	배포 Job 삭제는 관리자와 생성권한을 가진 파이프라인 참여자만 가능하다.***

##### <div id='3-2-2-4-5'/> 3.2.2.4.5. Job 작업 정렬
1.	파이프라인 상세페이지에서 각 Job의 “작업 정렬” 아이콘을 클릭한다.
![126](../images/pipeline/image126.png)
2.	현재 작업 그룹 내에서 정렬할 수 있는 나머지 Job의 번호의 목록이 drop down 메뉴로 보인다.
![127](../images/pipeline/image127.png)
3.	그중 정렬하고자 하는 번호를 클릭 시 그 번호의 Job 과 위치가 서로 바뀌게 되며 정렬된다.
![128](../images/pipeline/image128.jpg)

***※	Job 작업 정렬은 관리자와 생성권한을 가진 파이프라인 참여자만 가능하다.***

##### <div id='3-2-2-4-6'/> 3.2.2.4.6. 새 작업 그룹 추가
1.	파이프라인 상세페이지에서 “새 작업 그룹 추가” 버튼을 클릭한다.
![129](../images/pipeline/image129.png)
2.	Job 구성 상세페이지로 이동한다.
![130](../images/pipeline/image130.jpg)
3.	새로운 Job 한 개를 생성한 뒤 파이프라인 상세페이지로 이동한다. 이전 작업 그룹 아래로 점선이 생기며 새로 생성한 Job이 새로운 그룹 내로 나눠진 것을 확인할 수 있다.
![131](../images/pipeline/image131.png)

***※	Job 새 작업  그룹 추가는 관리자와 생성권한을 가진 파이프라인 참여자만 가능하다.***

### <div id='3-2-3'/> 3.2.3. 파이프라인 관리
본 장에서는 Cloud Foundry 정보를 등록하여 Job을 배포할 Cloud Foundry target URL을 연동하는 과정에 대하여 기술한다.
#### <div id='3-2-3-1'/> 3.2.3.1. Cloud Foundry 정보 관리
###### <div id='3-2-3-1-1'/> 3.2.3.1.1. Cloud Foundry 계정등록
1. Cloud Foundry 정보 관리 대시보드에서 우측 상단에 “Cloud Foundry 계정 등록” 버튼을 클릭한다.
![132](../images/pipeline/image132.png)
2. Cloud Foundry 계정 등록 페이지로 이동한다.
![133](../images/pipeline/image133.jpg)
3. 계정 명을 입력한 후 아이디와 비밀번호에는 Cloud Foundry 로그인에 필요한 아이디와 비밀번호를 입력한다.
![134](../images/pipeline/image134.png)
4. URL에는 “URL 관리” 버튼을 클릭한 후 팝업 창이 뜨면 “URL 등록” 버튼을 클릭하여 Cloud Foundry 계정 정보를 등록하도록 한다.<br>
![135](../images/pipeline/image135.png)
5. Cloud Foundry API 명(ex. api)을 입력하고, Job 배포 계정으로 사용하고자 하는 Cloud Foundry target API URL(ex. https://api.115.68.46.186.xip.io) 을 입력한 후 “URL 저장” 버튼을 클릭한다.
![136](../images/pipeline/image136.png)
6. URL이 등록되었음을 확인한다.<br>
![137](../images/pipeline/image137.png)
7. 다시 계정 등록 화면으로 돌아와 등록한 URL을 선택 후 나머지 값을 입력한다. 마지막으로 “등록” 버튼을 클릭한다.
![138](../images/pipeline/image138.png)
8. Cloud Foundry 정보 관리 대시보드에서 Cloud Foundry 계정 정보가 정상적으로 등록되었음을 확인한다.
![139](../images/pipeline/image139.png)

###### <div id='3-2-3-1-2'/> 3.2.3.1.2. Cloud Foundry 계정수정
1.	Cloud Foundry 정보 관리 대시보드에서 수정하고자 하는 계정을 클릭한다.
![140](../images/pipeline/image140.jpg)
2.	수정할 값들을 입력하고 “수정” 버튼을 클릭한다.
![141](../images/pipeline/image141.png)
3.	다시 대시보드를 통해 계정 상세 페이지로 이동 후 수정되었는지 확인한다.

### <div id='3-2-4'/> 3.2.4. 품질 관리
본 장에서는 테스트 Job을 통해 검사한 소스 코드와 관련하여 품질 이슈와 코딩 규칙, 품질 프로파일, 품질 게이트에 대한 설명을 기술한다.
#### <div id='3-2-4-1'/> 3.2.4.1. 품질 이슈
1.	품질 관리 메뉴에서 품질 이슈를 클릭하여 품질 이슈 대시보드로 이동한다.
![142](../images/pipeline/image142.jpg)
2.	“규칙상세” 버튼을 클릭한다.
![143](../images/pipeline/image143.jpg)
3.	오른쪽 상단의 “목록” 버튼을 클릭하면 Job 테스트 목록이 있는 품질 이슈 대시보드로 이동한다.

#### <div id='3-2-4-2'/> 3.2.4.2. 코딩 규칙
1.	품질 관리 메뉴에서 코딩 규칙을 클릭하여 코딩 규칙 대시보드로 이동한다.
![144](../images/pipeline/image144.jpg)
2.	“프로파일에 추가” 버튼을 클릭한 뒤 프로파일 추가 팝업 창에서 이슈 수준을 정한 후 “추가” 버튼을 클릭한다.
![145](../images/pipeline/image145.png)
3. 왼쪽 하단에 품질 프로파일 메뉴에서 이전 단계에서 선택한 Default^Default-QualityProfle 을 클릭하여 추가한 코딩 규칙이 추가되었는지 확인한다.<br>
![146](../images/pipeline/image146.png)
4.	“프로파일에 제거” 버튼을 클릭한다.
![147](../images/pipeline/image147.png)
5.	제거한 코딩 규칙이 품질 프로파일에서 삭제된 것을 확인한다.
![148](../images/pipeline/image148.png)

#### <div id='3-2-4-3'/> 3.2.4.3. 품질 프로파일
##### <div id='3-2-4-3-1'/> 3.2.4.3.1. 품질 프로파일 생성
1.	품질 관리 메뉴에서 품질 프로파일을 선택하여 품질 프로파일 대시보드로 이동한다.
![149](../images/pipeline/image149.jpg)
2.	우측 상단의 “생성” 버튼을 클릭한다.
![150](../images/pipeline/image150.png)
3.	품질 프로파일 명을 입력하고, 개발언어를 선택하여 “생성” 버튼을 클릭한다.
![151](../images/pipeline/image151.png)
4.	품질 프로파일이 생성된 것을 확인한다.
![152](../images/pipeline/image152.png)

##### <div id='3-2-4-3-2'/> 3.2.4.3.2. 품질 프로파일 복제
1.	품질 프로파일 대시보드에서 “복제” 버튼을 클릭한다.
![153](../images/pipeline/image153.png)
2.	복제할 품질 프로파일의 이름을 입력하고, “복제” 버튼을 클릭한다.
![154](../images/pipeline/image154.png)
3.	복제된 품질 프로파일을 확인한다.
![155](../images/pipeline/image155.png)

##### <div id='3-2-4-3-3'/> 3.2.4.3.3. 품질 프로파일 수정
1.	품질 프로파일 대시보드에서 “수정” 버튼을 클릭한다.
![156](../images/pipeline/image156.png)
2.	수정할 품질 프로파일 팝업창이 뜨면 품질 프로파일 명을 수정하고 “수정” 버튼을 클릭한다.
![157](../images/pipeline/image157.png)
3. 품질 프로파일 명이 수정되었음을 확인한다.
![158](../images/pipeline/image158.png)

##### <div id='3-2-4-3-4'/> 3.2.4.3.4. 품질 프로파일 프로젝트 연결
1.	품질 프로파일 대시보드에서 연결된 프로젝트 항목을 확인한다. (첫 번째 사진은 테스트 Job 구성 조회 시 품질 프로파일을 Default-QualityProfile 로 설정한 것이다. 그러므로 두 번째 사진에서 예시로 새로 생성한 품질 프로파일[QualityProfile_hrjin]에는 연결된 프로젝트가 보이지 않는다.)
![159](../images/pipeline/image159.jpg)
2.	연결된 프로젝트가 없을 경우 “미연결” 탭을 클릭한다.
![160](../images/pipeline/image160.png)
3.	해당 품질 프로파일과 연결할 테스트 Job 프로젝트를 선택한다. 품질 프로파일 1개 당 여러 프로젝트 연결이 가능하다.
![161](../images/pipeline/image161.png)
##### <div id='3-2-4-3-5'/> 3.2.4.3.5. 품질 프로파일 삭제
1.	품질 프로파일 대시보드에서 “삭제” 버튼을 클릭한다.
![162](../images/pipeline/image162.png)
2.	품질 프로파일이 삭제되었음을 확인한다.
![163](../images/pipeline/image163.png)


#### <div id='3-2-4-4'/> 3.2.4.4. 품질 게이트
##### <div id='3-2-4-4-1'/> 3.2.4.4.1. 품질 게이트 생성
1.	품질 관리 메뉴에서 품질 게이트를 선택하여 품질 게이트 대시보드로 이동한다.
![164](../images/pipeline/image164.jpg)
2.	우측 상단의 “생성” 버튼을 클릭한다.
![165](../images/pipeline/image165.png)
3.	품질 게이트 명을 입력하고, “생성” 버튼을 클릭한다.
![166](../images/pipeline/image166.png)
4.	품질 게이트가 생성된 것을 확인한다.
![167](../images/pipeline/image167.jpg)

##### <div id='3-2-4-4-2'/> 3.2.4.4.2. 품질 게이트 복제
1.	품질 게이트 대시보드에서 “복제” 버튼을 클릭한다.
![168](../images/pipeline/image168.png)
2.	복제할 품질 게이트의 이름을 입력하고, “복제” 버튼을 클릭한다.
![169](../images/pipeline/image169.png)
3.	복제된 품질 게이트를 확인한다.
![170](../images/pipeline/image170.png)

##### <div id='3-2-4-4-3'/> 3.2.4.4.3. 품질 게이트 수정
1.	품질 게이트 대시보드에서 “수정” 버튼을 클릭한다.
![171](../images/pipeline/image171.png)
2.	수정할 품질 게이트 팝업창이 뜨면 품질 게이트 명을 수정하고 “수정” 버튼을 클릭한다.
![172](../images/pipeline/image172.png)
3.	품질 게이트 명이 수정되었음을 확인한다.
![173](../images/pipeline/image173.png)

##### <div id='3-2-4-4-4'/> 3.2.4.4.4. 품질 게이트 조건추가
1.	품질 게이트 대시보드에서 Job 테스트 시 통과 기준이 되는 조건을 설정할 수 있는 조건 추가 부분을 확인한다. 사용자가 직접 조건을 추가하고 기준 설정이 가능하다.
![174](../images/pipeline/image174.png)
2.	조건에 따라 어느 기준 이상/이하가 될 시에 테스트를 통과시키도록 한다.
![175](../images/pipeline/image175.png)
3.	현재 ‘Default-QualityGate’ 가 기본 품질 게이트로 설정되어 있는데 이것을 참고로 한다.
![176](../images/pipeline/image176.jpg)

##### <div id='3-2-4-4-5'/> 3.2.4.4.5. 품질 게이트 프로젝트 연결
1. 품질 게이트 대시보드에서 연결된 프로젝트 항목을 확인한다. (첫 번째 사진은 테스트 Job 구성 조회 시 품질 게이트를 test-QualityGate 로 설정한 것이다. 그러므로 두번째 사진에서 연결된 프로젝트에 test2 파이프라인의 테스트 Job 이 보인다.)<br>
![159](../images/pipeline/image159.jpg)
2. 품질 게이트도 품질 프로파일과 마찬가지로 품질 게이트 1개당 여러 프로젝트 연결이 가능하다.
![177](../images/pipeline/image177.png)

##### <div id='3-2-4-4-6'/> 3.2.4.4.6. 품질 게이트 삭제
1.	품질 게이트 대시보드에서 “삭제” 버튼을 클릭한다.
![178](../images/pipeline/image178.png)
2.	품질 게이트가 삭제되었음을 확인한다.
![179](../images/pipeline/image179.png)

[002]:/use-guide/images/pipeline/image002.png
[003]:/use-guide/images/pipeline/image003.jpg
[004]:/use-guide/images/pipeline/image004.jpg
[005]:/use-guide/images/pipeline/image005.png
[006]:/use-guide/images/pipeline/image006.jpg
[007]:/use-guide/images/pipeline/image007.jpg
[008]:/use-guide/images/pipeline/image008.png
[009]:/use-guide/images/pipeline/image009.png
[010]:/use-guide/images/pipeline/image010.jpg
[011]:/use-guide/images/pipeline/image011.png
[012]:/use-guide/images/pipeline/image012.jpg
[013]:/use-guide/images/pipeline/image013.png
[014]:/use-guide/images/pipeline/image014.png
[015]:/use-guide/images/pipeline/image015.png
[016]:/use-guide/images/pipeline/image016.jpg
[017]:/use-guide/images/pipeline/image017.jpg
[018]:/use-guide/images/pipeline/image018.png
[019]:/use-guide/images/pipeline/image019.jpg
[020]:/use-guide/images/pipeline/image020.png
[021]:/use-guide/images/pipeline/image021.jpg
[022]:/use-guide/images/pipeline/image022.png
[023]:/use-guide/images/pipeline/image023.png
[024]:/use-guide/images/pipeline/image024.png
[025]:/use-guide/images/pipeline/image025.png
[026]:/use-guide/images/pipeline/image026.png
[027]:/use-guide/images/pipeline/image027.png
[028]:/use-guide/images/pipeline/image028.png
[029]:/use-guide/images/pipeline/image029.png
[030]:/use-guide/images/pipeline/image030.png
[031]:/use-guide/images/pipeline/image031.png
[032]:/use-guide/images/pipeline/image032.jpg
[033]:/use-guide/images/pipeline/image033.png
[034]:/use-guide/images/pipeline/image034.png
[035]:/use-guide/images/pipeline/image035.png
[036]:/use-guide/images/pipeline/image036.jpg
[037]:/use-guide/images/pipeline/image037.png
[038]:/use-guide/images/pipeline/image038.png
[039]:/use-guide/images/pipeline/image039.jpg
[040]:/use-guide/images/pipeline/image040.jpg
[041]:/use-guide/images/pipeline/image041.png
[042]:/use-guide/images/pipeline/image042.jpg
[043]:/use-guide/images/pipeline/image043.png
[044]:/use-guide/images/pipeline/image044.png
[045]:/use-guide/images/pipeline/image045.png
[046]:/use-guide/images/pipeline/image046.png
[047]:/use-guide/images/pipeline/image047.png
[048]:/use-guide/images/pipeline/image048.jpg
[049]:/use-guide/images/pipeline/image049.png
[050]:/use-guide/images/pipeline/image050.jpg
[051]:/use-guide/images/pipeline/image051.png
[052]:/use-guide/images/pipeline/image052.png
[053]:/use-guide/images/pipeline/image053.png
[053-2]:/use-guide/images/pipeline/image053(2).png
[054]:/use-guide/images/pipeline/image054.png
[055]:/use-guide/images/pipeline/image055.jpg
[056]:/use-guide/images/pipeline/image056.png
[057]:/use-guide/images/pipeline/image057.jpg
[058]:/use-guide/images/pipeline/image058.jpg
[059]:/use-guide/images/pipeline/image059.png
[060]:/use-guide/images/pipeline/image060.png
[061]:/use-guide/images/pipeline/image061.jpg
[062]:/use-guide/images/pipeline/image062.png
[063]:/use-guide/images/pipeline/image063.jpg
[064]:/use-guide/images/pipeline/image064.png
[065]:/use-guide/images/pipeline/image065.jpg
[066]:/use-guide/images/pipeline/image066.jpg
[067]:/use-guide/images/pipeline/image067.png
[068]:/use-guide/images/pipeline/image068.jpg
[069]:/use-guide/images/pipeline/image069.png
[070]:/use-guide/images/pipeline/image070.jpg
[071]:/use-guide/images/pipeline/image071.jpg
[072]:/use-guide/images/pipeline/image072.png
[073]:/use-guide/images/pipeline/image073.png
[074]:/use-guide/images/pipeline/image074.png
[075]:/use-guide/images/pipeline/image075.png
[076]:/use-guide/images/pipeline/image076.png
[077]:/use-guide/images/pipeline/image077.png
[078]:/use-guide/images/pipeline/image078.png
[079]:/use-guide/images/pipeline/image079.jpg
[080]:/use-guide/images/pipeline/image080.jpg
[081]:/use-guide/images/pipeline/image081.png
[082]:/use-guide/images/pipeline/image082.png
[083]:/use-guide/images/pipeline/image083.jpg
[084]:/use-guide/images/pipeline/image084.png
[084-2]:/use-guide/images/pipeline/image084(2).png
[084-3]:/use-guide/images/pipeline/image084(3).png
[085]:/use-guide/images/pipeline/image085.jpg
[086]:/use-guide/images/pipeline/image086.png
[087]:/use-guide/images/pipeline/image087.png
[087-2]:/use-guide/images/pipeline/image087(2).png
[088]:/use-guide/images/pipeline/image088.png
[089]:/use-guide/images/pipeline/image089.jpg
[090]:/use-guide/images/pipeline/image090.png
[091]:/use-guide/images/pipeline/image091.jpg
[092]:/use-guide/images/pipeline/image092.png
[093]:/use-guide/images/pipeline/image093.jpg
[094]:/use-guide/images/pipeline/image094.png
[095]:/use-guide/images/pipeline/image095.jpg
[096]:/use-guide/images/pipeline/image096.jpg
[097]:/use-guide/images/pipeline/image097.jpg
[098]:/use-guide/images/pipeline/image098.png
[099]:/use-guide/images/pipeline/image099.png
[100]:/use-guide/images/pipeline/image100.jpg
[101]:/use-guide/images/pipeline/image101.png
[102]:/use-guide/images/pipeline/image102.jpg
[103]:/use-guide/images/pipeline/image103.png
[104]:/use-guide/images/pipeline/image104.jpg
[105]:/use-guide/images/pipeline/image105.png
[106]:/use-guide/images/pipeline/image106.png
[107]:/use-guide/images/pipeline/image107.png
[108]:/use-guide/images/pipeline/image108.png
[109]:/use-guide/images/pipeline/image109.jpg
[110]:/use-guide/images/pipeline/image110.jpg
[111]:/use-guide/images/pipeline/image111.png
[112]:/use-guide/images/pipeline/image112.jpg
[113]:/use-guide/images/pipeline/image113.png
[114]:/use-guide/images/pipeline/image114.jpg
[115]:/use-guide/images/pipeline/image115.jpg
[116]:/use-guide/images/pipeline/image116.png
[117]:/use-guide/images/pipeline/image117.png
[118]:/use-guide/images/pipeline/image118.png
[119]:/use-guide/images/pipeline/image119.jpg
[120]:/use-guide/images/pipeline/image120.png
[121]:/use-guide/images/pipeline/image121.png
[122]:/use-guide/images/pipeline/image122.png
[123]:/use-guide/images/pipeline/image123.jpg
[124]:/use-guide/images/pipeline/image124.png
[125]:/use-guide/images/pipeline/image125.jpg
[126]:/use-guide/images/pipeline/image126.png
[127]:/use-guide/images/pipeline/image127.png
[128]:/use-guide/images/pipeline/image128.jpg
[129]:/use-guide/images/pipeline/image129.png
[130]:/use-guide/images/pipeline/image130.jpg
[131]:/use-guide/images/pipeline/image131.png
[132]:/use-guide/images/pipeline/image132.png
[133]:/use-guide/images/pipeline/image133.jpg
[134]:/use-guide/images/pipeline/image134.png
[135]:/use-guide/images/pipeline/image135.png
[136]:/use-guide/images/pipeline/image136.png
[137]:/use-guide/images/pipeline/image137.png
[138]:/use-guide/images/pipeline/image138.png
[139]:/use-guide/images/pipeline/image139.png
[140]:/use-guide/images/pipeline/image140.jpg
[141]:/use-guide/images/pipeline/image141.png
[142]:/use-guide/images/pipeline/image142.jpg
[143]:/use-guide/images/pipeline/image143.jpg
[144]:/use-guide/images/pipeline/image144.jpg
[145]:/use-guide/images/pipeline/image145.png
[146]:/use-guide/images/pipeline/image146.png
[147]:/use-guide/images/pipeline/image147.png
[148]:/use-guide/images/pipeline/image148.png
[149]:/use-guide/images/pipeline/image149.jpg
[150]:/use-guide/images/pipeline/image150.png
[151]:/use-guide/images/pipeline/image151.png
[152]:/use-guide/images/pipeline/image152.png
[153]:/use-guide/images/pipeline/image153.png
[154]:/use-guide/images/pipeline/image154.png
[155]:/use-guide/images/pipeline/image155.png
[156]:/use-guide/images/pipeline/image156.png
[157]:/use-guide/images/pipeline/image157.png
[158]:/use-guide/images/pipeline/image158.png
[159]:/use-guide/images/pipeline/image159.jpg
[160]:/use-guide/images/pipeline/image160.png
[161]:/use-guide/images/pipeline/image161.png
[162]:/use-guide/images/pipeline/image162.png
[163]:/use-guide/images/pipeline/image163.png
[164]:/use-guide/images/pipeline/image164.jpg
[165]:/use-guide/images/pipeline/image165.png
[166]:/use-guide/images/pipeline/image166.png
[167]:/use-guide/images/pipeline/image167.jpg
[168]:/use-guide/images/pipeline/image168.png
[169]:/use-guide/images/pipeline/image169.png
[170]:/use-guide/images/pipeline/image170.png
[171]:/use-guide/images/pipeline/image171.png
[172]:/use-guide/images/pipeline/image172.png
[173]:/use-guide/images/pipeline/image173.png
[174]:/use-guide/images/pipeline/image174.png
[175]:/use-guide/images/pipeline/image175.png
[176]:/use-guide/images/pipeline/image176.jpg
[177]:/use-guide/images/pipeline/image177.png
[178]:/use-guide/images/pipeline/image178.png
[179]:/use-guide/images/pipeline/image179.png