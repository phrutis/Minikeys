# Soft brute MiniKeys BTC - For Sale $300

![Serie1 coins](https://user-images.githubusercontent.com/82582647/185912181-afcef4e1-2c4b-4be1-be52-1e5d5a14511c.png)

This is the fastest program to find old Serie1 minikeys in the world :trophy:

| MiniKeys GPU Speed |
|---------------------------|

| GPU card   | --bits    | Speed/s   |
|------------|----------|-----------|
| RTX 4090   | 24       | 14.4 Gkeys |
| RTX 3090   | 24       | 6.2 Gkeys |
| RTX 3070   | 20       | 3.3 Gkeys |


### Usage:

``-b`` - Number of blocks in gpu (automatically assigned by default)</br>
```-t``` - Number of cores in gpu (automatically assigned by default)</br>
```-v``` - Display key generation in window</br>
```--input``` - Text file of BTC addresses Series1.txt with a new line (ex. Serie1.txt)</br>
```--rangeStart``` Start minikey Serie1 (ex. --rangeStart SVY4eSFCF4tMtMohEkpXkN)</br>
```--skip3``` - Skipping keys where there are 3 identical letters in a row.</br>
```--bits``` 8/16/20/24 (ex. --bits 16)</br>
```--random``` - Enable random mode</br>
```--randomseed``` - Eight-digit starting range number (ex. 12345678)</br>
```--randompos``` - Range length for sequential search (ex. 7, 8, 9)</br>
```--permutation``` -  Enable permutation mode</br>
```--permbase``` - Base58 alphabet for permutations</br>
```-d``` - gpu card id (ex. -d 0 or -d 1)</br>

**Linux (ubuntu) Nvidia**
</br><br>
For RTX 3090, 4090 - ```mk_86```</br>
For other cards - ```mk_61```

**Windows Nvidia**
<br><br>
For RTX 3090, 4090 - ```MK_86.exe```</br>
For other cards - ```MK_61.exe```</br>

## :zap: Quick start

## Sequential search mode 1
<br>
Minikey test: SRjnYZNo5d3wcgjw4k8L1b<br>
Minikey address: 1ACKFKm53PgwXy1XkYRnG36MNsR5JJpjsp

```MK_86.exe -v --bits 24 --rangeStart SRjnYZNo5d3wcgj1111111 --input test.txt -d 0```</br>

https://github.com/user-attachments/assets/4c568713-f42d-4a86-9ee7-ffbd492a6e4b

**Linux**</br>
Run: ```chmod +x mk_86```</br>
Run: ```./mk_86 -v --bits 24 --rangeStart SRjnYZNo5d3wcgj1111111 --input test.txt -d 0```

### Use --skip3
```MK_86.exe -v --skip3 --bits 24 --rangeStart SRjnYZNo5d3cccj1111111 --input test.txt -d 0```<br>

https://github.com/user-attachments/assets/3e893e9f-1001-4628-8a0b-e4f99a6d23ec

kipping keys where there are 3 identical letters in a row.</br>
```./mk_86 -v --skip3 --bits 24 --rangeStart SRjnYZNo5d3cccj1111111 --input test.txt -d 0```<br>
Search speed RTX 4090 increases 240 Gkeys/s (TURBO)</br>
When 3 identical letters are passed in a range, the skip will be disabled.</br>
If you get 3 of a kind again it will turn on

## Random search mode 2

Minikey test: Svdsde1Me6KbaQa6PtM563 (seed 20240003 windows)</br>
Minikey address: 1FVBSz8GFVdD5bwcrjXxr35CBHL2e5tw9o</br>
```MK_86.exe -v --bits 24 --random --randomseed 20240001 --randompos 7 --input test.txt -d 0```</br>

https://github.com/user-attachments/assets/8b1caaf9-9746-4de8-8064-3fb4a6adffab

**Linux**</br>
```./mk_86 -v --bits 24 --random --randomseed 20240001 --randompos 7 --input test.txt -d 0```

--randomseed 20240001</br>
A starting random key is generated that corresponds to the seed range 20220001</br>
(You can use any 8-digit seed 00000001 - 99999999)</br>
--randompos 7 (Length 7 characters)</br>
Start range: S + 13 characters from seed + 1111111</br>
End range: S + 13 characters from seed + zzzzzzz</br>
After length 7 has been completed a new starting key will be generated from the next seed 20240002 ..... next seed 20245894</br>
You can specify the length 8, 9, 10...

## Permutation mode 3

Minikey test: S1TEST1phrutisaBcDE736</br>
Minikey address: 1KamPdVF51cnBv8jCq3d5yStQMtsH9EPPY<br>
Prefix: S1TEST1 (Length 7 characters)<br>
Alphabet: phrutisaBcDE736 -> Bha6riu7tscpDE3 (Length 15 characters)<br>
```MK_86.exe -v --bits 24 --permutation --rangeStart S1TEST1 --permbase Bha6riu7tscpDE3 --input test.txt -d 0```

https://github.com/user-attachments/assets/7e64169f-294f-492e-a4ad-de9a8da15144

**Linux**</br>
```./mk_86 -v --bits 24 --permutation --rangeStart S1TEST1 --permbase Bha6riu7tscpDE3 --input test.txt -d 0```
<br>

In this mode, characters in a given alphabet are swapped.</br>
Use "--permutation" BEFORE "--rangeStart"!</br>
Don't use the same characters in the alphabet.</br>
Analyze open coins, select an alphabet from frequently dropped symbols
<hr>

## :coin: Minikeys Serie1

Number of minikeys Serie1 = 4907</br> 
Denomination of coins 1, 5, 10, 25, 500, 1000 BTC</br>
More information on the [Casascius tracker](https://casasciustracker.com)

In 2010-2012 bitcoin was worth cents.</br>
The coins did not provide crypto value.</br>
Beautiful physical coins were used as souvenirs, given as gifts, lost, thrown away.</br>
Many people simply did not know that there was a mini-key under the holagram.</br>
Suppose the person knew about the key</br>
2011 year 1 btc = $0.08</br>
Where can I spend $0.08?</br>

2012 year 1 btc = $1</br>
In 2013 you can buy pizza :)</br>
Then the rate began to rise.
<hr>

## :memo: Frequently Asked Questions<hr>

**Where to download 4907 addresses of coins series1 ?**
</br>
[**Download Serie1.txt**](https://github.com/cuda8/MiniKeys/blob/main/Serie1.txt)<br><br>
[Download 3 addresses for a quick test](https://github.com/cuda8/MiniKeys/blob/main/test.txt)
<hr>

**I launched the program hung (froze) what should**
<br><br>
The program needs time to create the table.<br>
Wait for start:<br>
For 24 bits = 10 minutes
<hr>

**I have a RTX 3060 TI card, and I have a low speed, how can speed**</br>

In the new drivers for 30xx Ti, 20xx Ti, a limiter is installed that slows down the speed by half.</br>
You need to download the old driver from six months ago. 496.13</br>
Delete the new driver, install the old driver, the speed will increase x2</br>
After searching, you can install new drivers.
<hr>

**I have many GPUs. How to start**
<br><br>
Run each GPU separately. Add your card id -d ?<br>
```MK_86.exe -v ... -d 0```<br>
```MK_86.exe -v ... -d 1```<br>
```MK_86.exe -v ... -d 2```<br>
```MK_86.exe -v ... -d 3```<br>
```MK_86.exe -v ... -d 4```<br>
```MK_86.exe -v ... -d 6```
<hr>

**Why can't you find my test key?**
<br><br>
The program checks only [valid keys](https://en.bitcoin.it/wiki/Mini_private_key_format) and uncompressed Legacy addresses 1...<br>
You can [generate a valid key](https://brainwalletx.github.io/) manually.

Key 22 characters + ? to SHA256 = Private key starting with 00...<br>
Then the key is without ? in SHA256 will be valid.<br>
Example<br>
SN87BVteCnEm4cWPmLNATM? -> SHA256 = Privkey: 0030e848687df9b66d43aa5e9d895dea1974c439285eda7860c0f7a0757b03da<br>
SN87BVteCnEm4cWPmLNATM = VALID KEY<br>

SN87BVteCnEm4cWPmLNATT? -> SHA256 = Privkey: b1f1e41071b431e9988ea43e900c4a4fdc7d2b9f8ee957a0e556cc38e1d699b2<br>
SN87BVteCnEm4cWPmLNATT = NO VALID KEY
<hr>

**How to buy the program?**
<br><br>
https://t.me/cuda8<br>
After payment you will receive 4 ready-made program files.<br>
2 program files for Ubuntu (mk_86 and mk_61)<br>
2 program files for Windows (MK _86.exe and MK _61.exe)<br>
Brief instructions, BTC address database Serie1.txt
<hr>

**Where can I get real mini keys casascius Serie1?**
<br><br>
![photo_2024-03-22_12-33-17](https://github.com/user-attachments/assets/170a44cb-2247-469c-86ea-e4309e886a6c)
<br>
![photo_2024-03-22_12-33-14](https://github.com/user-attachments/assets/a9ab1384-a741-4eb5-bf3c-9ad961a22fef)
<br>
They are hard to find, I only know 5<br>
SMgKFRQ6n64w8gV2dUwYte - emply<br>
S4b3N3oGqDqR5jNuxEvDwf - 2013 ???<br>
SkGh5HHYsweYWVidWasX7r - original<br>
SG64GZqySYwBm9KxE3wJ29 - ok<br>
SkK5VPtmTm3mQKYaJQFRZP - ok
<hr>


**The program without sources, I'm worried that my discovery will fly away to another person.**
<br><br>
Windows<br>
1. Press the key combination "Win+R" and enter the command "firewall.cpl".<br>
2. Go to the "Advanced settings" section and select "Outgoing connection rules".<br>
3. Click on the "Create rule" button, select the "For program" option and specify its path.<br>
4. Check the box next to "Block connection".<br>
5. Click "Next", specify "Name" and click "Finish". Now the selected program will not be able to connect to the network.

Linux<br>
sudo iptables -A OUTPUT -p tcp -m owner --uid-owner NAME_USER_NO_INET -j DROP<br>
sudo -u NAME_USER_NO_INET ./Minikeys ...<br>

Look for instructions on the Internet.<br>
if you don't know how to do it, for peace of mind, turn off the Internet
<hr>

**I have a mistake RTX 4090 Ubuntu**
<br><br>
```
./mk_86: error while loading shared libraries: libcudart.so.11.0:
cannot open shared object file: No such file or directory
```
For Ubuntu<br>
```sudo apt-get install libcudart.so.11.0```<br>
or install CUDA 11.7 [HIRE](https://developer.nvidia.com/cuda-11-7-0-download-archive?target_os=Linux&target_arch=x86_64&Distribution=Ubuntu&target_version=20.04&target_type=deb_local)

For vast.ai RTX 4090 USE:<br>
Image: nvidia/cuda:11.0.3-devel-ubuntu20.04

Image CUDA version: 11<br>
Incompatible images hidden<br>
Launch Type: jupyter

Or install CUDA 11.0.3 (11.7 max) on your Ubuntu PC
In Windows version it works in any CUDA 11.0 -> 12.3
<hr>
<br>
