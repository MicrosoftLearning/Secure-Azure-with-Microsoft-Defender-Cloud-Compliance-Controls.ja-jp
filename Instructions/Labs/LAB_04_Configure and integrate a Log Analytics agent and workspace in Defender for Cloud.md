---
lab:
  title: 演習 04 - Log Analytics エージェントを構成して Defender for Cloud のワークスペースと統合する
  module: Module 05 - Configure and integrate a Log Analytics agent and workspace in Defender for Cloud
---


>**注**: このラボを完了するには、管理者アクセス権のある [Azure サブスクリプション](https://azure.microsoft.com/en-us/free/?azure-portal=true) が必要です。 


Defender for Cloud は、セキュリティの脆弱性と脅威を監視するために、Azure 仮想マシン (VM)、仮想マシンスケールセット、IaaS コンテナー、および非 Azure (オンプレミスを含む) マシンからデータを収集します。 一部の Defender プランでは、ワークロードからデータを収集するために監視コンポーネントが必要になります。 Log Analytics エージェントがオンの場合、Defender for Cloud では、サポートされているすべての Azure VM と新しく作成されるものにエージェントをデプロイします。 

---

## スキルアップ タスク

- エージェントの種類に対して Log Analytics エージェントの既定値を使用します。

- ワークスペースを選択します。
  
- ワークスペース レベルで保存するセキュリティ イベント データのレベルを定義します。

## 演習の手順 

### Log Analytics エージェントとの統合を構成します。

>**注**: Log Analytics エージェントがオンの場合、Defender for Cloud では、サポートされているすべての Azure VM と新しく作成されるものにエージェントをデプロイします。 

1. ブラウザー セッションを開始し、[Azure portal メニュー](https://portal.azure.com/)にサインインします。
   
2. [Defender for Cloud] メニューで、 **[環境設定]** を開きます。

4. サブスクリプションを選択します。

5. Defender プランの [設定と監視の対象] 列で、**[設定と監視]** を選択します。

7. [Log Analytics] 行の [構成] 列で、**[構成の編集]** をクリックします。

8. 自動プロビジョニング構成テンプレートで、次の操作を実行します。

   - [ワークスペースの選択] で、**[カスタム ワークスペース]** をクリックします。

   - **ドロップダウン メニュー**をクリックし、以前に作成したワークスペースを**選択**します。

   - **[セキュリティ イベント ストレージ]** で**ドロップダウン メニュー**をクリックし、**[すべてのイベント]** を選択します。

   - 自動プロビジョニング テンプレートの下部にある **[適用]** をクリックします。
   
![image](https://github.com/MicrosoftLearning/Secure-Azure-services-and-workloads-with-Microsoft-Cloud-Security-Benchmark/assets/91347931/c1c812e7-b5ca-4caa-b8e6-34a6e4b325fd)




> **結果**: Microsoft Defender for Cloud で Log Analytics エージェントとワークスペースを構成しました。
