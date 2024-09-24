# -3

<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>이벤트/세미나 등록 페이지</title>
    <link rel="stylesheet" href="styles.css">
    <style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    background-color: #f4f4f4;
    color: #333;
    line-height: 1.6;
}

header {
    background: #007bff;
    color: white;
    padding: 20px 0;
    text-align: center;
}

header h1 {
    font-size: 2.5rem;
}

header p {
    font-size: 1.2rem;
    margin-top: 10px;
}

#event-details, #speakers, #register {
    max-width: 800px;
    margin: 20px auto;
    padding: 20px;
    background: white;
    border-radius: 8px;
    box-shadow: 0 2px 10px rgba(0,0,0,0.1);
}

h2 {
    margin-bottom: 15px;
    color: #007bff;
}

.speaker {
    margin-bottom: 10px;
}

form {
    display: flex;
    flex-direction: column;
}

label {
    margin-bottom: 5px;
}

input {
    margin-bottom: 15px;
    padding: 10px;
    border: 1px solid #ccc;
    border-radius: 5px;
}

button.cta {
    padding: 10px;
    background-color: #28a745;
    color: white;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}

button.cta:hover {
    background-color: #218838;
}

footer {
    text-align: center;
    padding: 20px;
    background: #333;
    color: white;
    margin-top: 20px;
}


</style>
</head>
<body>
    <header>
        <h1> 총회 세미나  </h1>
        <p>계약 체결 건에 대한 세미나 개최회</p>
    </header>
    
    <section id="event-details">
        <h2>이벤트 정보</h2>
        <p>일정: 2024년 09월 23일</p>
        <p>시간: 오후 1시 - 5시</p>
        <p>장소: 서울 강남구 세미나홀</p>
    </section>
    
    <section id="speakers">
        <h2>경영자 소개</h2>
        <div class="speaker">
            <h3>홍기롱</h3>
            <p>대한기업 총수</p>
        </div>
        <div class="speaker">
            <h3>김이박</h3>
            <p>경영 컨설던트</p>
        </div>
    </section>
    
    <section id="register">
        <h2>지금 등록하세요</h2>
        <form action="/submit" method="POST">
            <label for="name">이름:</label>
            <input type="text" id="name" name="name" required>
            
            <label for="email">이메일:</label>
            <input type="email" id="email" name="email" required>
            
            <button type="submit" class="cta">지금 등록하기</button>
        </form>
    </section>
    
    <footer>
        <p>© 2024 이벤트 주최자 & 대한기업</p>
    </footer>
</body>
</html>




