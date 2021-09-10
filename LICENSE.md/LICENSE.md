* tar파일로 압축하기 

tar -cvf "/저장할경로/압축파일명.tar" "압축할 폴더 또는 압축할 파일 경로"

* 해당 디렉토리부터 하위 디렉토리까지 파일 개수 출력 about inode error 

find . -maxdepth 1 -mindepth 1 -type d -exec ls -ld "{}"\; -exec sh -c "find {} -type f | wc -l" \;
