# โค Check Point
## ๐งก 01. ๋ฐ์ดํฐ์ ์ค๋น
- ์ํฌํธ (iris๊ธฐ์ค)
    - from sklearn.datasets import load_iris
- ์ค๋นํ  ๋ฐ์ดํฐ
    - iris_data = iris.data -> ํ์ต๋ฐ์ดํฐ
    - iris_label = iris.target  -> ์ ๋ต์ง

## ๐งก 02. ํ์ตํ  ๋ฐ์ดํฐ์ ํ์คํธ ๋ฐ์คํธ ๋ฐ์ดํฐ ๋ถ๋ฆฌ
- ์ํฌํธ
    - from sklearn.model_selection import train_test_split
- ํ์
    - X_train, X_test, y_train, y_test = train_test_split(ํ์ต๋ฐ์ดํฐ,  
                                                    ์ ๋ต์ง, 
                                                    ํ์คํธ ๋ฐ์ดํฐ ๋น์จ, 
                                                    ๋๋ค)

## ๐งก 03. ํ์ต ๋ชจ๋ธ ์ ์  ๋ฐ ํ์ต๊ณผ ์์ธก
- ์ํฌํธ 
    - ๋ชจ๋ธ๋ณ๋ก ์ํฌํธ ๋ฐฉ์์ด ์์ดํจ.

- ํ์ต ๋ชจ๋ธ ์ข๋ฅ
    1) DecisionTreeClassifier
    2) RandomForestClassifier
    3) SGDClassifier
    4) LogisticRegression

- ํ์
    - model = ๋ชจ๋ธ๋ช()
    - model.fit(ํ์ต๋ฐ์ดํฐ, ์ ๋ต ๋ฐ์ดํฐ)
    - y_pred = model.predict(ํ์คํธ ๋ฐ์ดํฐ)
    - X_train : ํ์ตํ  ๋ฐ์ดํฐ , y_train : ํ์ตํ  ๋ฐ์ดํฐ์ ์ ๋ต์ง
    - X_test : ํ์คํธํ  ๋ฐ์ดํฐ 
    - y_pred : ํ์คํธํ ๋ฐ์ดํฐ์ ๋ต์ง , y_test : ํ์คํธํ ๋ต์ง๋ ๋น๊ตํ  ์ค์  ์ ๋ต์ง
    
## ๐งก 04. ์ฑ๋ฅ ํ๊ฐ
- ์ํฌํธ
    - from sklearn.metrics import classification_report
    - ์ฌ๋ฌ๊ฐ์ง ์ฑ๋ฅํ๊ฐ(metrics)๋ฐฉ์์ด ์กด์ฌํจ.
- ํ์ 
    - classification_report(y_test, y_pred) 
    - ํ์คํธ๋ฐ์ดํฐ๋ฅผํตํด ์ป์ ๋ต๊ณผ ์ค์  ๋ต์ ๋น๊ตํ์ฌ ์ ํ๋ ์ธก์ 
    


