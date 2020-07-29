# Day10Project

//#include<stdlib.h>//malloc의 헤더
//#include<iostream>
//
////malloc이 할당한 영역은 heap영역이다.
//using namespace std;
//
//int main()
//{
//	int input = 0;
//	cin >> input;
//
//	int * ptr = (int*)malloc(sizeof(int) * input); //동적 할당
//	//메모리 할당을 받는다. void형으로 값을 넘겨준다. (void는 형이 없다)(어떤형으로 줄지 모르기 때문에void형이나 나중에 형 변환을 한다.)
//	//정해지지 않은 메모리에 할당을 받는다.
//	for (int i = 0; i < input; i++)
//	{
//		cout << i << "번째 값 입력 " << endl;
//
//		cin >> ptr[i];//(배열처럼 할당을 받는다)//배열처럼 쓴다.
//
//	}
//	cout << "입력 완료 " << endl;
//		
//
//	for (int i = 0; i < input; i++)
//	{
//		cout << ptr[i] << endl;
//
//	}
//	//malloc으로 할당을 받고 
//	free(ptr);//메모리를 해제한다.(메모리를 반환해준다.)
//	//이것이 포인터의 어려운 점이다. 
//	return 0;
//
//}
                            
//#include<stdio.h>
//#include<iostream>
//
//using namespace std;
//
//
//
//int main()
//{
//	//갯수와 크기로 메모리 할당을 받는 함수
//	//calloc은 malloc이랑 똑같은데 인자 크기가 다르다.
//	int * ptr = (int*)calloc(10, sizeof(int));
//	//ptr은 이미 할당되있는 주소를 쓴다.
	
	
	
//	//다시 메모리를 크기변경하는 realloc 
//
//	//이전에 할당된 메모리 크기를 변경하는 함수
//	ptr = (int*)realloc(ptr, sizeof(int) * 2);
//	//calloc이 10개를 받은 것을 realloc이 2개로 바꾼다.
//	//calloc한테 부족한 주소를 더 쓰게 할 수 있음.
	
	//realloc은 동정할당해제를 한번 더 안해도 된다.
	//malloc을 쓴 만큼 할당해제를 하면 된다.
//	
//	free(ptr);
//	//해제
//
//	ptr = nullptr;//nullpointer -> 이 포인터는 할당이 안되있어요(라는 뜻이다)
//
//	/*float * ptrf = nullptr;
//
//	if()
//		if(ptrF == nullptr)
//			할당해라*/
//
//
//	/*if (ptrF != nullptr)
//	{
//		free(ptrF);
//
//		prtF = nullptr;
//	}
//
//	ptrF = (float *)malloc(sizeof(float) * 4);
//*/
//
//
//	return 0;
//
//}
  
  //#include<Windows.h>
//#include<stdio.h>
//#include<iostream>
//#include<stdlib.h>
//#include<string>
//
//
//
//using namespace std;
//
//struct Character
//{
//	int level;
//	float attack;
//	float  defense;
//	//string name;
//	char * name;
//	
//};
//int main()
//{
//
////	Character * characters = (Character*)malloc(sizeof(Character) * 3);
////	//캐릭터가 3개 만들어짐 (메모리가 3개 잡힌다)
////	characters[0].attack = 100.0f;
////	characters[1].defense = 20.0f;
////	characters[2].level = 99;
////	free(characters);
//	int input = 0;
//	cout << "만들 캐릭터의 개수를 입력해주세요 : ";
//	cin >> input;
//
//	Character * characters = (Character*)malloc(sizeof(Character) * input);
//
//	for (int i = 0; i < input; i++)
//	{
//		//캐릭터형 이름에다가 255글자짜리 메로리를 확보0
//		//이름 메모리를 할당
//
//		/*char * temp = (char*)malloc(sizeof(char) * 255);*/
//		characters[i].name = (char*)malloc(sizeof(char) * 255);
//
//		cout << i + 1 << "번째 캐릭터의 이름을 입력헤주세요 : ";
//		cin >> characters[i].name;
//
//
//		/*cout << i + 1 << "번째 캐릭터의 이름을 입력헤주세요 : ";
//		cin >> temp;
//		characters[i].name =append(temp);
//*/
//		cout << i + 1 << "번째 캐릭터의 이름 : " << characters[i].name;
//		free(temp);
//
//
//		cout << i + 1 << "번째 캐릭터의 레밸을 입력헤주세요 : ";
//		cin >> characters[i].level;
//
//		cout << i + 1 << "번째 캐릭터의 공격력을 입력헤주세요 : ";
//		cin >> characters[i].attack;
//
//		cout << i + 1 << "번째 캐릭터의 방어력을 입력헤주세요 : ";
//		cin >> characters[i].defense;
//
//
//		system("cls");
//	}
//
//	system("cls");
//	int selection = 0;
//	cout << "캐릭터 정보 보기 (1~ " << input << ")" << endl;
//	cin >> selection;
//
//	cout << selection << "번째 캐릭터의 정보 " << endl;
//	cout << endl;
//	cout << selection << "번째 캐릭터의 이름 : " << characters[selection - 1].name << endl;
//	cout << selection << "번째 캐릭터의 레밸 : " << characters[selection - 1].level << endl;
//	cout << selection << "번째 캐릭터의 공력력 : " << characters[selection - 1].attack<< endl;
//	cout << selection << "번째 캐릭터의 방어력 : " << characters[selection - 1].defense << endl;
//
//	// 모든 캐릭터의 이름 메모리를 해제
//	for (int i = 0; i < input; i++)
//	{
//		free(characters[i].name);
//		//왜 이름만 하냐면 이름만 할당을 받아서
//	}
//
//	free(characters);
//
//	return 0;
//}
                              
                              
                              #include<stdio.h>
#include<iostream>
#include<stdlib.h>


using namespace std;


int main()
{
	int IntVar = 6;
	int * ptr = &IntVar;
	printf("IntVar = %d , *ptr = %d\n", IntVar, *ptr);

	float FloatVar1 = 0.78f;
	float * ptrF = nullptr;
	ptrF = &FloatVar1;

	printf("FloatVar1 = %f, *ptrF = %f\n", FloatVar1, *ptrF);

	int IntArray1[] =
	{
		3,5,1,4,8,2
	};

	ptr = IntArray1;

	printf("0 : *ptr = %d\n", *ptr);
	printf("0 : ptr = %d\n", (int)ptr);//주소값//int형 배열이기 때문에 4byte씩 증가함.

	ptr++;
	printf("1 : *ptr = %d\n", *ptr);
	printf("2 : ptr = %d\n", (int)ptr);//주소값

	ptr++;
	printf("3 : *ptr = %d\n", *ptr);
	printf("3 : ptr = %d\n", (int)ptr);//주소값

	ptr = IntArray1;

	
	printf("4 : *ptr = %d\n", *(ptr+3));
	printf("4 : ptr = %d\n", (int)(ptr + 3));//주소값

	printf("5 : *ptr = %d\n", *(ptr+5));
	printf("5 : ptr = %d\n", (int)(ptr + 5));//주소값
	
	ptr = IntArray1;
	printf("*ptr = %d\n", *ptr);
	printf(" ptr = %d\n", (int)ptr);

	ptr = &IntArray1[0];
	printf("*ptr = %d\n", *ptr);
	printf(" ptr = %d\n", (int)ptr);
	return 0;
}

//
//#include<stdio.h>
//#include<iostream>
//
//using namespace std;
//int memcount = 0;
//
//void Creatmemeoy(int ** pptr, int size)//포인터형 변수의 주소를 말함(*ptr)<-이거//주소값을 이중포인터로 넘겨준다.??????????????
//{
//	*pptr = (int*)malloc(sizeof(int) * size);
//	memcount++;
//}
//
//void Releasememeoy(int* ptr)
//{
//	free(ptr);
//	memcount--;
//}
//struct Temp
//{
//	char* str = nullptr;
//};
//
//int main()
//{
//	int * temp = nullptr;
//	Creatmemeoy(&temp, 3);//nullpointer는 주소를 *ptr을 쓰면 주소값이 없으니 **pptr에 넣는 것이다.
//
//	Releasememeoy(temp);
//
//
//	Temp t;
//	t.str = (char*)malloc(sizeof(char) * 255);
//	free(t.str);
//
//
//
//
//	return 0;
//
//}
//숙제
//N개의 숫자 중 최대값이 몇번째 있는지 찾아라
//- 숫자를 몇개(n개)까지 받을지 사용자로 부터 입력
//- n개 만큼 숫자를 입력받을 것
//- 모든 입력이 끝나면 최대값이 몇번째 있는지 인덱스 출력( ex) 0번 값이 최대값입니다.)
//- 최대값이 동일하게 2개 이상 있는 경우 인덱스가 가장 작은것이 최대값
//


  
