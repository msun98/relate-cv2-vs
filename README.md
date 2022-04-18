# relate-cv2-VisualStudio
**1. OpenCV 설치하기**

내가 사용하고 싶은 OpenCV 버전을 선택합니다. (비교적 최신 버전으로) 

OpenCV 페이지 바로가기 : https://opencv.org/releases/


**2. Visual Studio 프로젝트 생성하기**

1) Visual Studio의 프로젝트 속성에 Debug x64세팅

**3. Visual Studio 프로젝트 속성에서 경로 설정하기**
 ```
1) 디렉터리 경로 추가

C/C++ > 일반 > 추가 포함 디렉터리에 경로 추가 

경로 : C:\opencv\build\include (Opencv의 include 폴더 있는 경로)

 

2) 추가 라이브러리 경로 추가

링커 > 일반 > 추가 라이브러리 디렉터리에 경로 추가

경로 : C:\opencv\build\x64\vc14\lib

 

3) 추가종속성 추가 

링커 > 입력 > 추가 종속성에 Release의 경우 opencv_world341.lib를 추가하고, Debug의 경우 opencv_world341d.lib를 추가합니다.

 

4) 프로젝트 폴더에 .dll 파일 복사

프로젝트가 있는 폴더에 opencv_world341.dll, opencv_world341d.dll을 복사해줍니다. 

OpenCV 가 연동이 완료되었습니다. 
```

