---
lab:
  title: 演習 04 - データ収集ルールを作成して Azure Monitor エージェントをインストールする
  module: Module 05 - Create a data collection rule and install the Azure Monitor Agent
---


>**注**: このラボを完了するには、管理者アクセス権のある [Azure サブスクリプション](https://azure.microsoft.com/en-us/free/?azure-portal=true) が必要です。 


データ収集ルール (DCR) では収集するデータを指定しますが、Azure Monitor エージェントはこれらのルールを適用して、Azure、他のクラウド、またはオンプレミスの仮想マシンからログとメトリックを収集します。 これらを組み合わせることで、さまざまな環境で一貫性のある一元的な監視が可能になります。

---

## スキル タスク

- データ収集ルールを作成して定義します。

- データ収集のターゲット リソースを選択します。

- Azure Monitor エージェントをインストールします。
  
- データ ソースと収集先を構成します。

- 収集するデータ ソースの種類とデータを選択します。

- データ配信先を選択します。

## 演習の手順 

### データ収集ルールを作成して Azure Monitor エージェントをインストールします。

>**注**: Log Analytics ワークスペースまたは Azure Monitor ワークスペースと同じリージョンにデータ収集ルールを作成してください。 データ収集ルールは、テナント内の任意のサブスクリプションまたはリソース グループのマシンまたはコンテナーに関連付けることができます。 Azure Monitor エージェントは、Azure 仮想リソースに自動的にインストールされます。

1. ポータルの上部にある検索ボックスに、「**データ収集ルール**」と入力します。 検索結果にある **[データ収集ルール]** を選択します。
  
2. **[データ収集ルール]** ページで、**[+ 作成]** を選択します。
  
   ![image](https://github.com/user-attachments/assets/99b9ac51-f2f4-466f-80bb-79d74874b573)

3. **[データ収集ルールの作成] ブレード**の **[基本]** ページで、次の設定を指定します (他の設定は既定値のままにします)。

    |設定|値|
    |---|---|
    |**ルールの詳細**|
    |規則の名前|**dcr-1**|
    |サブスクリプション|サブスクリプションを選択します。|
    |Resource group|**az-rg-1**|
    |リージョン|**米国東部**|
    |プラットフォームの種類|**Windows**|
    |データ収集エンドポイント|既定の設定の "なし" のままにします。|

    ![image](https://github.com/user-attachments/assets/35c527cf-499d-44b9-966f-0114b8643ef2)

4. **[基本]** ページの下部にある **[次へ: リソース]** というラベルの付いた ボタンをクリックして次に進みます。
   
5. **[リソース]** ページで、**[+ リソースの追加]** を選択します。

    ![image](https://github.com/user-attachments/assets/6aabf2c9-bea2-47c1-9b0b-bf131cdec4e3)

6. **[スコープの選択]** テンプレートで、**[スコープ]** の **[サブスクリプション]** ボックスをオンにします。

    ![image](https://github.com/user-attachments/assets/2215e8cd-5047-4fc6-91ba-b2c645571bbd)

7. **[スコープの選択]** テンプレートの下部にある **[適用]** をクリックします。
  
8. **[リソース]** ページの下部にある **[次へ: 収集と配信]** を選択します。

    ![image](https://github.com/user-attachments/assets/717226c3-5ce0-454f-93a4-11b0e67d5a23)

9. **[収集と配信] ページ**で、**[+ データ ソースの追加]** をクリックします。

    ![image](https://github.com/user-attachments/assets/0809cf5b-a460-40d1-8508-e42ba7ce78c1)

10. **[データ ソースの追加]** テンプレートの **[データ ソースの種類]** で、次の設定を選択します。
    
    |設定|Value|
    |---|---|
    |**データ ソースの追加**|
    |リソースについて、収集するデータ ソースの種類とデータを選択します。|
    |データ ソースの種類*|**Windows イベント ログ**|
    |[基本] を選択するとイベント ログの収集が有効になります。|
    |収集するイベント ログとレベルを構成します。|
    |アプリケーション|**重大**、**エラー**、**警告**|
    |セキュリティ|**監査の成功**、**監査の失敗**|
    |System|**重大**、**エラー**、**警告**|

    ![image](https://github.com/user-attachments/assets/5bc891ea-8cef-4baa-95c4-a432364179b1)

12. **[データ ソースの追加]** テンプレートの下部にある **[次へ: 宛先]** を選択します。
   
13. **[データ ソースの追加]** テンプレートの **[宛先]** タブで、次の設定を選択します。
    
    |設定|Value|
    |---|---|
    |**データ ソースの追加**|
    |宛先|**+ 宛先の追加**|
    |変換先の型|**Azure Monitor ログ**|
    |サブスクリプション|サブスクリプションを選択します。|
    |宛先の詳細|**azwrkspc1a (az-rg-1**)|

    ![image](https://github.com/user-attachments/assets/e00c17c8-5a70-4caa-8504-92f482cc5e57)

14. **[データ ソースの追加]** テンプレートの下部にある **[データ ソース の追加]** を選択します。

    ![image](https://github.com/user-attachments/assets/4277089c-971c-4334-a49d-6ac6bfe93ff4)

15. **[収集と配信]** ページの下部にある **[確認および作成]** を選択します。

    ![image](https://github.com/user-attachments/assets/0235fed9-6309-444c-9269-b9dbd1118b63)

16. **[確認および作成]** ページの下部にある **[作成]** を選択します。

> **結果**: データ収集ルールが作成され、Azure Monitor エージェントがインストールされました。