<template>
  <div class="d-flex flex-column pa-4">
    <!-- title -->
    <h3>Where to Begin? Internet Addresses</h3>
    <p class="sentence__english">
      Because the Internet is a global network of computers each computer
      connected to the Internet must have a unique address.
    </p>
    <p class="sentence__korea">
      인터넷은 컴퓨터의 글로벌 네트워크이기 때문에
      <span class="wrong__word">인터넷에</span> 연결된 각 컴퓨터에는 고유한
      주소가 있어야 합니다.
    </p>
    <p class="sentence__english">
      Internet addresses are in the form nnn.nnn.nnn.nnn where nnn must be a
      number from 0 - 255.
    </p>
    <p class="sentence__korea">
      인터넷 주소는 nnn.nnn.nnn.nnn 형식입니다. 여기서 nnn은 0 - 255 사이의
      숫자여야 합니다.
    </p>
    <p class="sentence__english">
      This address is known as an IP address. (IP stands for Internet Protocol;
      more on this later.)
    </p>
    <p class="sentence__korea">
      이 주소를 IP 주소라고 합니다. IP는 인터넷 프로토콜의 약자이며 나중에 더
      설명해줄께.
    </p>
    <p class="sentence__english">
      The picture below illustrates two computers connected to the Internet;
    </p>
    <p class="sentence__korea">
      아래 그림은 인터넷에 연결된 두 대의 컴퓨터를 보여줍니다.
    </p>
    <p class="sentence__english">
      your computer with IP address 1.2.3.4 and another computer with IP address
      5.6.7.8.
    </p>
    <p class="sentence__korea">
      IP 주소가 1.2.3.4인 컴퓨터와 IP 주소가 5.6.7.8인 다른 컴퓨터.
    </p>
    <p class="sentence__english">
      The Internet is represented as an abstract object in-between.
    </p>
    <p class="sentence__korea">
      인터넷은 그 사이에 있는 추상적인 객체로 표현된다.
    </p>
    <p class="sentence__english">
      (As this paper progresses, the Internet portion of Diagram 1 will be
      explained and redrawn several times as the details of the Internet are
      exposed.)
    </p>
    <p class="sentence__korea">
      본 논문이 진행됨에 따라 인터넷의 세부 사항이 노출됨에 따라 다이어그램 1의
      인터넷 부분에 대해 설명하고 여러 번 다시 그릴 것입니다.
    </p>
    <img
      width="400px"
      src="http://web.stanford.edu/class/msande91si/www-spr04/readings/week1/InternetWhitepaper_files/ruswp_diag2.gif"
    />
    <p class="sentence__english">
      If you connect to the Internet through an Internet Service Provider (ISP),
      you are usually assigned a temporary IP address for the duration of your
      dial-in session.
    </p>
    <p class="sentence__korea">
      인터넷 서비스 제공업체(ISP)를 통해 인터넷에 연결하는 경우, 일반적으로 전화
      접속 세션 동안 임시 IP 주소가 할당됩니다.
    </p>
    <p class="sentence__english">
      If you connect to the Internet from a local area network (LAN) your
      computer might have a permanent IP address or it might obtain a temporary
      one from a DHCP (Dynamic Host Configuration Protocol) server.
    </p>
    <p class="sentence__korea">
      LAN(Local Area Network)에서 인터넷에 연결하는 경우 컴퓨터에 영구 IP가 있을
      수 있습니다. 또는 DHCP(Dynamic Host Configuration Protocol) 서버에서 임시
      주소를 얻을 수 있습니다.
    </p>
    <p class="sentence__english">
      In any case, if you are connected to the Internet, your computer has a
      unique IP address.
    </p>
    <p class="sentence__korea">
      어쨌든 인터넷에 연결되어 있으면 컴퓨터에는 고유한 IP 주소가 있습니다.
    </p>

    <h4>Check It Out - The Ping Program</h4>

    <p class="sentence__english">
      If you're using Microsoft Windows or a flavor of Unix and have a
      connection to the Internet,
    </p>
    <p class="sentence__korea">
      만약 너가인터넷이 연결된 Microsoft Windows 또는 Unix를 사용한다면
    </p>
    <p class="sentence__english">
      there is a handy program to see if a computer on the Internet is alive.
    </p>
    <p class="sentence__korea">
      그것은 만약 컴퓨터가 인터넷에서 살아있다면 볼 수 있는 핸디 프로그램 이다.
    </p>
    <p class="sentence__english">
      It's called ping, probably after the sound made by older submarine sonar
      systems.
    </p>
    <p class="sentence__korea">
      그것은 ping이라고 불린다. 아마 소리 후에 만든다 더 오래된
    </p>
    <p class="sentence__english">
      1 If you are using Windows, start a command prompt window.
    </p>
    <p class="sentence__korea">
      만약 너가 윈도우를 사용한다면 윈도우 커맨드 프롬프트를 시작해라.
    </p>
    <p class="sentence__english">
      If you're using a flavor of Unix, get to a command prompt.
    </p>
    <p class="sentence__korea">
      만약 너가 Unix를 사용한다면 커맨드 프롬프트를 시작해라.
    </p>
    <p class="sentence__english">
      Type ping www.yahoo.com. The ping program will send a 'ping' ping 타입
      www.yahoo.com.
    </p>
    <p class="sentence__korea">핑 소리가 나는 프로그램은 핑 단어를 보낸다.</p>
    <p class="sentence__english">
      (actually an ICMP (Internet Control Message Protocol) echo request
      message) to the named computer.
    </p>
    <p class="sentence__korea">
      사실 ICMP(Internet Control Message Protocol)는 이름을 가진 컴퓨터에게
      메세지를 요청한다.
    </p>
    <p class="sentence__english">
      The pinged computer will respond with a reply.
    </p>
    <p class="sentence__korea">핑 소리가나는 컴퓨터는 응답에 반응할 것이다.</p>
    <p class="sentence__english">
      The ping program will count the time
      <span class="doNotKnow__word">expired</span> until the reply comes back
      (if it does).
    </p>
    <p class="sentence__korea">
      핑 프로그램은 응답이 돌아오기까지 만료 시간을 셀 것이다.
    </p>
    <p class="sentence__english">
      Also, if you enter a domain name (i.e. www.yahoo.com) instead of an IP
      address, ping will resolve the domain name and display the computer's IP
      address.
    </p>
    <p class="sentence__korea">
      또한 만약 너가 도메인 이름 대신 IP주소에 들어온다면 핑은 도메인 이름을
      해결하고 컴퓨터의 IP 주소로 나타낼 것이다.
    </p>
    <p class="sentence__english">
      More on domain names and address resolution later.
    </p>
    <p class="sentence__korea">도메인 이름 그리고 주소 해결 후에</p>

    <p class="sentence__english"></p>
    <p class="sentence__korea"></p>
    <p class="sentence__english"></p>
    <p class="sentence__korea"></p>
  </div>
</template>

<script>
export default {
  name: "HowDoesTheInternetWork",

  components: {},
};
</script>

<style scoped lang="scss">
.wrong__word {
  color: red;
}
.doNotKnow__word {
  color: blue;
}
</style>
