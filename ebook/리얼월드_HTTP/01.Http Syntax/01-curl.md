
//curl

curl --http1.0 [-v] [-GET | -G] [-H "key: value"] url  


curl -v --http1.0 -A "Mozilla/5.0 (compatible; MSIE 10.0; Windows NT 6.1; Trident/6.0)" url

curl --http1.0 [-X POST] url


// Status Code

100 - 처리가 계속 진행중임을 나타낸다
200 - 성공했을 떄 의 응답
300 - 서버에서 클라이언트로 명령. 
400 - 클라이언트가 보낸 요청에 오류가 있다.
500 - 서버 내부에서 오류가 발생했다.

URL

URL 관용 표현, URI 공식 표현
자바에서는 URL클래스와 URI 클래스가 존재
https://www.oreilly.co.jp/index.shtml

schema : https
host: www.oreilly.co.jp
endpoint(경로) : index.shtml

스키마
http
https 통신 경로가 암호화 되는
mailto 메일러를 시작하는
file
ftp

ip 마다
65535 개의 포트가 존재

호스트명은 지정된 서버

포트 생량
HTTP 80
HTTPS 443

URL 상에서는 2000자까지 제약됨

https://www.punycoder.com/

퓨니코드 한글도메인.kr -> xn--bj0bj3i97fq8o5lq.kr

curl -d "{\"hello\": \"world\"}" -H "Content-Type: application/json" url


//파일에서 읽은 json파일 송수신
curl -d @test.json -H "Content-Type: application/json" url


<form method = "POST">
    <input name = "title">
    <input name = "author">
</form>

curl --http1.0 -G -d title="The Art Of Community" -d author="Jono Bacon" url

url 치환 =와 &은 각각 %3D와 %26









































