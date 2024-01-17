# test_gitnore

**1. 깃허브 commit 충돌 이슈** 현재 깃허브에 올라가 있는 Commit 버전과 자신이 수정해서 올리려고 하는 파일이 일치하지 않을 때 충돌이 발생. 깃허브에 올라가 있는 버전으로 pull해서 다시 자신이 변경한 코드를 push하는 방식으로 해결했다.

**2. Scanner 이슈** 조건문에서 조건을 비교할 때 변수를 사용하지 않고 scan.nextInt()를 사용해서 조건문을 실행할 때 마다 입력을 nextint()로 scan되는 값 만큼 반복해서 받아야 실행되는 이슈가 있어 변수를 지정하여 처리하였더니 제대로 동작함.

**3. lombok과 getConnection() 충돌 이슈** lombok의 @Getter와 java.sql.Connection.getConnection() 을 동시에 사용하려 할 때 충돌이 발생해서 mysql DB에 접속하기 위해 getConnection()을 사용하려면, @Getter를 사용하지 않아야 한다.
