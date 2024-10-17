---
lab:
  title: 演習 01 - Azure サブスクリプションで Defender for Servers プラン 2 を有効にする
  module: Module 02 - Enable Defender for Servers Plan 2 on your Azure subscription
---


>**注**: このラボを完了するには、管理者アクセス権のある [Azure サブスクリプション](https://azure.microsoft.com/en-us/free/?azure-portal=true) が必要です。 


この演習の主な目標は、Azure サブスクリプション内で Microsoft Defender for Servers プラン 2 を構成および有効化する実践的な体験を提供することです。 これにより、クラウド リソースを監視し、セキュリティ上の脅威から保護することができます。 

---

## スキルアップ タスク

- Microsoft Defender for Cloud の Defender for Servers プラン 2 を有効にします。
  
- 強化されたサーバーの機能を確認します。

## 演習の手順

### Microsoft Defender for Cloud のアップグレード

1. [[Azure portal]](https://portal.azure.com/) のメニューにサインインします。

2. Azure portal において、Azure portal ページの上部にある [リソース、サービス、ドキュメントの検索] テキスト ボックスに、「**Microsoft Defender for Cloud**」と入力し、**Enter** キーを押します。

3. **Microsoft Defender for Cloud** の **[管理] ブレード**で、**[環境設定]** に移動します。 **サブスクリプション** セクションが表示されるまで環境設定フォルダーを展開し、**サブスクリプション**をクリックして詳細を表示します。

   ![image](https://github.com/user-attachments/assets/32d2168e-458f-4872-9bf8-e8f050f24751)
   
3. **[設定]** ブレードの **[Defender プラン]** で、**[クラウド ワークロード保護 (CWP)]** を展開します。

4. **クラウド ワークロード保護 (CWP) プラン**の一覧から **[サーバー]** を選択します。 ページの右側で、**[状態]** を **[オフ]** から **[オン]** に変更し、**[保存]** をクリックします。

5. **[サーバー プラン 2]** の詳細を確認するには、**[プランの変更]** を選択します。

   注: クラウド ワークロード保護 (CWP) サーバー プランをオフからオンにすると、Microsoft Defender for Servers プラン 2 が有効になります。

   ![image](https://github.com/user-attachments/assets/869a38e4-464e-4be0-b02e-ce1b96f02978)
   
> **結果**: サブスクリプションで Microsoft Defender for Servers プラン 2 が有効になりました。
