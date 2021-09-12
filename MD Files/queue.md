# ㅇ 큐
- FIFO(First In First Out)
- 큐(Array)의 대표 메소드
    
    * 변수
        1. MAX          :   queue의 최대 저장 크기를 나타냄
        1. front        :   가장 먼저 들어온 변수의 위치(out의 대상)
        1. rear         :   가장 뒤에 들어오는 변수의 위치
        1. int[] queue  :   데이터를 저장할 배열

    * 메소드
        1. enqueue(push)()  : queue[rear]에 값을 저장하고 rear++ 해준다.
        1. dequeue(pop)()   : queue[front]를 반환하고 front++ 해준다.
        1. peek()       : queue[front]를 반환한다.
        1. isEmpty()    : 큐가 텅 빈 상태, front==rear
        1. isFull()     : 큐가 꽉 찬 상태, rear==MAX-1

    * ArrayQueue의 한계
        1. 최대 MAX값의 크기만큼의 데이터만 저장할 수 있다.<BR>
            -> 원형 큐 구현을 통해 해결 가능
        1. dequeue시 front앞의 저장공간이 의미없이 할당되어 있어 메모리 낭비가 발생한다.
<br>
<br>
- 원형 큐