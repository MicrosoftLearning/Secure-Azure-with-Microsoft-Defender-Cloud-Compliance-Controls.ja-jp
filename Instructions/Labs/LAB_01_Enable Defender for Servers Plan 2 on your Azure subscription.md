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

2. Azure portal の [リソース、サービス、ドキュメントの検索] テキスト ボックスで、Azure portal ページの上部に「Microsoft Defender for Cloud」と入力し、Enter キーを押します。

3. **Microsoft Defender for Cloud** の **[管理] ブレード**で、**[環境設定]** に移動します。 **[Ignite サブスクリプション]** セクションが表示されるまで環境設定フォルダーを展開し、**[Ignite サブスクリプション]** をクリックして詳細を表示します。

4. ご利用の **[サブスクリプション]** と、モジュール 02 で作成した **[Log Analytics ワークスペース]** を選択して、Microsoft Defender プランを有効にします。

5. ページの下部にある大きな青い **[アップグレード]** ボタンをクリックします。
   
    ![image](https://github.com/MicrosoftLearning/Secure-Azure-services-and-workloads-with-Microsoft-Cloud-Security-Benchmark/assets/91347931/256bd584-b04f-4d5b-81a7-c83dd1af3b4f)
   
6. **[Microsoft Defender for Cloud]** の **[はじめに]** ブレードで **[エージェントのインストール]** タブに移動して下へスクロールします。

    ![image](https://github.com/MicrosoftLearning/Secure-Azure-services-and-workloads-with-Microsoft-Cloud-Security-Benchmark/assets/91347931/8120ec8f-23dc-4636-bc45-b415c7894b8c)

7. エージェントをインストールするサブスクリプションに関連付けられたチェックボックスをオンにし、**[エージェントのインストール]** をクリックします。

### Microsoft Defender for Cloud のサブスクリプションをアップグレードするための代替アクション。

1. **[Microsoft Defender for Cloud]** に移動し、[管理] セクションの下にある左側のナビゲーション パネルで **[環境の設定]** をクリックします。
   
2. **[Microsoft Defender for Cloud] の [環境設定]** ブレードで **[すべて展開]** をクリックし、サブスクリプションが表示されるまで下にスクロールし、関連するサブスクリプションをクリックします。

3. **[設定] の [Defender プラン]** ブレードで **[すべてのプランを有効にする]** を選択し、**[保存]** をクリックします。

   ![image](https://github.com/MicrosoftLearning/Secure-Azure-services-and-workloads-with-Microsoft-Defender-for-Cloud-regulatory-compliance-controls/assets/91347931/4b684851-98ae-4720-a3e3-afa99aab8c43)




   

   
> **結果**: Azure サブスクリプションで Defender for Cloud がアップグレードされ、有効になりました。
