## DBMS in Linux
무언가의 데이터를 저장하기 위해선 파일 I/O의 과정을 거쳐 파일에 저장할 수 있어야합니다. 데이터를 저장하는 구조에는 수백가지가 있지만
그 중에서 B+ tree를 활용하고자 합니다. 기존의 B+ tree는 메모리 상에서만 동작했습니다. 이를 가공해 disk based b+ tree를 제작했습니다.
key를 트리에 삽입하거나 삭제할 수 있습니다. 해당 정보는 페이지의 leaf에 저장이 되고, 이는 파일에 반영됩니다. 지속적인 파일 I/O는 
성능저하를 일으킬 수 있으니 버퍼를 도입해 빈번한 파일 I/O의 호출을 줄이고, 성능을 높였습니다. 자세한 내용은 위키를 참고하십시오. 
Linux 기반이기 때문에 윈도우 환경에서는 동작하지 않습니다!
