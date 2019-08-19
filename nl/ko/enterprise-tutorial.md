---

copyright:
  years: 2019
lastupdated: "2019-07-26"

keywords: enterprise, enterprise account, create enterprise, set up enterprise, enterprise users, enterprise access, enterprise tutorial

subcollection: account

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:codeblock: .codeblock}
{:important: .important}
{:tip: .tip}
{:note: .note}

# 엔터프라이즈 시작하기
{: #enterprise-tutorial}

이 튜토리얼에서는 여러 {{site.data.keyword.Bluemix}} 계정의 사용량 비용을 관리하고 추적할 수 있도록 부서별로 엔터프라이즈를 설정하는 방법을 안내합니다. 이 튜토리얼을 완료하면 엔터프라이즈를 작성하고, 계정을 추가하여 계정 그룹으로 구성하고, 사용자를 초대하고, 구독을 탐색하는 방법을 학습할 수 있습니다.
{:shortdesc}

이 튜토리얼은 다음 구조로 엔터프라이즈를 작성하려 하는, *Example Corp*라는 가상의 회사를 사용합니다. 튜토리얼을 진행할 때는 각 단계를 자신의 조직 계정과 원하는 구조에 맞춰 조정하십시오. 

![ 조직의 부서에 따라 계정을 그룹화하는 4계층 엔터프라이즈입니다. 예를 들면 Marketing, Development, Sales와 같이 계정 그룹의 이름을 지정할 수 있습니다. 이들 계정 그룹은 해당 부서의 팀에 속한 계정을 포함합니다. 예를 들면, Sales 계정 그룹은 Direct, Online, 및 Enablement에 대한 계정을 포함합니다. ](images/enterprise-by-dept.svg "조직의 부서에 따라 계정을 체계화하는 엔터프라이즈입니다. "){: caption="Figure 1. An enterprise that is organized by department" caption-side="bottom"}

## 시작하기 전에
{: #setting-prereqs}

엔터프라이즈에서 계정 관리, 청구, 리소스, 사용자 및 액세스 권한 관리가 이뤄지는 방식에 대한 기본 원리를 알아보려면 [엔터프라이즈의 개념](/docs/account?topic=account-enterprise)을 읽으십시오. 

엔터프라이즈를 작성하는 데 기반 계정 역할을 하는 구독 계정에서 필요한 액세스 권한이 있는지 확인하십시오. 엔터프라이즈를 작성하려면 계정 소유자이거나, 청구 계정 관리 서비스에 대한 관리자 역할이 있어야 합니다. 

계정으로부터 엔터프라이즈를 작성하는 것과 기존 계정을 가져오는 것은 실행 취소할 수 없습니다. 이 튜토리얼에서는 부서별로 엔터프라이즈를 구성하기 위해 따를 수 있는 단계의 예를 제공하지만, 사용자는 자기 조직의 필요성에 따라 엔터프라이즈 구조를 신중하게 계획해야 합니다.
{:important}

## 1단계. 엔터프라이즈 작성
{: #create_enterprise_tutorial}

엔터프라이즈는 기존 구독 계정으로부터 작성됩니다. 엔터프라이즈를 작성하면 계정이 엔터프라이즈 계층 구조에 추가됩니다. 청구는 엔터프라이즈에 의해 관리되도록 전환되지만, 해당 사용자 및 리소스는 동일하게 유지되며 전혀 영향을 받지 않습니다. 계정에 미치는 영향에 대한 전체 설명은 [엔터프라이즈 작성](/docs/account?topic=account-create-enterprise)을 참조하십시오. 

1. **관리** > **엔터프라이즈**로 이동하여 **작성**을 클릭하십시오. 
2. 엔터프라이즈를 식별하기 위해 회사 이름(예: Example Corp)을 입력하십시오. 
3. 회사의 도메인(예: `examplecorp.com`)을 입력하십시오. 
4. 계정에 미치는 영향에 대한 정보를 검토하고 **계정에 미치는 영향을 이해했습니다**를 선택하십시오. 그 후 **작성**을 클릭하십시오. 이 계정은 이제 영구적으로 엔터프라이즈의 일부가 되며 제거할 수 없습니다. 

엔터프라이즈가 작성되고 나면 엔터프라이즈 대시보드로 이동됩니다. 여기서는 엔터프라이즈 세부사항, 계정, 사용자 및 청구 정보를 볼 수 있습니다. **계정** 페이지로 이동하여 엔터프라이즈 구조를 보면 다음 계정을 볼 수 있습니다. 
  * 엔터프라이즈와 동일한 이름을 가진 엔터프라이즈 계정. 이 계정은 엔터프라이즈 관리에 사용됩니다. 
  * 엔터프라이즈를 작성하는 데 사용한 계정. 사용자는 아무런 영향 없이 계속해서 리소스에 대해 작업할 수 있습니다. 

## 2단계. 계정 그룹을 사용하여 엔터프라이즈 구조 작성
{: #account_groups_tutorial}

계정 그룹을 사용하여 서로 관련된 계정을 체계화하십시오. Example Corp. 엔터프라이즈 계층 구조의 두 번째 및 세 번째 계층은 Marketing, Development, Sales, Design, 및 Engineering 계정 그룹을 포함하고 있습니다. 계정 그룹을 작성하려면 다음 단계를 완료하십시오. 

1. 엔터프라이즈 대시보드에서 **계정**을 클릭하여 엔터프라이즈의 계정 및 계정 그룹을 보십시오. 
2. 계정 그룹 섹션에서 **작성**을 클릭하십시오. 
3. 계정 그룹 이름(예: `Marketing`)을 입력하십시오. 
4. 담당자 필드에 해당 계정 그룹의 기본 담당자로 지정할 사용자의 IBM ID를 입력하십시오. 계정 그룹은 리소스를 포함할 수 없으므로 계정의 경우와 같은 소유자가 없습니다. 
5. **Example Corp**를 상위 계정으로 선택하십시오. 
6. **작성**을 클릭하십시오.

위 단계를 반복하여 Sales, Development, Design 및 Engineering 계정 그룹을 작성하십시오. Design 및 Engineering 계정 그룹을 작성할 때는 Development를 상위 계정 그룹으로 추가하십시오. 

## 3단계. 기존 계정 가져오기
{: #existing_accounts_tutorial}

엔터프라이즈 구조를 작성했으므로 이제 기존 계정을 엔터프라이즈로 가져올 수 있습니다. 계정은 가져오면 해당 엔터프라이즈에 영구적으로 추가됩니다. 엔터프라이즈를 작성하는 경우와 마찬가지로, 가져오는 계정의 청구는 엔터프라이즈에 의해 관리되도록 전환되지만 해당 사용자 및 리소스는 동일하게 유지됩니다. 세부사항은 [기존 계정 가져오기](/docs/account?topic=account-enterprise-add#add-accounts)를 참조하십시오. 

기존 계정을 가져오려면 다음 액세스 권한이 필요합니다. 

* 가져오는 계정에서 사용자가 계정 소유자이거나, 사용자에게 계정 내의 엔터프라이즈 및 청구 계정 관리 서비스에 대한 관리자 역할이 있어야 합니다. 
* 엔터프라이즈에서 사용자에게 엔터프라이즈 서비스에 대한 편집자 또는 관리자 역할이 있고, 청구 서비스에 대한 관리자 역할이 있어야 합니다. 

다음 단계를 완료하여 예로 사용되는 UX-UI 계정을 Design 계정 그룹으로 가져오십시오. 
1. 엔터프라이즈 대시보드에서 **계정**을 클릭하여 엔터프라이즈의 계정 및 계정 그룹을 보십시오. 
2. 계정 섹션에서 **추가** > **계정 가져오기**를 클릭하십시오. 
3. **계정** 목록에서 **UX-UI**를 선택하십시오. 

  표시되는 계정이 없는 경우에는 기존 계정에서 적절한 액세스 권한이 없을 가능성이 높습니다.
  {: tip}

4. **Design**을 UX-UI 계정의 상위로 선택하십시오. 이는 해당 계정이 엔터프라이즈 계층 구조에서 차지하는 위치를 결정합니다. 
5. 계정에 미치는 영향에 대한 정보를 검토하고 **계정에 미치는 영향을 이해했습니다**를 선택하십시오. 그 후 **가져오기**를 클릭하십시오. 

추가 계정을 가져오려면 위 단계를 반복하십시오. 

## 4단계. 새 계정 작성
{: #create-accounts_tutorial}

엔터프라이즈에서 새 계정을 작성할 수 있습니다. 이 계정은 종량과금제 계정으로 작성되며 사용량은 엔터프라이즈에 청구됩니다. 계정을 작성하려면 엔터프라이즈 서비스에 대한 편집자 또는 관리자 역할이 있는 액세스 정책이 필요합니다. 

다음 단계를 완료하여 예로 사용되는 Web 계정을 엔터프라이즈에서 작성하십시오. 

1. 엔터프라이즈 대시보드에서 **계정**을 클릭하여 엔터프라이즈의 계정 및 계정 그룹을 보십시오. 
1. 계정 섹션에서 **추가** > **계정 작성**을 선택하십시오. 
1. `Web`을 계정의 이름으로 입력하십시오. 
1. 다른 사용자를 계정 소유자로 지정하려는 경우에는 **소유자** 필드에 해당 사용자의 IBM ID를 입력하십시오. 계정 소유자는 계정을 관리하기 위한 전체 액세스 권한을 갖습니다. 
1. **Marketing**을 이 계정의 상위로 선택하십시오. 
1. **작성**을 클릭하십시오.

계정을 작성하고 나면, 계정 소유자는 계정에 로그인하여 다른 사용자를 초대하고 이들의 액세스 권한을 관리할 수 있습니다. 

추가 계정을 작성하려면 위 단계를 반복하십시오. 예를 들면, Example Corp 엔터프라이즈는 다음 하위 계정 및 상위 계정 그룹 계층 구조를 갖습니다. 

| 하위 | 상위 |
| ----- | -------|
| Print | Marketing |
| Frontend |엔지니어링 |
| Backend |엔지니어링 |
| Direct | Sales |
| Online | Sales |
| Enablement | Sales |
{:caption="표 1. 하위 계정 및 상위 계정 그룹 계층 구조" caption-side="top"}

## 5단계. 구독 탐색
{: #explore-sub_tutorial}

엔터프라이즈 대시보드에서 엔터프라이즈의 구독을 탐색할 수 있습니다. 엔터프라이즈로 가져온 계정의 기존 구독은 엔터프라이즈 계정으로 이동되어 엔터프라이즈 [크레딧 풀](/docs/billing-usage?topic=billing-usage-enterprise#credit-pool)에 추가됩니다. 

1. **대시보드**를 클릭하여 엔터프라이즈 대시보드로 되돌아가십시오. 청구 섹션에서는 사용 가능한 크레딧, 잔여 크레딧 및 구독 만기 날짜를 볼 수 있습니다. 
1. 엔터프라이즈의 모든 구독에 대한 세부사항을 보려면 **구독 보기**를 클릭하십시오. 

   플랫폼 구독 섹션에서는 구독 시작 날짜, 종료 날짜, 시작 크레딧 및 사용 가능한 크레딧을 볼 수 있습니다. 크레딧을 추가하려는 경우에는 추가 구독을 구매하고 구독 코드를 적용할 수 있습니다. 

## 6단계. 하위 계정의 사용자에게 리소스 작성을 위한 액세스 권한 지정
{: #users_create_resources}

시작하기 전에 리소스를 작성할 계정으로 전환하십시오. 이 튜토리얼의 경우에는 *Print* 계정으로 전환하십시오. 계정의 사용자가 카탈로그로부터 리소스를 작성하고 이를 리소스 그룹에 지정하도록 하려면 두 가지 유형의 액세스 정책을 지정해야 합니다. 
* 리소스 그룹에 대한 뷰어 이상의 역할이 있는 액세스 정책을 지정하십시오. 
* 서비스에 대한 편집자 또는 관리자 역할이 있는 액세스 정책을 지정하십시오. 

필요한 액세스 권한을 지정하려면 다음 단계를 완료하십시오. 

1. **관리** > **액세스(IAM)**로 이동하고 **사용자**를 선택하십시오.
2. 목록에서 사용자 이름을 선택하십시오.
3. **액세스 정책** 탭 > **액세스 지정**을 클릭하십시오. 
4. **리소스 그룹 내의 액세스 지정**을 클릭하십시오. 
5. 사용자에게 액세스 권한을 지정할 리소스 그룹을 선택하십시오. 
6. 리소스 그룹에 대해 뷰어 이상의 역할을 선택하십시오. 
7. 사용자에게 액세스 권한을 지정할 서비스를 선택하십시오. 
  * 사용자가 모든 서비스를 프로비저닝할 수 있도록 하려면 **모든 서비스**를 선택하십시오. 
  * 사용자에게 특정 액세스 권한을 지정하려면 목록에서 서비스를 선택하십시오. 사용자가 선택된 서비스에 대해서만 액세스 권한을 갖습니다. 
8. 편집자 또는 관리자 역할을 선택하십시오. 
9. **지정**을 클릭하십시오.

## 7단계. 모든 계정의 사용량 보기
{: #usage_tutorial}

1. Example Corp 엔터프라이즈 계정에 로그인하십시오. 
2. **관리 > 청구 및 사용량**으로 이동하여 **사용량**을 선택하십시오.

   사용량 페이지는 엔터프라이즈의 모든 사용량에 대한 비용을 계정 및 계정 그룹으로 구분하여 표시합니다. 클래식 인프라 서비스의 사용량 정보는 현재 청구 기간에 대해 포함되지 않습니다. 자세한 정보는 [클래식 인프라 리소스의 사용량 보기](/docs/billing-usage?topic=billing-usage-infra-usage)를 참조하십시오. 
3. 테이블의 **Marketing**을 클릭하여 이 계정 그룹의 사용량을 보십시오. 엔터프라이즈 레벨과 마찬가지로, 사용량은 계정 및 계정 그룹으로 구분됩니다. 
4. 리소스별 사용량을 보려면 테이블에서 계정 그룹을 클릭하거나 **엔터프라이즈** 메뉴에서 계정을 선택하여 계정 레벨로 이동하십시오. 해당 시간 범위 동안 사용된 각 리소스 유형에 대한 비용이 표시됩니다. 

Development, Sales, Design 및 Engineering 계정 그룹에 대해 위 단계를 반복하십시오. 

   엔터프라이즈 계정에서는 리소스 플랜 또는 인스턴스에 대한 사용량 데이터를 볼 수 없으며, 이를 위해서는 해당 계정 자체에 대한 액세스 권한이 필요합니다. 계정에 대한 데이터를 보려면 **계정으로 전환**을 클릭하십시오. 계정의 리소스 및 서비스에 대한 청구 액세스 권한이 필요합니다. 자세한 정보는 [사용량 보기](/docs/billing-usage?topic=billing-usage-viewingusage)를 참조하십시오. 

엔터프라이즈 계정에서는 엔터프라이즈의 계정에 의해 발생한 사용량에 대해서만 데이터가 표시됩니다. 계정이 엔터프라이즈에 추가되기 전의 사용량을 보려면 해당 계정에 로그인하여 관련 시간 범위를 선택하십시오.
{: note}