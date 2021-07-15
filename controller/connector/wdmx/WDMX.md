# WDMX

[WDMX 사용법](WDMX-MANUAL.md)

## v3.2 2020/08/04 신민정

### 생산 지시서 번호
* 발주 번호 : X
* 번호 미확인시 사유 : 기존 PCB 설계 변경
* 요청 담당자 : 한도희
* 요청일 : 2020/08/04

###  BOM 품목코드
* H0000593

### DRC(Design Rule Check)
* 확인

### 수정 내역
* LD11 : APA1606SECK -> LED GREEN
* PS1-3 : TVB270RSC-L -> PRCP-NSMF020/30X 회로 수정

----------

## v3.1 2019/06/05 신민정

### 생산 지시서 번호
* 발주 번호 : X
* 번호 미확인시 사유 : 기존 PCB 설계 변경
* 요청 담당자 : 한도희
* 요청일 : 2019/06/05

###  BOM 품목코드
* H0000491

### DRC(Design Rule Check)
* 확인

### 수정 내역
* ZD1 삭제
* SN65HVD1785D DMX +,- pin 수정

----------

## v3.0 2019/05/21 신민정

### 생산 지시서 번호
* 발주 번호 : X
* 번호 미확인시 사유 : 기존 PCB 설계 변경
* 요청 담당자 : 한도희
* 요청일 : 2019/05/20

###  BOM 품목코드
* H0000484

### DRC(Design Rule Check)
* 확인

### 수정 내역
* IRQ - CS pin 연결
* TX 단에 MOSI - GND ← 0Ω 추가
* 표준 엔토스 커넥터 기준으로 변경
* R14 6.8k → 7.5k 로 변경
* PCB 외곽 사이즈 변경
* LD8(→LD11수정) 위치 DMX512M-MINI 의 LD3 과 동일하게 변경
* SW1 library 변경

----------

## v0.1 2019/01/16 한도희

### 생산 지시서 번호
* 발주 번호 : X
* 번호 미확인시 사유 : 신규 개발
* 요청 담당자 : 김주현
* 요청일 : 

###  BOM 품목코드
* H0000405

### DRC(Design Rule Check)
* 확인

### 수정 내역
* CRMX TIMO 사용 무선 DMX 구현
* 전자파 인증 목표
* (https://github.com/enthusapp/pcb/issues/8)
