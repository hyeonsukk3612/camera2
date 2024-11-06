CX = g++                   # 컴파일러를 g++로 설정
CXFLAGS = -g -Wall         # 컴파일러 플래그
CVFLAGS = `pkg-config opencv4 --cflags --libs`  # OpenCV 라이브러리 플래그

SRCS = main.cpp            # 소스 파일 목록
TARGET = camera            # 생성될 실행 파일 이름

$(TARGET):$(SRCS)          # 타겟 규칙
        $(CX) $(CXFLAGS) -o $(TARGET) $(SRCS) $(CVFLAGS)  # 컴파일 명령

.PHONY: clean              # clean을 가짜 타겟으로 선언

clean:                     # clean 타겟
        rm -f $(OBJS) $(TARGET)  # 오브젝트 파일과 실행 파일 삭제
