# 삼성 데스크탑5 DM500T9Z-AD5A 해킨토시
 
 ## 시스템 상세정보

 | Item | Details |
 | - | - |
 | Model | Samsung Desktop 5 DM500T9Z-AD5A |
 | CPU | Intel Core i5-9400 |
 | SSD | Samsung MZNLN256HAJQ-000 240 GB *(Stock)* / TeamGroup L3 EVO 480 GB *(External macOS Disk)* |
 | HDD | WDC WD10EZEX-22MFCA0 1 TB |
 | Graphics | Intel UHD Graphics 630 |
 | RAM | Samsung 8GB 2667 MHz DDR4 DIMM |
 | Ethernet | Realtek RTL8168 Gigabit Ethernet Controller |
 | Wi-Fi / Bluetooth | CNVi Intel Wireless-AC 9560 *(Can be replaced with BCM94360NG)* |
 | Card Reader | Realtek 3-in-1 (SD/SDHC/SDXC) Card Reader |
 | Audio | Realtek ALC662 |
 | UEFI BIOS Utility | Aptio Setup Utility P05OEC.040.190723.CL |

 ## 설치 방법

 1. [Configuration.pdf](https://github.com/acidanthera/OpenCorePkg/blob/master/Docs/Configuration.pdf)를 정독합니다.
 2. [Dortania guides](https://dortania.github.io/getting-started/)를 정독합니다.
 3. macOS 인스톨러 USB를 준비합니다.
 4. USB의 EFI 파티션에 OC와 BOOT 폴더를 붙여넣으습니다.
 5. USB로 부팅해서 macOS Installer를 선택한 후 설치합니다.
 6. SSD의 EFI 파티션을 마운트한 후 USB EFI를 SSD의 EFI로 붙여넣습니다.
 7. SMBIOS의 시리얼 숫자들을 새로 생성하십시오.
 - Note: 경우에 따라서 별도 패치가 필요할 수 있습니다.
     - 전력관리를 최대 활성화하고자 하는 경우 -- [MSR 0xE2 (CFG Lock) 해제](#mrs-0xe2-cfg-lock-해제)

 ## MSR 0xE2 (CFG Lock) 해제

 1. [Dortania 가이드](https://dortania.github.io/OpenCore-Post-Install/misc/msr-lock.html)를 참고하십시오.
 - Note: 자신의 컴퓨터의 바이오스 버전을 확실히 알아야 합니다. 버전이 다르다면 컴퓨터에 이상이 생길 수 있습니다. 혹은 바이오스 버전 조회와 상관 없이 OpenCore에서 제공되는 ControlMsrE2.efi를 사용해볼 수도 있습니다. 어떤 결정을 하던지 책임은 본인에게 있습니다.

 ## 설치 완료 후
  
  1. Configuration.pdf와 Dortania 가이드를 다시 한 번 정독하십시오.

 ## Acknowledgment

 Apple for macOS

 The Acidanthera team for OpenCore and many kexts

 The Dortania team for OpenCore guides
