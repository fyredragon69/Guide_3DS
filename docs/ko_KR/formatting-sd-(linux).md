# SD 포맷하기 (Linux)

## 중요

이곳은 3DS와 쓰기 위한 SD 카드를 포맷하는 부가 섹션입니다.

만약 3DS가 이미 SD 카드를 인식한다면, 이 가이드는 따를 필요가 없습니다.

이 페이지는 Linux 사용자를 위한 페이지입니다. 만약 Linux에서 하는 것이 아니라면, [SD 포맷하기 (Windows)](formatting-sd-\(windows\))나 [SD 포맷하기 (Mac)](formatting-sd-\(mac\)) 페이지들을 찾아봐 주세요.

## 진행 방법

1. SD 카드가 삽입되어 있지 **않아야** 합니다
2. Linux 터미널을 시작해 주세요
3. `watch "lsblk"`를 입력해 주세요
4. SD 카드를 컴퓨터에 삽입해 주세요
5. 출력값을 확인해 주세요. 아래와 같이 보일 것입니다:
    ```
    NAME        MAJ:MIN RM   SIZE RO TYPE MOUNTPOINT
    mmcblk0     179:0    0   3,8G  0 disk
    └─mmcblk0p1 179:1    0   3,7G  0 part /run/media/user/FFFF-FFFF
    ```
6. 장치 이름을 기록해 두세요. 위 예시에서는 `mmcblk0p1`입니다.
    - `RO` 값이 1이라면, 잠금 슬라이드가 내려가 있지는 않은지 확인해 주세요
7. CTRL + C 를 입력해 메뉴를 닫으세요
8. SD 카드 포멧을 위해 다음을 실행하세요:
    - 2GB 이하: `sudo mkfs.fat /dev/(device name from above) -s 64 -F 16`
        - 이것은 32KB 클러스터 크기를 가진 FAT16 파티션을 SD카드에 생성합니다
    - 4GB - 128GB: `sudo mkfs.fat /dev/(device name from above) -s 64 -F 32`
        - 이것은 32KB 클러스터 크기를 가진 FAT32 파티션을 SD카드에 생성합니다
    - 128GB 이상: `sudo mkfs.fat /dev/(device name from above) -s 128 -F 32`
        - 이것은 64KB 클러스터 크기를 가진 FAT32 파티션을 SD카드에 생성합니다

## 문제 해결

- SD 카드를 콘솔에서 여전히 감지되지 않거나 포맷 이후로도 엉뚱한 용량을 표시할 경우
    - SD 카드가 나뉘었거나 미할당 공간이 있을 가능성이 있습니다. [해당 링크](https://wiki.hacks.guide/wiki/SD_Clean/Linux)의 가이드를 따라 SD 카드를 다시 포맷해 주세요
