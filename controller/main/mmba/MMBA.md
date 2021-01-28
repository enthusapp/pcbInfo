# MMBA

## v3.0 2021/01/26 신민정

### 생산 지시서 번호
* 발주 번호 : X
* 번호 미확인시 사유 : 생산 예정
* 요청 담당자 : 김주현
* 요청일 : 2021/01/14

### BOM 품목코드
* H0000627
* H0000628

### DRC(Design Rule Check)
* 확인

### 수정 내역
* 24 V 전원 입력단 인덕터 제거
* FAN 고정 홀 추가
* FAN 커넥터 B2B-XH-A로 변경(MFPlayer와 동일)
* FPGA - CPU EMI cap 47pF/50V(1608) 위치 변경
* Sub CPU 회로 제거
* FPGA(EP4CE6E22C8N) 적용
* 전원 입력 2576 이중 회로 적용
* 2576 쪽 cap 47pF/50V(1608)추가
* FPGA → CPU 사이에 EMI cap 47pF/50V(1608)추가
* RasberryPI VCC 입력에 MFPlayer10 과 같이 전원 cap 추가
* 오실레이터 51 MHz, 16 MHz 에 EMI cap 47pF/50V(1608)추가

----------

## v2.0 2020/05/28 김주현

### BOM 품목코드
* H0000579
* H0000582
