# ntrboot 플래싱 (DSi)

## 중요

진행하기 앞서서, [ntrboot](ntrboot) 에 대한 모든 정보를 숙지해주세요.

이 수단은 닌텐도 DSi와 이와 호환되는 플래시카트가 필요합니다. 이 방법은 플래시카드를 DSi에 삽입해 ntrboot flasher `.nds` 를 실행하는 방법입니다. 이 말은, 플래시 카트리지가 닌텐도 DSi 버전에서 `.nds` 파일 구동을 지원해야 한다는 의미입니다. 자세한 내용은 [ntrboot] (ntrboot) 의 플래시카트 표를 참조해 주시기 바랍니다.

::: danger

아주 드문 경우지만 설치를 시도한 플래시카드가 짝퉁일 경우 설치 과정 중 카트리지가 **벽돌**이 되고 이후 카트리지를 사용할 수 없게되는 경우가 있습니다. 그러하기 때문에 매우 적은 확율이지만 정품 플래시카트만 지원 됩니다. 복재품 카드를 주문할 가능성을 줄이기 위하여, [NDS Card](https://www.nds-card.com/)같이 신뢰할 수 있는 사이트를 이용하여 구매 하시길 바랍니다.

:::

## 준비물

- ntrboot를 설치할 수 있는 플래시카트
- 두 개의 콘솔들
    - **소스 DSi**: 플래시카트와 호환되는 닌텐도 DSi.
    - **타겟 3DS** CFW를 설치할 3DS
- 최신 버전의 [ds_ntrboot_flasher](https://github.com/ntrteam/ds_ntrboot_flasher/releases/latest) (`ds_ntrboot_flasher_dsi.nds`)

## 진행 방법

### 섹션 I - 준비 작업

1. **소스 DSi**를 종료해 주세요
2. DS 플래시카트의 SD 카드를 컴퓨터에 삽입해 주세요
3. 플래시카트의 SD 카드에 `ds_ntrboot_flasher.nds`를 복사해 주세요
4. 플래시카트의 SD 카드를 다시 플래시카트에 삽입해 주세요
5. **소스 DSi**에 ntrboot와 호환되는 DS / DSi 플래시카트를 삽입해 주세요

### 섹션 II - ntrboot 플래싱

1. **소스 DSi**에서 플래시카트를 이용해 `ds_ntrboot_flasher_dsi.nds`를 실행해 주세요
2. (A)를 눌러 진행해 주세요
3. (위) 버튼과 (아래) 버튼을 눌러 삽입되 있는 플래시카트를 선택해 주세요
4. (A)를 눌러 진행해 주세요
5. (A)를 눌러 "inject ntrboothax"을 선택해 주세요
6. (A)를 눌러 "RETAIL"을 선택해 주세요
7. (A)를 눌러 진행해 주세요
8. "EXIT"를 선택해 주세요

___

::: tip

[boot9strap 설치 (ntrboot)](installing-boot9strap-\(ntrboot\))로 계속합니다

:::
