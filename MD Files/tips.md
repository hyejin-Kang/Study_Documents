# ㅇ 배열 표현하기
1. 반복문 활용
1. print(Arrays.toString(arr));
___

# ㅇ while문 입력받기 (feat. EOF)
* 파일 형태등의 외부 요소로부터 입력받을 때 사용<br>
    -> 입력과 동시에 null여부를 판단하여 탈출 조건을 준다.
    ```java
    while ((str=br.readLine())!=null)
    ```
___
 
# ㅇ String -> char[]로 변환하기
*  String.toCharArray()
    ```java
    char[] arr = br.readLine.toCharArray();
    ```
___
# ㅇ char -> 아스키코드
*   int<->char 자동형변환
    ```java
    int a = 'a';    //-> a=97
    char b = 97;    //-> b=a

    for(int i ='a'; i<='z'; i++){
        System.out.println(i);  //-> 97 ~ 122 출력
    }
    ```
___
 
# ㅇ StringToeken EOF
*   .hasMoreTokens()
    ```java
    while(st.hasMoreTokens()) {
			st.nextToken();
			cnt++;
		}
    ```
___
 
# ㅇ System.in.read()
*   스트림으로부터 하나의 문자를 받아옴
*   0 또는 한자리의 숫자를 입력한다는 전제일 경우 많이 사용
*   버퍼에서 하나씩 빼오기 때문에 for문을 통해 자릿수 하나 씩 불러올 수 있다.
    ```java
    for (int i = 0; i < A.length; i++) {
			A[i] = System.in.read()-'0';    
            //-> A의 자릿수를 아스키코드로 받아온 후 0의 아스키코드를 뺀다.
		}
    ```
___
 