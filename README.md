# servlet

###순수 java 파일만 이용

###webcontainer에서 class로 컴파일되고 링크과정을 거쳐 사용자에게 response됨

####ex) url mapping
localhost:8080/TEST

####포트번호 뒤에 적히게 되는게 mapping 된 주소가 된다.


##jsp는 븃단
contorller model은 servlet으로 만들게됨?

servlet  mapping
was에있는 servlet을 호출함
servlet 이름이 길고 복잡한 것을 간결하고 보안에 취약하지 않게 mapping

##방법 1
web.xml으로 mapping
서블릿 등록 해주고 매핑해주고 url-pattern 지정 하면 끝남
ex) <servelt>
	<servlet-name>servletEx</servlet-name>
	<servlet-class>com.servlet.ServletEx</servlet-class>
    </servlet>
    <servlet-mapping>
	<servlet-name>servletEx</servlet-name>
	<url-pattern>/SE</url-pattern>
    </servlet-mapping>

##방법 2
java 어노테이션 mapping 
흔히 어노테이션에 url mapping값 적어주면됨

web.xml과 java 어노테이션 둘다 mapping 해도 되긴한다.
