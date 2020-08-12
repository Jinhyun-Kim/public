# dRAST_QCdataAnalyzer

## 1. User Environment Setting
### 1.1. install R
* download [R 3.5.2](https://cran.r-project.org/bin/windows/base/old/3.5.2) or execute R-3.5.2-win.exe
* install with default setting
### 1.2. envrironment variable setting
* 내 PC (우클릭) -> 속성 -> 고급 시스템 설정 -> 고급 탭 -> 환경변수 -> 사용자 변수
- 사용자 변수 탭 -> 새로 만들기 -> 아래 값을 추가
<pre><code>변수 이름 : R_LIBS 
변수 값 : C:/Program Files/R/R-3.5.2/library</code></pre>
- 사용자 변수 에서 변수값 Path를 찾아서 더블클릭 -> 새로만들기 -> 아래 값을 추가
<pre><code>C:\Program Files\R\R-3.5.2\bin\x64</code></pre>

### 1.3. install R libary
* R x64 3.5.2를 관리자 권한으로 실행
* Enter following commends to install library (Select CRAN mirror : Korea or nearby country)
<pre><code>install.packages("pillar")
install.packages("stringr")
install.packages("pracma")
install.packages("tidyr")
install.packages("ggplot2")
install.packages("dplyr")</code></pre>
### 1.4 install Visual C++ 2013 Redistributable x86 
* From folowing [link](https://www.microsoft.com/ko-kr/download/details.aspx?id=40784)
* Or by executing vcredist_x86.exe
### 1.5 reboot PC
### 1.6. 주의
* 도스창이 블럭선택될시 프로그램이 멈춤. 이때에 엔터를 쳐서 블럭선택을 제거해주어야 함.
* dRAST실험 진행시 이미지 파일들이 저장되도록 세팅하여 실험진행
* dRAST이미지가 한국어가 없는 경로에 저장되어있어야함
* dRAST 데이터 폴더 내에 .sample.dat파일이 없으면 작동하지 않음
* Recommened folderName
<pre><code>YYYYMMDD PanelLotNumber KIT/DRY(re) S17/E19</code></pre>

## 2. Usage
* QCdataAnalyzer.exe 실행
* Add Sample 버튼 클릭 -> QC데이터가 포함된 폴더 선택
* Make QC Report 버튼 클릭 -> dRAST 데이터 폴더의 상위폴더에 "QC reports"폴더가 생성됨
* Create Plot버튼 클릭
