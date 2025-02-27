---
lab:
  title: 演習 01 - サーバー用に Microsoft Defender for Cloud の強化されたセキュリティ機能を構成する
  module: Module 02 - Enable Defender for Cloud on Your Azure Subscription
---


>**注**: このラボを完了するには、管理者アクセス権のある [Azure サブスクリプション](https://azure.microsoft.com/en-us/free/?azure-portal=true) が必要です。 


この演習の主な目標は、Azure サブスクリプション内で Microsoft Defender for Servers プラン 2 を構成および有効化する実践的な体験を提供することです。 これにより、クラウド リソースを監視し、セキュリティ上の脅威から保護することができます。 

---

## スキルアップ タスク

- サーバー用に Microsoft Defender for Cloud の強化されたセキュリティ機能を構成する
  
- Microsoft Defender for Servers プラン 2 の強化されたセキュリティ機能を確認する

## 演習の手順

### サーバー用に Microsoft Defender for Cloud の強化されたセキュリティ機能を構成する

1.  ブラウザー セッションを開始し、[Azure portal メニュー](https://portal.azure.com/)にサインインします。         

2. Azure portal において、Azure portal ページの上部にある [リソース、サービス、ドキュメントの検索] テキスト ボックスに、「**Microsoft Defender for Cloud**」と入力し、**Enter** キーを押します。

3. **Microsoft Defender for Cloud** の **[管理] ブレード**で、**[環境設定]** に移動します。 **サブスクリプション** セクションが表示されるまで環境設定フォルダーを展開し、**サブスクリプション**をクリックして詳細を表示します。

   ![image](https://github.com/user-attachments/assets/3b25dd82-e09e-4f8a-b85e-c9bc6c4bd488)
   
4. **[設定]** ブレードの **[Defender プラン]** で、**[クラウド ワークロード保護 (CWP)]** を展開します。

5. **クラウド ワークロード保護 (CWP) プラン**の一覧から **[サーバー]** を選択します。 ページの右側で、**[状態]** を **[オフ]** から **[オン]** に変更し、**[保存]** をクリックします。

6. **Microsoft Defender for Servers プラン 2** の詳細を確認するには、**[プランの変更]** を選択します。

   注: クラウド ワークロード保護 (CWP) サーバー プランをオフからオンにすると、Microsoft Defender for Servers プラン 2 が有効になります。
 
   ![image](https://github.com/user-attachments/assets/de434a75-345a-4023-83f1-fa53fcb5f288)
   
> **結果**: サブスクリプションで Microsoft Defender for Servers プラン 2 が有効になりました。
