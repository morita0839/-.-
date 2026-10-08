<!docytype html>
<html lang="ja">
<머리>
<meta charset=>UTF-8">
<meta 이름="viewport" 콘텐츠="width=장치 너비, initial 스케일=1">
<title>日本語名刺メーカー</title>
<스타일>
body{margin:0;background:#f2f2f2;font-family:Arial,"Noto Sans JP",sans-serif;color:#222;padding:30px}
.wrap{최대 너비:1000 px;margin:자동;디스플레이:그리드;그리드-template-columns:1fr 1.2fr;갭:30 px}
.패널,.card{배경:흰색;경계-radius:16px;박스-shadow:0 10px 30px #0001}
.패널{padding:25 px} h1{margin-탑:0}
라벨 {디스플레이:블록;margin:14 px 0 5 px;font 무게:볼드}
입력, 텍스트 영역{폭:100%;padding:10 px;경계:1px 솔리드 #ccc;경계-radius:7px;박스-sizing:경계-박스;font 크기:15px}
텍스트 영역 {높이:70 px}
.preview{디스플레이:플렉스;align-items:센터;justify-콘텐츠:센터}
.카드{폭:90%;aspect-ratio:1.75/1;padding:38px;박스-sizing:보더-박스;위치:relative;보더-왼쪽:8px 솔리드 #222}
.회사{font 사이즈:14 px;편지 spacing:2 px;색상:#666;margin 하의:30 px}
.name{font 사이즈:32 px;font 무게:bold}.kana{font 사이즈:13 px;색상:#777;margin:5 px 0 25 px}
.위치{margin-바닥:20px}.contact{font-크기:13px;선 높이:1.8}
.mark{위치:절대;오른쪽:25 px;아래:18 px;색상:#aaa;font 크기:11 px}
@media(최대 너비:800 px){.랩 {그리드-template-columns:1fr}카드 {폭:100%}}
</스타일>
</머리>
<바디>
<div class="wrap">
<섹션 클래스="패널">
<h1>🇯🇵 日本語名刺メーカー</h1>
<p>入力した内容が右側の名刺にリアルタイムで反映されます。</p>
<label>会社名, 所属</label><입력 ID="회사" 값="東京国際株式会社">
<label>氏名</label><입력 ID="이름" 값="金 在潤">
<label>フリガナ</label><입력 ID="카나" 값="キム 및 ジェユン">
<label>役職</label><입력 ID="위치" 값="学生 및 国際交流担当">
<label>電話番号</label><입력 ID="phone" 값="03-1234-5678">
<label>メール</label><입력 ID="email" 값="example@example.com ">
<label>住所</label><textarea id="address">東京都新宿区西新宿1-1-1</textarea>
</섹션>
<섹션 클래스="preview">
<div class="card">
<div class="company" ID="oCompany"></div>
<div class="name" id="oName"></div>
<div class="kana" id="oKana"></div>
<div class="position" id="oPosition"></div>
<div class="contact">TEL <span id="oPhone"></span><br>메일 <span id="oEmail"></span><br><span id="oAddress"></span><div>
<div class="mark">名刺 / MEISH</div>
</div>
</섹션>
</div>
<스크립트>
constids=["회사"], "이름", "카나", "위치", "전화", "이메일", "주소"];
기능. 갱신하다(){
ids.forEach(x=>document.getElementById("o"+x[0]).TopCase()+x.slice(1)).textContent=document.getElementById(x.value);
}
ids.forEach(x=>document.getElementById(x).addEventListener("입력", 업데이트); 업데이트 ();
</script>
</body>
</html>
