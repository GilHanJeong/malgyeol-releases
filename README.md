# 말결 설치판 내려받기

말결은 카카오톡 대화로 내 낱말·말끝·언어 표지를 살펴보는 교육용 성찰 도구예요. 숫자는 점수가 아니라 내 말을 돌아보는 자료예요.

- 소개와 웹·라이트판: https://hyang.pdlab.kr/tools/malgyeol/
- 이 저장소에는 **Windows 설치 파일**만 올려요. 말결 프로그램 코드는 여기 없어요.

## 설치

1. [Releases](https://github.com/GilHanJeong/malgyeol-releases/releases/latest)에서 `Malgyeol-<판>-windows-x64-setup.exe`를 받아요.
2. 실행하면 내 계정에 설치돼요(관리자 권한 필요 없음). Windows 10·11 64비트에서 써요.
3. 학생 화면에 필요한 Microsoft WebView2가 없으면 설치할 때 함께 깔아요(인터넷 필요).

Windows가 "알 수 없는 게시자"라고 경고할 수 있어요. 아직 코드 서명을 하지 않았기 때문이에요. 받은 파일이 맞는지는 같은 릴리스의 `SHA256SUMS.txt`로 확인할 수 있어요.

```powershell
Get-FileHash .\Malgyeol-0.19.1-windows-x64-setup.exe -Algorithm SHA256
```

## 새 판

설치한 말결은 켤 때 새 판이 있는지 확인하고 알려 줘요. '업데이트'를 누르면 받아서 설치하고 다시 열려요. 이때 보내는 것은 판 정보 요청뿐이에요. 대화·파일 이름·분석 결과는 보내지 않아요.

## 함께 쓰는 프로그램

말결은 형태소 분석기 [Kiwi](https://github.com/bab2min/Kiwi)(LGPL-2.1) 등 공개 소프트웨어를 써요. 각 릴리스의 `Malgyeol-<판>-third-party-source.zip`에 그 판에서 쓴 외부 라이브러리 소스와 라이선스가 있어요. 설치 폴더의 `_internal\licenses`에도 고지문이 있어요.
