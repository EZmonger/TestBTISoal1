﻿# TestBTISoal1
# TestBTISoal1
# TestBTISoal1

Jawaban soal C - G

C. SQL Test
RESULT_1
SELECT item
FROM ASSET
GROUP BY item

RESULT_2
SELECT 
a1.user_id,
STUFF((SELECT ‘, ‘ + CAST(a2.item AS varchar) 
FROM ASSET a2
WHERE a2.user_id = a1.user_id
FOR XML PATH(‘’)), 1, 1, ‘’) AS [asset]
FROM ASSET a1
GROUP BY a1.user_id
ORDER BY a1.user_id

D. ERD Test
 
E. Function
1. 
n = input()

for (int i = 1; i <= n; i++){
	for(int j = 1; j <= n; j++){
		if(j > i){
			print(j+2, end="")
		}
		print(j, end="")
		if(j == i){
			print("**")
		}
	}
	print()
}
2. 
selisih(arr){
	int max = 0

	for(int i = 0; i < arr.length(); i++){
		if(i+1 == arr.length()){
			continue;
		}
		if(arr[i] > arr[i+1]){
			selisih = arr[i] - arr[i+1]
			if(max < selisih){
				max = selisih
			}
		}
	

	}

	return max;
}

F. 
- Cypress = aplikasi open source untuk melakukan testing secara otomatis
- Kubernetes = aplikasi open source untuk melakukan software deployment
- ORM = Teknik programming untuk melakukan mapping atau kueri data dari database dengan object oriented
- Class = suatu template pada programming untuk membuat suatu object
- Function = operasi untuk melakukan suatu instruksi dalam pemograman
- DevOps = suatu methodology dalam software development, menggunakan tools-tools untuk pemograman
- Docker = mirip container untuk membawakan software dalam bentuk package

G.
Architecture yang terbaik adalah architecture Object oriented progra
