코드스피츠 2강 1회차


== 전략객체

< 	통화요금   > 	 			   <  멤버쉽, 통신 요금,다양한 정책 ...  >   < 멤버쉽, 통신 요금 >

Implement -> Extends (중복제거) ->      합성 (확장 가능성이 있어보임)    	-> Extends (구체적인 요구사항이 정해짐, 유연성의 정적 제약을 주고 싶음) 

	


     Next(Call)					List<Call>
							|
							|
							|
							|
							|
							|							


요구사항 정의 단계 파악단계가 보임 


--------------------------------------------------------

protocol 무조건 {
	func 구현()
}
 
--------------------------------------------------------

protocol 무조건 {
	
}

extension 무조건 {
	func 구현() {

	}
}

--------------------------------------------------------

// 아 이거는 확장 가능성 커!!!!!!!!!!!!!!!!!!!!

// 유연한거죠 갈아끼울수도 있고


protocol 무조건 {
	
}

extension 무조건 {
	func 구현() {

	}
}

class AAA {
	init(무조건)
}

--------------------------------------------------------

// 여기서 복합성 폭발이야!!! 
// 조금은 제약을 주고싶다..........

// 타입 갯수가 정해지면

protocol AAA: 무조건 {
	
}

extension AAA {
	
}

--------------------------------------------------------




