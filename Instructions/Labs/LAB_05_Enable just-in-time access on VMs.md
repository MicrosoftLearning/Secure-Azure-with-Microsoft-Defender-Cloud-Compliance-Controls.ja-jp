---
lab:
  title: 演習 05 - VM 上で Just-In-Time アクセスを有効にする
  module: Module 06 - Explore just-in-time VM access
---


>**注**: このラボを完了するには、管理者アクセス権のある [Azure サブスクリプション](https://azure.microsoft.com/en-us/free/?azure-portal=true) が必要です。 


Microsoft Defender for Cloud の Just-In-Time (JIT) アクセスを使用して、Azure 仮想マシン (VM) を未承認のネットワーク アクセスから保護できます。 多くの場合、ファイアウォールには、VM が攻撃に対して脆弱なままにする許可規則が含まれています。 JIT を使用すると、アクセスが必要な場合、必要なポート、必要な期間だけ VM へのアクセスを許可できます。 

---

## スキルアップ タスク

- Azure portal から VM で JIT を有効にする

- Azure portal から JIT が有効になっている VM へのアクセスを要求します。

## 演習の手順 

### Azure 仮想マシンから VM で JIT を有効にする

>**注**: Azure portal の Azure 仮想マシンページから、VM 上の JIT を有効にすることができます。

1. ポータルの上部にある検索ボックスに、「**仮想マシン**」と入力します。 検索結果から **[仮想マシン]** を選択します。

2. **vm-1** を選択します。
 
3. vm-1 の **[設定]** セクションから **[構成]** を選択します。
   
4. **[Just-In-Time アクセス]** で、**[Just-In-Time を有効にする]** を選択します。

5. 「**Just-in-time VM アクセス**」で、**[Microsoft Defender for Cloud を開く]** というリンクをクリックします。

6. 既定では、VM の Just-In-Time アクセスでは次の設定が使用されます。

   - Windows マシン
   
     - RDP ポート: 3389
     - 最大許容アクセス: 3 時間
     - 許可されているソース IP アドレス: すべて

   - Linux マシン
     - SSH ポート: 22
     - 最大許容アクセス: 3 時間
     - 許可されているソース IP アドレス: すべて
   
7. 既定では、VM の Just-In-Time アクセスでは次の設定が使用されます。

   - **[構成済み]** タブで、ポートを追加する VM を右クリックして、[編集] を選択します。
  
 ![image](https://github.com/MicrosoftLearning/Secure-Azure-services-and-workloads-with-Microsoft-Defender-for-Cloud-regulatory-compliance-controls/assets/91347931/66cf98b6-2ce0-43c7-a7be-b5d69bcfac1d)

   - **[JIT VM アクセス構成]** では、既に保護されているポートの既存の設定を編集するか、新しいカスタム ポートを追加できます。
   - ポートの編集が終わったら、 **[保存]** を選択します。   

### Azure 仮想マシンの接続ページから JIT 対応 VM へのアクセスを要求します。

>**注**: VM で JIT が有効になっている場合は、VM に接続するためのアクセス権を要求する必要があります。 JIT を有効にした方法に関係なく、サポートされているいずれかの方法でアクセス権を要求できます。
   
1. Azure portal で仮想マシンのページを開きます。

2. 接続先の VM を選択し、 **[接続]** ページを開きます。

   - Azure により、その VM で JIT が有効になっているかどうかが確認されます。

        - VM に対して JIT が有効になっていない場合は、有効にするように求められます。
    
        - JIT が有効になっている場合は、**[アクセス権の要求]** を選択し、要求元の IP、時間の範囲、その VM 用に構成されているポートを指定して、アクセス要求を渡します。

![image](https://github.com/MicrosoftLearning/Secure-Azure-services-and-workloads-with-Microsoft-Defender-for-Cloud-regulatory-compliance-controls/assets/91347931/7e454150-bc04-47bc-afa1-e0a1e8af17f9)






> **結果**: VM で JIT を有効にする方法と、Microsoft Defender for Cloud で JIT が有効になっている VM へのアクセスを要求する方法について、さまざまな方法を確認しました。
