# Flutter
## Flutter Reference 
[Flutter Gallery](https://github.com/flutter/gallery#flutter-gallery)
[Flutter Dart Pad](https://dartpad.dev/)
[Flutter Package](https://pub.dev/)

### Flutter 프로젝트 생성
>ctrl + shift + p  
>flutter new project  
>application

### Flutter simulator 실행
>ctrl + shift + p
>flutter launch emualator
>choice

### Type
- int, double, num
- var, dynamic

### Class
- 클래스 : 객체를 생성하기 위해 작성하는 설계도
- 생성자 : 클래스 생성시 최초 호출되는 함수
- 상속 : 클래스의 속성과 함수를 확장하기 위해 활용

### 비동기
- Java의 thread 대신 비동기 처리를 위해 지원
```
class MyApp extends StatelessWidget {
 // StatelessWidget : 화면이 바뀔때 바뀌지 않는 (고정)
 // StatefullWidget : 화면이 바뀔때 바뀌는 (유동)
  const MyApp({super.key});

  @override
  Widget build(BuildContext context) {
	// 
    return MaterialApp(
      title: 'Flutter Demo',
      theme: ThemeData(
        colorScheme: ColorScheme.fromSeed(seedColor: Colors.deepPurple),
        useMaterial3: true,
      ),
      home: const MyHomePage(title: 'Home Page'),
    );
  }
}


class _MyHomePageState extends State<MyHomePage> {
  int _counter = 0;

  void _incrementCounter() {
    setState(() {
// setState : 활성 상태
      _counter++;
    });
  }
```

### Flutter - Widget
center - child 한개  
column - children 여러개  
pup.yaml → `dependencies`  
패키지 추가 .pup install  

### Flutter - Layout

- Row / Column
- Container
- ScrollView
- ListView
- GridView
- PageView
- BottomNAVIGATIONBAR

### 재정렬
code → Reformat Code with ‘dart format’
<code>
stf → statefullwidget
stl → statelesswidget
