# 삽입 기법 vs 수정 기법

##
수정 기법

# 1. File 확인
```
# file [파일명]
```
# 2. 파일 시그니처 확인
```
# hexeditor [파일명]
```

# 3. 숨겨진 파일 추출 시그니쳐 확인
```
# 해당 파일 바이너리 내부에 다른 파일 있는지 확인
binwalk [파일명]

# 이미지/오디오 내부에 숨겨진 파일 추출 
steghide --extract -sf [파일명]
stegcracker [파일명] /usr/share/wordlists/rockyou.txt     # 비밀번호 필요 시 brute force 가능
```

# 3. 이미지 크기 변경
파일 헤더 구조 참고해서 raw값 (가로) (세로) 변경하기

