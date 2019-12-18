# dRAST_QCdataAnalyzer

## 1. User Environment Setting
### 1.1. install R
* download R : [R 3.5.2](https://cran.r-project.org/bin/windows/base/old/3.5.2)
* install with default setting
### 1.2. envrironment variable setting
* 내 PC (우클릭) -> 속성 -> 고급 시스템 설정 -> 고급 탭 -> 환경변수 -> 사용자 변수
* 변수값 Path를 찾아서 더블클릭 -> 아래 값을 추가
<pre><code>C:\Program Files\R\R-3.5.2\bin\x64</code></pre>
### 1.3. install R libary
* open R x64 3.5.2
* enter following commends to install library
<pre><code>install.packages("stringr")
install.packages("pracma")
install.packages("tidyr")
install.packages("ggplot2")
install.packages("dplyr")</code></pre>

### 1.4. 주의
* dRAST실험 진행시 이미지 파일들이 저장되도록 세팅하여 실험진행
* dRAST이미지가 한국가 없는 경로에 저장되어있어야함
* Recommened folderName
<pre><code>YYYYMMDD PanelLotNumber KIT/DRY(re) S17/E19</code></pre>

## 2. Usage
* QCdataAnalyzer.exe 실행
* Add Sample 버튼 클릭 -> QC데이터가 포함된 폴더 선택
* Make QC Report 버튼 클릭 -> 결과를 출력할 폴더 선택
* Create Plot버튼 클릭
