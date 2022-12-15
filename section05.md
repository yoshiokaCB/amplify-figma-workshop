# 5. Amplify Studio の設定

ここでは、Amplify にアクセスし、Amplify Studio を利用して Figma のデザインをコンポーネントとして読み込み、データベースとの紐付けを設定します。

また、リスト表示用（Collection）のコンポーネントも作成します。

![amplifystudio](./img/amplify01.png)

1. AWS マネージメントコンソールから **Amplify** にアクセスします。

---

![amplifystudio](./img/amplify02.png)

1. `amplify init` を実行したことによりアプリケーション名 amplifyhomes が作成されています。クリックして詳細を表示します。

---

![amplifystudio](./img/amplify03.png)

1. 「**Amplify Studio をセットアップ**」をクリックします。

---

![amplifystudio](./img/amplify04.png)

1. **Amplify Studio を有効にします。** を **on** にします。

---

![amplifystudio](./img/amplify05.png)

1. **backend environment** の url をクリックして Amplify Studio にアクセスします。

---

<img src="./img/amplify06.png" alt="amplifystudio" width="500" />

1. 認証を要求されるので、「**Log in with AWS Account**」をクリックします。
1. 無事に認証が終わると Amplufy Studio が起動します。

---

![amplifystudio](./img/amplifystudio02.png)

1. 画面左メニューの「**UI Library**」メニューをクリックし、続けて右上の「**Sync with Figma**」をクリックします。

---

<img src="./img/amplifystudio03.png" alt="amplifystudio" width="700" />

1. 先ほど Figma でコピーした**リンク**を貼り付け、「**Countinue**」をクリックします。

---

<img src="./img/amplifystudio03-1.png" alt="amplifystudio" width="500" />

1. 「**アクセスを許可**」をクリックします。

---

<img src="./img/amplifystudio04.png" alt="amplifystudio" width="500" />

1. 「**Accept all changes**」をクリックします。

---

<img src="./img/amplifystudio05.png" alt="amplifystudio" width="370" />

1. 「**Accept all**」をクリックします。

---

![amplifystudio](./img/amplifystudio06.png)

1. Components に先ほど Figma で編集したコンポーネントがあることを確認します。

---

![amplifystudio](./img/amplifystudio07.png)

1. 次に画面左のメニューの「**Data**」をクリックし、続けて「**Add model**」をクリックします。

画像を参考に **table:News** を入力します。

Add a field をクリックして、  
- Field name: **title**, Type **String** 
- Field name: **paragraph**, Type **String**

を入力します。

1. 入力が終わったら画面右上の「**Save and Deploy**」をクリックします。

---

![amplifystudio](./img/amplifystudio08.png)

1. 「**Deploy**」をクリックします。

---

![amplifystudio](./img/amplifystudio09.png)

1. 画面のように表示されたらデプロイ終了です。

---

![amplifystudio](./img/amplifystudio10.png)

1. 画面左メニューの「**Content**」をクリックし、続けて「**Auto-geenerate seed data**」をクリックし、ダミーデータを作成します。

---

![amplifystudio](./img/amplifystudio11.png)

1. 画像を参考に、「**How many rows ...**」は **5**
1. 「**Add constraint**」をクリックし、**title**, **paragraph** にそれぞれ設定をして、「**Generate data**」をクリックします。

---

![amplifystudio](./img/amplifystudio12.png)

1. 画像のようにデータが作成されていることを確認します。(ランダムに生成されるため、データの内容は一致しません)

---

![amplifystudio](./img/amplifystudio13.png)

1. 画面左メニューの「**UI Library**」をクリックし、「**Components**」から Figma で作成した「**NewsItem**」をクリックし、「**Configure**」をクリックして編集画面にアクセスします。

---

![amplifystudio](./img/amplifystudio14.png)

1. 画面左のツリー表示のメニューを展開し「**Title**」をクリックし、画面左に表示される「**Set text label**」をクリックします。

---

<img src="./img/amplifystudio15.png" alt="amplifystudio" width="400" />

1. **news** の **news.title** を選択します。

---

<img src="./img/amplifystudio16.png" alt="amplifystudio" width="400" />

1. 画像のような表示になっていれば OK です。

---

![amplifystudio](./img/amplifystudio17.png)

1. 続けて同じように **Paragraph** の設定もします。

---

<img src="./img/amplifystudio18.png" alt="amplifystudio" width="400" />

1. **news** の **news.paragraph** を選択します。
1. 画面のような表示にします。

---

![amplifystudio](./img/amplifystudio19.png)

1. 続けて画面右上の「**Create collection**」をクリックします。

---

![amplifystudio](./img/amplifystudio20.png)

1. 「**NewsItemCollection**」と入力して「**Create**」をクリックします。

---

![amplifystudio](./img/amplifystudio21.png)

---

[-> 6. Cloud9 でアプリケーションの設定](./section06.md "06")

[-> トップへ戻る](./README.md "top")
