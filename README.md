# StudyBottomNavigation(BottomNavionView + Navigation)

## 절차
1) activity_main에 BottomNavigationView 추가
2) menu 리소스 폴더, 파일 추가
3) menu 파일안에 BNV에 들어갈 아이템 추가
4) 항목 개수에 맞춰서 프래그먼트 생성
5) navigation 리소스 폴더, 파일 추가
6) navigation 파일안에 프래그먼트 추가 (서로 연결하지 않음)
7) activity_main에 NavhostFragment추가 후 fragment로 변경
8) activity_main에 
```
        BottomNavigationView bnv = findViewById(R.id.nav_view);
        NavController navController = Navigation.findNavController(this, R.id.fragment_id);
        NavigationUI.setupWithNavController(bnv, navController);
```
추가
