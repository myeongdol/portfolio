쉘스크립트
========
-- utf-8로 변경
 iconv -c -f EUC-KR -t UTF-8 test.csv > text.txt
 
<code>
cat 지번* > buga.txt
echo $?
if [[ $? -ne 0 ]]; 
then
    echo "부가정보 데이터 통합 실패"
    exit 3
else
    iconv -c -f EUC-KR -t UTF-8 buga.txt > buga-utf8.txt
fi
</code>
