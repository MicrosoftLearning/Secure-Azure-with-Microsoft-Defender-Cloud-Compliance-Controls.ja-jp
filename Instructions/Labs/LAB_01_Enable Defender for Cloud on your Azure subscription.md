---
lab:
  title: 演習 01 - Azure サブスクリプションで Defender for Cloud を有効にする
  module: Module 02 - Enable Defender for Cloud on your Azure subscription
---


>**注**: このラボを完了するには、管理者アクセス権のある [Azure サブスクリプション](https://azure.microsoft.com/en-us/free/?azure-portal=true) が必要です。 


この演習の主な目標は、Azure サブスクリプションで Microsoft Defender for Cloud の構成と有効化に関する実践的な体験を提供することです。 これにより、クラウド リソースを監視し、セキュリティ上の脅威から保護することができます。 

---

## スキルアップ タスク

- Microsoft Defender for Cloud のサブスクリプションをアップグレードする。
  
- 包括的なカバレッジを実現するために、必要なマシンに Microsoft Monitoring Agent をデプロイする。

## 演習の手順

### Microsoft Defender for Cloud のアップグレード

1. [[Azure portal]](https://portal.azure.com/) のメニューにサインインします。

2. Azure portal の [リソース、サービス、ドキュメントの検索] テキスト ボックスで、Azure portal ページの上部に「Microsoft Defender for Cloud」と入力し、Enter キーを押します。

3. **Microsoft Defender for Cloud** の **[はじめに]** ブレードで **[アップグレード]** タブに移動し、**[強化されたセキュリティ機能で保護するサブスクリプションとワークスペースを選択してください]** セクションが表示されるまで下にスクロールします。

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
