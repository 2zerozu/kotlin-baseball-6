## 기능목록
1. computer에 1~9 서로 다른 임의의 수 3개를 리스트에 저장한다.
   1. 랜덤 숫자를 생성한다
   2. computer 리스트에 저장된 값과 일치하지 않을 때 저장한다
   3. computer size는 3이 되도록 한다

2. 사용자가 입력한 user 3자리를 리스트로 저장한다
    1. `do-while`문을 활용하여 `computer!=user`일 때 반복
    2. user의 길이가 3이 아닐 때 `IllegalArgumentException` 발생
    3. user가 숫자가 아닐 때(`NumberFormatException`) `IllegalArgumentException` 발생

3. computer와 user의 값을 비교하여 ball과 strike를 계산한다
    1. computer의 값을 `forEachIndexed`를 이용하여 computer[index]와 user[index]가 같으면 strike++
   2. computer의 값이 user에 있다면 ball++
   3. 결과값을 print 해준다

4. computer와 user의 값이 같아지면 재시작할건지 물어본다
    1. 1을 누르면 true를, 2를 누르면 false를, 이외 숫자를 누르면 `IllegalArgumentException` 발생
   2. 위의 1,2,3번 과정을 1을 눌렀을 때 반복한다
   3. 2를 누르면 종료된다