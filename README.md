## How to get keys

Open ` /data/data/app.source.getcontact/shared_prefs/GetContactSettingsPref.xml` 

* AES key: `FINAL_KEY`
* token: `TOKEN`
* exp: `PRIVATE_KEY`


## How to run 

- Create and run venv
```shell script
[ ! -d venv ] && python3 -m venv venv; source venv/bin/activate
```

- Install requirements
```shell script
pip3 install -r requirements.txt
```

- Console output
```shell script
python3 ./src/main.py -p +79291045342
```
Output:
```
Phone: +79291045342
User: Андрей Тимофеев
Tag list: 
	 Андрей Тимофеев
	 Андрей Спб
	 Андрей Челентос
	 Андрей Катин
	 Андрей
	 Онлрей
	 Экс Бойфренд Aka Реальный Долбоеб
	 Андрей Chelentos
	 Andrey Tymofeev
	 Андрей Тим
	 Андрюша :
	 Андрей 💑
	 .andrey
	 Andrey
Remain count: 194
```

- Console JSON-format output 
```shell script
python3 ./src/main.py -j -p +79291045342
```
Output:
```json5
{'name': None, 'phoneNumber': '+79291045342', 'country': 'RU', 'displayName': 'Андрей Тимофеев', 'profileImage': None, 'email': None, 'is_spam': False, 'remain_count': 194, 'tags': ['Андрей Тимофеев', 'Андрей Спб', 'Андрей Челентос', 'Андрей Катин', 'Андрей', 'Онлрей', 'Экс Бойфренд Aka Реальный Долбоеб', 'Андрей Chelentos', 'Andrey Tymofeev', 'Андрей Тим', 'Андрюша :', 'Андрей 💑', '.andrey', 'Andrey']}
```